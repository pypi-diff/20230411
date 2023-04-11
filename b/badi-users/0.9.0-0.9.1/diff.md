# Comparing `tmp/badi_users-0.9.0.tar.gz` & `tmp/badi_users-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "badi_users-0.9.0.tar", last modified: Thu Mar 30 06:07:45 2023, max compression
+gzip compressed data, was "badi_users-0.9.1.tar", last modified: Tue Apr 11 04:59:14 2023, max compression
```

## Comparing `badi_users-0.9.0.tar` & `badi_users-0.9.1.tar`

### file list

```diff
@@ -1,311 +1,311 @@
-drwxrwxrwx   0        0        0        0 2023-03-30 06:07:45.416543 badi_users-0.9.0/
--rw-rw-rw-   0        0        0     1093 2022-09-24 06:05:13.000000 badi_users-0.9.0/LICENSE
--rw-rw-rw-   0        0        0     1066 2022-11-10 17:03:20.000000 badi_users-0.9.0/MANIFEST.in
--rw-rw-rw-   0        0        0      419 2023-03-30 06:07:45.415546 badi_users-0.9.0/PKG-INFO
--rw-rw-rw-   0        0        0      143 2022-10-02 09:04:41.000000 badi_users-0.9.0/README.md
-drwxrwxrwx   0        0        0        0 2023-03-30 06:07:42.975492 badi_users-0.9.0/badi_ticket/
--rw-rw-rw-   0        0        0        0 2023-03-27 19:00:31.000000 badi_users-0.9.0/badi_ticket/__init__.py
--rw-rw-rw-   0        0        0      143 2023-03-27 19:00:31.000000 badi_users-0.9.0/badi_ticket/admin.py
--rw-rw-rw-   0        0        0     9560 2023-03-28 07:22:27.000000 badi_users-0.9.0/badi_ticket/api.py
--rw-rw-rw-   0        0        0      129 2023-03-27 19:00:31.000000 badi_users-0.9.0/badi_ticket/apps.py
-drwxrwxrwx   0        0        0        0 2023-03-30 06:07:42.916939 badi_users-0.9.0/badi_ticket/locale/
-drwxrwxrwx   0        0        0        0 2023-03-30 06:07:42.917135 badi_users-0.9.0/badi_ticket/locale/fa/
-drwxrwxrwx   0        0        0        0 2023-03-30 06:07:42.977455 badi_users-0.9.0/badi_ticket/locale/fa/LC_MESSAGES/
--rw-rw-rw-   0        0        0     2415 2023-03-30 05:20:05.000000 badi_users-0.9.0/badi_ticket/locale/fa/LC_MESSAGES/django.mo
-drwxrwxrwx   0        0        0        0 2023-03-30 06:07:42.978452 badi_users-0.9.0/badi_ticket/migrations/
--rw-rw-rw-   0        0        0        0 2022-08-06 18:28:13.000000 badi_users-0.9.0/badi_ticket/migrations/__init__.py
--rw-rw-rw-   0        0        0     3022 2023-03-27 19:00:31.000000 badi_users-0.9.0/badi_ticket/models.py
--rw-rw-rw-   0        0        0      313 2023-03-27 19:00:31.000000 badi_users-0.9.0/badi_ticket/routers.py
--rw-rw-rw-   0        0        0     2082 2023-03-27 19:00:31.000000 badi_users-0.9.0/badi_ticket/serializers.py
-drwxrwxrwx   0        0        0        0 2023-03-30 06:07:42.917930 badi_users-0.9.0/badi_ticket/static/
-drwxrwxrwx   0        0        0        0 2023-03-30 06:07:42.917930 badi_users-0.9.0/badi_ticket/static/ticket/
-drwxrwxrwx   0        0        0        0 2023-03-30 06:07:42.986431 badi_users-0.9.0/badi_ticket/static/ticket/js/
--rw-rw-rw-   0        0        0     2147 2023-03-27 19:00:31.000000 badi_users-0.9.0/badi_ticket/static/ticket/js/chat.js
-drwxrwxrwx   0        0        0        0 2023-03-30 06:07:42.987428 badi_users-0.9.0/badi_ticket/templates/
--rw-rw-rw-   0        0        0        0 2023-03-27 19:00:31.000000 badi_users-0.9.0/badi_ticket/templates/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-30 06:07:42.992417 badi_users-0.9.0/badi_ticket/templates/ticket/
--rw-rw-rw-   0        0        0     6358 2023-03-27 19:00:31.000000 badi_users-0.9.0/badi_ticket/templates/ticket/admin_tickets.html
--rw-rw-rw-   0        0        0     5265 2023-03-27 19:00:31.000000 badi_users-0.9.0/badi_ticket/templates/ticket/message_list.html
--rw-rw-rw-   0        0        0     9642 2023-03-27 19:00:31.000000 badi_users-0.9.0/badi_ticket/templates/ticket/my_tickets.html
--rw-rw-rw-   0        0        0     7102 2023-03-28 07:19:11.000000 badi_users-0.9.0/badi_ticket/templates/ticket/ticket_create.html
--rw-rw-rw-   0        0        0     1639 2023-03-27 19:00:31.000000 badi_users-0.9.0/badi_ticket/templates/ticket/ticket_update.html
--rw-rw-rw-   0        0        0       63 2023-03-27 19:00:31.000000 badi_users-0.9.0/badi_ticket/tests.py
--rw-rw-rw-   0        0        0      583 2023-03-27 19:00:31.000000 badi_users-0.9.0/badi_ticket/urls.py
--rw-rw-rw-   0        0        0     1997 2023-03-28 07:12:21.000000 badi_users-0.9.0/badi_ticket/views.py
-drwxrwxrwx   0        0        0        0 2023-03-30 06:07:43.022248 badi_users-0.9.0/badi_user/
--rw-rw-rw-   0        0        0        0 2023-03-27 19:00:31.000000 badi_users-0.9.0/badi_user/__init__.py
--rw-rw-rw-   0        0        0      166 2023-03-27 19:00:31.000000 badi_users-0.9.0/badi_user/admin.py
-drwxrwxrwx   0        0        0        0 2023-03-30 06:07:43.037181 badi_users-0.9.0/badi_user/api/
--rw-rw-rw-   0        0        0        0 2023-03-27 19:00:31.000000 badi_users-0.9.0/badi_user/api/__init__.py
--rw-rw-rw-   0        0        0    29693 2023-03-27 19:00:31.000000 badi_users-0.9.0/badi_user/api/api.py
--rw-rw-rw-   0        0        0      485 2023-03-27 19:00:31.000000 badi_users-0.9.0/badi_user/api/routers.py
--rw-rw-rw-   0        0        0     6013 2023-03-27 19:00:31.000000 badi_users-0.9.0/badi_user/api/serializers.py
--rw-rw-rw-   0        0        0      183 2023-03-27 19:00:31.000000 badi_users-0.9.0/badi_user/apps.py
--rw-rw-rw-   0        0        0     3428 2023-03-27 19:00:31.000000 badi_users-0.9.0/badi_user/filter.py
-drwxrwxrwx   0        0        0        0 2023-03-30 06:07:42.925913 badi_users-0.9.0/badi_user/locale/
-drwxrwxrwx   0        0        0        0 2023-03-30 06:07:42.926910 badi_users-0.9.0/badi_user/locale/fa/
-drwxrwxrwx   0        0        0        0 2023-03-30 06:07:43.039176 badi_users-0.9.0/badi_user/locale/fa/LC_MESSAGES/
--rw-rw-rw-   0        0        0     3834 2023-03-30 05:20:05.000000 badi_users-0.9.0/badi_user/locale/fa/LC_MESSAGES/django.mo
-drwxrwxrwx   0        0        0        0 2023-03-30 06:07:43.040176 badi_users-0.9.0/badi_user/migrations/
--rw-rw-rw-   0        0        0        0 2022-08-06 18:28:13.000000 badi_users-0.9.0/badi_user/migrations/__init__.py
--rw-rw-rw-   0        0        0     6551 2023-03-27 19:00:31.000000 badi_users-0.9.0/badi_user/models.py
-drwxrwxrwx   0        0        0        0 2023-03-30 06:07:43.046110 badi_users-0.9.0/badi_user/templates/
--rw-rw-rw-   0        0        0        0 2023-03-27 19:00:31.000000 badi_users-0.9.0/badi_user/templates/__init__.py
--rw-rw-rw-   0        0        0       27 2023-03-27 19:00:31.000000 badi_users-0.9.0/badi_user/templates/badi-user-test.html
-drwxrwxrwx   0        0        0        0 2023-03-30 06:07:43.048107 badi_users-0.9.0/badi_user/templates/group/
--rw-rw-rw-   0        0        0     8558 2023-03-27 19:00:31.000000 badi_users-0.9.0/badi_user/templates/group/group_create.html
--rw-rw-rw-   0        0        0     5472 2023-03-27 19:00:31.000000 badi_users-0.9.0/badi_user/templates/group/group_update.html
-drwxrwxrwx   0        0        0        0 2023-03-30 06:07:43.049105 badi_users-0.9.0/badi_user/templates/log/
--rw-rw-rw-   0        0        0     3987 2023-03-27 19:00:31.000000 badi_users-0.9.0/badi_user/templates/log/log_list.html
-drwxrwxrwx   0        0        0        0 2023-03-30 06:07:43.051121 badi_users-0.9.0/badi_user/templates/login-theme/
--rw-rw-rw-   0        0        0     7336 2023-03-27 19:00:31.000000 badi_users-0.9.0/badi_user/templates/login-theme/login-1.html
-drwxrwxrwx   0        0        0        0 2023-03-30 06:07:43.055089 badi_users-0.9.0/badi_user/templates/member/
--rw-rw-rw-   0        0        0     6863 2023-03-27 19:00:31.000000 badi_users-0.9.0/badi_user/templates/member/member_create.html
--rw-rw-rw-   0        0        0    22635 2023-03-27 19:00:31.000000 badi_users-0.9.0/badi_user/templates/member/member_list.html
--rw-rw-rw-   0        0        0     4783 2023-03-28 07:29:01.000000 badi_users-0.9.0/badi_user/templates/member/member_self_update.html
--rw-rw-rw-   0        0        0     6525 2023-03-27 19:00:31.000000 badi_users-0.9.0/badi_user/templates/member/member_update.html
-drwxrwxrwx   0        0        0        0 2023-03-30 06:07:43.058080 badi_users-0.9.0/badi_user/templates/user/
--rw-rw-rw-   0        0        0     6745 2023-03-27 19:00:31.000000 badi_users-0.9.0/badi_user/templates/user/change_password.html
--rw-rw-rw-   0        0        0     5973 2023-03-27 19:00:31.000000 badi_users-0.9.0/badi_user/templates/user/user_create.html
--rw-rw-rw-   0        0        0     4019 2023-03-27 19:00:31.000000 badi_users-0.9.0/badi_user/templates/user/user_list.html
--rw-rw-rw-   0        0        0     5005 2023-03-27 19:00:31.000000 badi_users-0.9.0/badi_user/templates/user/user_update.html
-drwxrwxrwx   0        0        0        0 2023-03-30 06:07:43.060075 badi_users-0.9.0/badi_user/templatetags/
--rw-rw-rw-   0        0        0        0 2023-03-27 19:00:31.000000 badi_users-0.9.0/badi_user/templatetags/__init__.py
--rw-rw-rw-   0        0        0     5950 2023-03-27 19:00:31.000000 badi_users-0.9.0/badi_user/templatetags/appfilter.py
--rw-rw-rw-   0        0        0      500 2023-03-27 19:00:31.000000 badi_users-0.9.0/badi_user/tests.py
-drwxrwxrwx   0        0        0        0 2023-03-30 06:07:43.092987 badi_users-0.9.0/badi_user/ui/
--rw-rw-rw-   0        0        0        0 2023-03-27 19:00:31.000000 badi_users-0.9.0/badi_user/ui/__init__.py
--rw-rw-rw-   0        0        0     1484 2023-03-27 19:00:31.000000 badi_users-0.9.0/badi_user/ui/forms.py
--rw-rw-rw-   0        0        0      320 2023-03-27 19:00:31.000000 badi_users-0.9.0/badi_user/ui/log_views.py
--rw-rw-rw-   0        0        0     1706 2023-03-28 08:00:41.000000 badi_users-0.9.0/badi_user/ui/member_views.py
--rw-rw-rw-   0        0        0      672 2023-03-27 19:00:31.000000 badi_users-0.9.0/badi_user/ui/notification_views.py
--rw-rw-rw-   0        0        0      644 2023-03-27 19:00:31.000000 badi_users-0.9.0/badi_user/ui/roles_views.py
--rw-rw-rw-   0        0        0     1614 2023-03-27 19:00:31.000000 badi_users-0.9.0/badi_user/ui/urls.py
--rw-rw-rw-   0        0        0     2633 2023-03-27 19:00:31.000000 badi_users-0.9.0/badi_user/ui/views.py
-drwxrwxrwx   0        0        0        0 2023-03-30 06:07:43.112935 badi_users-0.9.0/badi_users.egg-info/
--rw-rw-rw-   0        0        0      419 2023-03-30 06:07:42.000000 badi_users-0.9.0/badi_users.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    10750 2023-03-30 06:07:42.000000 badi_users-0.9.0/badi_users.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-30 06:07:42.000000 badi_users-0.9.0/badi_users.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-03-30 06:07:42.000000 badi_users-0.9.0/badi_users.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-30 06:07:43.190142 badi_users-0.9.0/badi_utils/
--rw-rw-rw-   0        0        0        0 2022-09-24 05:54:56.000000 badi_users-0.9.0/badi_utils/__init__.py
--rw-rw-rw-   0        0        0     6835 2022-09-24 08:08:59.000000 badi_users-0.9.0/badi_utils/date_calc.py
--rw-rw-rw-   0        0        0    28225 2023-01-30 19:13:21.000000 badi_users-0.9.0/badi_utils/dynamic.py
--rw-rw-rw-   0        0        0    22478 2022-12-03 08:13:14.000000 badi_users-0.9.0/badi_utils/dynamic_api.py
--rw-rw-rw-   0        0        0     3412 2022-10-29 14:49:57.000000 badi_users-0.9.0/badi_utils/dynamic_models.py
--rw-rw-rw-   0        0        0     2990 2022-09-26 04:39:36.000000 badi_users-0.9.0/badi_utils/email.py
--rw-rw-rw-   0        0        0      252 2022-09-26 05:16:38.000000 badi_users-0.9.0/badi_utils/errors.py
--rw-rw-rw-   0        0        0     1509 2022-11-12 15:50:44.000000 badi_users-0.9.0/badi_utils/logging.py
--rw-rw-rw-   0        0        0      947 2022-08-06 18:28:12.000000 badi_users-0.9.0/badi_utils/responses.py
--rw-rw-rw-   0        0        0      904 2023-02-06 12:51:34.000000 badi_users-0.9.0/badi_utils/rss.py
--rw-rw-rw-   0        0        0     1529 2022-09-24 12:31:48.000000 badi_users-0.9.0/badi_utils/select2.py
--rw-rw-rw-   0        0        0     2132 2023-03-27 18:55:33.000000 badi_users-0.9.0/badi_utils/sms.py
-drwxrwxrwx   0        0        0        0 2023-03-30 06:07:42.931065 badi_users-0.9.0/badi_utils/static/
-drwxrwxrwx   0        0        0        0 2023-03-30 06:07:42.932289 badi_users-0.9.0/badi_utils/static/badi_utils/
-drwxrwxrwx   0        0        0        0 2023-03-30 06:07:43.196126 badi_users-0.9.0/badi_utils/static/badi_utils/css/
--rw-rw-rw-   0        0        0    40504 2023-01-30 18:56:15.000000 badi_users-0.9.0/badi_utils/static/badi_utils/css/custom.css
-drwxrwxrwx   0        0        0        0 2023-03-30 06:07:43.636473 badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/
--rw-rw-rw-   0        0        0    59778 2022-08-14 04:14:25.000000 badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum).eot
--rw-rw-rw-   0        0        0    59532 2022-08-14 04:14:25.000000 badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum).ttf
--rw-rw-rw-   0        0        0    38401 2022-08-14 04:14:25.000000 badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum).woff
--rw-rw-rw-   0        0        0    31304 2022-08-14 04:14:25.000000 badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum).woff2
--rw-rw-rw-   0        0        0    59778 2022-08-14 04:14:25.000000 badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_2.eot
--rw-rw-rw-   0        0        0    31992 2022-08-14 04:14:25.000000 badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold.eot
--rw-rw-rw-   0        0        0    57268 2022-08-14 04:14:26.000000 badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold.ttf
--rw-rw-rw-   0        0        0    36069 2022-08-14 04:14:26.000000 badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold.woff
--rw-rw-rw-   0        0        0    28856 2022-08-14 04:14:26.000000 badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold.woff2
--rw-rw-rw-   0        0        0    31992 2022-08-14 04:14:26.000000 badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold_2.eot
--rw-rw-rw-   0        0        0    35477 2022-08-14 04:14:26.000000 badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light.eot
--rw-rw-rw-   0        0        0    60584 2022-08-14 04:14:26.000000 badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light.ttf
--rw-rw-rw-   0        0        0    39557 2022-08-14 04:14:26.000000 badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light.woff
--rw-rw-rw-   0        0        0    32344 2022-08-14 04:14:26.000000 badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light.woff2
--rw-rw-rw-   0        0        0    35477 2022-08-14 04:14:26.000000 badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light_2.eot
--rw-rw-rw-   0        0        0    32043 2022-08-14 04:14:26.000000 badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium.eot
--rw-rw-rw-   0        0        0    58192 2022-08-14 04:14:26.000000 badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium.ttf
--rw-rw-rw-   0        0        0    36145 2022-08-14 04:14:26.000000 badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium.woff
--rw-rw-rw-   0        0        0    28912 2022-08-14 04:14:26.000000 badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium.woff2
--rw-rw-rw-   0        0        0    32043 2022-08-14 04:14:26.000000 badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium_2.eot
--rw-rw-rw-   0        0        0    33102 2022-08-14 04:14:26.000000 badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight.eot
--rw-rw-rw-   0        0        0    56352 2022-08-14 04:14:26.000000 badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight.ttf
--rw-rw-rw-   0        0        0    36913 2022-08-14 04:14:26.000000 badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight.woff
--rw-rw-rw-   0        0        0    30072 2022-08-14 04:14:26.000000 badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight.woff2
--rw-rw-rw-   0        0        0    33102 2022-08-14 04:14:26.000000 badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight_2.eot
--rw-rw-rw-   0        0        0    58886 2022-08-14 04:14:26.000000 badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb.eot
--rw-rw-rw-   0        0        0    38473 2022-08-14 04:14:26.000000 badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb.woff
--rw-rw-rw-   0        0        0    31320 2022-08-14 04:14:26.000000 badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb.woff2
--rw-rw-rw-   0        0        0    58886 2022-08-14 04:14:26.000000 badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_2.eot
--rw-rw-rw-   0        0        0    57974 2022-08-14 04:14:26.000000 badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold.eot
--rw-rw-rw-   0        0        0    57760 2022-08-14 04:14:26.000000 badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold.ttf
--rw-rw-rw-   0        0        0    36629 2022-08-14 04:14:26.000000 badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold.woff
--rw-rw-rw-   0        0        0    29688 2022-08-14 04:14:26.000000 badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold.woff2
--rw-rw-rw-   0        0        0    57974 2022-08-14 04:14:26.000000 badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold_2.eot
--rw-rw-rw-   0        0        0    57974 2022-08-14 04:14:26.000000 badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold_3.eot
--rw-rw-rw-   0        0        0    35458 2022-08-14 04:14:26.000000 badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light.eot
--rw-rw-rw-   0        0        0    59968 2022-08-14 04:14:26.000000 badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light.ttf
--rw-rw-rw-   0        0        0    39693 2022-08-14 04:14:26.000000 badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light.woff
--rw-rw-rw-   0        0        0    32420 2022-08-14 04:14:26.000000 badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light.woff2
--rw-rw-rw-   0        0        0    35458 2022-08-14 04:14:26.000000 badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light_2.eot
--rw-rw-rw-   0        0        0    31983 2022-08-14 04:14:26.000000 badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium.eot
--rw-rw-rw-   0        0        0    57544 2022-08-14 04:14:26.000000 badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium.ttf
--rw-rw-rw-   0        0        0    36141 2022-08-14 04:14:26.000000 badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium.woff
--rw-rw-rw-   0        0        0    28916 2022-08-14 04:14:26.000000 badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium.woff2
--rw-rw-rw-   0        0        0    31983 2022-08-14 04:14:26.000000 badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium_2.eot
--rw-rw-rw-   0        0        0    33044 2022-08-14 04:14:26.000000 badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight.eot
--rw-rw-rw-   0        0        0    55640 2022-08-14 04:14:26.000000 badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight.ttf
--rw-rw-rw-   0        0        0    36945 2022-08-14 04:14:26.000000 badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight.woff
--rw-rw-rw-   0        0        0    29840 2022-08-14 04:14:26.000000 badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight.woff2
--rw-rw-rw-   0        0        0    33044 2022-08-14 04:14:26.000000 badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight_2.eot
--rw-rw-rw-   0        0        0    93376 2022-08-14 04:14:26.000000 badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/Ray-Black.ttf
--rw-rw-rw-   0        0        0    94304 2022-08-14 04:14:26.000000 badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/Ray-Bold.ttf
--rw-rw-rw-   0        0        0    94740 2022-08-14 04:14:26.000000 badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/Ray.ttf
-drwxrwxrwx   0        0        0        0 2023-03-30 06:07:43.738169 badi_users-0.9.0/badi_utils/static/badi_utils/js/
--rw-rw-rw-   0        0        0   478686 2023-01-03 13:51:41.000000 badi_users-0.9.0/badi_utils/static/badi_utils/js/apexchart.js
--rw-rw-rw-   0        0        0    19110 2022-08-14 04:14:25.000000 badi_users-0.9.0/badi_utils/static/badi_utils/js/api-login.js
--rw-rw-rw-   0        0        0    20445 2022-12-01 13:15:11.000000 badi_users-0.9.0/badi_utils/static/badi_utils/js/api.js
--rw-rw-rw-   0        0        0    25944 2023-03-29 06:15:03.000000 badi_users-0.9.0/badi_utils/static/badi_utils/js/base.js
--rw-rw-rw-   0        0        0     2149 2022-08-14 04:14:25.000000 badi_users-0.9.0/badi_utils/static/badi_utils/js/chat.js
--rw-rw-rw-   0        0        0     3167 2022-08-14 04:14:25.000000 badi_users-0.9.0/badi_utils/static/badi_utils/js/custom-vue.js
--rw-rw-rw-   0        0        0    18560 2023-03-27 14:51:58.000000 badi_users-0.9.0/badi_utils/static/badi_utils/js/datatable.js
--rw-rw-rw-   0        0        0     2470 2022-08-15 18:25:55.000000 badi_users-0.9.0/badi_utils/static/badi_utils/js/image-field.js
--rw-rw-rw-   0        0        0    30541 2023-03-29 06:13:24.000000 badi_users-0.9.0/badi_utils/static/badi_utils/js/main.js
--rw-rw-rw-   0        0        0      959 2022-08-14 04:14:26.000000 badi_users-0.9.0/badi_utils/static/badi_utils/js/notification.js
--rw-rw-rw-   0        0        0     2213 2022-08-14 04:14:26.000000 badi_users-0.9.0/badi_utils/static/badi_utils/js/pagination-vue.js
--rw-rw-rw-   0        0        0    20317 2023-03-30 04:45:54.000000 badi_users-0.9.0/badi_utils/static/badi_utils/js/tableexport.js
--rw-rw-rw-   0        0        0      654 2022-08-14 04:14:26.000000 badi_users-0.9.0/badi_utils/static/badi_utils/js/transaction.js
--rw-rw-rw-   0        0        0   354110 2022-08-14 04:14:26.000000 badi_users-0.9.0/badi_utils/static/badi_utils/js/vue.js
--rw-rw-rw-   0        0        0   268386 2023-03-30 05:07:06.000000 badi_users-0.9.0/badi_utils/static/badi_utils/js/xlsx.mini.min.js
-drwxrwxrwx   0        0        0        0 2023-03-30 06:07:43.744961 badi_users-0.9.0/badi_utils/templates/
--rw-rw-rw-   0        0        0        0 2022-09-24 07:28:02.000000 badi_users-0.9.0/badi_utils/templates/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-30 06:07:45.019600 badi_users-0.9.0/badi_utils/templates/component/
--rw-rw-rw-   0        0        0     1777 2022-10-25 06:27:38.000000 badi_users-0.9.0/badi_utils/templates/component/createModal.html
--rw-rw-rw-   0        0        0     1645 2022-08-14 04:14:27.000000 badi_users-0.9.0/badi_utils/templates/component/createTitle.html
--rw-rw-rw-   0        0        0     1054 2022-08-14 04:14:27.000000 badi_users-0.9.0/badi_utils/templates/component/filter-form.html
--rw-rw-rw-   0        0        0      729 2022-08-14 04:14:27.000000 badi_users-0.9.0/badi_utils/templates/component/form-errors.html
--rw-rw-rw-   0        0        0     1340 2022-08-14 04:14:27.000000 badi_users-0.9.0/badi_utils/templates/component/form-progressbar-js.html
--rw-rw-rw-   0        0        0      491 2022-08-14 04:14:27.000000 badi_users-0.9.0/badi_utils/templates/component/form-progressbar.html
--rw-rw-rw-   0        0        0      342 2022-08-14 04:14:27.000000 badi_users-0.9.0/badi_utils/templates/component/form.html
--rw-rw-rw-   0        0        0     1231 2022-08-14 04:14:27.000000 badi_users-0.9.0/badi_utils/templates/component/image-field.html
--rw-rw-rw-   0        0        0    34439 2022-08-14 04:14:27.000000 badi_users-0.9.0/badi_utils/templates/component/index-menu.html
--rw-rw-rw-   0        0        0     2346 2022-08-14 04:14:27.000000 badi_users-0.9.0/badi_utils/templates/component/input.html
--rw-rw-rw-   0        0        0       69 2022-08-14 04:14:27.000000 badi_users-0.9.0/badi_utils/templates/component/loader.html
--rw-rw-rw-   0        0        0      468 2022-10-02 09:59:19.000000 badi_users-0.9.0/badi_utils/templates/component/menu-item.html
--rw-rw-rw-   0        0        0      362 2022-10-02 09:59:19.000000 badi_users-0.9.0/badi_utils/templates/component/menu-list.html
--rw-rw-rw-   0        0        0      746 2022-08-14 04:14:27.000000 badi_users-0.9.0/badi_utils/templates/component/messages.html
--rw-rw-rw-   0        0        0     1134 2022-12-31 05:14:56.000000 badi_users-0.9.0/badi_utils/templates/component/pagination-vue.html
--rw-rw-rw-   0        0        0      361 2022-08-14 04:14:27.000000 badi_users-0.9.0/badi_utils/templates/component/profile_item.html
--rw-rw-rw-   0        0        0      204 2022-08-14 04:14:27.000000 badi_users-0.9.0/badi_utils/templates/component/space-between.html
--rw-rw-rw-   0        0        0      430 2022-10-02 09:59:19.000000 badi_users-0.9.0/badi_utils/templates/component/svg-button-with-text.html
--rw-rw-rw-   0        0        0      428 2022-10-02 09:59:19.000000 badi_users-0.9.0/badi_utils/templates/component/svg-button.html
--rw-rw-rw-   0        0        0     1411 2022-08-14 04:14:27.000000 badi_users-0.9.0/badi_utils/templates/component/table-item.html
--rw-rw-rw-   0        0        0     2114 2022-08-14 04:14:27.000000 badi_users-0.9.0/badi_utils/templates/component/user-card.html
--rw-rw-rw-   0        0        0      257 2022-08-14 04:14:27.000000 badi_users-0.9.0/badi_utils/templates/component/yesno.html
-drwxrwxrwx   0        0        0        0 2023-03-30 06:07:45.299884 badi_users-0.9.0/badi_utils/templates/svg/
--rw-rw-rw-   0        0        0     1949 2022-08-06 18:28:13.000000 badi_users-0.9.0/badi_utils/templates/svg/Incoming-box.html
--rw-rw-rw-   0        0        0     1159 2022-08-06 18:28:13.000000 badi_users-0.9.0/badi_utils/templates/svg/add-user.html
--rw-rw-rw-   0        0        0     1092 2022-08-06 18:28:13.000000 badi_users-0.9.0/badi_utils/templates/svg/address-book.html
--rw-rw-rw-   0        0        0     1095 2022-08-06 18:28:13.000000 badi_users-0.9.0/badi_utils/templates/svg/arrow-left.html
--rw-rw-rw-   0        0        0     1081 2022-08-06 18:28:13.000000 badi_users-0.9.0/badi_utils/templates/svg/arrow-right.html
--rw-rw-rw-   0        0        0     2024 2022-08-14 04:14:27.000000 badi_users-0.9.0/badi_utils/templates/svg/bitcoin.html
--rw-rw-rw-   0        0        0      697 2022-08-06 18:28:13.000000 badi_users-0.9.0/badi_utils/templates/svg/box.html
--rw-rw-rw-   0        0        0     1378 2022-08-06 18:28:13.000000 badi_users-0.9.0/badi_utils/templates/svg/calendar-day.html
--rw-rw-rw-   0        0        0     1489 2022-08-06 18:28:13.000000 badi_users-0.9.0/badi_utils/templates/svg/calendar-gym.html
--rw-rw-rw-   0        0        0      925 2022-08-06 18:28:13.000000 badi_users-0.9.0/badi_utils/templates/svg/calendar.html
--rw-rw-rw-   0        0        0     1223 2022-12-01 08:20:56.000000 badi_users-0.9.0/badi_utils/templates/svg/call.html
--rw-rw-rw-   0        0        0     1385 2022-08-06 18:28:13.000000 badi_users-0.9.0/badi_utils/templates/svg/category.html
--rw-rw-rw-   0        0        0     1270 2022-08-14 04:14:27.000000 badi_users-0.9.0/badi_utils/templates/svg/chat.html
--rw-rw-rw-   0        0        0      938 2022-08-06 18:28:13.000000 badi_users-0.9.0/badi_utils/templates/svg/check.html
--rw-rw-rw-   0        0        0      344 2022-08-06 18:28:13.000000 badi_users-0.9.0/badi_utils/templates/svg/circle.html
--rw-rw-rw-   0        0        0     1686 2022-08-06 18:28:13.000000 badi_users-0.9.0/badi_utils/templates/svg/city.html
--rw-rw-rw-   0        0        0     1430 2022-08-06 18:28:13.000000 badi_users-0.9.0/badi_utils/templates/svg/clipboard-list.html
--rw-rw-rw-   0        0        0     2247 2022-08-06 18:28:13.000000 badi_users-0.9.0/badi_utils/templates/svg/clock.html
--rw-rw-rw-   0        0        0      645 2022-08-06 18:28:13.000000 badi_users-0.9.0/badi_utils/templates/svg/close.html
--rw-rw-rw-   0        0        0     2483 2022-08-06 18:28:13.000000 badi_users-0.9.0/badi_utils/templates/svg/collection.html
--rw-rw-rw-   0        0        0     1046 2022-08-14 04:14:27.000000 badi_users-0.9.0/badi_utils/templates/svg/comment.html
--rw-rw-rw-   0        0        0     1103 2022-08-06 18:28:13.000000 badi_users-0.9.0/badi_utils/templates/svg/dashboard.html
--rw-rw-rw-   0        0        0      893 2022-08-06 18:28:13.000000 badi_users-0.9.0/badi_utils/templates/svg/delete.html
--rw-rw-rw-   0        0        0     1505 2022-08-06 18:28:13.000000 badi_users-0.9.0/badi_utils/templates/svg/download.html
--rw-rw-rw-   0        0        0      901 2022-08-06 18:28:13.000000 badi_users-0.9.0/badi_utils/templates/svg/edit.html
--rw-rw-rw-   0        0        0     1361 2022-08-06 18:28:13.000000 badi_users-0.9.0/badi_utils/templates/svg/file-check.html
--rw-rw-rw-   0        0        0      988 2022-08-06 18:28:13.000000 badi_users-0.9.0/badi_utils/templates/svg/file.html
--rw-rw-rw-   0        0        0     2111 2022-08-06 18:28:13.000000 badi_users-0.9.0/badi_utils/templates/svg/film.html
--rw-rw-rw-   0        0        0      681 2022-08-14 04:14:27.000000 badi_users-0.9.0/badi_utils/templates/svg/fire.html
--rw-rw-rw-   0        0        0     1648 2022-08-06 18:28:13.000000 badi_users-0.9.0/badi_utils/templates/svg/group-chat.html
--rw-rw-rw-   0        0        0     1213 2022-08-06 18:28:13.000000 badi_users-0.9.0/badi_utils/templates/svg/group.html
--rw-rw-rw-   0        0        0     1394 2022-08-14 04:14:27.000000 badi_users-0.9.0/badi_utils/templates/svg/half_star.html
--rw-rw-rw-   0        0        0      944 2022-08-06 18:28:13.000000 badi_users-0.9.0/badi_utils/templates/svg/home.html
--rw-rw-rw-   0        0        0     1906 2022-08-14 04:14:27.000000 badi_users-0.9.0/badi_utils/templates/svg/hourse.html
--rw-rw-rw-   0        0        0      631 2022-08-06 18:28:13.000000 badi_users-0.9.0/badi_utils/templates/svg/image.html
--rw-rw-rw-   0        0        0      508 2022-08-06 18:28:13.000000 badi_users-0.9.0/badi_utils/templates/svg/info.html
--rw-rw-rw-   0        0        0     1394 2022-08-06 18:28:13.000000 badi_users-0.9.0/badi_utils/templates/svg/interview.html
--rw-rw-rw-   0        0        0     1389 2022-08-06 18:28:13.000000 badi_users-0.9.0/badi_utils/templates/svg/key.html
--rw-rw-rw-   0        0        0     2472 2022-08-06 18:28:13.000000 badi_users-0.9.0/badi_utils/templates/svg/logout.html
--rw-rw-rw-   0        0        0      940 2022-08-14 04:14:27.000000 badi_users-0.9.0/badi_utils/templates/svg/mail.html
--rw-rw-rw-   0        0        0      731 2022-08-06 18:28:13.000000 badi_users-0.9.0/badi_utils/templates/svg/map.html
--rw-rw-rw-   0        0        0     1601 2022-08-06 18:28:13.000000 badi_users-0.9.0/badi_utils/templates/svg/message.html
--rw-rw-rw-   0        0        0     1607 2022-08-06 18:28:13.000000 badi_users-0.9.0/badi_utils/templates/svg/messages.html
--rw-rw-rw-   0        0        0      683 2022-08-14 04:14:27.000000 badi_users-0.9.0/badi_utils/templates/svg/notification.html
--rw-rw-rw-   0        0        0      708 2022-08-06 18:28:13.000000 badi_users-0.9.0/badi_utils/templates/svg/plus.html
--rw-rw-rw-   0        0        0      753 2022-08-14 04:14:27.000000 badi_users-0.9.0/badi_utils/templates/svg/puzzle.html
--rw-rw-rw-   0        0        0      882 2022-08-14 04:14:27.000000 badi_users-0.9.0/badi_utils/templates/svg/question.html
--rw-rw-rw-   0        0        0     1174 2022-08-06 18:28:13.000000 badi_users-0.9.0/badi_utils/templates/svg/refresh.html
--rw-rw-rw-   0        0        0     1416 2022-08-06 18:28:13.000000 badi_users-0.9.0/badi_utils/templates/svg/safe.html
--rw-rw-rw-   0        0        0     1091 2022-09-21 07:25:46.000000 badi_users-0.9.0/badi_utils/templates/svg/search.html
--rw-rw-rw-   0        0        0     1114 2022-08-06 18:28:13.000000 badi_users-0.9.0/badi_utils/templates/svg/shield-protected.html
--rw-rw-rw-   0        0        0     1219 2022-08-06 18:28:13.000000 badi_users-0.9.0/badi_utils/templates/svg/shield-user.html
--rw-rw-rw-   0        0        0      451 2022-08-06 18:28:13.000000 badi_users-0.9.0/badi_utils/templates/svg/slide.html
--rw-rw-rw-   0        0        0     1587 2022-08-06 18:28:13.000000 badi_users-0.9.0/badi_utils/templates/svg/timer.html
--rw-rw-rw-   0        0        0     1043 2022-08-06 18:28:13.000000 badi_users-0.9.0/badi_utils/templates/svg/town.html
--rw-rw-rw-   0        0        0      804 2022-08-06 18:28:13.000000 badi_users-0.9.0/badi_utils/templates/svg/user.html
--rw-rw-rw-   0        0        0      936 2022-08-06 18:28:13.000000 badi_users-0.9.0/badi_utils/templates/svg/wallet.html
--rw-rw-rw-   0        0        0      933 2022-08-06 18:28:13.000000 badi_users-0.9.0/badi_utils/templates/svg/warning.html
--rw-rw-rw-   0        0        0       19 2022-09-27 11:24:17.000000 badi_users-0.9.0/badi_utils/templates/test.html
-drwxrwxrwx   0        0        0        0 2023-03-30 06:07:45.306835 badi_users-0.9.0/badi_utils/templatetags/
--rw-rw-rw-   0        0        0        0 2022-09-24 07:28:02.000000 badi_users-0.9.0/badi_utils/templatetags/__init__.py
--rw-rw-rw-   0        0        0      148 2022-09-27 11:23:20.000000 badi_users-0.9.0/badi_utils/templatetags/badi_utils.py
--rw-rw-rw-   0        0        0     7102 2023-02-16 09:10:01.000000 badi_users-0.9.0/badi_utils/utils.py
--rw-rw-rw-   0        0        0     1911 2022-09-26 05:21:35.000000 badi_users-0.9.0/badi_utils/validations.py
-drwxrwxrwx   0        0        0        0 2023-03-30 06:07:45.321795 badi_users-0.9.0/badi_visit/
--rw-rw-rw-   0        0        0        0 2022-08-14 04:14:27.000000 badi_users-0.9.0/badi_visit/__init__.py
--rw-rw-rw-   0        0        0      167 2022-11-10 16:59:20.000000 badi_users-0.9.0/badi_visit/admin.py
-drwxrwxrwx   0        0        0        0 2023-03-30 06:07:45.329773 badi_users-0.9.0/badi_visit/api/
--rw-rw-rw-   0        0        0        0 2022-10-24 15:37:24.000000 badi_users-0.9.0/badi_visit/api/__init__.py
--rw-rw-rw-   0        0        0     2871 2022-11-10 16:59:20.000000 badi_users-0.9.0/badi_visit/api/api.py
--rw-rw-rw-   0        0        0      208 2022-11-10 16:59:20.000000 badi_users-0.9.0/badi_visit/api/routers.py
--rw-rw-rw-   0        0        0      185 2022-11-10 16:59:20.000000 badi_users-0.9.0/badi_visit/apps.py
-drwxrwxrwx   0        0        0        0 2023-03-30 06:07:45.331771 badi_users-0.9.0/badi_visit/migrations/
--rw-rw-rw-   0        0        0        0 2022-08-14 04:14:27.000000 badi_users-0.9.0/badi_visit/migrations/__init__.py
--rw-rw-rw-   0        0        0     1614 2022-11-10 16:59:20.000000 badi_users-0.9.0/badi_visit/models.py
--rw-rw-rw-   0        0        0       63 2022-08-14 04:14:27.000000 badi_users-0.9.0/badi_visit/tests.py
-drwxrwxrwx   0        0        0        0 2023-03-30 06:07:45.362686 badi_users-0.9.0/badi_wallet/
--rw-rw-rw-   0        0        0        0 2023-03-27 19:00:31.000000 badi_users-0.9.0/badi_wallet/__init__.py
--rw-rw-rw-   0        0        0     8873 2023-03-27 19:00:31.000000 badi_users-0.9.0/badi_wallet/action.py
--rw-rw-rw-   0        0        0      202 2023-03-27 19:00:31.000000 badi_users-0.9.0/badi_wallet/admin.py
-drwxrwxrwx   0        0        0        0 2023-03-30 06:07:45.378646 badi_users-0.9.0/badi_wallet/api/
--rw-rw-rw-   0        0        0        0 2023-03-27 19:00:31.000000 badi_users-0.9.0/badi_wallet/api/__init__.py
--rw-rw-rw-   0        0        0      241 2023-03-27 19:00:31.000000 badi_users-0.9.0/badi_wallet/api/routers.py
--rw-rw-rw-   0        0        0      543 2023-03-27 19:00:31.000000 badi_users-0.9.0/badi_wallet/api/serializers.py
--rw-rw-rw-   0        0        0     8037 2023-03-29 08:19:18.000000 badi_users-0.9.0/badi_wallet/api/view_sets.py
--rw-rw-rw-   0        0        0      243 2023-03-27 19:00:31.000000 badi_users-0.9.0/badi_wallet/apps.py
--rw-rw-rw-   0        0        0      350 2023-03-28 19:16:55.000000 badi_users-0.9.0/badi_wallet/filter.py
-drwxrwxrwx   0        0        0        0 2023-03-30 06:07:42.934567 badi_users-0.9.0/badi_wallet/locale/
-drwxrwxrwx   0        0        0        0 2023-03-30 06:07:42.934567 badi_users-0.9.0/badi_wallet/locale/fa/
-drwxrwxrwx   0        0        0        0 2023-03-30 06:07:45.384630 badi_users-0.9.0/badi_wallet/locale/fa/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1633 2023-03-30 05:20:05.000000 badi_users-0.9.0/badi_wallet/locale/fa/LC_MESSAGES/django.mo
-drwxrwxrwx   0        0        0        0 2023-03-30 06:07:45.386622 badi_users-0.9.0/badi_wallet/migrations/
--rw-rw-rw-   0        0        0        0 2022-08-06 18:28:13.000000 badi_users-0.9.0/badi_wallet/migrations/__init__.py
--rw-rw-rw-   0        0        0     3146 2023-03-30 05:05:34.000000 badi_users-0.9.0/badi_wallet/models.py
-drwxrwxrwx   0        0        0        0 2023-03-30 06:07:45.386622 badi_users-0.9.0/badi_wallet/templates/
--rw-rw-rw-   0        0        0        0 2023-03-27 19:00:31.000000 badi_users-0.9.0/badi_wallet/templates/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-30 06:07:45.402579 badi_users-0.9.0/badi_wallet/templates/transaction/
--rw-rw-rw-   0        0        0     6145 2023-03-29 08:22:24.000000 badi_users-0.9.0/badi_wallet/templates/transaction/all_transaction_list.html
--rw-rw-rw-   0        0        0    10786 2023-03-30 06:06:40.000000 badi_users-0.9.0/badi_wallet/templates/transaction/all_transaction_report.html
--rw-rw-rw-   0        0        0     2251 2023-03-27 19:00:31.000000 badi_users-0.9.0/badi_wallet/templates/transaction/request-transaction.html
--rw-rw-rw-   0        0        0     6203 2023-03-29 08:22:11.000000 badi_users-0.9.0/badi_wallet/templates/transaction/transaction_list.html
--rw-rw-rw-   0        0        0     3547 2023-03-27 19:00:31.000000 badi_users-0.9.0/badi_wallet/templates/transaction/transaction_result.html
--rw-rw-rw-   0        0        0       63 2023-03-27 19:00:31.000000 badi_users-0.9.0/badi_wallet/tests.py
-drwxrwxrwx   0        0        0        0 2023-03-30 06:07:45.414549 badi_users-0.9.0/badi_wallet/ui/
--rw-rw-rw-   0        0        0        0 2023-03-27 19:00:31.000000 badi_users-0.9.0/badi_wallet/ui/__init__.py
--rw-rw-rw-   0        0        0      577 2023-03-28 19:11:37.000000 badi_users-0.9.0/badi_wallet/ui/urls.py
--rw-rw-rw-   0        0        0     1449 2023-03-28 19:16:42.000000 badi_users-0.9.0/badi_wallet/ui/views.py
--rw-rw-rw-   0        0        0       42 2023-03-30 06:07:45.416543 badi_users-0.9.0/setup.cfg
--rw-rw-rw-   0        0        0      498 2023-03-30 06:07:26.000000 badi_users-0.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 04:59:14.154015 badi_users-0.9.1/
+-rw-rw-rw-   0        0        0     1093 2022-09-24 06:05:13.000000 badi_users-0.9.1/LICENSE
+-rw-rw-rw-   0        0        0     1066 2022-11-10 17:03:20.000000 badi_users-0.9.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      419 2023-04-11 04:59:14.153019 badi_users-0.9.1/PKG-INFO
+-rw-rw-rw-   0        0        0      143 2022-10-02 09:04:41.000000 badi_users-0.9.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 04:59:13.208749 badi_users-0.9.1/badi_ticket/
+-rw-rw-rw-   0        0        0        0 2023-03-30 05:25:47.000000 badi_users-0.9.1/badi_ticket/__init__.py
+-rw-rw-rw-   0        0        0      143 2023-03-30 05:25:47.000000 badi_users-0.9.1/badi_ticket/admin.py
+-rw-rw-rw-   0        0        0     9834 2023-04-11 04:41:41.000000 badi_users-0.9.1/badi_ticket/api.py
+-rw-rw-rw-   0        0        0      129 2023-03-30 05:25:47.000000 badi_users-0.9.1/badi_ticket/apps.py
+drwxrwxrwx   0        0        0        0 2023-04-11 04:59:13.178108 badi_users-0.9.1/badi_ticket/locale/
+drwxrwxrwx   0        0        0        0 2023-04-11 04:59:13.178108 badi_users-0.9.1/badi_ticket/locale/fa/
+drwxrwxrwx   0        0        0        0 2023-04-11 04:59:13.209748 badi_users-0.9.1/badi_ticket/locale/fa/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     2415 2023-03-30 05:25:47.000000 badi_users-0.9.1/badi_ticket/locale/fa/LC_MESSAGES/django.mo
+drwxrwxrwx   0        0        0        0 2023-04-11 04:59:13.210744 badi_users-0.9.1/badi_ticket/migrations/
+-rw-rw-rw-   0        0        0        0 2022-08-06 18:28:13.000000 badi_users-0.9.1/badi_ticket/migrations/__init__.py
+-rw-rw-rw-   0        0        0     3022 2023-04-11 04:15:46.000000 badi_users-0.9.1/badi_ticket/models.py
+-rw-rw-rw-   0        0        0      313 2023-03-30 05:25:47.000000 badi_users-0.9.1/badi_ticket/routers.py
+-rw-rw-rw-   0        0        0     2082 2023-03-30 05:25:47.000000 badi_users-0.9.1/badi_ticket/serializers.py
+drwxrwxrwx   0        0        0        0 2023-04-11 04:59:13.179105 badi_users-0.9.1/badi_ticket/static/
+drwxrwxrwx   0        0        0        0 2023-04-11 04:59:13.180103 badi_users-0.9.1/badi_ticket/static/ticket/
+drwxrwxrwx   0        0        0        0 2023-04-11 04:59:13.211743 badi_users-0.9.1/badi_ticket/static/ticket/js/
+-rw-rw-rw-   0        0        0     2147 2023-03-30 05:25:47.000000 badi_users-0.9.1/badi_ticket/static/ticket/js/chat.js
+drwxrwxrwx   0        0        0        0 2023-04-11 04:59:13.212739 badi_users-0.9.1/badi_ticket/templates/
+-rw-rw-rw-   0        0        0        0 2023-03-30 05:25:47.000000 badi_users-0.9.1/badi_ticket/templates/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 04:59:13.216729 badi_users-0.9.1/badi_ticket/templates/ticket/
+-rw-rw-rw-   0        0        0     6358 2023-03-30 05:25:47.000000 badi_users-0.9.1/badi_ticket/templates/ticket/admin_tickets.html
+-rw-rw-rw-   0        0        0     5265 2023-03-30 05:25:47.000000 badi_users-0.9.1/badi_ticket/templates/ticket/message_list.html
+-rw-rw-rw-   0        0        0     9642 2023-03-30 05:25:47.000000 badi_users-0.9.1/badi_ticket/templates/ticket/my_tickets.html
+-rw-rw-rw-   0        0        0     8023 2023-04-11 04:53:00.000000 badi_users-0.9.1/badi_ticket/templates/ticket/ticket_create.html
+-rw-rw-rw-   0        0        0     1639 2023-03-30 05:25:47.000000 badi_users-0.9.1/badi_ticket/templates/ticket/ticket_update.html
+-rw-rw-rw-   0        0        0       63 2023-03-30 05:25:47.000000 badi_users-0.9.1/badi_ticket/tests.py
+-rw-rw-rw-   0        0        0      583 2023-03-30 05:25:47.000000 badi_users-0.9.1/badi_ticket/urls.py
+-rw-rw-rw-   0        0        0     2057 2023-04-11 04:56:26.000000 badi_users-0.9.1/badi_ticket/views.py
+drwxrwxrwx   0        0        0        0 2023-04-11 04:59:13.222757 badi_users-0.9.1/badi_user/
+-rw-rw-rw-   0        0        0        0 2023-03-27 19:00:31.000000 badi_users-0.9.1/badi_user/__init__.py
+-rw-rw-rw-   0        0        0      166 2023-03-27 19:00:31.000000 badi_users-0.9.1/badi_user/admin.py
+drwxrwxrwx   0        0        0        0 2023-04-11 04:59:13.225750 badi_users-0.9.1/badi_user/api/
+-rw-rw-rw-   0        0        0        0 2023-03-27 19:00:31.000000 badi_users-0.9.1/badi_user/api/__init__.py
+-rw-rw-rw-   0        0        0    29693 2023-03-27 19:00:31.000000 badi_users-0.9.1/badi_user/api/api.py
+-rw-rw-rw-   0        0        0      485 2023-03-27 19:00:31.000000 badi_users-0.9.1/badi_user/api/routers.py
+-rw-rw-rw-   0        0        0     6013 2023-03-27 19:00:31.000000 badi_users-0.9.1/badi_user/api/serializers.py
+-rw-rw-rw-   0        0        0      183 2023-03-27 19:00:31.000000 badi_users-0.9.1/badi_user/apps.py
+-rw-rw-rw-   0        0        0     3428 2023-03-27 19:00:31.000000 badi_users-0.9.1/badi_user/filter.py
+drwxrwxrwx   0        0        0        0 2023-04-11 04:59:13.181474 badi_users-0.9.1/badi_user/locale/
+drwxrwxrwx   0        0        0        0 2023-04-11 04:59:13.182471 badi_users-0.9.1/badi_user/locale/fa/
+drwxrwxrwx   0        0        0        0 2023-04-11 04:59:13.231734 badi_users-0.9.1/badi_user/locale/fa/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     3834 2023-03-30 05:20:05.000000 badi_users-0.9.1/badi_user/locale/fa/LC_MESSAGES/django.mo
+drwxrwxrwx   0        0        0        0 2023-04-11 04:59:13.232730 badi_users-0.9.1/badi_user/migrations/
+-rw-rw-rw-   0        0        0        0 2022-08-06 18:28:13.000000 badi_users-0.9.1/badi_user/migrations/__init__.py
+-rw-rw-rw-   0        0        0     6551 2023-03-27 19:00:31.000000 badi_users-0.9.1/badi_user/models.py
+drwxrwxrwx   0        0        0        0 2023-04-11 04:59:13.233727 badi_users-0.9.1/badi_user/templates/
+-rw-rw-rw-   0        0        0        0 2023-03-27 19:00:31.000000 badi_users-0.9.1/badi_user/templates/__init__.py
+-rw-rw-rw-   0        0        0       27 2023-03-27 19:00:31.000000 badi_users-0.9.1/badi_user/templates/badi-user-test.html
+drwxrwxrwx   0        0        0        0 2023-04-11 04:59:13.235723 badi_users-0.9.1/badi_user/templates/group/
+-rw-rw-rw-   0        0        0     8558 2023-03-27 19:00:31.000000 badi_users-0.9.1/badi_user/templates/group/group_create.html
+-rw-rw-rw-   0        0        0     5472 2023-03-27 19:00:31.000000 badi_users-0.9.1/badi_user/templates/group/group_update.html
+drwxrwxrwx   0        0        0        0 2023-04-11 04:59:13.236720 badi_users-0.9.1/badi_user/templates/log/
+-rw-rw-rw-   0        0        0     3987 2023-03-27 19:00:31.000000 badi_users-0.9.1/badi_user/templates/log/log_list.html
+drwxrwxrwx   0        0        0        0 2023-04-11 04:59:13.237717 badi_users-0.9.1/badi_user/templates/login-theme/
+-rw-rw-rw-   0        0        0     7336 2023-03-27 19:00:31.000000 badi_users-0.9.1/badi_user/templates/login-theme/login-1.html
+drwxrwxrwx   0        0        0        0 2023-04-11 04:59:13.240744 badi_users-0.9.1/badi_user/templates/member/
+-rw-rw-rw-   0        0        0     6863 2023-03-27 19:00:31.000000 badi_users-0.9.1/badi_user/templates/member/member_create.html
+-rw-rw-rw-   0        0        0    22635 2023-03-27 19:00:31.000000 badi_users-0.9.1/badi_user/templates/member/member_list.html
+-rw-rw-rw-   0        0        0     4783 2023-03-28 07:29:01.000000 badi_users-0.9.1/badi_user/templates/member/member_self_update.html
+-rw-rw-rw-   0        0        0     6525 2023-03-27 19:00:31.000000 badi_users-0.9.1/badi_user/templates/member/member_update.html
+drwxrwxrwx   0        0        0        0 2023-04-11 04:59:13.244423 badi_users-0.9.1/badi_user/templates/user/
+-rw-rw-rw-   0        0        0     6745 2023-03-27 19:00:31.000000 badi_users-0.9.1/badi_user/templates/user/change_password.html
+-rw-rw-rw-   0        0        0     5973 2023-03-27 19:00:31.000000 badi_users-0.9.1/badi_user/templates/user/user_create.html
+-rw-rw-rw-   0        0        0     4019 2023-03-27 19:00:31.000000 badi_users-0.9.1/badi_user/templates/user/user_list.html
+-rw-rw-rw-   0        0        0     5005 2023-03-27 19:00:31.000000 badi_users-0.9.1/badi_user/templates/user/user_update.html
+drwxrwxrwx   0        0        0        0 2023-04-11 04:59:13.246419 badi_users-0.9.1/badi_user/templatetags/
+-rw-rw-rw-   0        0        0        0 2023-03-27 19:00:31.000000 badi_users-0.9.1/badi_user/templatetags/__init__.py
+-rw-rw-rw-   0        0        0     5950 2023-03-27 19:00:31.000000 badi_users-0.9.1/badi_user/templatetags/appfilter.py
+-rw-rw-rw-   0        0        0      500 2023-03-27 19:00:31.000000 badi_users-0.9.1/badi_user/tests.py
+drwxrwxrwx   0        0        0        0 2023-04-11 04:59:13.253401 badi_users-0.9.1/badi_user/ui/
+-rw-rw-rw-   0        0        0        0 2023-03-27 19:00:31.000000 badi_users-0.9.1/badi_user/ui/__init__.py
+-rw-rw-rw-   0        0        0     1484 2023-03-27 19:00:31.000000 badi_users-0.9.1/badi_user/ui/forms.py
+-rw-rw-rw-   0        0        0      320 2023-03-27 19:00:31.000000 badi_users-0.9.1/badi_user/ui/log_views.py
+-rw-rw-rw-   0        0        0     1706 2023-03-28 08:00:41.000000 badi_users-0.9.1/badi_user/ui/member_views.py
+-rw-rw-rw-   0        0        0      672 2023-03-27 19:00:31.000000 badi_users-0.9.1/badi_user/ui/notification_views.py
+-rw-rw-rw-   0        0        0      644 2023-03-27 19:00:31.000000 badi_users-0.9.1/badi_user/ui/roles_views.py
+-rw-rw-rw-   0        0        0     1614 2023-03-27 19:00:31.000000 badi_users-0.9.1/badi_user/ui/urls.py
+-rw-rw-rw-   0        0        0     2633 2023-03-27 19:00:31.000000 badi_users-0.9.1/badi_user/ui/views.py
+drwxrwxrwx   0        0        0        0 2023-04-11 04:59:13.270388 badi_users-0.9.1/badi_users.egg-info/
+-rw-rw-rw-   0        0        0      419 2023-04-11 04:59:12.000000 badi_users-0.9.1/badi_users.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    10750 2023-04-11 04:59:13.000000 badi_users-0.9.1/badi_users.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 04:59:12.000000 badi_users-0.9.1/badi_users.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-04-11 04:59:12.000000 badi_users-0.9.1/badi_users.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-11 04:59:13.282323 badi_users-0.9.1/badi_utils/
+-rw-rw-rw-   0        0        0        0 2022-09-24 05:54:56.000000 badi_users-0.9.1/badi_utils/__init__.py
+-rw-rw-rw-   0        0        0     6835 2022-09-24 08:08:59.000000 badi_users-0.9.1/badi_utils/date_calc.py
+-rw-rw-rw-   0        0        0    28225 2023-01-30 19:13:21.000000 badi_users-0.9.1/badi_utils/dynamic.py
+-rw-rw-rw-   0        0        0    22478 2022-12-03 08:13:14.000000 badi_users-0.9.1/badi_utils/dynamic_api.py
+-rw-rw-rw-   0        0        0     3412 2022-10-29 14:49:57.000000 badi_users-0.9.1/badi_utils/dynamic_models.py
+-rw-rw-rw-   0        0        0     2990 2022-09-26 04:39:36.000000 badi_users-0.9.1/badi_utils/email.py
+-rw-rw-rw-   0        0        0      252 2022-09-26 05:16:38.000000 badi_users-0.9.1/badi_utils/errors.py
+-rw-rw-rw-   0        0        0     1509 2022-11-12 15:50:44.000000 badi_users-0.9.1/badi_utils/logging.py
+-rw-rw-rw-   0        0        0      947 2022-08-06 18:28:12.000000 badi_users-0.9.1/badi_utils/responses.py
+-rw-rw-rw-   0        0        0      904 2023-02-06 12:51:34.000000 badi_users-0.9.1/badi_utils/rss.py
+-rw-rw-rw-   0        0        0     1529 2022-09-24 12:31:48.000000 badi_users-0.9.1/badi_utils/select2.py
+-rw-rw-rw-   0        0        0     2132 2023-03-27 18:55:33.000000 badi_users-0.9.1/badi_utils/sms.py
+drwxrwxrwx   0        0        0        0 2023-04-11 04:59:13.186256 badi_users-0.9.1/badi_utils/static/
+drwxrwxrwx   0        0        0        0 2023-04-11 04:59:13.187252 badi_users-0.9.1/badi_utils/static/badi_utils/
+drwxrwxrwx   0        0        0        0 2023-04-11 04:59:13.288338 badi_users-0.9.1/badi_utils/static/badi_utils/css/
+-rw-rw-rw-   0        0        0    40504 2023-01-30 18:56:15.000000 badi_users-0.9.1/badi_utils/static/badi_utils/css/custom.css
+drwxrwxrwx   0        0        0        0 2023-04-11 04:59:13.774756 badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/
+-rw-rw-rw-   0        0        0    59778 2022-08-14 04:14:25.000000 badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum).eot
+-rw-rw-rw-   0        0        0    59532 2022-08-14 04:14:25.000000 badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum).ttf
+-rw-rw-rw-   0        0        0    38401 2022-08-14 04:14:25.000000 badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum).woff
+-rw-rw-rw-   0        0        0    31304 2022-08-14 04:14:25.000000 badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum).woff2
+-rw-rw-rw-   0        0        0    59778 2022-08-14 04:14:25.000000 badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_2.eot
+-rw-rw-rw-   0        0        0    31992 2022-08-14 04:14:25.000000 badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold.eot
+-rw-rw-rw-   0        0        0    57268 2022-08-14 04:14:26.000000 badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold.ttf
+-rw-rw-rw-   0        0        0    36069 2022-08-14 04:14:26.000000 badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold.woff
+-rw-rw-rw-   0        0        0    28856 2022-08-14 04:14:26.000000 badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold.woff2
+-rw-rw-rw-   0        0        0    31992 2022-08-14 04:14:26.000000 badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold_2.eot
+-rw-rw-rw-   0        0        0    35477 2022-08-14 04:14:26.000000 badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light.eot
+-rw-rw-rw-   0        0        0    60584 2022-08-14 04:14:26.000000 badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light.ttf
+-rw-rw-rw-   0        0        0    39557 2022-08-14 04:14:26.000000 badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light.woff
+-rw-rw-rw-   0        0        0    32344 2022-08-14 04:14:26.000000 badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light.woff2
+-rw-rw-rw-   0        0        0    35477 2022-08-14 04:14:26.000000 badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light_2.eot
+-rw-rw-rw-   0        0        0    32043 2022-08-14 04:14:26.000000 badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium.eot
+-rw-rw-rw-   0        0        0    58192 2022-08-14 04:14:26.000000 badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium.ttf
+-rw-rw-rw-   0        0        0    36145 2022-08-14 04:14:26.000000 badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium.woff
+-rw-rw-rw-   0        0        0    28912 2022-08-14 04:14:26.000000 badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium.woff2
+-rw-rw-rw-   0        0        0    32043 2022-08-14 04:14:26.000000 badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium_2.eot
+-rw-rw-rw-   0        0        0    33102 2022-08-14 04:14:26.000000 badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight.eot
+-rw-rw-rw-   0        0        0    56352 2022-08-14 04:14:26.000000 badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight.ttf
+-rw-rw-rw-   0        0        0    36913 2022-08-14 04:14:26.000000 badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight.woff
+-rw-rw-rw-   0        0        0    30072 2022-08-14 04:14:26.000000 badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight.woff2
+-rw-rw-rw-   0        0        0    33102 2022-08-14 04:14:26.000000 badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight_2.eot
+-rw-rw-rw-   0        0        0    58886 2022-08-14 04:14:26.000000 badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb.eot
+-rw-rw-rw-   0        0        0    38473 2022-08-14 04:14:26.000000 badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb.woff
+-rw-rw-rw-   0        0        0    31320 2022-08-14 04:14:26.000000 badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb.woff2
+-rw-rw-rw-   0        0        0    58886 2022-08-14 04:14:26.000000 badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_2.eot
+-rw-rw-rw-   0        0        0    57974 2022-08-14 04:14:26.000000 badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold.eot
+-rw-rw-rw-   0        0        0    57760 2022-08-14 04:14:26.000000 badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold.ttf
+-rw-rw-rw-   0        0        0    36629 2022-08-14 04:14:26.000000 badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold.woff
+-rw-rw-rw-   0        0        0    29688 2022-08-14 04:14:26.000000 badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold.woff2
+-rw-rw-rw-   0        0        0    57974 2022-08-14 04:14:26.000000 badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold_2.eot
+-rw-rw-rw-   0        0        0    57974 2022-08-14 04:14:26.000000 badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold_3.eot
+-rw-rw-rw-   0        0        0    35458 2022-08-14 04:14:26.000000 badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light.eot
+-rw-rw-rw-   0        0        0    59968 2022-08-14 04:14:26.000000 badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light.ttf
+-rw-rw-rw-   0        0        0    39693 2022-08-14 04:14:26.000000 badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light.woff
+-rw-rw-rw-   0        0        0    32420 2022-08-14 04:14:26.000000 badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light.woff2
+-rw-rw-rw-   0        0        0    35458 2022-08-14 04:14:26.000000 badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light_2.eot
+-rw-rw-rw-   0        0        0    31983 2022-08-14 04:14:26.000000 badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium.eot
+-rw-rw-rw-   0        0        0    57544 2022-08-14 04:14:26.000000 badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium.ttf
+-rw-rw-rw-   0        0        0    36141 2022-08-14 04:14:26.000000 badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium.woff
+-rw-rw-rw-   0        0        0    28916 2022-08-14 04:14:26.000000 badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium.woff2
+-rw-rw-rw-   0        0        0    31983 2022-08-14 04:14:26.000000 badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium_2.eot
+-rw-rw-rw-   0        0        0    33044 2022-08-14 04:14:26.000000 badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight.eot
+-rw-rw-rw-   0        0        0    55640 2022-08-14 04:14:26.000000 badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight.ttf
+-rw-rw-rw-   0        0        0    36945 2022-08-14 04:14:26.000000 badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight.woff
+-rw-rw-rw-   0        0        0    29840 2022-08-14 04:14:26.000000 badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight.woff2
+-rw-rw-rw-   0        0        0    33044 2022-08-14 04:14:26.000000 badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight_2.eot
+-rw-rw-rw-   0        0        0    93376 2022-08-14 04:14:26.000000 badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/Ray-Black.ttf
+-rw-rw-rw-   0        0        0    94304 2022-08-14 04:14:26.000000 badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/Ray-Bold.ttf
+-rw-rw-rw-   0        0        0    94740 2022-08-14 04:14:26.000000 badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/Ray.ttf
+drwxrwxrwx   0        0        0        0 2023-04-11 04:59:14.030940 badi_users-0.9.1/badi_utils/static/badi_utils/js/
+-rw-rw-rw-   0        0        0   478686 2023-01-03 13:51:41.000000 badi_users-0.9.1/badi_utils/static/badi_utils/js/apexchart.js
+-rw-rw-rw-   0        0        0    19110 2022-08-14 04:14:25.000000 badi_users-0.9.1/badi_utils/static/badi_utils/js/api-login.js
+-rw-rw-rw-   0        0        0    20445 2022-12-01 13:15:11.000000 badi_users-0.9.1/badi_utils/static/badi_utils/js/api.js
+-rw-rw-rw-   0        0        0    25944 2023-03-29 06:15:03.000000 badi_users-0.9.1/badi_utils/static/badi_utils/js/base.js
+-rw-rw-rw-   0        0        0     2149 2022-08-14 04:14:25.000000 badi_users-0.9.1/badi_utils/static/badi_utils/js/chat.js
+-rw-rw-rw-   0        0        0     3167 2022-08-14 04:14:25.000000 badi_users-0.9.1/badi_utils/static/badi_utils/js/custom-vue.js
+-rw-rw-rw-   0        0        0    18560 2023-03-27 14:51:58.000000 badi_users-0.9.1/badi_utils/static/badi_utils/js/datatable.js
+-rw-rw-rw-   0        0        0     2470 2022-08-15 18:25:55.000000 badi_users-0.9.1/badi_utils/static/badi_utils/js/image-field.js
+-rw-rw-rw-   0        0        0    30541 2023-03-29 06:13:24.000000 badi_users-0.9.1/badi_utils/static/badi_utils/js/main.js
+-rw-rw-rw-   0        0        0      959 2022-08-14 04:14:26.000000 badi_users-0.9.1/badi_utils/static/badi_utils/js/notification.js
+-rw-rw-rw-   0        0        0     2213 2022-08-14 04:14:26.000000 badi_users-0.9.1/badi_utils/static/badi_utils/js/pagination-vue.js
+-rw-rw-rw-   0        0        0    20317 2023-03-30 04:45:54.000000 badi_users-0.9.1/badi_utils/static/badi_utils/js/tableexport.js
+-rw-rw-rw-   0        0        0      654 2022-08-14 04:14:26.000000 badi_users-0.9.1/badi_utils/static/badi_utils/js/transaction.js
+-rw-rw-rw-   0        0        0   354110 2022-08-14 04:14:26.000000 badi_users-0.9.1/badi_utils/static/badi_utils/js/vue.js
+-rw-rw-rw-   0        0        0   268386 2023-03-30 05:07:06.000000 badi_users-0.9.1/badi_utils/static/badi_utils/js/xlsx.mini.min.js
+drwxrwxrwx   0        0        0        0 2023-04-11 04:59:14.033838 badi_users-0.9.1/badi_utils/templates/
+-rw-rw-rw-   0        0        0        0 2022-09-24 07:28:02.000000 badi_users-0.9.1/badi_utils/templates/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 04:59:14.057274 badi_users-0.9.1/badi_utils/templates/component/
+-rw-rw-rw-   0        0        0     1777 2022-10-25 06:27:38.000000 badi_users-0.9.1/badi_utils/templates/component/createModal.html
+-rw-rw-rw-   0        0        0     1645 2022-08-14 04:14:27.000000 badi_users-0.9.1/badi_utils/templates/component/createTitle.html
+-rw-rw-rw-   0        0        0     1054 2022-08-14 04:14:27.000000 badi_users-0.9.1/badi_utils/templates/component/filter-form.html
+-rw-rw-rw-   0        0        0      729 2022-08-14 04:14:27.000000 badi_users-0.9.1/badi_utils/templates/component/form-errors.html
+-rw-rw-rw-   0        0        0     1340 2022-08-14 04:14:27.000000 badi_users-0.9.1/badi_utils/templates/component/form-progressbar-js.html
+-rw-rw-rw-   0        0        0      491 2022-08-14 04:14:27.000000 badi_users-0.9.1/badi_utils/templates/component/form-progressbar.html
+-rw-rw-rw-   0        0        0      342 2022-08-14 04:14:27.000000 badi_users-0.9.1/badi_utils/templates/component/form.html
+-rw-rw-rw-   0        0        0     1231 2022-08-14 04:14:27.000000 badi_users-0.9.1/badi_utils/templates/component/image-field.html
+-rw-rw-rw-   0        0        0    34439 2022-08-14 04:14:27.000000 badi_users-0.9.1/badi_utils/templates/component/index-menu.html
+-rw-rw-rw-   0        0        0     2346 2022-08-14 04:14:27.000000 badi_users-0.9.1/badi_utils/templates/component/input.html
+-rw-rw-rw-   0        0        0       69 2022-08-14 04:14:27.000000 badi_users-0.9.1/badi_utils/templates/component/loader.html
+-rw-rw-rw-   0        0        0      468 2022-10-02 09:59:19.000000 badi_users-0.9.1/badi_utils/templates/component/menu-item.html
+-rw-rw-rw-   0        0        0      362 2022-10-02 09:59:19.000000 badi_users-0.9.1/badi_utils/templates/component/menu-list.html
+-rw-rw-rw-   0        0        0      746 2022-08-14 04:14:27.000000 badi_users-0.9.1/badi_utils/templates/component/messages.html
+-rw-rw-rw-   0        0        0     1134 2022-12-31 05:14:56.000000 badi_users-0.9.1/badi_utils/templates/component/pagination-vue.html
+-rw-rw-rw-   0        0        0      361 2022-08-14 04:14:27.000000 badi_users-0.9.1/badi_utils/templates/component/profile_item.html
+-rw-rw-rw-   0        0        0      204 2022-08-14 04:14:27.000000 badi_users-0.9.1/badi_utils/templates/component/space-between.html
+-rw-rw-rw-   0        0        0      430 2022-10-02 09:59:19.000000 badi_users-0.9.1/badi_utils/templates/component/svg-button-with-text.html
+-rw-rw-rw-   0        0        0      428 2022-10-02 09:59:19.000000 badi_users-0.9.1/badi_utils/templates/component/svg-button.html
+-rw-rw-rw-   0        0        0     1411 2022-08-14 04:14:27.000000 badi_users-0.9.1/badi_utils/templates/component/table-item.html
+-rw-rw-rw-   0        0        0     2114 2022-08-14 04:14:27.000000 badi_users-0.9.1/badi_utils/templates/component/user-card.html
+-rw-rw-rw-   0        0        0      257 2022-08-14 04:14:27.000000 badi_users-0.9.1/badi_utils/templates/component/yesno.html
+drwxrwxrwx   0        0        0        0 2023-04-11 04:59:14.118111 badi_users-0.9.1/badi_utils/templates/svg/
+-rw-rw-rw-   0        0        0     1949 2022-08-06 18:28:13.000000 badi_users-0.9.1/badi_utils/templates/svg/Incoming-box.html
+-rw-rw-rw-   0        0        0     1159 2022-08-06 18:28:13.000000 badi_users-0.9.1/badi_utils/templates/svg/add-user.html
+-rw-rw-rw-   0        0        0     1092 2022-08-06 18:28:13.000000 badi_users-0.9.1/badi_utils/templates/svg/address-book.html
+-rw-rw-rw-   0        0        0     1095 2022-08-06 18:28:13.000000 badi_users-0.9.1/badi_utils/templates/svg/arrow-left.html
+-rw-rw-rw-   0        0        0     1081 2022-08-06 18:28:13.000000 badi_users-0.9.1/badi_utils/templates/svg/arrow-right.html
+-rw-rw-rw-   0        0        0     2024 2022-08-14 04:14:27.000000 badi_users-0.9.1/badi_utils/templates/svg/bitcoin.html
+-rw-rw-rw-   0        0        0      697 2022-08-06 18:28:13.000000 badi_users-0.9.1/badi_utils/templates/svg/box.html
+-rw-rw-rw-   0        0        0     1378 2022-08-06 18:28:13.000000 badi_users-0.9.1/badi_utils/templates/svg/calendar-day.html
+-rw-rw-rw-   0        0        0     1489 2022-08-06 18:28:13.000000 badi_users-0.9.1/badi_utils/templates/svg/calendar-gym.html
+-rw-rw-rw-   0        0        0      925 2022-08-06 18:28:13.000000 badi_users-0.9.1/badi_utils/templates/svg/calendar.html
+-rw-rw-rw-   0        0        0     1223 2022-12-01 08:20:56.000000 badi_users-0.9.1/badi_utils/templates/svg/call.html
+-rw-rw-rw-   0        0        0     1385 2022-08-06 18:28:13.000000 badi_users-0.9.1/badi_utils/templates/svg/category.html
+-rw-rw-rw-   0        0        0     1270 2022-08-14 04:14:27.000000 badi_users-0.9.1/badi_utils/templates/svg/chat.html
+-rw-rw-rw-   0        0        0      938 2022-08-06 18:28:13.000000 badi_users-0.9.1/badi_utils/templates/svg/check.html
+-rw-rw-rw-   0        0        0      344 2022-08-06 18:28:13.000000 badi_users-0.9.1/badi_utils/templates/svg/circle.html
+-rw-rw-rw-   0        0        0     1686 2022-08-06 18:28:13.000000 badi_users-0.9.1/badi_utils/templates/svg/city.html
+-rw-rw-rw-   0        0        0     1430 2022-08-06 18:28:13.000000 badi_users-0.9.1/badi_utils/templates/svg/clipboard-list.html
+-rw-rw-rw-   0        0        0     2247 2022-08-06 18:28:13.000000 badi_users-0.9.1/badi_utils/templates/svg/clock.html
+-rw-rw-rw-   0        0        0      645 2022-08-06 18:28:13.000000 badi_users-0.9.1/badi_utils/templates/svg/close.html
+-rw-rw-rw-   0        0        0     2483 2022-08-06 18:28:13.000000 badi_users-0.9.1/badi_utils/templates/svg/collection.html
+-rw-rw-rw-   0        0        0     1046 2022-08-14 04:14:27.000000 badi_users-0.9.1/badi_utils/templates/svg/comment.html
+-rw-rw-rw-   0        0        0     1103 2022-08-06 18:28:13.000000 badi_users-0.9.1/badi_utils/templates/svg/dashboard.html
+-rw-rw-rw-   0        0        0      893 2022-08-06 18:28:13.000000 badi_users-0.9.1/badi_utils/templates/svg/delete.html
+-rw-rw-rw-   0        0        0     1505 2022-08-06 18:28:13.000000 badi_users-0.9.1/badi_utils/templates/svg/download.html
+-rw-rw-rw-   0        0        0      901 2022-08-06 18:28:13.000000 badi_users-0.9.1/badi_utils/templates/svg/edit.html
+-rw-rw-rw-   0        0        0     1361 2022-08-06 18:28:13.000000 badi_users-0.9.1/badi_utils/templates/svg/file-check.html
+-rw-rw-rw-   0        0        0      988 2022-08-06 18:28:13.000000 badi_users-0.9.1/badi_utils/templates/svg/file.html
+-rw-rw-rw-   0        0        0     2111 2022-08-06 18:28:13.000000 badi_users-0.9.1/badi_utils/templates/svg/film.html
+-rw-rw-rw-   0        0        0      681 2022-08-14 04:14:27.000000 badi_users-0.9.1/badi_utils/templates/svg/fire.html
+-rw-rw-rw-   0        0        0     1648 2022-08-06 18:28:13.000000 badi_users-0.9.1/badi_utils/templates/svg/group-chat.html
+-rw-rw-rw-   0        0        0     1213 2022-08-06 18:28:13.000000 badi_users-0.9.1/badi_utils/templates/svg/group.html
+-rw-rw-rw-   0        0        0     1394 2022-08-14 04:14:27.000000 badi_users-0.9.1/badi_utils/templates/svg/half_star.html
+-rw-rw-rw-   0        0        0      944 2022-08-06 18:28:13.000000 badi_users-0.9.1/badi_utils/templates/svg/home.html
+-rw-rw-rw-   0        0        0     1906 2022-08-14 04:14:27.000000 badi_users-0.9.1/badi_utils/templates/svg/hourse.html
+-rw-rw-rw-   0        0        0      631 2022-08-06 18:28:13.000000 badi_users-0.9.1/badi_utils/templates/svg/image.html
+-rw-rw-rw-   0        0        0      508 2022-08-06 18:28:13.000000 badi_users-0.9.1/badi_utils/templates/svg/info.html
+-rw-rw-rw-   0        0        0     1394 2022-08-06 18:28:13.000000 badi_users-0.9.1/badi_utils/templates/svg/interview.html
+-rw-rw-rw-   0        0        0     1389 2022-08-06 18:28:13.000000 badi_users-0.9.1/badi_utils/templates/svg/key.html
+-rw-rw-rw-   0        0        0     2472 2022-08-06 18:28:13.000000 badi_users-0.9.1/badi_utils/templates/svg/logout.html
+-rw-rw-rw-   0        0        0      940 2022-08-14 04:14:27.000000 badi_users-0.9.1/badi_utils/templates/svg/mail.html
+-rw-rw-rw-   0        0        0      731 2022-08-06 18:28:13.000000 badi_users-0.9.1/badi_utils/templates/svg/map.html
+-rw-rw-rw-   0        0        0     1601 2022-08-06 18:28:13.000000 badi_users-0.9.1/badi_utils/templates/svg/message.html
+-rw-rw-rw-   0        0        0     1607 2022-08-06 18:28:13.000000 badi_users-0.9.1/badi_utils/templates/svg/messages.html
+-rw-rw-rw-   0        0        0      683 2022-08-14 04:14:27.000000 badi_users-0.9.1/badi_utils/templates/svg/notification.html
+-rw-rw-rw-   0        0        0      708 2022-08-06 18:28:13.000000 badi_users-0.9.1/badi_utils/templates/svg/plus.html
+-rw-rw-rw-   0        0        0      753 2022-08-14 04:14:27.000000 badi_users-0.9.1/badi_utils/templates/svg/puzzle.html
+-rw-rw-rw-   0        0        0      882 2022-08-14 04:14:27.000000 badi_users-0.9.1/badi_utils/templates/svg/question.html
+-rw-rw-rw-   0        0        0     1174 2022-08-06 18:28:13.000000 badi_users-0.9.1/badi_utils/templates/svg/refresh.html
+-rw-rw-rw-   0        0        0     1416 2022-08-06 18:28:13.000000 badi_users-0.9.1/badi_utils/templates/svg/safe.html
+-rw-rw-rw-   0        0        0     1091 2022-09-21 07:25:46.000000 badi_users-0.9.1/badi_utils/templates/svg/search.html
+-rw-rw-rw-   0        0        0     1114 2022-08-06 18:28:13.000000 badi_users-0.9.1/badi_utils/templates/svg/shield-protected.html
+-rw-rw-rw-   0        0        0     1219 2022-08-06 18:28:13.000000 badi_users-0.9.1/badi_utils/templates/svg/shield-user.html
+-rw-rw-rw-   0        0        0      451 2022-08-06 18:28:13.000000 badi_users-0.9.1/badi_utils/templates/svg/slide.html
+-rw-rw-rw-   0        0        0     1587 2022-08-06 18:28:13.000000 badi_users-0.9.1/badi_utils/templates/svg/timer.html
+-rw-rw-rw-   0        0        0     1043 2022-08-06 18:28:13.000000 badi_users-0.9.1/badi_utils/templates/svg/town.html
+-rw-rw-rw-   0        0        0      804 2022-08-06 18:28:13.000000 badi_users-0.9.1/badi_utils/templates/svg/user.html
+-rw-rw-rw-   0        0        0      936 2022-08-06 18:28:13.000000 badi_users-0.9.1/badi_utils/templates/svg/wallet.html
+-rw-rw-rw-   0        0        0      933 2022-08-06 18:28:13.000000 badi_users-0.9.1/badi_utils/templates/svg/warning.html
+-rw-rw-rw-   0        0        0       19 2022-09-27 11:24:17.000000 badi_users-0.9.1/badi_utils/templates/test.html
+drwxrwxrwx   0        0        0        0 2023-04-11 04:59:14.119108 badi_users-0.9.1/badi_utils/templatetags/
+-rw-rw-rw-   0        0        0        0 2022-09-24 07:28:02.000000 badi_users-0.9.1/badi_utils/templatetags/__init__.py
+-rw-rw-rw-   0        0        0      148 2022-09-27 11:23:20.000000 badi_users-0.9.1/badi_utils/templatetags/badi_utils.py
+-rw-rw-rw-   0        0        0     7102 2023-02-16 09:10:01.000000 badi_users-0.9.1/badi_utils/utils.py
+-rw-rw-rw-   0        0        0     1911 2022-09-26 05:21:35.000000 badi_users-0.9.1/badi_utils/validations.py
+drwxrwxrwx   0        0        0        0 2023-04-11 04:59:14.125094 badi_users-0.9.1/badi_visit/
+-rw-rw-rw-   0        0        0        0 2022-08-14 04:14:27.000000 badi_users-0.9.1/badi_visit/__init__.py
+-rw-rw-rw-   0        0        0      167 2022-11-10 16:59:20.000000 badi_users-0.9.1/badi_visit/admin.py
+drwxrwxrwx   0        0        0        0 2023-04-11 04:59:14.128085 badi_users-0.9.1/badi_visit/api/
+-rw-rw-rw-   0        0        0        0 2022-10-24 15:37:24.000000 badi_users-0.9.1/badi_visit/api/__init__.py
+-rw-rw-rw-   0        0        0     2871 2022-11-10 16:59:20.000000 badi_users-0.9.1/badi_visit/api/api.py
+-rw-rw-rw-   0        0        0      208 2022-11-10 16:59:20.000000 badi_users-0.9.1/badi_visit/api/routers.py
+-rw-rw-rw-   0        0        0      185 2022-11-10 16:59:20.000000 badi_users-0.9.1/badi_visit/apps.py
+drwxrwxrwx   0        0        0        0 2023-04-11 04:59:14.129082 badi_users-0.9.1/badi_visit/migrations/
+-rw-rw-rw-   0        0        0        0 2022-08-14 04:14:27.000000 badi_users-0.9.1/badi_visit/migrations/__init__.py
+-rw-rw-rw-   0        0        0     1614 2022-11-10 16:59:20.000000 badi_users-0.9.1/badi_visit/models.py
+-rw-rw-rw-   0        0        0       63 2022-08-14 04:14:27.000000 badi_users-0.9.1/badi_visit/tests.py
+drwxrwxrwx   0        0        0        0 2023-04-11 04:59:14.137062 badi_users-0.9.1/badi_wallet/
+-rw-rw-rw-   0        0        0        0 2023-03-27 19:00:31.000000 badi_users-0.9.1/badi_wallet/__init__.py
+-rw-rw-rw-   0        0        0     8873 2023-03-27 19:00:31.000000 badi_users-0.9.1/badi_wallet/action.py
+-rw-rw-rw-   0        0        0      202 2023-03-27 19:00:31.000000 badi_users-0.9.1/badi_wallet/admin.py
+drwxrwxrwx   0        0        0        0 2023-04-11 04:59:14.141050 badi_users-0.9.1/badi_wallet/api/
+-rw-rw-rw-   0        0        0        0 2023-03-27 19:00:31.000000 badi_users-0.9.1/badi_wallet/api/__init__.py
+-rw-rw-rw-   0        0        0      241 2023-03-27 19:00:31.000000 badi_users-0.9.1/badi_wallet/api/routers.py
+-rw-rw-rw-   0        0        0      543 2023-03-27 19:00:31.000000 badi_users-0.9.1/badi_wallet/api/serializers.py
+-rw-rw-rw-   0        0        0     8037 2023-03-29 08:19:18.000000 badi_users-0.9.1/badi_wallet/api/view_sets.py
+-rw-rw-rw-   0        0        0      243 2023-03-27 19:00:31.000000 badi_users-0.9.1/badi_wallet/apps.py
+-rw-rw-rw-   0        0        0      350 2023-03-28 19:16:55.000000 badi_users-0.9.1/badi_wallet/filter.py
+drwxrwxrwx   0        0        0        0 2023-04-11 04:59:13.191527 badi_users-0.9.1/badi_wallet/locale/
+drwxrwxrwx   0        0        0        0 2023-04-11 04:59:13.191527 badi_users-0.9.1/badi_wallet/locale/fa/
+drwxrwxrwx   0        0        0        0 2023-04-11 04:59:14.143077 badi_users-0.9.1/badi_wallet/locale/fa/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     1633 2023-03-30 05:20:05.000000 badi_users-0.9.1/badi_wallet/locale/fa/LC_MESSAGES/django.mo
+drwxrwxrwx   0        0        0        0 2023-04-11 04:59:14.144041 badi_users-0.9.1/badi_wallet/migrations/
+-rw-rw-rw-   0        0        0        0 2022-08-06 18:28:13.000000 badi_users-0.9.1/badi_wallet/migrations/__init__.py
+-rw-rw-rw-   0        0        0     3146 2023-03-30 05:05:34.000000 badi_users-0.9.1/badi_wallet/models.py
+drwxrwxrwx   0        0        0        0 2023-04-11 04:59:14.145039 badi_users-0.9.1/badi_wallet/templates/
+-rw-rw-rw-   0        0        0        0 2023-03-27 19:00:31.000000 badi_users-0.9.1/badi_wallet/templates/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 04:59:14.149029 badi_users-0.9.1/badi_wallet/templates/transaction/
+-rw-rw-rw-   0        0        0     6145 2023-03-29 08:22:24.000000 badi_users-0.9.1/badi_wallet/templates/transaction/all_transaction_list.html
+-rw-rw-rw-   0        0        0    10786 2023-03-30 06:06:40.000000 badi_users-0.9.1/badi_wallet/templates/transaction/all_transaction_report.html
+-rw-rw-rw-   0        0        0     2251 2023-03-27 19:00:31.000000 badi_users-0.9.1/badi_wallet/templates/transaction/request-transaction.html
+-rw-rw-rw-   0        0        0     6203 2023-03-29 08:22:11.000000 badi_users-0.9.1/badi_wallet/templates/transaction/transaction_list.html
+-rw-rw-rw-   0        0        0     3547 2023-03-27 19:00:31.000000 badi_users-0.9.1/badi_wallet/templates/transaction/transaction_result.html
+-rw-rw-rw-   0        0        0       63 2023-03-27 19:00:31.000000 badi_users-0.9.1/badi_wallet/tests.py
+drwxrwxrwx   0        0        0        0 2023-04-11 04:59:14.152022 badi_users-0.9.1/badi_wallet/ui/
+-rw-rw-rw-   0        0        0        0 2023-03-27 19:00:31.000000 badi_users-0.9.1/badi_wallet/ui/__init__.py
+-rw-rw-rw-   0        0        0      577 2023-03-28 19:11:37.000000 badi_users-0.9.1/badi_wallet/ui/urls.py
+-rw-rw-rw-   0        0        0     1449 2023-03-28 19:16:42.000000 badi_users-0.9.1/badi_wallet/ui/views.py
+-rw-rw-rw-   0        0        0       42 2023-04-11 04:59:14.154015 badi_users-0.9.1/setup.cfg
+-rw-rw-rw-   0        0        0      498 2023-04-11 04:58:51.000000 badi_users-0.9.1/setup.py
```

### Comparing `badi_users-0.9.0/LICENSE` & `badi_users-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/MANIFEST.in` & `badi_users-0.9.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_ticket/api.py` & `badi_users-0.9.1/badi_ticket/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,30 +37,38 @@
         count += 1
 
     BADI_AUTH_CONFIG.get('sms').get('sms_panel').board_send(users, message_text)
     return count
 
 
 class TicketViewSet(DynamicModelApi):
-    columns = ['id', 'writer', 'title', 'created_at', 'is_closed', ]
-    order_columns = ['id', 'writer', 'title', 'created_at', 'is_closed', ]
+    columns = ['id', 'writer', 'title', 'is_closed', 'created_at', ]
+    order_columns = ['id', 'writer', 'title', 'is_closed', 'created_at', ]
     model = Ticket
     queryset = Ticket.objects.all()
     serializer_class = TicketCreateSerializer
     custom_perms = {
         'datatable': True,
+        'create': True,
     }
 
     def render_column(self, row, column):
-        if column == 'title':
+        if column == 'is_closed':
             if self.request.user.is_admin:
                 count = row.messages.filter(is_seen_by_admin=False).count()
             else:
                 count = row.messages.filter(is_seen=False).count()
-            return '{0} ({1} {2})'.format(row.title, count, _("New message")) if count else row.title
+            first = row.messages.all().order_by('-pk').first()
+            last_message = -1
+            if first:
+                if first.writer.is_admin and self.request.user.is_admin:
+                    last_message = 0
+                else:
+                    last_message = 1
+            return [row.is_closed, count, last_message]
         return super().render_column(row, column)
 
     def filter_queryset(self, qs):
         if self.request.user.is_member():
             return Ticket.objects.filter(writer=self.request.user)
         return super().filter_queryset(qs)
```

### Comparing `badi_users-0.9.0/badi_ticket/locale/fa/LC_MESSAGES/django.mo` & `badi_users-0.9.1/badi_ticket/locale/fa/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_ticket/models.py` & `badi_users-0.9.1/badi_ticket/models.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -22,16 +22,16 @@
         permissions = (
             ('can_ticket', _('Manage Tickets')),
         )
 
     writer = models.ForeignKey(User, null=True, related_name='tickets', on_delete=models.CASCADE,
                                verbose_name=_('Member'))
     title = models.CharField(max_length=255, verbose_name=_('Title'))
-    created_at = models.DateTimeField(auto_now_add=True, blank=True, verbose_name=_("Created at"))
     is_closed = models.BooleanField(default=False, verbose_name=_('is Closed'))
+    created_at = models.DateTimeField(auto_now_add=True, blank=True, verbose_name=_("Created at"))
 
     def __str__(self):
         return self.title + ' (' + self.writer.__str__() + ')'
 
     def unread_messages(self, user):
         if user.is_admin:
             return self.messages.filter(is_seen_by_admin=False)
```

### Comparing `badi_users-0.9.0/badi_ticket/serializers.py` & `badi_users-0.9.1/badi_ticket/serializers.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_ticket/static/ticket/js/chat.js` & `badi_users-0.9.1/badi_ticket/static/ticket/js/chat.js`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_ticket/templates/ticket/admin_tickets.html` & `badi_users-0.9.1/badi_ticket/templates/ticket/admin_tickets.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_ticket/templates/ticket/message_list.html` & `badi_users-0.9.1/badi_ticket/templates/ticket/message_list.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_ticket/templates/ticket/my_tickets.html` & `badi_users-0.9.1/badi_ticket/templates/ticket/my_tickets.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_ticket/templates/ticket/ticket_create.html` & `badi_users-0.9.1/badi_ticket/templates/ticket/ticket_create.html`

 * *Files 7% similar despite different names*

```diff
@@ -37,30 +37,30 @@
 												<label class="d-none">
 													<input type="hidden" value="{{ object.writer }}" name="writer">
 												</label>
 												{% if request.user.is_admin %}
 												{{form.writer}}
 												{% endif %}
 											</div>
-											<div class="card-footer">
-												<button type="button" class="btn btn-light-primary font-weight-bold"
+											<div class="card-footer p-2">
+												<button type="button" class="btn mx-2 btn-light-primary font-weight-bold"
 														data-dismiss="modal">{% trans "Cancel" %}
 												</button>
 												<button class="btn btn-primary">
-													{% trans "Submit" %}
+													{% trans "Submit" %} {% trans "Ticket" %}
 												</button>
 											</div>
 										</form>
 									</div>
 								</div>
 							</div>
                             <div class="card-toolbar">
                                 <button type="button" class="btn btn-primary" data-toggle="modal"
                                         data-target="#ticketModal">
-                                    {% trans "Create" %} {% trans "Ticket" %}
+                                    {% trans "Submit" %} {% trans "Ticket" %}
                                 </button>
                             </div>
 
                         </div>
                         <div class="card-body">
                             {% if not disableTable %}
                                 <table class="table table-striped table-custom-border text-center table-rounded table-borderless table-thead-primary"
@@ -131,14 +131,34 @@
                 .prepend(
                 {% else %}
                 .html(
             {% endif %}
             `
     <a href="messages/${data[0]}" data-skin="dark" data-toggle="tooltip" data-placement="top" title="" data-original-title="{% trans 'Messages' %}" class="btn btn-sm btn-light-primary btn-icon"><span class="svg-icon svg-icon-md">{% include 'svg/message.html' %}</span></button>
                 `)
+				const status_list = data[3]
+				const is_closed = status_list[0]
+				const count = status_list[1]
+				let last_message = status_list[2]
+				let color = 'dark'
+				if(last_message === -1){
+                    last_message = '{% trans "no message yet" %}'
+                } else if(last_message === 0){
+                    last_message = '{% trans "waiting to answer" %}'
+					color = 'danger'
+                } else if(last_message === 1){
+                    last_message = '{% trans "answered" %}'
+					color = 'success'
+                }
+				$(`td:eq(1)`, row).html(
+                    `<label class="label label-xl label-inline font-weight-bold label-light-${color}">
+						<span class="label label-xl mr-2 label-dot label-${color}"></span> {% trans "Ticket" %}: ${is_closed ? '{% trans "close" %}' : '{% trans "open" %}'} - ${last_message}
+					</label>
+`
+				)
 
             },
 
         });
 
         $('#form_ticket').on('submit', function (e) {
             e.preventDefault();
```

#### html2text {}

```diff
@@ -2,13 +2,13 @@
 static %} {% load widget_tweaks %} {% load i18n %} {% block body %}
 **** {% trans "List" %} {{ model_name }} ****
 ** {% trans "Create" %} {% trans "Ticket" %} **
 
 {% csrf_token %}
 {% trans "Title" %}: [title               ]
    {% if request.user.is_admin %} {{form.writer}} {% endif %}
-{% trans "Cancel" %}   {% trans "Submit" %}
- {% trans "Create" %} {% trans "Ticket" %}
+{% trans "Cancel" %}   {% trans "Submit" %} {% trans "Ticket" %}
+ {% trans "Submit" %} {% trans "Ticket" %}
 {% if not disableTable %}
 {% endif %}
  {% endblock %} {% block script %}
  {% endblock %}
```

### Comparing `badi_users-0.9.0/badi_ticket/templates/ticket/ticket_update.html` & `badi_users-0.9.1/badi_ticket/templates/ticket/ticket_update.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_ticket/urls.py` & `badi_users-0.9.1/badi_ticket/urls.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_ticket/views.py` & `badi_users-0.9.1/badi_ticket/views.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from badi_utils.dynamic import DynamicCreateView, DynamicListView, DynamicUpdateView
 from badi_ticket.models import Message, Ticket
 from django.contrib.auth import get_user_model
+from django.utils.translation import gettext_lazy as _
 
 User = get_user_model()
 
 
 class TicketListView(DynamicListView):
     # permission_required = ROLES_ADMIN_TEACHER
     permission_required = True
     model = Ticket
-    datatable_cols = ['#', 'کاربر', 'عنوان', 'تاریخ ایجاد', 'بسته شده', ]
+    datatable_cols = ['#', _('Member'), _('Title'), _('Status'), _("Created at")]
 
 
 class TicketCreateView(DynamicCreateView):
     model = Ticket
     success_url = '/ticket/ticket/list'
     permission_required = True
-    datatable_cols = model().get_datatable_verbose_names()
+    datatable_cols = ['#', _('Member'), _('Title'), _('Status'), _("Created at")]
     # permission_required = ROLES_ADMIN_TEACHER
     form_fields = ['title', 'writer']
 
     # updateURL = '/ticket/ticket/update/0'
 
     def get_extra_context(self, context):
         context['form'].fields['writer'].queryset = User.objects.none()
```

### Comparing `badi_users-0.9.0/badi_user/api/api.py` & `badi_users-0.9.1/badi_user/api/api.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_user/api/serializers.py` & `badi_users-0.9.1/badi_user/api/serializers.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_user/filter.py` & `badi_users-0.9.1/badi_user/filter.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_user/locale/fa/LC_MESSAGES/django.mo` & `badi_users-0.9.1/badi_user/locale/fa/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_user/models.py` & `badi_users-0.9.1/badi_user/models.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_user/templates/group/group_create.html` & `badi_users-0.9.1/badi_user/templates/group/group_create.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_user/templates/group/group_update.html` & `badi_users-0.9.1/badi_user/templates/group/group_update.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_user/templates/log/log_list.html` & `badi_users-0.9.1/badi_user/templates/log/log_list.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_user/templates/login-theme/login-1.html` & `badi_users-0.9.1/badi_user/templates/login-theme/login-1.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_user/templates/member/member_create.html` & `badi_users-0.9.1/badi_user/templates/member/member_create.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_user/templates/member/member_list.html` & `badi_users-0.9.1/badi_user/templates/member/member_list.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_user/templates/member/member_self_update.html` & `badi_users-0.9.1/badi_user/templates/member/member_self_update.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_user/templates/member/member_update.html` & `badi_users-0.9.1/badi_user/templates/member/member_update.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_user/templates/user/change_password.html` & `badi_users-0.9.1/badi_user/templates/user/change_password.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_user/templates/user/user_create.html` & `badi_users-0.9.1/badi_user/templates/user/user_create.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_user/templates/user/user_list.html` & `badi_users-0.9.1/badi_user/templates/user/user_list.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_user/templates/user/user_update.html` & `badi_users-0.9.1/badi_user/templates/user/user_update.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_user/templatetags/appfilter.py` & `badi_users-0.9.1/badi_user/templatetags/appfilter.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_user/ui/forms.py` & `badi_users-0.9.1/badi_user/ui/forms.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_user/ui/member_views.py` & `badi_users-0.9.1/badi_user/ui/member_views.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_user/ui/notification_views.py` & `badi_users-0.9.1/badi_user/ui/notification_views.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_user/ui/roles_views.py` & `badi_users-0.9.1/badi_user/ui/roles_views.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_user/ui/urls.py` & `badi_users-0.9.1/badi_user/ui/urls.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_user/ui/views.py` & `badi_users-0.9.1/badi_user/ui/views.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_users.egg-info/SOURCES.txt` & `badi_users-0.9.1/badi_users.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/date_calc.py` & `badi_users-0.9.1/badi_utils/date_calc.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/dynamic.py` & `badi_users-0.9.1/badi_utils/dynamic.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/dynamic_api.py` & `badi_users-0.9.1/badi_utils/dynamic_api.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/dynamic_models.py` & `badi_users-0.9.1/badi_utils/dynamic_models.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/email.py` & `badi_users-0.9.1/badi_utils/email.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/logging.py` & `badi_users-0.9.1/badi_utils/logging.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/responses.py` & `badi_users-0.9.1/badi_utils/responses.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/rss.py` & `badi_users-0.9.1/badi_utils/rss.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/select2.py` & `badi_users-0.9.1/badi_utils/select2.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/sms.py` & `badi_users-0.9.1/badi_utils/sms.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/static/badi_utils/css/custom.css` & `badi_users-0.9.1/badi_utils/static/badi_utils/css/custom.css`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum).eot` & `badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum).eot`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum).ttf` & `badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum).ttf`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum).woff` & `badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum).woff`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum).woff2` & `badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum).woff2`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_2.eot` & `badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_2.eot`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold.eot` & `badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold.eot`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold.ttf` & `badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold.ttf`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold.woff` & `badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold.woff`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold.woff2` & `badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold.woff2`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold_2.eot` & `badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold_2.eot`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light.eot` & `badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light.eot`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light.ttf` & `badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light.ttf`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light.woff` & `badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light.woff`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light.woff2` & `badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light.woff2`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light_2.eot` & `badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light_2.eot`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium.eot` & `badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium.eot`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium.ttf` & `badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium.ttf`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium.woff` & `badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium.woff`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium.woff2` & `badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium.woff2`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium_2.eot` & `badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium_2.eot`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight.eot` & `badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight.eot`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight.ttf` & `badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight.ttf`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight.woff` & `badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight.woff`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight.woff2` & `badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight.woff2`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight_2.eot` & `badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight_2.eot`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb.eot` & `badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb.eot`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb.woff` & `badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb.woff`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb.woff2` & `badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb.woff2`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_2.eot` & `badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_2.eot`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold.eot` & `badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold.eot`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold.ttf` & `badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold.ttf`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold.woff` & `badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold.woff`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold.woff2` & `badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold.woff2`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold_2.eot` & `badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold_2.eot`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold_3.eot` & `badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold_3.eot`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light.eot` & `badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light.eot`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light.ttf` & `badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light.ttf`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light.woff` & `badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light.woff`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light.woff2` & `badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light.woff2`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light_2.eot` & `badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light_2.eot`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium.eot` & `badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium.eot`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium.ttf` & `badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium.ttf`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium.woff` & `badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium.woff`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium.woff2` & `badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium.woff2`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium_2.eot` & `badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium_2.eot`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight.eot` & `badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight.eot`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight.ttf` & `badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight.ttf`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight.woff` & `badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight.woff`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight.woff2` & `badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight.woff2`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight_2.eot` & `badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight_2.eot`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/Ray-Black.ttf` & `badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/Ray-Black.ttf`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/Ray-Bold.ttf` & `badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/Ray-Bold.ttf`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/static/badi_utils/css/fonts/Ray.ttf` & `badi_users-0.9.1/badi_utils/static/badi_utils/css/fonts/Ray.ttf`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/static/badi_utils/js/apexchart.js` & `badi_users-0.9.1/badi_utils/static/badi_utils/js/apexchart.js`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/static/badi_utils/js/api-login.js` & `badi_users-0.9.1/badi_utils/static/badi_utils/js/api-login.js`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/static/badi_utils/js/api.js` & `badi_users-0.9.1/badi_utils/static/badi_utils/js/api.js`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/static/badi_utils/js/base.js` & `badi_users-0.9.1/badi_utils/static/badi_utils/js/base.js`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/static/badi_utils/js/chat.js` & `badi_users-0.9.1/badi_utils/static/badi_utils/js/chat.js`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/static/badi_utils/js/custom-vue.js` & `badi_users-0.9.1/badi_utils/static/badi_utils/js/custom-vue.js`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/static/badi_utils/js/datatable.js` & `badi_users-0.9.1/badi_utils/static/badi_utils/js/datatable.js`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/static/badi_utils/js/image-field.js` & `badi_users-0.9.1/badi_utils/static/badi_utils/js/image-field.js`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/static/badi_utils/js/main.js` & `badi_users-0.9.1/badi_utils/static/badi_utils/js/main.js`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/static/badi_utils/js/notification.js` & `badi_users-0.9.1/badi_utils/static/badi_utils/js/notification.js`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/static/badi_utils/js/pagination-vue.js` & `badi_users-0.9.1/badi_utils/static/badi_utils/js/pagination-vue.js`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/static/badi_utils/js/tableexport.js` & `badi_users-0.9.1/badi_utils/static/badi_utils/js/tableexport.js`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/static/badi_utils/js/transaction.js` & `badi_users-0.9.1/badi_utils/static/badi_utils/js/transaction.js`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/static/badi_utils/js/vue.js` & `badi_users-0.9.1/badi_utils/static/badi_utils/js/vue.js`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/static/badi_utils/js/xlsx.mini.min.js` & `badi_users-0.9.1/badi_utils/static/badi_utils/js/xlsx.mini.min.js`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/templates/component/createModal.html` & `badi_users-0.9.1/badi_utils/templates/component/createModal.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/templates/component/createTitle.html` & `badi_users-0.9.1/badi_utils/templates/component/createTitle.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/templates/component/filter-form.html` & `badi_users-0.9.1/badi_utils/templates/component/filter-form.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/templates/component/form-errors.html` & `badi_users-0.9.1/badi_utils/templates/component/form-errors.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/templates/component/form-progressbar-js.html` & `badi_users-0.9.1/badi_utils/templates/component/form-progressbar-js.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/templates/component/image-field.html` & `badi_users-0.9.1/badi_utils/templates/component/image-field.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/templates/component/index-menu.html` & `badi_users-0.9.1/badi_utils/templates/component/index-menu.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/templates/component/input.html` & `badi_users-0.9.1/badi_utils/templates/component/input.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/templates/component/messages.html` & `badi_users-0.9.1/badi_utils/templates/component/messages.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/templates/component/pagination-vue.html` & `badi_users-0.9.1/badi_utils/templates/component/pagination-vue.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/templates/component/table-item.html` & `badi_users-0.9.1/badi_utils/templates/component/table-item.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/templates/component/user-card.html` & `badi_users-0.9.1/badi_utils/templates/component/user-card.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/templates/svg/Incoming-box.html` & `badi_users-0.9.1/badi_utils/templates/svg/Incoming-box.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/templates/svg/add-user.html` & `badi_users-0.9.1/badi_utils/templates/svg/add-user.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/templates/svg/address-book.html` & `badi_users-0.9.1/badi_utils/templates/svg/address-book.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/templates/svg/arrow-left.html` & `badi_users-0.9.1/badi_utils/templates/svg/arrow-left.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/templates/svg/arrow-right.html` & `badi_users-0.9.1/badi_utils/templates/svg/arrow-right.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/templates/svg/bitcoin.html` & `badi_users-0.9.1/badi_utils/templates/svg/bitcoin.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/templates/svg/box.html` & `badi_users-0.9.1/badi_utils/templates/svg/box.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/templates/svg/calendar-day.html` & `badi_users-0.9.1/badi_utils/templates/svg/calendar-day.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/templates/svg/calendar-gym.html` & `badi_users-0.9.1/badi_utils/templates/svg/calendar-gym.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/templates/svg/calendar.html` & `badi_users-0.9.1/badi_utils/templates/svg/calendar.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/templates/svg/call.html` & `badi_users-0.9.1/badi_utils/templates/svg/call.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/templates/svg/category.html` & `badi_users-0.9.1/badi_utils/templates/svg/category.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/templates/svg/chat.html` & `badi_users-0.9.1/badi_utils/templates/svg/chat.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/templates/svg/check.html` & `badi_users-0.9.1/badi_utils/templates/svg/check.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/templates/svg/city.html` & `badi_users-0.9.1/badi_utils/templates/svg/city.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/templates/svg/clipboard-list.html` & `badi_users-0.9.1/badi_utils/templates/svg/clipboard-list.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/templates/svg/clock.html` & `badi_users-0.9.1/badi_utils/templates/svg/clock.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/templates/svg/close.html` & `badi_users-0.9.1/badi_utils/templates/svg/close.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/templates/svg/collection.html` & `badi_users-0.9.1/badi_utils/templates/svg/collection.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/templates/svg/comment.html` & `badi_users-0.9.1/badi_utils/templates/svg/comment.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/templates/svg/dashboard.html` & `badi_users-0.9.1/badi_utils/templates/svg/dashboard.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/templates/svg/delete.html` & `badi_users-0.9.1/badi_utils/templates/svg/delete.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/templates/svg/download.html` & `badi_users-0.9.1/badi_utils/templates/svg/download.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/templates/svg/edit.html` & `badi_users-0.9.1/badi_utils/templates/svg/edit.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/templates/svg/file-check.html` & `badi_users-0.9.1/badi_utils/templates/svg/file-check.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/templates/svg/file.html` & `badi_users-0.9.1/badi_utils/templates/svg/file.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/templates/svg/film.html` & `badi_users-0.9.1/badi_utils/templates/svg/film.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/templates/svg/fire.html` & `badi_users-0.9.1/badi_utils/templates/svg/fire.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/templates/svg/group-chat.html` & `badi_users-0.9.1/badi_utils/templates/svg/group-chat.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/templates/svg/group.html` & `badi_users-0.9.1/badi_utils/templates/svg/group.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/templates/svg/half_star.html` & `badi_users-0.9.1/badi_utils/templates/svg/half_star.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/templates/svg/home.html` & `badi_users-0.9.1/badi_utils/templates/svg/home.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/templates/svg/hourse.html` & `badi_users-0.9.1/badi_utils/templates/svg/hourse.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/templates/svg/image.html` & `badi_users-0.9.1/badi_utils/templates/svg/image.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/templates/svg/interview.html` & `badi_users-0.9.1/badi_utils/templates/svg/interview.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/templates/svg/key.html` & `badi_users-0.9.1/badi_utils/templates/svg/key.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/templates/svg/logout.html` & `badi_users-0.9.1/badi_utils/templates/svg/logout.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/templates/svg/mail.html` & `badi_users-0.9.1/badi_utils/templates/svg/mail.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/templates/svg/map.html` & `badi_users-0.9.1/badi_utils/templates/svg/map.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/templates/svg/message.html` & `badi_users-0.9.1/badi_utils/templates/svg/message.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/templates/svg/messages.html` & `badi_users-0.9.1/badi_utils/templates/svg/messages.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/templates/svg/notification.html` & `badi_users-0.9.1/badi_utils/templates/svg/notification.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/templates/svg/plus.html` & `badi_users-0.9.1/badi_utils/templates/svg/plus.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/templates/svg/puzzle.html` & `badi_users-0.9.1/badi_utils/templates/svg/puzzle.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/templates/svg/question.html` & `badi_users-0.9.1/badi_utils/templates/svg/question.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/templates/svg/refresh.html` & `badi_users-0.9.1/badi_utils/templates/svg/refresh.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/templates/svg/safe.html` & `badi_users-0.9.1/badi_utils/templates/svg/safe.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/templates/svg/search.html` & `badi_users-0.9.1/badi_utils/templates/svg/search.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/templates/svg/shield-protected.html` & `badi_users-0.9.1/badi_utils/templates/svg/shield-protected.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/templates/svg/shield-user.html` & `badi_users-0.9.1/badi_utils/templates/svg/shield-user.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/templates/svg/timer.html` & `badi_users-0.9.1/badi_utils/templates/svg/timer.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/templates/svg/town.html` & `badi_users-0.9.1/badi_utils/templates/svg/town.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/templates/svg/user.html` & `badi_users-0.9.1/badi_utils/templates/svg/user.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/templates/svg/wallet.html` & `badi_users-0.9.1/badi_utils/templates/svg/wallet.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/templates/svg/warning.html` & `badi_users-0.9.1/badi_utils/templates/svg/warning.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/utils.py` & `badi_users-0.9.1/badi_utils/utils.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_utils/validations.py` & `badi_users-0.9.1/badi_utils/validations.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_visit/api/api.py` & `badi_users-0.9.1/badi_visit/api/api.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_visit/models.py` & `badi_users-0.9.1/badi_visit/models.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_wallet/action.py` & `badi_users-0.9.1/badi_wallet/action.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_wallet/api/serializers.py` & `badi_users-0.9.1/badi_wallet/api/serializers.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_wallet/api/view_sets.py` & `badi_users-0.9.1/badi_wallet/api/view_sets.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_wallet/locale/fa/LC_MESSAGES/django.mo` & `badi_users-0.9.1/badi_wallet/locale/fa/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_wallet/models.py` & `badi_users-0.9.1/badi_wallet/models.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_wallet/templates/transaction/all_transaction_list.html` & `badi_users-0.9.1/badi_wallet/templates/transaction/all_transaction_list.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_wallet/templates/transaction/all_transaction_report.html` & `badi_users-0.9.1/badi_wallet/templates/transaction/all_transaction_report.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_wallet/templates/transaction/request-transaction.html` & `badi_users-0.9.1/badi_wallet/templates/transaction/request-transaction.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_wallet/templates/transaction/transaction_list.html` & `badi_users-0.9.1/badi_wallet/templates/transaction/transaction_list.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_wallet/templates/transaction/transaction_result.html` & `badi_users-0.9.1/badi_wallet/templates/transaction/transaction_result.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_wallet/ui/urls.py` & `badi_users-0.9.1/badi_wallet/ui/urls.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.0/badi_wallet/ui/views.py` & `badi_users-0.9.1/badi_wallet/ui/views.py`

 * *Files identical despite different names*

