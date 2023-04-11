# Comparing `tmp/NEMO-4.4.1.tar.gz` & `tmp/NEMO-4.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NEMO-4.4.1.tar", last modified: Tue Jan 31 03:24:27 2023, max compression
+gzip compressed data, was "NEMO-4.5.0.tar", last modified: Tue Apr 11 20:19:03 2023, max compression
```

## Comparing `NEMO-4.4.1.tar` & `NEMO-4.5.0.tar`

### file list

```diff
@@ -1,468 +1,481 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 03:24:27.684621 NEMO-4.4.1/
--rw-rw-rw-   0 root         (0) root         (0)     1644 2023-01-25 14:56:31.000000 NEMO-4.4.1/LICENSE.md
--rw-rw-rw-   0 root         (0) root         (0)      131 2023-01-25 14:56:31.000000 NEMO-4.4.1/MANIFEST.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 03:24:27.628619 NEMO-4.4.1/NEMO/
--rw-rw-rw-   0 root         (0) root         (0)      820 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2996 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/actions.py
--rw-rw-rw-   0 root         (0) root         (0)    47357 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/admin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 03:24:27.628619 NEMO-4.4.1/NEMO/apps/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/apps/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 03:24:27.629619 NEMO-4.4.1/NEMO/apps/area_access/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/apps/area_access/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 03:24:27.619619 NEMO-4.4.1/NEMO/apps/area_access/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 03:24:27.629619 NEMO-4.4.1/NEMO/apps/area_access/static/area_access/
--rw-rw-rw-   0 root         (0) root         (0)      304 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/apps/area_access/static/area_access/area_access.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 03:24:27.619619 NEMO-4.4.1/NEMO/apps/area_access/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 03:24:27.631619 NEMO-4.4.1/NEMO/apps/area_access/templates/area_access/
--rw-rw-rw-   0 root         (0) root         (0)     1531 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/apps/area_access/templates/area_access/already_logged_in.html
--rw-rw-rw-   0 root         (0) root         (0)      349 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/apps/area_access/templates/area_access/badge_not_found.html
--rw-rw-rw-   0 root         (0) root         (0)     9067 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/apps/area_access/templates/area_access/base.html
--rw-rw-rw-   0 root         (0) root         (0)      664 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/apps/area_access/templates/area_access/choose_project.html
--rw-rw-rw-   0 root         (0) root         (0)       54 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/apps/area_access/templates/area_access/door_is_open.html
--rw-rw-rw-   0 root         (0) root         (0)      236 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/apps/area_access/templates/area_access/farewell_screen.html
--rw-rw-rw-   0 root         (0) root         (0)      143 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/apps/area_access/templates/area_access/inactive.html
--rw-rw-rw-   0 root         (0) root         (0)      363 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/apps/area_access/templates/area_access/login_success.html
--rw-rw-rw-   0 root         (0) root         (0)      244 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/apps/area_access/templates/area_access/logout_success.html
--rw-rw-rw-   0 root         (0) root         (0)      666 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/apps/area_access/templates/area_access/logout_warning.html
--rw-rw-rw-   0 root         (0) root         (0)      239 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/apps/area_access/templates/area_access/no_active_projects.html
--rw-rw-rw-   0 root         (0) root         (0)      338 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/apps/area_access/templates/area_access/not_logged_in.html
--rw-rw-rw-   0 root         (0) root         (0)      210 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/apps/area_access/templates/area_access/physical_access_denied.html
--rw-rw-rw-   0 root         (0) root         (0)      566 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/apps/area_access/templates/area_access/resource_unavailable.html
--rw-rw-rw-   0 root         (0) root         (0)      224 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/apps/area_access/templates/area_access/welcome_screen.html
--rw-rw-rw-   0 root         (0) root         (0)      629 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/apps/area_access/urls.py
--rw-rw-rw-   0 root         (0) root         (0)    12286 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/apps/area_access/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 03:24:27.631619 NEMO-4.4.1/NEMO/apps/kiosk/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/apps/kiosk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 03:24:27.619619 NEMO-4.4.1/NEMO/apps/kiosk/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 03:24:27.632619 NEMO-4.4.1/NEMO/apps/kiosk/static/kiosk/
--rw-rw-rw-   0 root         (0) root         (0)      116 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/apps/kiosk/static/kiosk/kiosk.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 03:24:27.619619 NEMO-4.4.1/NEMO/apps/kiosk/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 03:24:27.633619 NEMO-4.4.1/NEMO/apps/kiosk/templates/kiosk/
--rw-rw-rw-   0 root         (0) root         (0)      170 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/apps/kiosk/templates/kiosk/acknowledgement.html
--rw-rw-rw-   0 root         (0) root         (0)     2125 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/apps/kiosk/templates/kiosk/category_choices.html
--rw-rw-rw-   0 root         (0) root         (0)     2012 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/apps/kiosk/templates/kiosk/choices.html
--rw-rw-rw-   0 root         (0) root         (0)     1072 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/apps/kiosk/templates/kiosk/error.html
--rw-rw-rw-   0 root         (0) root         (0)     2923 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/apps/kiosk/templates/kiosk/individual_reservation.html
--rw-rw-rw-   0 root         (0) root         (0)    12184 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/apps/kiosk/templates/kiosk/kiosk.html
--rw-rw-rw-   0 root         (0) root         (0)      240 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/apps/kiosk/templates/kiosk/location_directory.html
--rw-rw-rw-   0 root         (0) root         (0)      901 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/apps/kiosk/templates/kiosk/success.html
--rw-rw-rw-   0 root         (0) root         (0)    16575 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/apps/kiosk/templates/kiosk/tool_information.html
--rw-rw-rw-   0 root         (0) root         (0)     1108 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/apps/kiosk/templates/kiosk/tool_project_selection_snippet.html
--rw-rw-rw-   0 root         (0) root         (0)     4472 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/apps/kiosk/templates/kiosk/tool_reservation.html
--rw-rw-rw-   0 root         (0) root         (0)     1198 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/apps/kiosk/urls.py
--rw-rw-rw-   0 root         (0) root         (0)    13616 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/apps/kiosk/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 03:24:27.634619 NEMO-4.4.1/NEMO/apps/sensors/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/apps/sensors/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6683 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/apps/sensors/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      539 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/apps/sensors/customizations.py
--rw-rw-rw-   0 root         (0) root         (0)     5237 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/apps/sensors/evaluators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 03:24:27.634619 NEMO-4.4.1/NEMO/apps/sensors/management/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/apps/sensors/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 03:24:27.635619 NEMO-4.4.1/NEMO/apps/sensors/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/apps/sensors/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      278 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/apps/sensors/management/commands/manage_sensor_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 03:24:27.635619 NEMO-4.4.1/NEMO/apps/sensors/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     7794 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/apps/sensors/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/apps/sensors/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12959 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/apps/sensors/models.py
--rw-rw-rw-   0 root         (0) root         (0)     4482 2023-01-31 03:24:16.000000 NEMO-4.4.1/NEMO/apps/sensors/sensors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 03:24:27.619619 NEMO-4.4.1/NEMO/apps/sensors/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 03:24:27.637619 NEMO-4.4.1/NEMO/apps/sensors/static/sensors/
--rw-rw-rw-   0 root         (0) root         (0)   408236 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/apps/sensors/static/sensors/chart.js
--rw-rw-rw-   0 root         (0) root         (0)   195090 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/apps/sensors/static/sensors/chart.min.js
--rw-rw-rw-   0 root         (0) root         (0)     1376 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/apps/sensors/static/sensors/chartjs-adapter-moment.js
--rw-rw-rw-   0 root         (0) root         (0)     7659 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/apps/sensors/static/sensors/daterangepicker.css
--rw-rw-rw-   0 root         (0) root         (0)    66305 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/apps/sensors/static/sensors/daterangepicker.js
--rw-rw-rw-   0 root         (0) root         (0)      608 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/apps/sensors/static/sensors/sensors.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 03:24:27.620619 NEMO-4.4.1/NEMO/apps/sensors/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 03:24:27.637619 NEMO-4.4.1/NEMO/apps/sensors/templates/customizations/
--rw-rw-rw-   0 root         (0) root         (0)     3624 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/apps/sensors/templates/customizations/customizations_sensors.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 03:24:27.637619 NEMO-4.4.1/NEMO/apps/sensors/templates/sensors/
--rw-rw-rw-   0 root         (0) root         (0)      347 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/apps/sensors/templates/sensors/sensor_alerts.html
--rw-rw-rw-   0 root         (0) root         (0)    15165 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/apps/sensors/templates/sensors/sensor_data.html
--rw-rw-rw-   0 root         (0) root         (0)     2539 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/apps/sensors/templates/sensors/sensors.html
--rw-rw-rw-   0 root         (0) root         (0)      790 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/apps/sensors/urls.py
--rw-rw-rw-   0 root         (0) root         (0)     5069 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/apps/sensors/views.py
--rw-rw-rw-   0 root         (0) root         (0)     3397 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/context_processors.py
--rw-rw-rw-   0 root         (0) root         (0)     5787 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/decorators.py
--rw-rw-rw-   0 root         (0) root         (0)     4513 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     3833 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/fields.py
--rw-rw-rw-   0 root         (0) root         (0)    14507 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/forms.py
--rw-rw-rw-   0 root         (0) root         (0)    16418 2023-01-31 03:24:16.000000 NEMO-4.4.1/NEMO/interlocks.py
--rw-rw-rw-   0 root         (0) root         (0)      404 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/manage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 03:24:27.637619 NEMO-4.4.1/NEMO/management/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 03:24:27.639619 NEMO-4.4.1/NEMO/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      385 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/management/commands/cancel_unused_reservations.py
--rw-rw-rw-   0 root         (0) root         (0)      382 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/management/commands/create_closure_alerts.py
--rw-rw-rw-   0 root         (0) root         (0)      376 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/management/commands/manage_recurring_charges.py
--rw-rw-rw-   0 root         (0) root         (0)      431 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/management/commands/manage_tool_qualifications.py
--rw-rw-rw-   0 root         (0) root         (0)      417 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/management/commands/send_email_out_of_time_reservation_notification.py
--rw-rw-rw-   0 root         (0) root         (0)      415 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/management/commands/send_email_reservation_ending_reminders.py
--rw-rw-rw-   0 root         (0) root         (0)      408 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/management/commands/send_email_reservation_reminders.py
--rw-rw-rw-   0 root         (0) root         (0)      554 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/management/commands/send_email_usage_reminders.py
--rw-rw-rw-   0 root         (0) root         (0)      456 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/management/commands/send_email_user_access_expiration_reminders.py
--rw-rw-rw-   0 root         (0) root         (0)      406 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/management/commands/send_email_weekend_access_notification.py
--rw-rw-rw-   0 root         (0) root         (0)     5454 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/middleware.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 03:24:27.643620 NEMO-4.4.1/NEMO/migrations/
--rw-rw-rw-   0 root         (0) root         (0)    50307 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/migrations/0001_version_1_0_0.py
--rw-rw-rw-   0 root         (0) root         (0)    32962 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/migrations/0002_version_1_0_0_squashed.py
--rw-rw-rw-   0 root         (0) root         (0)     7988 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/migrations/0012_version_2_0_0_squashed.py
--rw-rw-rw-   0 root         (0) root         (0)     9904 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/migrations/0020_version_3_0_0.py
--rw-rw-rw-   0 root         (0) root         (0)     1712 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/migrations/0021_version_3_1_0.py
--rw-rw-rw-   0 root         (0) root         (0)     1095 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/migrations/0022_version_3_3_0.py
--rw-rw-rw-   0 root         (0) root         (0)      913 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/migrations/0023_badgereader.py
--rw-rw-rw-   0 root         (0) root         (0)      705 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/migrations/0024_contactinformation_user.py
--rw-rw-rw-   0 root         (0) root         (0)     2674 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/migrations/0025_version_3_6_0.py
--rw-rw-rw-   0 root         (0) root         (0)     5405 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/migrations/0026_version_3_7_0.py
--rw-rw-rw-   0 root         (0) root         (0)      420 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/migrations/0027_version_3_8_0.py
--rw-rw-rw-   0 root         (0) root         (0)     2233 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/migrations/0028_version_3_9_0.py
--rw-rw-rw-   0 root         (0) root         (0)     1127 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/migrations/0030_version_3_9_2.py
--rw-rw-rw-   0 root         (0) root         (0)     2785 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/migrations/0031_version_3_10_0.py
--rw-rw-rw-   0 root         (0) root         (0)     3166 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/migrations/0032_version_3_11_0.py
--rw-rw-rw-   0 root         (0) root         (0)      380 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/migrations/0033_version_3_12_0.py
--rw-rw-rw-   0 root         (0) root         (0)      372 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/migrations/0034_version_3_13_0.py
--rw-rw-rw-   0 root         (0) root         (0)     6747 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/migrations/0035_version_3_14_0.py
--rw-rw-rw-   0 root         (0) root         (0)     7792 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/migrations/0036_version_3_15_0.py
--rw-rw-rw-   0 root         (0) root         (0)     3717 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/migrations/0037_version_3_16_0.py
--rw-rw-rw-   0 root         (0) root         (0)      935 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/migrations/0038_version_4_0_0.py
--rw-rw-rw-   0 root         (0) root         (0)     3601 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/migrations/0039_version_4_1_0.py
--rw-rw-rw-   0 root         (0) root         (0)     2444 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/migrations/0040_version_4_2_0.py
--rw-rw-rw-   0 root         (0) root         (0)      487 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/migrations/0041_version_4_2_1.py
--rw-rw-rw-   0 root         (0) root         (0)    16454 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/migrations/0042_version_4_3_0.py
--rw-rw-rw-   0 root         (0) root         (0)      524 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/migrations/0043_version_4_3_2.py
--rw-rw-rw-   0 root         (0) root         (0)     5420 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/migrations/0044_version_4_4_0.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1914 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/migrations_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     3855 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/model_tree.py
--rw-rw-rw-   0 root         (0) root         (0)   141743 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/models.py
--rw-rw-rw-   0 root         (0) root         (0)      870 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/permissions.py
--rw-rw-rw-   0 root         (0) root         (0)     9943 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/provisioning.py
--rw-rw-rw-   0 root         (0) root         (0)     5797 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/rates.py
--rw-rw-rw-   0 root         (0) root         (0)     1037 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/rest_filter_backend.py
--rw-rw-rw-   0 root         (0) root         (0)     6000 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/serializers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 03:24:27.647620 NEMO-4.4.1/NEMO/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 03:24:27.647620 NEMO-4.4.1/NEMO/static/admin/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 03:24:27.647620 NEMO-4.4.1/NEMO/static/admin/physical_access_level/
--rw-rw-rw-   0 root         (0) root         (0)      607 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/static/admin/physical_access_level/access_level.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 03:24:27.648620 NEMO-4.4.1/NEMO/static/admin/questions_preview/
--rw-rw-rw-   0 root         (0) root         (0)     4124 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/static/admin/questions_preview/questions_preview.css
--rw-rw-rw-   0 root         (0) root         (0)     1372 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/static/admin/questions_preview/questions_preview.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 03:24:27.648620 NEMO-4.4.1/NEMO/static/admin/reservation_questions/
--rw-rw-rw-   0 root         (0) root         (0)      247 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/static/admin/reservation_questions/reservation_questions.js
--rw-rw-rw-   0 root         (0) root         (0)     1225 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/static/admin/time_options_override.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 03:24:27.648620 NEMO-4.4.1/NEMO/static/admin/tool/
--rw-rw-rw-   0 root         (0) root         (0)     1437 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/static/admin/tool/tool.js
--rw-rw-rw-   0 root         (0) root         (0)     1278 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/static/badge_reader.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 03:24:27.620619 NEMO-4.4.1/NEMO/static/bootstrap/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 03:24:27.650620 NEMO-4.4.1/NEMO/static/bootstrap/css/
--rw-rw-rw-   0 root         (0) root         (0)    22608 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/static/bootstrap/css/bootstrap-theme.css
--rw-rw-rw-   0 root         (0) root         (0)    43339 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/static/bootstrap/css/bootstrap-theme.css.map
--rw-rw-rw-   0 root         (0) root         (0)    19963 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/static/bootstrap/css/bootstrap-theme.min.css
--rw-rw-rw-   0 root         (0) root         (0)   141622 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/static/bootstrap/css/bootstrap.css
--rw-rw-rw-   0 root         (0) root         (0)   380986 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/static/bootstrap/css/bootstrap.css.map
--rw-rw-rw-   0 root         (0) root         (0)   117305 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/static/bootstrap/css/bootstrap.min.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 03:24:27.651620 NEMO-4.4.1/NEMO/static/bootstrap/fonts/
--rw-rw-rw-   0 root         (0) root         (0)    20127 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.eot
--rw-rw-rw-   0 root         (0) root         (0)   108738 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.svg
--rw-rw-rw-   0 root         (0) root         (0)    45404 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.ttf
--rw-rw-rw-   0 root         (0) root         (0)    23424 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.woff
--rw-rw-rw-   0 root         (0) root         (0)    18028 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.woff2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 03:24:27.651620 NEMO-4.4.1/NEMO/static/bootstrap/js/
--rw-rw-rw-   0 root         (0) root         (0)    67546 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/static/bootstrap/js/bootstrap.js
--rw-rw-rw-   0 root         (0) root         (0)    35951 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/static/bootstrap/js/bootstrap.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 03:24:27.651620 NEMO-4.4.1/NEMO/static/datetimepicker/
--rw-rw-rw-   0 root         (0) root         (0)     9020 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/static/datetimepicker/bootstrap-datetimepicker.css
--rw-rw-rw-   0 root         (0) root         (0)   105978 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/static/datetimepicker/bootstrap-datetimepicker.js
--rw-rw-rw-   0 root         (0) root         (0)     1150 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/static/favicon.ico
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 03:24:27.653620 NEMO-4.4.1/NEMO/static/fullcalendar/
--rw-rw-rw-   0 root         (0) root         (0)    28531 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/static/fullcalendar/fullcalendar.css
--rw-rw-rw-   0 root         (0) root         (0)   357749 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/static/fullcalendar/fullcalendar.js
--rw-rw-rw-   0 root         (0) root         (0)    13687 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/static/fullcalendar/fullcalendar.min.css
--rw-rw-rw-   0 root         (0) root         (0)   168700 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/static/fullcalendar/fullcalendar.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 03:24:27.653620 NEMO-4.4.1/NEMO/static/icons/
--rw-rw-rw-   0 root         (0) root         (0)    24065 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/static/icons/agreement.png
--rw-rw-rw-   0 root         (0) root         (0)    16685 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/static/icons/caution.png
--rw-rw-rw-   0 root         (0) root         (0)     4664 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/static/icons/preferences.png
--rw-rw-rw-   0 root         (0) root         (0)   247387 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/static/jquery.js
--rw-rw-rw-   0 root         (0) root         (0)    84320 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/static/jquery.min.js
--rw-rw-rw-   0 root         (0) root         (0)  1183392 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/static/jumbotron_watermark.bmp
--rw-rw-rw-   0 root         (0) root         (0)     1017 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/static/mobile.js
--rw-rw-rw-   0 root         (0) root         (0)   174603 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/static/moment.js
--rw-rw-rw-   0 root         (0) root         (0)    58102 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/static/moment.min.js
--rw-rw-rw-   0 root         (0) root         (0)    86041 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/static/moment.min.js.map
--rw-rw-rw-   0 root         (0) root         (0)    13843 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/static/nemo.css
--rw-rw-rw-   0 root         (0) root         (0)    20061 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/static/nemo.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 03:24:27.654620 NEMO-4.4.1/NEMO/static/numpad/
--rw-rw-rw-   0 root         (0) root         (0)    12285 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/static/numpad/custom_numpad.jquery.js
--rw-rw-rw-   0 root         (0) root         (0)      255 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/static/numpad/numpad.jquery.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 03:24:27.655620 NEMO-4.4.1/NEMO/static/pickadate/
--rw-rw-rw-   0 root         (0) root         (0)     3795 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/static/pickadate/default.css
--rw-rw-rw-   0 root         (0) root         (0)     6040 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/static/pickadate/default.date.css
--rw-rw-rw-   0 root         (0) root         (0)     2785 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/static/pickadate/default.time.css
--rw-rw-rw-   0 root         (0) root         (0)    48215 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/static/pickadate/picker.date.js
--rw-rw-rw-   0 root         (0) root         (0)    36941 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/static/pickadate/picker.js
--rw-rw-rw-   0 root         (0) root         (0)    31899 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/static/pickadate/picker.time.js
--rw-rw-rw-   0 root         (0) root         (0)       25 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/static/robots.txt
--rw-rw-rw-   0 root         (0) root         (0)    48446 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/static/typeahead.jquery.js
--rw-rw-rw-   0 root         (0) root         (0)    20748 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/static/typeahead.jquery.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 03:24:27.655620 NEMO-4.4.1/NEMO/static/virtualkeyboard/
--rw-rw-rw-   0 root         (0) root         (0)   113008 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/static/virtualkeyboard/jquery.keyboard.js
--rw-rw-rw-   0 root         (0) root         (0)    47325 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/static/virtualkeyboard/jquery.keyboard.min.js
--rw-rw-rw-   0 root         (0) root         (0)     7848 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/static/virtualkeyboard/keyboard-basic.css
--rw-rw-rw-   0 root         (0) root         (0)     5889 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/static/virtualkeyboard/keyboard-basic.min.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 03:24:27.657620 NEMO-4.4.1/NEMO/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 03:24:27.658620 NEMO-4.4.1/NEMO/templates/abuse/
--rw-rw-rw-   0 root         (0) root         (0)     4059 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/abuse/abuse.html
--rw-rw-rw-   0 root         (0) root         (0)      580 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/abuse/user_drill_down.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 03:24:27.659620 NEMO-4.4.1/NEMO/templates/accounts_and_projects/
--rw-rw-rw-   0 root         (0) root         (0)     7318 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/accounts_and_projects/account_and_projects.html
--rw-rw-rw-   0 root         (0) root         (0)     6352 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/accounts_and_projects/accounts_and_projects.html
--rw-rw-rw-   0 root         (0) root         (0)     2843 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/accounts_and_projects/create_account.html
--rw-rw-rw-   0 root         (0) root         (0)     4943 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/accounts_and_projects/create_project.html
--rw-rw-rw-   0 root         (0) root         (0)      888 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/accounts_and_projects/documents_for_project.html
--rw-rw-rw-   0 root         (0) root         (0)     2336 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/accounts_and_projects/projects.html
--rw-rw-rw-   0 root         (0) root         (0)      859 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/accounts_and_projects/users_for_project.html
--rw-rw-rw-   0 root         (0) root         (0)      433 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/acknowledgement.html
--rw-rw-rw-   0 root         (0) root         (0)     4694 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/alerts.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 03:24:27.660620 NEMO-4.4.1/NEMO/templates/area_access/
--rw-rw-rw-   0 root         (0) root         (0)     2951 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/area_access/area_access.html
--rw-rw-rw-   0 root         (0) root         (0)     1687 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/area_access/calendar_self_login.html
--rw-rw-rw-   0 root         (0) root         (0)     1111 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/area_access/change_project.html
--rw-rw-rw-   0 root         (0) root         (0)     1141 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/area_access/login_areas.html
--rw-rw-rw-   0 root         (0) root         (0)     1245 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/area_access/new_area_access_record.html
--rw-rw-rw-   0 root         (0) root         (0)     1938 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/area_access/new_area_access_record_details.html
--rw-rw-rw-   0 root         (0) root         (0)     1454 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/area_access/self_login.html
--rw-rw-rw-   0 root         (0) root         (0)      837 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/authorization_failed.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 03:24:27.660620 NEMO-4.4.1/NEMO/templates/base/
--rw-rw-rw-   0 root         (0) root         (0)      308 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/base/footer.html
--rw-rw-rw-   0 root         (0) root         (0)      292 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/base/impersonate_header.html
--rw-rw-rw-   0 root         (0) root         (0)     2671 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/base/navbar.html
--rw-rw-rw-   0 root         (0) root         (0)     2246 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/base/navbar_admin.html
--rw-rw-rw-   0 root         (0) root         (0)     1155 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/base/navbar_main.html
--rw-rw-rw-   0 root         (0) root         (0)      247 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/base/popup.html
--rw-rw-rw-   0 root         (0) root         (0)     5535 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/base.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 03:24:27.662620 NEMO-4.4.1/NEMO/templates/calendar/
--rw-rw-rw-   0 root         (0) root         (0)    24260 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/calendar/calendar.html
--rw-rw-rw-   0 root         (0) root         (0)     1381 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/calendar/configuration.html
--rw-rw-rw-   0 root         (0) root         (0)     2834 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/calendar/configuration_helper.html
--rw-rw-rw-   0 root         (0) root         (0)     1254 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/calendar/policy_dialog.html
--rw-rw-rw-   0 root         (0) root         (0)     1300 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/calendar/project_choice.html
--rw-rw-rw-   0 root         (0) root         (0)     1335 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/calendar/proxy_reservation.html
--rw-rw-rw-   0 root         (0) root         (0)     1862 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/calendar/reservation_event_feed.html
--rw-rw-rw-   0 root         (0) root         (0)     1619 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/calendar/reservation_questions.html
--rw-rw-rw-   0 root         (0) root         (0)     1285 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/calendar/reservation_warning.html
--rw-rw-rw-   0 root         (0) root         (0)     4094 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/calendar/scheduled_outage_information.html
--rw-rw-rw-   0 root         (0) root         (0)     2011 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/calendar/specific_user_feed.html
--rw-rw-rw-   0 root         (0) root         (0)     2543 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/calendar/usage_event_feed.html
--rw-rw-rw-   0 root         (0) root         (0)     5940 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/configuration_agenda.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 03:24:27.663620 NEMO-4.4.1/NEMO/templates/consumables/
--rw-rw-rw-   0 root         (0) root         (0)     8048 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/consumables/consumables.html
--rw-rw-rw-   0 root         (0) root         (0)     1518 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/consumables/consumables_order.html
--rw-rw-rw-   0 root         (0) root         (0)    11695 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/consumables/recurring_charge.html
--rw-rw-rw-   0 root         (0) root         (0)     5491 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/consumables/recurring_charges.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 03:24:27.663620 NEMO-4.4.1/NEMO/templates/contact/
--rw-rw-rw-   0 root         (0) root         (0)      692 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/contact/contact_staff.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 03:24:27.665620 NEMO-4.4.1/NEMO/templates/customizations/
--rw-rw-rw-   0 root         (0) root         (0)     1848 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/customizations/customizations.html
--rw-rw-rw-   0 root         (0) root         (0)     2571 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/customizations/customizations_application.html
--rw-rw-rw-   0 root         (0) root         (0)     7722 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/customizations/customizations_calendar.html
--rw-rw-rw-   0 root         (0) root         (0)     7247 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/customizations/customizations_dashboard.html
--rw-rw-rw-   0 root         (0) root         (0)     4125 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/customizations/customizations_emails.html
--rw-rw-rw-   0 root         (0) root         (0)     2468 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/customizations/customizations_interlock.html
--rw-rw-rw-   0 root         (0) root         (0)     3857 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/customizations/customizations_projects_and_accounts.html
--rw-rw-rw-   0 root         (0) root         (0)     2205 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/customizations/customizations_rates.html
--rw-rw-rw-   0 root         (0) root         (0)     3442 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/customizations/customizations_recurring_charges.html
--rw-rw-rw-   0 root         (0) root         (0)     7458 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/customizations/customizations_requests.html
--rw-rw-rw-   0 root         (0) root         (0)     3621 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/customizations/customizations_safety.html
--rw-rw-rw-   0 root         (0) root         (0)    26354 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/customizations/customizations_templates.html
--rw-rw-rw-   0 root         (0) root         (0)     5010 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/customizations/customizations_tool_qualification.html
--rw-rw-rw-   0 root         (0) root         (0)     1731 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/customizations/customizations_upload.html
--rw-rw-rw-   0 root         (0) root         (0)     4841 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/customizations/customizations_user.html
--rw-rw-rw-   0 root         (0) root         (0)      441 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/display_success_and_redirect.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 03:24:27.665620 NEMO-4.4.1/NEMO/templates/email/
--rw-rw-rw-   0 root         (0) root         (0)     7800 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/email/compose_email.html
--rw-rw-rw-   0 root         (0) root         (0)     3153 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/email/email_broadcast.html
--rw-rw-rw-   0 root         (0) root         (0)     1045 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/email/email_form.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 03:24:27.666620 NEMO-4.4.1/NEMO/templates/event_details/
--rw-rw-rw-   0 root         (0) root         (0)      751 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/event_details/area_access_details.html
--rw-rw-rw-   0 root         (0) root         (0)     1347 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/event_details/outage_details.html
--rw-rw-rw-   0 root         (0) root         (0)     9602 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/event_details/reservation_details.html
--rw-rw-rw-   0 root         (0) root         (0)      589 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/event_details/usage_details.html
--rw-rw-rw-   0 root         (0) root         (0)      426 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/facility_rules.html
--rw-rw-rw-   0 root         (0) root         (0)     1247 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/feedback.html
--rw-rw-rw-   0 root         (0) root         (0)      937 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/history.html
--rw-rw-rw-   0 root         (0) root         (0)     1217 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/impersonate.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 03:24:27.666620 NEMO-4.4.1/NEMO/templates/jumbotron/
--rw-rw-rw-   0 root         (0) root         (0)     2059 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/jumbotron/jumbotron.html
--rw-rw-rw-   0 root         (0) root         (0)     3635 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/jumbotron/jumbotron_content.html
--rw-rw-rw-   0 root         (0) root         (0)     8390 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/landing.html
--rw-rw-rw-   0 root         (0) root         (0)     3497 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/login.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 03:24:27.667620 NEMO-4.4.1/NEMO/templates/maintenance/
--rw-rw-rw-   0 root         (0) root         (0)     1558 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/maintenance/closed_task_details.html
--rw-rw-rw-   0 root         (0) root         (0)     5566 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/maintenance/maintenance.html
--rw-rw-rw-   0 root         (0) root         (0)     7450 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/maintenance/pending_task_details.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 03:24:27.668620 NEMO-4.4.1/NEMO/templates/mobile/
--rw-rw-rw-   0 root         (0) root         (0)      762 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/mobile/cancellation_result.html
--rw-rw-rw-   0 root         (0) root         (0)     1916 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/mobile/choose_item.html
--rw-rw-rw-   0 root         (0) root         (0)      453 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/mobile/error.html
--rw-rw-rw-   0 root         (0) root         (0)     1025 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/mobile/individual_outage.html
--rw-rw-rw-   0 root         (0) root         (0)     2625 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/mobile/individual_reservation.html
--rw-rw-rw-   0 root         (0) root         (0)     5899 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/mobile/new_reservation.html
--rw-rw-rw-   0 root         (0) root         (0)      313 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/mobile/no_active_projects.html
--rw-rw-rw-   0 root         (0) root         (0)      777 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/mobile/reservation_success.html
--rw-rw-rw-   0 root         (0) root         (0)     1442 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/mobile/view_calendar.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 03:24:27.668620 NEMO-4.4.1/NEMO/templates/news/
--rw-rw-rw-   0 root         (0) root         (0)      981 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/news/archived_news.html
--rw-rw-rw-   0 root         (0) root         (0)     1027 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/news/new_news_form.html
--rw-rw-rw-   0 root         (0) root         (0)     1198 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/news/news_update_form.html
--rw-rw-rw-   0 root         (0) root         (0)     2038 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/news/recent_news.html
--rw-rw-rw-   0 root         (0) root         (0)      209 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/no_project.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 03:24:27.669620 NEMO-4.4.1/NEMO/templates/occupancy/
--rw-rw-rw-   0 root         (0) root         (0)      408 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/occupancy/occupancy.html
--rw-rw-rw-   0 root         (0) root         (0)     1841 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/occupancy/occupancy_content.html
--rw-rw-rw-   0 root         (0) root         (0)     1147 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/occupancy/occupancy_count.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 03:24:27.669620 NEMO-4.4.1/NEMO/templates/pagination/
--rw-rw-rw-   0 root         (0) root         (0)      865 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/pagination/pagination_base.html
--rw-rw-rw-   0 root         (0) root         (0)      521 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/pagination/pagination_column.html
--rw-rw-rw-   0 root         (0) root         (0)      673 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/pagination/pagination_pages.html
--rw-rw-rw-   0 root         (0) root         (0)      642 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/pagination/pagination_selector.html
--rw-rw-rw-   0 root         (0) root         (0)     2551 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/qualifications.html
--rw-rw-rw-   0 root         (0) root         (0)     5462 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/refresh_sidebar_icons.html
--rw-rw-rw-   0 root         (0) root         (0)     9145 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/remote_work.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 03:24:27.669620 NEMO-4.4.1/NEMO/templates/requests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 03:24:27.670621 NEMO-4.4.1/NEMO/templates/requests/access_requests/
--rw-rw-rw-   0 root         (0) root         (0)     7352 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/requests/access_requests/access_request.html
--rw-rw-rw-   0 root         (0) root         (0)     3172 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/requests/access_requests/access_requests.html
--rw-rw-rw-   0 root         (0) root         (0)     3523 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/requests/access_requests/access_requests_table.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 03:24:27.670621 NEMO-4.4.1/NEMO/templates/requests/buddy_requests/
--rw-rw-rw-   0 root         (0) root         (0)     3910 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/requests/buddy_requests/buddy_request.html
--rw-rw-rw-   0 root         (0) root         (0)     5605 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/requests/buddy_requests/buddy_requests.html
--rw-rw-rw-   0 root         (0) root         (0)     2940 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/requests/user_requests.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 03:24:27.671620 NEMO-4.4.1/NEMO/templates/resources/
--rw-rw-rw-   0 root         (0) root         (0)     2950 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/resources/modify_resource.html
--rw-rw-rw-   0 root         (0) root         (0)     3846 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/resources/resource_details.html
--rw-rw-rw-   0 root         (0) root         (0)     1329 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/resources/resources.html
--rw-rw-rw-   0 root         (0) root         (0)     3807 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/resources/scheduled_outage.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 03:24:27.672621 NEMO-4.4.1/NEMO/templates/safety/
--rw-rw-rw-   0 root         (0) root         (0)     3036 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/safety/safety.html
--rw-rw-rw-   0 root         (0) root         (0)     1828 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/safety/safety_base.html
--rw-rw-rw-   0 root         (0) root         (0)     7713 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/safety/safety_data_sheets.html
--rw-rw-rw-   0 root         (0) root         (0)     1955 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/safety/safety_issues.html
--rw-rw-rw-   0 root         (0) root         (0)     1723 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/safety/safety_issues_create.html
--rw-rw-rw-   0 root         (0) root         (0)     1687 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/safety/safety_issues_resolved.html
--rw-rw-rw-   0 root         (0) root         (0)     1727 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/safety/safety_issues_update.html
--rw-rw-rw-   0 root         (0) root         (0)     1713 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/safety/safety_items.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 03:24:27.672621 NEMO-4.4.1/NEMO/templates/snippets/
--rw-rw-rw-   0 root         (0) root         (0)      516 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/snippets/button.html
--rw-rw-rw-   0 root         (0) root         (0)      904 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/snippets/contact_person.html
--rw-rw-rw-   0 root         (0) root         (0)     1128 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/snippets/embedded_document.html
--rw-rw-rw-   0 root         (0) root         (0)     1603 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/snippets/tool_info.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 03:24:27.673621 NEMO-4.4.1/NEMO/templates/staff_charges/
--rw-rw-rw-   0 root         (0) root         (0)      796 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/staff_charges/change_status.html
--rw-rw-rw-   0 root         (0) root         (0)     1181 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/staff_charges/choose_project.html
--rw-rw-rw-   0 root         (0) root         (0)      434 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/staff_charges/end_area_charge.html
--rw-rw-rw-   0 root         (0) root         (0)     1112 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/staff_charges/new_staff_charge.html
--rw-rw-rw-   0 root         (0) root         (0)      953 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/staff_charges/reminder.html
--rw-rw-rw-   0 root         (0) root         (0)     1795 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/staff_charges/staff_charges_base.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 03:24:27.674621 NEMO-4.4.1/NEMO/templates/status_dashboard/
--rw-rw-rw-   0 root         (0) root         (0)     1554 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/status_dashboard/occupancy.html
--rw-rw-rw-   0 root         (0) root         (0)     8659 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/status_dashboard/staff.html
--rw-rw-rw-   0 root         (0) root         (0)     7728 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/status_dashboard/staff_absence.html
--rw-rw-rw-   0 root         (0) root         (0)     5799 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/status_dashboard/status_dashboard.html
--rw-rw-rw-   0 root         (0) root         (0)     3534 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/status_dashboard/tools.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 03:24:27.674621 NEMO-4.4.1/NEMO/templates/tasks/
--rw-rw-rw-   0 root         (0) root         (0)     2542 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/tasks/resolve.html
--rw-rw-rw-   0 root         (0) root         (0)     5037 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/tasks/update.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 03:24:27.675621 NEMO-4.4.1/NEMO/templates/tool_control/
--rw-rw-rw-   0 root         (0) root         (0)      873 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/tool_control/get_projects.html
--rw-rw-rw-   0 root         (0) root         (0)      679 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/tool_control/interlock_error.html
--rw-rw-rw-   0 root         (0) root         (0)     3502 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/tool_control/past_tasks_and_comments.html
--rw-rw-rw-   0 root         (0) root         (0)     2472 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/tool_control/qualified_users.html
--rw-rw-rw-   0 root         (0) root         (0)    15436 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/tool_control/tool_control.html
--rw-rw-rw-   0 root         (0) root         (0)    34646 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/tool_control/tool_status.html
--rw-rw-rw-   0 root         (0) root         (0)     6067 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/tool_control/usage_data.html
--rw-rw-rw-   0 root         (0) root         (0)      409 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/tool_control/use_tool_for_other.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 03:24:27.675621 NEMO-4.4.1/NEMO/templates/training/
--rw-rw-rw-   0 root         (0) root         (0)      512 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/training/get_projects.html
--rw-rw-rw-   0 root         (0) root         (0)     4700 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/training/training.html
--rw-rw-rw-   0 root         (0) root         (0)     1460 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/training/training_entry.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 03:24:27.676621 NEMO-4.4.1/NEMO/templates/usage/
--rw-rw-rw-   0 root         (0) root         (0)     3573 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/usage/billing.html
--rw-rw-rw-   0 root         (0) root         (0)     4138 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/usage/usage.html
--rw-rw-rw-   0 root         (0) root         (0)     6781 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/usage/usage_base.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 03:24:27.676621 NEMO-4.4.1/NEMO/templates/users/
--rw-rw-rw-   0 root         (0) root         (0)    20751 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/users/create_or_modify_user.html
--rw-rw-rw-   0 root         (0) root         (0)     7896 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/users/preferences.html
--rw-rw-rw-   0 root         (0) root         (0)     3758 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/users/safe_deactivation.html
--rw-rw-rw-   0 root         (0) root         (0)     4160 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templates/users/users.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 03:24:27.677621 NEMO-4.4.1/NEMO/templatetags/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templatetags/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6852 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/templatetags/custom_tags_and_filters.py
--rw-rw-rw-   0 root         (0) root         (0)    23378 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/urls.py
--rw-rw-rw-   0 root         (0) root         (0)    21246 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 03:24:27.683621 NEMO-4.4.1/NEMO/views/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/views/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4308 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/views/abuse.py
--rw-rw-rw-   0 root         (0) root         (0)    13160 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/views/access_requests.py
--rw-rw-rw-   0 root         (0) root         (0)     7626 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/views/accounts_and_projects.py
--rw-rw-rw-   0 root         (0) root         (0)     1812 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/views/alerts.py
--rw-rw-rw-   0 root         (0) root         (0)     9617 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/views/api.py
--rw-rw-rw-   0 root         (0) root         (0)    12115 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/views/api_billing.py
--rw-rw-rw-   0 root         (0) root         (0)    18892 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/views/area_access.py
--rw-rw-rw-   0 root         (0) root         (0)    11921 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/views/authentication.py
--rw-rw-rw-   0 root         (0) root         (0)     6293 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/views/buddy_requests.py
--rw-rw-rw-   0 root         (0) root         (0)    68965 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/views/calendar.py
--rw-rw-rw-   0 root         (0) root         (0)     1867 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/views/configuration_agenda.py
--rw-rw-rw-   0 root         (0) root         (0)      174 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/views/constants.py
--rw-rw-rw-   0 root         (0) root         (0)    10085 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/views/consumables.py
--rw-rw-rw-   0 root         (0) root         (0)      467 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/views/contact_staff.py
--rw-rw-rw-   0 root         (0) root         (0)    15069 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/views/customization.py
--rw-rw-rw-   0 root         (0) root         (0)     1335 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/views/documents.py
--rw-rw-rw-   0 root         (0) root         (0)     9978 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/views/email.py
--rw-rw-rw-   0 root         (0) root         (0)     1973 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/views/event_details.py
--rw-rw-rw-   0 root         (0) root         (0)     1482 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/views/feedback.py
--rw-rw-rw-   0 root         (0) root         (0)     1672 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/views/get_projects.py
--rw-rw-rw-   0 root         (0) root         (0)     4168 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/views/history.py
--rw-rw-rw-   0 root         (0) root         (0)     1027 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/views/jumbotron.py
--rw-rw-rw-   0 root         (0) root         (0)     3293 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/views/landing.py
--rw-rw-rw-   0 root         (0) root         (0)     2289 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/views/maintenance.py
--rw-rw-rw-   0 root         (0) root         (0)     8094 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/views/mobile.py
--rw-rw-rw-   0 root         (0) root         (0)     3304 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/views/news.py
--rw-rw-rw-   0 root         (0) root         (0)     4618 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/views/notifications.py
--rw-rw-rw-   0 root         (0) root         (0)     1326 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/views/pagination.py
--rw-rw-rw-   0 root         (0) root         (0)    39192 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/views/policy.py
--rw-rw-rw-   0 root         (0) root         (0)     4322 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/views/qualifications.py
--rw-rw-rw-   0 root         (0) root         (0)     4381 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/views/remote_work.py
--rw-rw-rw-   0 root         (0) root         (0)     3697 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/views/resources.py
--rw-rw-rw-   0 root         (0) root         (0)     8835 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/views/safety.py
--rw-rw-rw-   0 root         (0) root         (0)      932 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/views/sidebar.py
--rw-rw-rw-   0 root         (0) root         (0)     5545 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/views/staff_charges.py
--rw-rw-rw-   0 root         (0) root         (0)    19849 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/views/status_dashboard.py
--rw-rw-rw-   0 root         (0) root         (0)    12934 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/views/tasks.py
--rw-rw-rw-   0 root         (0) root         (0)    22987 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/views/tool_control.py
--rw-rw-rw-   0 root         (0) root         (0)     5176 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/views/training.py
--rw-rw-rw-   0 root         (0) root         (0)     1909 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/views/tutorials.py
--rw-rw-rw-   0 root         (0) root         (0)    17744 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/views/usage.py
--rw-rw-rw-   0 root         (0) root         (0)      906 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/views/user_requests.py
--rw-rw-rw-   0 root         (0) root         (0)    20220 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/views/users.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 03:24:27.683621 NEMO-4.4.1/NEMO/widgets/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/widgets/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2534 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/widgets/configuration_editor.py
--rw-rw-rw-   0 root         (0) root         (0)    24042 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/widgets/dynamic_form.py
--rw-rw-rw-   0 root         (0) root         (0)     8029 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/widgets/item_tree.py
--rw-rw-rw-   0 root         (0) root         (0)       88 2023-01-25 14:56:31.000000 NEMO-4.4.1/NEMO/wsgi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 03:24:27.628619 NEMO-4.4.1/NEMO.egg-info/
--rw-r--r--   0 root         (0) root         (0)      900 2023-01-31 03:24:27.000000 NEMO-4.4.1/NEMO.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    15893 2023-01-31 03:24:27.000000 NEMO-4.4.1/NEMO.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-31 03:24:27.000000 NEMO-4.4.1/NEMO.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       55 2023-01-31 03:24:27.000000 NEMO-4.4.1/NEMO.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      265 2023-01-31 03:24:27.000000 NEMO-4.4.1/NEMO.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-01-31 03:24:27.000000 NEMO-4.4.1/NEMO.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      900 2023-01-31 03:24:27.684621 NEMO-4.4.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3528 2023-01-25 14:56:31.000000 NEMO-4.4.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 03:24:27.684621 NEMO-4.4.1/resources/
--rw-rw-rw-   0 root         (0) root         (0)     3945 2023-01-25 14:56:32.000000 NEMO-4.4.1/resources/splash_pad_settings.py
--rw-r--r--   0 root         (0) root         (0)      109 2023-01-31 03:24:27.684621 NEMO-4.4.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1458 2023-01-31 03:24:16.000000 NEMO-4.4.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:19:03.496289 NEMO-4.5.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1644 2023-04-11 20:18:49.000000 NEMO-4.5.0/LICENSE.md
+-rw-rw-rw-   0 root         (0) root         (0)      131 2023-04-11 20:18:49.000000 NEMO-4.5.0/MANIFEST.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:19:03.433289 NEMO-4.5.0/NEMO/
+-rw-rw-rw-   0 root         (0) root         (0)     1254 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4594 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/actions.py
+-rw-rw-rw-   0 root         (0) root         (0)    48608 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/admin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:19:03.434289 NEMO-4.5.0/NEMO/apps/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/apps/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:19:03.434289 NEMO-4.5.0/NEMO/apps/area_access/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/apps/area_access/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:19:03.422289 NEMO-4.5.0/NEMO/apps/area_access/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:19:03.435289 NEMO-4.5.0/NEMO/apps/area_access/static/area_access/
+-rw-rw-rw-   0 root         (0) root         (0)      304 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/apps/area_access/static/area_access/area_access.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:19:03.422289 NEMO-4.5.0/NEMO/apps/area_access/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:19:03.437289 NEMO-4.5.0/NEMO/apps/area_access/templates/area_access/
+-rw-rw-rw-   0 root         (0) root         (0)     1531 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/apps/area_access/templates/area_access/already_logged_in.html
+-rw-rw-rw-   0 root         (0) root         (0)      349 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/apps/area_access/templates/area_access/badge_not_found.html
+-rw-rw-rw-   0 root         (0) root         (0)     9067 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/apps/area_access/templates/area_access/base.html
+-rw-rw-rw-   0 root         (0) root         (0)      664 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/apps/area_access/templates/area_access/choose_project.html
+-rw-rw-rw-   0 root         (0) root         (0)       54 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/apps/area_access/templates/area_access/door_is_open.html
+-rw-rw-rw-   0 root         (0) root         (0)      236 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/apps/area_access/templates/area_access/farewell_screen.html
+-rw-rw-rw-   0 root         (0) root         (0)      143 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/apps/area_access/templates/area_access/inactive.html
+-rw-rw-rw-   0 root         (0) root         (0)      363 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/apps/area_access/templates/area_access/login_success.html
+-rw-rw-rw-   0 root         (0) root         (0)      244 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/apps/area_access/templates/area_access/logout_success.html
+-rw-rw-rw-   0 root         (0) root         (0)      666 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/apps/area_access/templates/area_access/logout_warning.html
+-rw-rw-rw-   0 root         (0) root         (0)      239 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/apps/area_access/templates/area_access/no_active_projects.html
+-rw-rw-rw-   0 root         (0) root         (0)      338 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/apps/area_access/templates/area_access/not_logged_in.html
+-rw-rw-rw-   0 root         (0) root         (0)      210 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/apps/area_access/templates/area_access/physical_access_denied.html
+-rw-rw-rw-   0 root         (0) root         (0)      566 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/apps/area_access/templates/area_access/resource_unavailable.html
+-rw-rw-rw-   0 root         (0) root         (0)      224 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/apps/area_access/templates/area_access/welcome_screen.html
+-rw-rw-rw-   0 root         (0) root         (0)      629 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/apps/area_access/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)    12271 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/apps/area_access/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:19:03.438289 NEMO-4.5.0/NEMO/apps/kiosk/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/apps/kiosk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:19:03.422289 NEMO-4.5.0/NEMO/apps/kiosk/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:19:03.438289 NEMO-4.5.0/NEMO/apps/kiosk/static/kiosk/
+-rw-rw-rw-   0 root         (0) root         (0)      116 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/apps/kiosk/static/kiosk/kiosk.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:19:03.423289 NEMO-4.5.0/NEMO/apps/kiosk/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:19:03.440289 NEMO-4.5.0/NEMO/apps/kiosk/templates/kiosk/
+-rw-rw-rw-   0 root         (0) root         (0)      170 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/apps/kiosk/templates/kiosk/acknowledgement.html
+-rw-rw-rw-   0 root         (0) root         (0)     2125 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/apps/kiosk/templates/kiosk/category_choices.html
+-rw-rw-rw-   0 root         (0) root         (0)     2012 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/apps/kiosk/templates/kiosk/choices.html
+-rw-rw-rw-   0 root         (0) root         (0)     1072 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/apps/kiosk/templates/kiosk/error.html
+-rw-rw-rw-   0 root         (0) root         (0)     2923 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/apps/kiosk/templates/kiosk/individual_reservation.html
+-rw-rw-rw-   0 root         (0) root         (0)    12184 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/apps/kiosk/templates/kiosk/kiosk.html
+-rw-rw-rw-   0 root         (0) root         (0)      240 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/apps/kiosk/templates/kiosk/location_directory.html
+-rw-rw-rw-   0 root         (0) root         (0)      901 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/apps/kiosk/templates/kiosk/success.html
+-rw-rw-rw-   0 root         (0) root         (0)    16575 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/apps/kiosk/templates/kiosk/tool_information.html
+-rw-rw-rw-   0 root         (0) root         (0)     1108 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/apps/kiosk/templates/kiosk/tool_project_selection_snippet.html
+-rw-rw-rw-   0 root         (0) root         (0)     4472 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/apps/kiosk/templates/kiosk/tool_reservation.html
+-rw-rw-rw-   0 root         (0) root         (0)     1198 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/apps/kiosk/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)    13550 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/apps/kiosk/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:19:03.441289 NEMO-4.5.0/NEMO/apps/sensors/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/apps/sensors/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6966 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/apps/sensors/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      539 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/apps/sensors/customizations.py
+-rw-rw-rw-   0 root         (0) root         (0)     5237 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/apps/sensors/evaluators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:19:03.441289 NEMO-4.5.0/NEMO/apps/sensors/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/apps/sensors/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:19:03.442289 NEMO-4.5.0/NEMO/apps/sensors/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/apps/sensors/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      278 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/apps/sensors/management/commands/manage_sensor_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:19:03.442289 NEMO-4.5.0/NEMO/apps/sensors/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     7794 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/apps/sensors/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/apps/sensors/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12955 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/apps/sensors/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     4564 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/apps/sensors/sensors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:19:03.423289 NEMO-4.5.0/NEMO/apps/sensors/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:19:03.444289 NEMO-4.5.0/NEMO/apps/sensors/static/sensors/
+-rw-rw-rw-   0 root         (0) root         (0)   408236 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/apps/sensors/static/sensors/chart.js
+-rw-rw-rw-   0 root         (0) root         (0)   195090 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/apps/sensors/static/sensors/chart.min.js
+-rw-rw-rw-   0 root         (0) root         (0)     1376 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/apps/sensors/static/sensors/chartjs-adapter-moment.js
+-rw-rw-rw-   0 root         (0) root         (0)     7659 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/apps/sensors/static/sensors/daterangepicker.css
+-rw-rw-rw-   0 root         (0) root         (0)    66305 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/apps/sensors/static/sensors/daterangepicker.js
+-rw-rw-rw-   0 root         (0) root         (0)      608 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/apps/sensors/static/sensors/sensors.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:19:03.423289 NEMO-4.5.0/NEMO/apps/sensors/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:19:03.444289 NEMO-4.5.0/NEMO/apps/sensors/templates/customizations/
+-rw-rw-rw-   0 root         (0) root         (0)     3701 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/apps/sensors/templates/customizations/customizations_sensors.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:19:03.445289 NEMO-4.5.0/NEMO/apps/sensors/templates/sensors/
+-rw-rw-rw-   0 root         (0) root         (0)      347 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/apps/sensors/templates/sensors/sensor_alerts.html
+-rw-rw-rw-   0 root         (0) root         (0)    15165 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/apps/sensors/templates/sensors/sensor_data.html
+-rw-rw-rw-   0 root         (0) root         (0)     2615 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/apps/sensors/templates/sensors/sensors.html
+-rw-rw-rw-   0 root         (0) root         (0)      790 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/apps/sensors/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)     5069 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/apps/sensors/views.py
+-rw-rw-rw-   0 root         (0) root         (0)     3966 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/context_processors.py
+-rw-rw-rw-   0 root         (0) root         (0)     5778 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)     4513 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3833 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/fields.py
+-rw-rw-rw-   0 root         (0) root         (0)    12935 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/forms.py
+-rw-rw-rw-   0 root         (0) root         (0)    17700 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/interlocks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:19:03.445289 NEMO-4.5.0/NEMO/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:19:03.447289 NEMO-4.5.0/NEMO/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      385 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/management/commands/cancel_unused_reservations.py
+-rw-rw-rw-   0 root         (0) root         (0)      382 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/management/commands/create_closure_alerts.py
+-rw-rw-rw-   0 root         (0) root         (0)      376 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/management/commands/manage_recurring_charges.py
+-rw-rw-rw-   0 root         (0) root         (0)      431 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/management/commands/manage_tool_qualifications.py
+-rw-rw-rw-   0 root         (0) root         (0)      417 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/management/commands/send_email_out_of_time_reservation_notification.py
+-rw-rw-rw-   0 root         (0) root         (0)      415 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/management/commands/send_email_reservation_ending_reminders.py
+-rw-rw-rw-   0 root         (0) root         (0)      408 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/management/commands/send_email_reservation_reminders.py
+-rw-rw-rw-   0 root         (0) root         (0)      554 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/management/commands/send_email_usage_reminders.py
+-rw-rw-rw-   0 root         (0) root         (0)      456 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/management/commands/send_email_user_access_expiration_reminders.py
+-rw-rw-rw-   0 root         (0) root         (0)      406 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/management/commands/send_email_weekend_access_notification.py
+-rw-rw-rw-   0 root         (0) root         (0)     5578 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/middleware.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:19:03.451289 NEMO-4.5.0/NEMO/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)    50307 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/migrations/0001_version_1_0_0.py
+-rw-rw-rw-   0 root         (0) root         (0)    32962 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/migrations/0002_version_1_0_0_squashed.py
+-rw-rw-rw-   0 root         (0) root         (0)     7988 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/migrations/0012_version_2_0_0_squashed.py
+-rw-rw-rw-   0 root         (0) root         (0)     9904 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/migrations/0020_version_3_0_0.py
+-rw-rw-rw-   0 root         (0) root         (0)     1712 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/migrations/0021_version_3_1_0.py
+-rw-rw-rw-   0 root         (0) root         (0)     1095 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/migrations/0022_version_3_3_0.py
+-rw-rw-rw-   0 root         (0) root         (0)      913 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/migrations/0023_badgereader.py
+-rw-rw-rw-   0 root         (0) root         (0)      705 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/migrations/0024_contactinformation_user.py
+-rw-rw-rw-   0 root         (0) root         (0)     2674 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/migrations/0025_version_3_6_0.py
+-rw-rw-rw-   0 root         (0) root         (0)     5405 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/migrations/0026_version_3_7_0.py
+-rw-rw-rw-   0 root         (0) root         (0)      420 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/migrations/0027_version_3_8_0.py
+-rw-rw-rw-   0 root         (0) root         (0)     2233 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/migrations/0028_version_3_9_0.py
+-rw-rw-rw-   0 root         (0) root         (0)     1127 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/migrations/0030_version_3_9_2.py
+-rw-rw-rw-   0 root         (0) root         (0)     2785 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/migrations/0031_version_3_10_0.py
+-rw-rw-rw-   0 root         (0) root         (0)     3166 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/migrations/0032_version_3_11_0.py
+-rw-rw-rw-   0 root         (0) root         (0)      380 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/migrations/0033_version_3_12_0.py
+-rw-rw-rw-   0 root         (0) root         (0)      372 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/migrations/0034_version_3_13_0.py
+-rw-rw-rw-   0 root         (0) root         (0)     6747 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/migrations/0035_version_3_14_0.py
+-rw-rw-rw-   0 root         (0) root         (0)     7792 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/migrations/0036_version_3_15_0.py
+-rw-rw-rw-   0 root         (0) root         (0)     3717 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/migrations/0037_version_3_16_0.py
+-rw-rw-rw-   0 root         (0) root         (0)      935 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/migrations/0038_version_4_0_0.py
+-rw-rw-rw-   0 root         (0) root         (0)     3601 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/migrations/0039_version_4_1_0.py
+-rw-rw-rw-   0 root         (0) root         (0)     2444 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/migrations/0040_version_4_2_0.py
+-rw-rw-rw-   0 root         (0) root         (0)      487 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/migrations/0041_version_4_2_1.py
+-rw-rw-rw-   0 root         (0) root         (0)    16454 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/migrations/0042_version_4_3_0.py
+-rw-rw-rw-   0 root         (0) root         (0)      524 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/migrations/0043_version_4_3_2.py
+-rw-rw-rw-   0 root         (0) root         (0)     5420 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/migrations/0044_version_4_4_0.py
+-rw-rw-rw-   0 root         (0) root         (0)    13653 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/migrations/0045_version_4_5_0.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2304 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/migrations_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     5874 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/mixins.py
+-rw-rw-rw-   0 root         (0) root         (0)     3855 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/model_tree.py
+-rw-rw-rw-   0 root         (0) root         (0)   151437 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     1076 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/parsers.py
+-rw-rw-rw-   0 root         (0) root         (0)      870 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)    49395 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/policy.py
+-rw-rw-rw-   0 root         (0) root         (0)     9943 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/provisioning.py
+-rw-rw-rw-   0 root         (0) root         (0)     5646 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/rates.py
+-rw-rw-rw-   0 root         (0) root         (0)     1037 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/rest_filter_backend.py
+-rw-rw-rw-   0 root         (0) root         (0)     9310 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/serializers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:19:03.455289 NEMO-4.5.0/NEMO/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:19:03.455289 NEMO-4.5.0/NEMO/static/admin/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:19:03.455289 NEMO-4.5.0/NEMO/static/admin/physical_access_level/
+-rw-rw-rw-   0 root         (0) root         (0)      607 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/static/admin/physical_access_level/access_level.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:19:03.456289 NEMO-4.5.0/NEMO/static/admin/questions_preview/
+-rw-rw-rw-   0 root         (0) root         (0)     4122 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/static/admin/questions_preview/questions_preview.css
+-rw-rw-rw-   0 root         (0) root         (0)     1372 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/static/admin/questions_preview/questions_preview.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:19:03.456289 NEMO-4.5.0/NEMO/static/admin/reservation_questions/
+-rw-rw-rw-   0 root         (0) root         (0)      247 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/static/admin/reservation_questions/reservation_questions.js
+-rw-rw-rw-   0 root         (0) root         (0)     1225 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/static/admin/time_options_override.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:19:03.456289 NEMO-4.5.0/NEMO/static/admin/tool/
+-rw-rw-rw-   0 root         (0) root         (0)     1437 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/static/admin/tool/tool.js
+-rw-rw-rw-   0 root         (0) root         (0)     1278 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/static/badge_reader.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:19:03.424289 NEMO-4.5.0/NEMO/static/bootstrap/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:19:03.457289 NEMO-4.5.0/NEMO/static/bootstrap/css/
+-rw-rw-rw-   0 root         (0) root         (0)    22608 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/static/bootstrap/css/bootstrap-theme.css
+-rw-rw-rw-   0 root         (0) root         (0)    43339 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/static/bootstrap/css/bootstrap-theme.css.map
+-rw-rw-rw-   0 root         (0) root         (0)    19963 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/static/bootstrap/css/bootstrap-theme.min.css
+-rw-rw-rw-   0 root         (0) root         (0)   141622 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/static/bootstrap/css/bootstrap.css
+-rw-rw-rw-   0 root         (0) root         (0)   380986 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/static/bootstrap/css/bootstrap.css.map
+-rw-rw-rw-   0 root         (0) root         (0)   117305 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/static/bootstrap/css/bootstrap.min.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:19:03.458289 NEMO-4.5.0/NEMO/static/bootstrap/fonts/
+-rw-rw-rw-   0 root         (0) root         (0)    20127 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.eot
+-rw-rw-rw-   0 root         (0) root         (0)   108738 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.svg
+-rw-rw-rw-   0 root         (0) root         (0)    45404 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.ttf
+-rw-rw-rw-   0 root         (0) root         (0)    23424 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.woff
+-rw-rw-rw-   0 root         (0) root         (0)    18028 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.woff2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:19:03.459289 NEMO-4.5.0/NEMO/static/bootstrap/js/
+-rw-rw-rw-   0 root         (0) root         (0)    67546 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/static/bootstrap/js/bootstrap.js
+-rw-rw-rw-   0 root         (0) root         (0)    35951 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/static/bootstrap/js/bootstrap.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:19:03.459289 NEMO-4.5.0/NEMO/static/datetimepicker/
+-rw-rw-rw-   0 root         (0) root         (0)     9020 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/static/datetimepicker/bootstrap-datetimepicker.css
+-rw-rw-rw-   0 root         (0) root         (0)   105978 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/static/datetimepicker/bootstrap-datetimepicker.js
+-rw-rw-rw-   0 root         (0) root         (0)     1150 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/static/favicon.ico
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:19:03.460289 NEMO-4.5.0/NEMO/static/fullcalendar/
+-rw-rw-rw-   0 root         (0) root         (0)    28531 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/static/fullcalendar/fullcalendar.css
+-rw-rw-rw-   0 root         (0) root         (0)   357749 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/static/fullcalendar/fullcalendar.js
+-rw-rw-rw-   0 root         (0) root         (0)    13687 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/static/fullcalendar/fullcalendar.min.css
+-rw-rw-rw-   0 root         (0) root         (0)   168700 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/static/fullcalendar/fullcalendar.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:19:03.461289 NEMO-4.5.0/NEMO/static/icons/
+-rw-rw-rw-   0 root         (0) root         (0)    24065 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/static/icons/agreement.png
+-rw-rw-rw-   0 root         (0) root         (0)    16685 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/static/icons/caution.png
+-rw-rw-rw-   0 root         (0) root         (0)     4664 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/static/icons/preferences.png
+-rw-rw-rw-   0 root         (0) root         (0)   247387 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/static/jquery.js
+-rw-rw-rw-   0 root         (0) root         (0)    84320 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/static/jquery.min.js
+-rw-rw-rw-   0 root         (0) root         (0)  1183392 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/static/jumbotron_watermark.bmp
+-rw-rw-rw-   0 root         (0) root         (0)     1017 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/static/mobile.js
+-rw-rw-rw-   0 root         (0) root         (0)   174603 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/static/moment.js
+-rw-rw-rw-   0 root         (0) root         (0)    58102 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/static/moment.min.js
+-rw-rw-rw-   0 root         (0) root         (0)    86041 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/static/moment.min.js.map
+-rw-rw-rw-   0 root         (0) root         (0)    15594 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/static/nemo.css
+-rw-rw-rw-   0 root         (0) root         (0)    20155 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/static/nemo.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:19:03.461289 NEMO-4.5.0/NEMO/static/numpad/
+-rw-rw-rw-   0 root         (0) root         (0)    12285 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/static/numpad/custom_numpad.jquery.js
+-rw-rw-rw-   0 root         (0) root         (0)      255 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/static/numpad/numpad.jquery.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:19:03.462289 NEMO-4.5.0/NEMO/static/pickadate/
+-rw-rw-rw-   0 root         (0) root         (0)     3795 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/static/pickadate/default.css
+-rw-rw-rw-   0 root         (0) root         (0)     6040 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/static/pickadate/default.date.css
+-rw-rw-rw-   0 root         (0) root         (0)     2785 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/static/pickadate/default.time.css
+-rw-rw-rw-   0 root         (0) root         (0)    48215 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/static/pickadate/picker.date.js
+-rw-rw-rw-   0 root         (0) root         (0)    36941 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/static/pickadate/picker.js
+-rw-rw-rw-   0 root         (0) root         (0)    31899 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/static/pickadate/picker.time.js
+-rw-rw-rw-   0 root         (0) root         (0)       25 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/static/robots.txt
+-rw-rw-rw-   0 root         (0) root         (0)    48446 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/static/typeahead.jquery.js
+-rw-rw-rw-   0 root         (0) root         (0)    20748 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/static/typeahead.jquery.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:19:03.463289 NEMO-4.5.0/NEMO/static/virtualkeyboard/
+-rw-rw-rw-   0 root         (0) root         (0)   113008 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/static/virtualkeyboard/jquery.keyboard.js
+-rw-rw-rw-   0 root         (0) root         (0)    47325 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/static/virtualkeyboard/jquery.keyboard.min.js
+-rw-rw-rw-   0 root         (0) root         (0)     7848 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/static/virtualkeyboard/keyboard-basic.css
+-rw-rw-rw-   0 root         (0) root         (0)     5889 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/static/virtualkeyboard/keyboard-basic.min.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:19:03.465289 NEMO-4.5.0/NEMO/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:19:03.465289 NEMO-4.5.0/NEMO/templates/abuse/
+-rw-rw-rw-   0 root         (0) root         (0)     4059 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/abuse/abuse.html
+-rw-rw-rw-   0 root         (0) root         (0)      580 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/abuse/user_drill_down.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:19:03.466289 NEMO-4.5.0/NEMO/templates/accounts_and_projects/
+-rw-rw-rw-   0 root         (0) root         (0)     7380 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/accounts_and_projects/account_and_projects.html
+-rw-rw-rw-   0 root         (0) root         (0)     6415 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/accounts_and_projects/accounts_and_projects.html
+-rw-rw-rw-   0 root         (0) root         (0)     2843 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/accounts_and_projects/create_account.html
+-rw-rw-rw-   0 root         (0) root         (0)     5002 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/accounts_and_projects/create_project.html
+-rw-rw-rw-   0 root         (0) root         (0)      888 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/accounts_and_projects/documents_for_project.html
+-rw-rw-rw-   0 root         (0) root         (0)     3530 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/accounts_and_projects/projects.html
+-rw-rw-rw-   0 root         (0) root         (0)      924 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/accounts_and_projects/users_for_project.html
+-rw-rw-rw-   0 root         (0) root         (0)      433 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/acknowledgement.html
+-rw-rw-rw-   0 root         (0) root         (0)     4694 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/alerts.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:19:03.467289 NEMO-4.5.0/NEMO/templates/area_access/
+-rw-rw-rw-   0 root         (0) root         (0)     2951 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/area_access/area_access.html
+-rw-rw-rw-   0 root         (0) root         (0)     1687 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/area_access/calendar_self_login.html
+-rw-rw-rw-   0 root         (0) root         (0)     1111 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/area_access/change_project.html
+-rw-rw-rw-   0 root         (0) root         (0)     1141 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/area_access/login_areas.html
+-rw-rw-rw-   0 root         (0) root         (0)     1245 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/area_access/new_area_access_record.html
+-rw-rw-rw-   0 root         (0) root         (0)     1938 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/area_access/new_area_access_record_details.html
+-rw-rw-rw-   0 root         (0) root         (0)     1454 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/area_access/self_login.html
+-rw-rw-rw-   0 root         (0) root         (0)      837 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/authorization_failed.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:19:03.468289 NEMO-4.5.0/NEMO/templates/base/
+-rw-rw-rw-   0 root         (0) root         (0)      308 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/base/footer.html
+-rw-rw-rw-   0 root         (0) root         (0)      292 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/base/impersonate_header.html
+-rw-rw-rw-   0 root         (0) root         (0)       37 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/base/navbar.html
+-rw-rw-rw-   0 root         (0) root         (0)     7633 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/base/navbar_base.html
+-rw-rw-rw-   0 root         (0) root         (0)      247 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/base/popup.html
+-rw-rw-rw-   0 root         (0) root         (0)     5811 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/base.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:19:03.470289 NEMO-4.5.0/NEMO/templates/calendar/
+-rw-rw-rw-   0 root         (0) root         (0)    24260 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/calendar/calendar.html
+-rw-rw-rw-   0 root         (0) root         (0)     1381 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/calendar/configuration.html
+-rw-rw-rw-   0 root         (0) root         (0)     2834 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/calendar/configuration_helper.html
+-rw-rw-rw-   0 root         (0) root         (0)     1254 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/calendar/policy_dialog.html
+-rw-rw-rw-   0 root         (0) root         (0)     1300 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/calendar/project_choice.html
+-rw-rw-rw-   0 root         (0) root         (0)     1335 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/calendar/proxy_reservation.html
+-rw-rw-rw-   0 root         (0) root         (0)     1862 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/calendar/reservation_event_feed.html
+-rw-rw-rw-   0 root         (0) root         (0)     1619 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/calendar/reservation_questions.html
+-rw-rw-rw-   0 root         (0) root         (0)     1285 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/calendar/reservation_warning.html
+-rw-rw-rw-   0 root         (0) root         (0)     4094 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/calendar/scheduled_outage_information.html
+-rw-rw-rw-   0 root         (0) root         (0)     2011 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/calendar/specific_user_feed.html
+-rw-rw-rw-   0 root         (0) root         (0)     2543 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/calendar/usage_event_feed.html
+-rw-rw-rw-   0 root         (0) root         (0)     6530 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/configuration_agenda.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:19:03.470289 NEMO-4.5.0/NEMO/templates/consumables/
+-rw-rw-rw-   0 root         (0) root         (0)     8048 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/consumables/consumables.html
+-rw-rw-rw-   0 root         (0) root         (0)     1518 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/consumables/consumables_order.html
+-rw-rw-rw-   0 root         (0) root         (0)    11695 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/consumables/recurring_charge.html
+-rw-rw-rw-   0 root         (0) root         (0)     5491 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/consumables/recurring_charges.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:19:03.470289 NEMO-4.5.0/NEMO/templates/contact/
+-rw-rw-rw-   0 root         (0) root         (0)      692 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/contact/contact_staff.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:19:03.473289 NEMO-4.5.0/NEMO/templates/customizations/
+-rw-rw-rw-   0 root         (0) root         (0)     1848 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/customizations/customizations.html
+-rw-rw-rw-   0 root         (0) root         (0)     2318 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/customizations/customizations_application.html
+-rw-rw-rw-   0 root         (0) root         (0)     7799 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/customizations/customizations_calendar.html
+-rw-rw-rw-   0 root         (0) root         (0)     7324 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/customizations/customizations_dashboard.html
+-rw-rw-rw-   0 root         (0) root         (0)     4202 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/customizations/customizations_emails.html
+-rw-rw-rw-   0 root         (0) root         (0)     2545 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/customizations/customizations_interlock.html
+-rw-rw-rw-   0 root         (0) root         (0)     5553 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/customizations/customizations_projects_and_accounts.html
+-rw-rw-rw-   0 root         (0) root         (0)     2224 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/customizations/customizations_rates.html
+-rw-rw-rw-   0 root         (0) root         (0)     3519 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/customizations/customizations_recurring_charges.html
+-rw-rw-rw-   0 root         (0) root         (0)     2183 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/customizations/customizations_remote_work.html
+-rw-rw-rw-   0 root         (0) root         (0)    16061 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/customizations/customizations_requests.html
+-rw-rw-rw-   0 root         (0) root         (0)     3678 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/customizations/customizations_safety.html
+-rw-rw-rw-   0 root         (0) root         (0)    27806 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/customizations/customizations_templates.html
+-rw-rw-rw-   0 root         (0) root         (0)     8661 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/customizations/customizations_tool.html
+-rw-rw-rw-   0 root         (0) root         (0)     1731 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/customizations/customizations_upload.html
+-rw-rw-rw-   0 root         (0) root         (0)     5214 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/customizations/customizations_user.html
+-rw-rw-rw-   0 root         (0) root         (0)      441 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/display_success_and_redirect.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:19:03.473289 NEMO-4.5.0/NEMO/templates/email/
+-rw-rw-rw-   0 root         (0) root         (0)     7800 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/email/compose_email.html
+-rw-rw-rw-   0 root         (0) root         (0)     3153 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/email/email_broadcast.html
+-rw-rw-rw-   0 root         (0) root         (0)     1045 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/email/email_form.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:19:03.474289 NEMO-4.5.0/NEMO/templates/event_details/
+-rw-rw-rw-   0 root         (0) root         (0)      751 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/event_details/area_access_details.html
+-rw-rw-rw-   0 root         (0) root         (0)     1347 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/event_details/outage_details.html
+-rw-rw-rw-   0 root         (0) root         (0)     9603 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/event_details/reservation_details.html
+-rw-rw-rw-   0 root         (0) root         (0)      589 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/event_details/usage_details.html
+-rw-rw-rw-   0 root         (0) root         (0)      426 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/facility_rules.html
+-rw-rw-rw-   0 root         (0) root         (0)     1247 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/feedback.html
+-rw-rw-rw-   0 root         (0) root         (0)      937 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/history.html
+-rw-rw-rw-   0 root         (0) root         (0)     1217 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/impersonate.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:19:03.474289 NEMO-4.5.0/NEMO/templates/jumbotron/
+-rw-rw-rw-   0 root         (0) root         (0)     2059 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/jumbotron/jumbotron.html
+-rw-rw-rw-   0 root         (0) root         (0)     3635 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/jumbotron/jumbotron_content.html
+-rw-rw-rw-   0 root         (0) root         (0)     8671 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/landing.html
+-rw-rw-rw-   0 root         (0) root         (0)     3496 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/login.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:19:03.475289 NEMO-4.5.0/NEMO/templates/maintenance/
+-rw-rw-rw-   0 root         (0) root         (0)     1558 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/maintenance/closed_task_details.html
+-rw-rw-rw-   0 root         (0) root         (0)     5566 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/maintenance/maintenance.html
+-rw-rw-rw-   0 root         (0) root         (0)     7450 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/maintenance/pending_task_details.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:19:03.476289 NEMO-4.5.0/NEMO/templates/mobile/
+-rw-rw-rw-   0 root         (0) root         (0)      762 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/mobile/cancellation_result.html
+-rw-rw-rw-   0 root         (0) root         (0)     1916 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/mobile/choose_item.html
+-rw-rw-rw-   0 root         (0) root         (0)      453 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/mobile/error.html
+-rw-rw-rw-   0 root         (0) root         (0)     1025 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/mobile/individual_outage.html
+-rw-rw-rw-   0 root         (0) root         (0)     2625 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/mobile/individual_reservation.html
+-rw-rw-rw-   0 root         (0) root         (0)     5899 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/mobile/new_reservation.html
+-rw-rw-rw-   0 root         (0) root         (0)      313 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/mobile/no_active_projects.html
+-rw-rw-rw-   0 root         (0) root         (0)      777 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/mobile/reservation_success.html
+-rw-rw-rw-   0 root         (0) root         (0)     1442 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/mobile/view_calendar.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:19:03.477289 NEMO-4.5.0/NEMO/templates/news/
+-rw-rw-rw-   0 root         (0) root         (0)      981 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/news/archived_news.html
+-rw-rw-rw-   0 root         (0) root         (0)     1027 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/news/new_news_form.html
+-rw-rw-rw-   0 root         (0) root         (0)     1198 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/news/news_update_form.html
+-rw-rw-rw-   0 root         (0) root         (0)     2038 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/news/recent_news.html
+-rw-rw-rw-   0 root         (0) root         (0)      209 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/no_project.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:19:03.477289 NEMO-4.5.0/NEMO/templates/occupancy/
+-rw-rw-rw-   0 root         (0) root         (0)      408 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/occupancy/occupancy.html
+-rw-rw-rw-   0 root         (0) root         (0)     1841 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/occupancy/occupancy_content.html
+-rw-rw-rw-   0 root         (0) root         (0)     1147 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/occupancy/occupancy_count.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:19:03.478289 NEMO-4.5.0/NEMO/templates/pagination/
+-rw-rw-rw-   0 root         (0) root         (0)      865 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/pagination/pagination_base.html
+-rw-rw-rw-   0 root         (0) root         (0)      521 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/pagination/pagination_column.html
+-rw-rw-rw-   0 root         (0) root         (0)      673 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/pagination/pagination_pages.html
+-rw-rw-rw-   0 root         (0) root         (0)      642 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/pagination/pagination_selector.html
+-rw-rw-rw-   0 root         (0) root         (0)     2841 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/qualifications.html
+-rw-rw-rw-   0 root         (0) root         (0)     5462 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/refresh_sidebar_icons.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:19:03.478289 NEMO-4.5.0/NEMO/templates/remote_work/
+-rw-rw-rw-   0 root         (0) root         (0)    10561 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/remote_work/remote_work.html
+-rw-rw-rw-   0 root         (0) root         (0)     1081 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/remote_work/remote_work_base.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:19:03.478289 NEMO-4.5.0/NEMO/templates/requests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:19:03.479289 NEMO-4.5.0/NEMO/templates/requests/access_requests/
+-rw-rw-rw-   0 root         (0) root         (0)     7754 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/requests/access_requests/access_request.html
+-rw-rw-rw-   0 root         (0) root         (0)     3450 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/requests/access_requests/access_requests.html
+-rw-rw-rw-   0 root         (0) root         (0)     3480 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/requests/access_requests/access_requests_table.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:19:03.479289 NEMO-4.5.0/NEMO/templates/requests/adjustment_requests/
+-rw-rw-rw-   0 root         (0) root         (0)     8607 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/requests/adjustment_requests/adjustment_request.html
+-rw-rw-rw-   0 root         (0) root         (0)     3733 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/requests/adjustment_requests/adjustment_requests.html
+-rw-rw-rw-   0 root         (0) root         (0)     6659 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/requests/adjustment_requests/adjustment_requests_table.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:19:03.480289 NEMO-4.5.0/NEMO/templates/requests/buddy_requests/
+-rw-rw-rw-   0 root         (0) root         (0)     3910 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/requests/buddy_requests/buddy_request.html
+-rw-rw-rw-   0 root         (0) root         (0)     5602 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/requests/buddy_requests/buddy_requests.html
+-rw-rw-rw-   0 root         (0) root         (0)     4246 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/requests/user_requests.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:19:03.480289 NEMO-4.5.0/NEMO/templates/resources/
+-rw-rw-rw-   0 root         (0) root         (0)     2950 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/resources/modify_resource.html
+-rw-rw-rw-   0 root         (0) root         (0)     3846 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/resources/resource_details.html
+-rw-rw-rw-   0 root         (0) root         (0)     1423 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/resources/resources.html
+-rw-rw-rw-   0 root         (0) root         (0)     3807 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/resources/scheduled_outage.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:19:03.481289 NEMO-4.5.0/NEMO/templates/rest_framework/
+-rw-rw-rw-   0 root         (0) root         (0)     2736 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/rest_framework/api.html
+-rw-rw-rw-   0 root         (0) root         (0)      446 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/rest_framework/custom_error.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:19:03.482289 NEMO-4.5.0/NEMO/templates/safety/
+-rw-rw-rw-   0 root         (0) root         (0)     3112 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/safety/safety.html
+-rw-rw-rw-   0 root         (0) root         (0)     1831 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/safety/safety_base.html
+-rw-rw-rw-   0 root         (0) root         (0)     7754 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/safety/safety_data_sheets.html
+-rw-rw-rw-   0 root         (0) root         (0)     1990 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/safety/safety_issues.html
+-rw-rw-rw-   0 root         (0) root         (0)     1723 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/safety/safety_issues_create.html
+-rw-rw-rw-   0 root         (0) root         (0)     1722 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/safety/safety_issues_resolved.html
+-rw-rw-rw-   0 root         (0) root         (0)     1762 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/safety/safety_issues_update.html
+-rw-rw-rw-   0 root         (0) root         (0)     1713 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/safety/safety_items.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:19:03.482289 NEMO-4.5.0/NEMO/templates/snippets/
+-rw-rw-rw-   0 root         (0) root         (0)      516 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/snippets/button.html
+-rw-rw-rw-   0 root         (0) root         (0)      904 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/snippets/contact_person.html
+-rw-rw-rw-   0 root         (0) root         (0)     1128 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/snippets/embedded_document.html
+-rw-rw-rw-   0 root         (0) root         (0)     1673 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/snippets/tool_info.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:19:03.483289 NEMO-4.5.0/NEMO/templates/staff_charges/
+-rw-rw-rw-   0 root         (0) root         (0)      860 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/staff_charges/change_status.html
+-rw-rw-rw-   0 root         (0) root         (0)     1242 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/staff_charges/choose_project.html
+-rw-rw-rw-   0 root         (0) root         (0)      498 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/staff_charges/end_area_charge.html
+-rw-rw-rw-   0 root         (0) root         (0)     1198 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/staff_charges/new_staff_charge.html
+-rw-rw-rw-   0 root         (0) root         (0)      953 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/staff_charges/reminder.html
+-rw-rw-rw-   0 root         (0) root         (0)     1854 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/staff_charges/staff_charges_base.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:19:03.484289 NEMO-4.5.0/NEMO/templates/status_dashboard/
+-rw-rw-rw-   0 root         (0) root         (0)     1554 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/status_dashboard/occupancy.html
+-rw-rw-rw-   0 root         (0) root         (0)     8659 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/status_dashboard/staff.html
+-rw-rw-rw-   0 root         (0) root         (0)     7728 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/status_dashboard/staff_absence.html
+-rw-rw-rw-   0 root         (0) root         (0)     5799 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/status_dashboard/status_dashboard.html
+-rw-rw-rw-   0 root         (0) root         (0)     3534 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/status_dashboard/tools.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:19:03.485289 NEMO-4.5.0/NEMO/templates/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)     2542 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/tasks/resolve.html
+-rw-rw-rw-   0 root         (0) root         (0)     5037 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/tasks/update.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:19:03.486289 NEMO-4.5.0/NEMO/templates/tool_control/
+-rw-rw-rw-   0 root         (0) root         (0)      873 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/tool_control/get_projects.html
+-rw-rw-rw-   0 root         (0) root         (0)      679 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/tool_control/interlock_error.html
+-rw-rw-rw-   0 root         (0) root         (0)     3502 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/tool_control/past_tasks_and_comments.html
+-rw-rw-rw-   0 root         (0) root         (0)     2472 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/tool_control/qualified_users.html
+-rw-rw-rw-   0 root         (0) root         (0)    15540 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/tool_control/tool_control.html
+-rw-rw-rw-   0 root         (0) root         (0)    36294 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/tool_control/tool_status.html
+-rw-rw-rw-   0 root         (0) root         (0)     6142 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/tool_control/usage_data.html
+-rw-rw-rw-   0 root         (0) root         (0)      409 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/tool_control/use_tool_for_other.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:19:03.487289 NEMO-4.5.0/NEMO/templates/training/
+-rw-rw-rw-   0 root         (0) root         (0)      512 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/training/get_projects.html
+-rw-rw-rw-   0 root         (0) root         (0)     4964 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/training/training.html
+-rw-rw-rw-   0 root         (0) root         (0)     1596 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/training/training_entry.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:19:03.487289 NEMO-4.5.0/NEMO/templates/usage/
+-rw-rw-rw-   0 root         (0) root         (0)      495 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/usage/adjustment_request_button.html
+-rw-rw-rw-   0 root         (0) root         (0)     3573 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/usage/billing.html
+-rw-rw-rw-   0 root         (0) root         (0)     9302 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/usage/usage.html
+-rw-rw-rw-   0 root         (0) root         (0)     6781 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/usage/usage_base.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:19:03.488289 NEMO-4.5.0/NEMO/templates/users/
+-rw-rw-rw-   0 root         (0) root         (0)    20751 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/users/create_or_modify_user.html
+-rw-rw-rw-   0 root         (0) root         (0)     8054 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/users/preferences.html
+-rw-rw-rw-   0 root         (0) root         (0)     3758 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/users/safe_deactivation.html
+-rw-rw-rw-   0 root         (0) root         (0)     4160 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templates/users/users.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:19:03.488289 NEMO-4.5.0/NEMO/templatetags/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templatetags/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7211 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/templatetags/custom_tags_and_filters.py
+-rw-rw-rw-   0 root         (0) root         (0)    25064 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)    23455 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:19:03.495289 NEMO-4.5.0/NEMO/views/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/views/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4308 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/views/abuse.py
+-rw-rw-rw-   0 root         (0) root         (0)    14736 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/views/access_requests.py
+-rw-rw-rw-   0 root         (0) root         (0)     8275 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/views/accounts_and_projects.py
+-rw-rw-rw-   0 root         (0) root         (0)    17076 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/views/adjustment_requests.py
+-rw-rw-rw-   0 root         (0) root         (0)     1812 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/views/alerts.py
+-rw-rw-rw-   0 root         (0) root         (0)    13935 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/views/api.py
+-rw-rw-rw-   0 root         (0) root         (0)    12115 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/views/api_billing.py
+-rw-rw-rw-   0 root         (0) root         (0)     2013 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/views/api_file_import.py
+-rw-rw-rw-   0 root         (0) root         (0)    18830 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/views/area_access.py
+-rw-rw-rw-   0 root         (0) root         (0)    11992 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/views/authentication.py
+-rw-rw-rw-   0 root         (0) root         (0)     6625 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/views/buddy_requests.py
+-rw-rw-rw-   0 root         (0) root         (0)    68771 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/views/calendar.py
+-rw-rw-rw-   0 root         (0) root         (0)     1867 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/views/configuration_agenda.py
+-rw-rw-rw-   0 root         (0) root         (0)      174 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/views/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)    10021 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/views/consumables.py
+-rw-rw-rw-   0 root         (0) root         (0)      467 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/views/contact_staff.py
+-rw-rw-rw-   0 root         (0) root         (0)    17713 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/views/customization.py
+-rw-rw-rw-   0 root         (0) root         (0)     1335 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/views/documents.py
+-rw-rw-rw-   0 root         (0) root         (0)     9978 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/views/email.py
+-rw-rw-rw-   0 root         (0) root         (0)     1973 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/views/event_details.py
+-rw-rw-rw-   0 root         (0) root         (0)     1482 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/views/feedback.py
+-rw-rw-rw-   0 root         (0) root         (0)     1672 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/views/get_projects.py
+-rw-rw-rw-   0 root         (0) root         (0)     4168 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/views/history.py
+-rw-rw-rw-   0 root         (0) root         (0)     1027 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/views/jumbotron.py
+-rw-rw-rw-   0 root         (0) root         (0)     3293 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/views/landing.py
+-rw-rw-rw-   0 root         (0) root         (0)     2289 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/views/maintenance.py
+-rw-rw-rw-   0 root         (0) root         (0)     8059 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/views/mobile.py
+-rw-rw-rw-   0 root         (0) root         (0)     3356 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/views/news.py
+-rw-rw-rw-   0 root         (0) root         (0)     5188 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/views/notifications.py
+-rw-rw-rw-   0 root         (0) root         (0)     1326 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/views/pagination.py
+-rw-rw-rw-   0 root         (0) root         (0)     4822 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/views/qualifications.py
+-rw-rw-rw-   0 root         (0) root         (0)     9965 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/views/remote_work.py
+-rw-rw-rw-   0 root         (0) root         (0)     3700 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/views/resources.py
+-rw-rw-rw-   0 root         (0) root         (0)     8877 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/views/safety.py
+-rw-rw-rw-   0 root         (0) root         (0)      932 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/views/sidebar.py
+-rw-rw-rw-   0 root         (0) root         (0)    19900 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/views/status_dashboard.py
+-rw-rw-rw-   0 root         (0) root         (0)    12963 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/views/tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)    23605 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/views/tool_control.py
+-rw-rw-rw-   0 root         (0) root         (0)     5953 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/views/training.py
+-rw-rw-rw-   0 root         (0) root         (0)     1909 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/views/tutorials.py
+-rw-rw-rw-   0 root         (0) root         (0)    18008 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/views/usage.py
+-rw-rw-rw-   0 root         (0) root         (0)     1049 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/views/user_requests.py
+-rw-rw-rw-   0 root         (0) root         (0)    20715 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/views/users.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:19:03.496289 NEMO-4.5.0/NEMO/widgets/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/widgets/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2968 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/widgets/configuration_editor.py
+-rw-rw-rw-   0 root         (0) root         (0)    26295 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/widgets/dynamic_form.py
+-rw-rw-rw-   0 root         (0) root         (0)     8029 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/widgets/item_tree.py
+-rw-rw-rw-   0 root         (0) root         (0)       88 2023-04-11 20:18:49.000000 NEMO-4.5.0/NEMO/wsgi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:19:03.434289 NEMO-4.5.0/NEMO.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      904 2023-04-11 20:19:03.000000 NEMO-4.5.0/NEMO.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    16399 2023-04-11 20:19:03.000000 NEMO-4.5.0/NEMO.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 20:19:03.000000 NEMO-4.5.0/NEMO.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2023-04-11 20:19:03.000000 NEMO-4.5.0/NEMO.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      263 2023-04-11 20:19:03.000000 NEMO-4.5.0/NEMO.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-04-11 20:19:03.000000 NEMO-4.5.0/NEMO.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      904 2023-04-11 20:19:03.496289 NEMO-4.5.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4098 2023-04-11 20:18:49.000000 NEMO-4.5.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:19:03.496289 NEMO-4.5.0/resources/
+-rw-rw-rw-   0 root         (0) root         (0)     3957 2023-04-11 20:18:49.000000 NEMO-4.5.0/resources/splash_pad_settings.py
+-rw-r--r--   0 root         (0) root         (0)      109 2023-04-11 20:19:03.497289 NEMO-4.5.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1460 2023-04-11 20:18:49.000000 NEMO-4.5.0/setup.py
```

### Comparing `NEMO-4.4.1/LICENSE.md` & `NEMO-4.5.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/actions.py` & `NEMO-4.5.0/NEMO/actions.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,43 +1,67 @@
-from django.contrib import messages
+from django.contrib import admin, messages
+from django.db.models import Max
 from django.urls import reverse
 from django.utils.safestring import mark_safe
 
-from NEMO.models import User, Area, Tool
+from NEMO.models import Area, Interlock, Tool, User
+from NEMO.views.access_requests import access_csv_export
+from NEMO.views.adjustment_requests import adjustments_csv_export
 
 
+@admin.action(description="Lock selected interlocks")
 def lock_selected_interlocks(model_admin, request, queryset):
 	for interlock in queryset:
 		try:
-			interlock.lock()
-			messages.success(request, f"{interlock} has been successfully locked")
+			command_succeeded = interlock.lock()
+			if command_succeeded:
+				messages.success(request, f"{interlock} has been successfully locked")
+			else:
+				messages.error(request, f"{interlock} could not be locked. {interlock.most_recent_reply}")
 		except Exception as error:
 			messages.error(request, f"{interlock} could not be locked due to the following error: {str(error)}")
 
 
+@admin.action(description="Unlock selected interlocks")
 def unlock_selected_interlocks(model_admin, request, queryset):
 	for interlock in queryset:
 		try:
-			interlock.unlock()
-			messages.success(request, f"{interlock} has been successfully unlocked")
+			command_succeeded = interlock.unlock()
+			if command_succeeded:
+				messages.success(request, f"{interlock} has been successfully unlocked")
+			else:
+				messages.error(request, f"{interlock} could not be unlocked. {interlock.most_recent_reply}")
 		except Exception as error:
 			messages.error(request, f"{interlock} could not be unlocked due to the following error: {str(error)}")
 
 
+@admin.action(description="Synchronize selected interlocks with tool usage")
 def synchronize_with_tool_usage(model_admin, request, queryset):
 	for interlock in queryset:
 		# Ignore interlocks with no tool assigned, and ignore interlocks connected to doors
 		if not hasattr(interlock, "tool") or hasattr(interlock, "door"):
 			continue
 		if interlock.tool.in_use():
 			interlock.unlock()
 		else:
 			interlock.lock()
 
 
+@admin.action(description="Create next interlock")
+def create_next_interlock(model_admin, request, queryset):
+	for interlock in queryset:
+		new_interlock = Interlock()
+		new_interlock.card = interlock.card
+		new_interlock.unit_id = interlock.unit_id
+		max_channel = Interlock.objects.filter(card=interlock.card).aggregate(Max("channel"))["channel__max"]
+		new_interlock.channel = max_channel + 1 if max_channel is not None else None
+		new_interlock.save()
+
+
+@admin.action(description="Duplicate selected tool configuration")
 def duplicate_tool_configuration(model_admin, request, queryset):
 	for tool in queryset:
 		original_name = tool.name
 		new_name = "Copy of " + tool.name
 		try:
 			if Tool.objects.filter(name=new_name).exists():
 				messages.error(
@@ -79,9 +103,20 @@
 				)
 		except Exception as error:
 			messages.error(
 				request, f"{original_name} could not be duplicated because of the following error: {str(error)}"
 			)
 
 
+@admin.action(description="Rebuild area tree")
 def rebuild_area_tree(model_admin, request, queryset):
 	Area.objects.rebuild()
+
+
+@admin.action(description="Export selected adjustment requests in CSV")
+def adjustment_requests_export_csv(modeladmin, request, queryset):
+	return adjustments_csv_export(queryset.all())
+
+
+@admin.action(description="Export selected access requests in CSV")
+def access_requests_export_csv(modeladmin, request, queryset):
+	return access_csv_export(queryset.all())
```

### Comparing `NEMO-4.4.1/NEMO/admin.py` & `NEMO-4.5.0/NEMO/admin.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,71 +4,74 @@
 
 from django import forms
 from django.contrib import admin
 from django.contrib.admin import register
 from django.contrib.admin.decorators import display
 from django.contrib.admin.widgets import FilteredSelectMultiple
 from django.contrib.auth.models import Permission
+from django.contrib.contenttypes.admin import GenericStackedInline
 from django.db.models import Q
 from django.db.models.fields.files import FieldFile
 from django.forms import BaseInlineFormSet
 from django.template.defaultfilters import linebreaksbr, urlencode
-from django.urls import reverse
-from django.utils.html import format_html
 from django.utils.safestring import mark_safe
 from mptt.admin import DraggableMPTTAdmin, MPTTAdminForm, TreeRelatedFieldListFilter
 
 from NEMO.actions import (
+	access_requests_export_csv,
+	adjustment_requests_export_csv,
+	create_next_interlock,
 	duplicate_tool_configuration,
 	lock_selected_interlocks,
 	rebuild_area_tree,
 	synchronize_with_tool_usage,
 	unlock_selected_interlocks,
 )
 from NEMO.forms import BuddyRequestForm, RecurringConsumableChargeForm, UserPreferencesForm
 from NEMO.models import (
 	Account,
 	AccountType,
 	ActivityHistory,
+	AdjustmentRequest,
 	Alert,
 	AlertCategory,
 	Area,
 	AreaAccessRecord,
 	BadgeReader,
 	BuddyRequest,
-	BuddyRequestMessage,
 	Chemical,
 	ChemicalHazard,
 	Closure,
 	ClosureTime,
 	Comment,
 	Configuration,
 	ConfigurationHistory,
 	Consumable,
 	ConsumableCategory,
 	ConsumableWithdraw,
 	ContactInformation,
 	ContactInformationCategory,
 	Customization,
-	Discipline,
 	Door,
 	EmailLog,
 	Interlock,
 	InterlockCard,
 	InterlockCardCategory,
 	LandingPageChoice,
 	MembershipHistory,
 	News,
 	Notification,
 	OnboardingPhase,
 	PhysicalAccessLevel,
 	PhysicalAccessLog,
 	Project,
+	ProjectDiscipline,
 	ProjectDocuments,
 	RecurringConsumableCharge,
+	RequestMessage,
 	Reservation,
 	ReservationQuestions,
 	Resource,
 	ResourceCategory,
 	SafetyCategory,
 	SafetyIssue,
 	SafetyItem,
@@ -86,31 +89,29 @@
 	TaskHistory,
 	TaskImages,
 	TaskStatus,
 	TemporaryPhysicalAccess,
 	TemporaryPhysicalAccessRequest,
 	Tool,
 	ToolDocuments,
+	ToolQualificationGroup,
 	ToolUsageCounter,
 	TrainingSession,
 	UsageEvent,
 	User,
 	UserDocuments,
 	UserPreferences,
 	UserType,
 	record_active_state,
 	record_local_many_to_many_changes,
 	record_remote_many_to_many_changes_and_save,
 )
-from NEMO.utilities import format_daterange
-from NEMO.widgets.dynamic_form import (
-	DynamicForm,
-	PostUsageFloatFieldQuestion,
-	PostUsageNumberFieldQuestion,
-)
+from NEMO.utilities import admin_get_item, format_daterange
+from NEMO.views.customization import ProjectsAccountsCustomization
+from NEMO.widgets.dynamic_form import DynamicForm, PostUsageFloatFieldQuestion, PostUsageNumberFieldQuestion
 
 
 # Formset to require at least one inline form
 class AtLeastOneRequiredInlineFormSet(BaseInlineFormSet):
 	def clean(self):
 		super().clean()
 		if any(self.errors):
@@ -155,67 +156,23 @@
 		if self.instance.pk:
 			self.fields["qualified_users"].initial = self.instance.user_set.all()
 			self.fields["required_resources"].initial = self.instance.required_resource_set.all()
 			self.fields["nonrequired_resources"].initial = self.instance.nonrequired_resource_set.all()
 
 	def clean(self):
 		cleaned_data = super().clean()
-		parent_tool = cleaned_data.get("parent_tool")
-		category = cleaned_data.get("_category")
-		location = cleaned_data.get("_location")
-		phone_number = cleaned_data.get("_phone_number")
-		primary_owner = cleaned_data.get("_primary_owner")
 		image = cleaned_data.get("_image")
 
 		# only resize if an image is present and has changed
 		if image and not isinstance(image, FieldFile):
 			from NEMO.utilities import resize_image
 
 			# resize image to 500x500 maximum
 			cleaned_data["_image"] = resize_image(image, 500)
 
-		if parent_tool:
-			if parent_tool.id == self.instance.id:
-				self.add_error("parent_tool", "You cannot select the parent to be the tool itself.")
-			# in case of alternate tool, remove everything except parent_tool and name
-			data = dict([(k, v) for k, v in self.cleaned_data.items() if k == "parent_tool" or k == "name"])
-			# an alternate tool is never visible
-			data["visible"] = False
-			return data
-		else:
-			if not category:
-				self.add_error("_category", "This field is required.")
-			if not location:
-				self.add_error("_location", "This field is required.")
-			if not phone_number:
-				self.add_error("_phone_number", "This field is required.")
-			if not primary_owner:
-				self.add_error("_primary_owner", "This field is required.")
-
-			post_usage_questions = cleaned_data.get("_post_usage_questions")
-			# Validate _post_usage_questions JSON format
-			if post_usage_questions:
-				try:
-					loads(post_usage_questions)
-				except ValueError:
-					self.add_error("_post_usage_questions", "This field needs to be a valid JSON string")
-				try:
-					DynamicForm(post_usage_questions).validate("tool_usage_group_question", self.instance.id)
-				except Exception:
-					error_info = sys.exc_info()
-					self.add_error("_post_usage_questions", error_info[0].__name__ + ": " + str(error_info[1]))
-
-			policy_off_between_times = cleaned_data.get("_policy_off_between_times")
-			policy_off_start_time = cleaned_data.get("_policy_off_start_time")
-			policy_off_end_time = cleaned_data.get("_policy_off_end_time")
-			if policy_off_between_times and (not policy_off_start_time or not policy_off_end_time):
-				if not policy_off_start_time:
-					self.add_error("_policy_off_start_time", "Start time must be specified")
-				if not policy_off_end_time:
-					self.add_error("_policy_off_end_time", "End time must be specified")
 		return cleaned_data
 
 
 class ToolDocumentsInline(admin.TabularInline):
 	model = ToolDocuments
 	extra = 1
 
@@ -226,19 +183,20 @@
 	list_display = (
 		"name_display",
 		"_category",
 		"visible",
 		"operational_display",
 		"problematic",
 		"is_configurable",
+		"has_post_usage_questions",
 		"id",
 	)
 	filter_horizontal = ("_backup_owners", "_superusers")
 	search_fields = ("name", "_description", "_serial")
-	list_filter = ("visible", "_operational", "_category", "_location")
+	list_filter = ("visible", "_operational", "_category", "_location", ("_requires_area_access", admin.RelatedOnlyFieldListFilter))
 	readonly_fields = ("_post_usage_preview",)
 	actions = [duplicate_tool_configuration]
 	form = ToolAdminForm
 	fieldsets = (
 		(
 			None,
 			{
@@ -295,51 +253,62 @@
 					"_allow_delayed_logoff",
 				)
 			},
 		),
 		("Dependencies", {"fields": ("required_resources", "nonrequired_resources")}),
 	)
 
+	@admin.display(description="Questions", ordering="post_usage_questions", boolean=True)
+	def has_post_usage_questions(self, obj: Tool):
+		return True if obj.post_usage_questions else False
+
 	def _post_usage_preview(self, obj):
 		if obj.id:
 			form_validity_div = '<div id="form_validity"></div>' if obj.post_usage_questions else ""
 			return mark_safe(
 				'<div class="questions_preview">{}{}</div><div class="help questions_preview_help">Save form to preview post usage questions</div>'.format(
 					DynamicForm(obj.post_usage_questions).render("tool_usage_group_question", obj.id), form_validity_div
 				)
 			)
 
 	def formfield_for_foreignkey(self, db_field, request, **kwargs):
 		""" We only want non children tool to be eligible as parents """
 		if db_field.name == "parent_tool":
 			kwargs["queryset"] = Tool.objects.filter(parent_tool__isnull=True)
+		# Limit interlock selection to ones not already linked
+		if db_field.name == "_interlock":
+			kwargs["queryset"] = Interlock.objects.filter(tool__isnull=True, door__isnull=True)
 		return super().formfield_for_foreignkey(db_field, request, **kwargs)
 
 	def save_model(self, request, obj, form, change):
 		"""
-		Explicitly record any project membership changes.
+		Explicitly record any project membership changes on non-child tools.
 		"""
 		if obj.parent_tool:
-			if obj.pk:
-				# if this is an update (from regular to child tool), we want to make sure we are creating
-				# a clean version. In case the previous tool had fields that are now irrelevant
-				clean_alt_tool = Tool(**form.cleaned_data)
-				clean_alt_tool.pk = obj.pk
-				obj = clean_alt_tool
 			super(ToolAdmin, self).save_model(request, obj, form, change)
 		else:
 			record_remote_many_to_many_changes_and_save(
 				request, obj, form, change, "qualified_users", super(ToolAdmin, self).save_model
 			)
 			if "required_resources" in form.changed_data:
 				obj.required_resource_set.set(form.cleaned_data["required_resources"])
 			if "nonrequired_resources" in form.changed_data:
 				obj.nonrequired_resource_set.set(form.cleaned_data["nonrequired_resources"])
 
 
+@register(ToolQualificationGroup)
+class ToolQualificationGroup(admin.ModelAdmin):
+	list_display = ["name", "get_tools"]
+	filter_horizontal = ["tools"]
+
+	@admin.display(description="Tools", ordering="tools")
+	def get_tools(self, obj: ToolQualificationGroup):
+		return mark_safe("<br>".join([str(tool) for tool in obj.tools.all()]))
+
+
 class AreaAdminForm(MPTTAdminForm):
 	class Meta:
 		model = Area
 		fields = "__all__"
 
 	area_calendar_color = forms.CharField(
 		required=False, max_length=9, initial="#88B7CD", widget=forms.TextInput(attrs={"type": "color"})
@@ -419,28 +388,28 @@
 			parent_area.is_now_a_parent()
 		super(AreaAdmin, self).save_model(request, obj, form, change)
 
 
 @register(TrainingSession)
 class TrainingSessionAdmin(admin.ModelAdmin):
 	list_display = ("id", "trainer", "trainee", "tool", "project", "type", "date", "duration", "qualified")
-	list_filter = ("qualified", "date", "type", "tool")
+	list_filter = ("qualified", "date", "type", ("tool", admin.RelatedOnlyFieldListFilter), ("project", admin.RelatedOnlyFieldListFilter), ("trainer", admin.RelatedOnlyFieldListFilter), ("trainee", admin.RelatedOnlyFieldListFilter))
 	date_hierarchy = "date"
 
 	def formfield_for_foreignkey(self, db_field, request, **kwargs):
 		""" We only want staff user and tool superusers to be possible trainers """
 		if db_field.name == "trainer":
 			kwargs["queryset"] = User.objects.filter(Q(is_staff=True) | Q(superuser_for_tools__isnull=False)).distinct()
 		return super().formfield_for_foreignkey(db_field, request, **kwargs)
 
 
 @register(StaffCharge)
 class StaffChargeAdmin(admin.ModelAdmin):
 	list_display = ("id", "staff_member", "customer", "start", "end")
-	list_filter = ("start",)
+	list_filter = ("start", ("customer", admin.RelatedOnlyFieldListFilter), ("staff_member", admin.RelatedOnlyFieldListFilter))
 	date_hierarchy = "start"
 
 
 @register(AreaAccessRecord)
 class AreaAccessRecordAdmin(admin.ModelAdmin):
 	list_display = ("id", "customer", "area", "project", "start", "end")
 	list_filter = (("area", TreeRelatedFieldListFilter), "start")
@@ -467,15 +436,15 @@
 	date_hierarchy = "modification_time"
 
 
 @register(Account)
 class AccountAdmin(admin.ModelAdmin):
 	list_display = ("name", "id", "active", "type", "start_date")
 	search_fields = ("name",)
-	list_filter = ("active", "type", "start_date")
+	list_filter = ("active", ("type", admin.RelatedOnlyFieldListFilter), "start_date")
 
 	def save_model(self, request, obj, form, change):
 		""" Audit account and project active status. """
 		super(AccountAdmin, self).save_model(request, obj, form, change)
 		record_active_state(request, obj, form, "active", not change)
 
 
@@ -494,44 +463,38 @@
 		queryset=User.objects.all(),
 		required=False,
 		widget=FilteredSelectMultiple(verbose_name="Principal investigators", is_stacked=False),
 	)
 
 	def __init__(self, *args, **kwargs):
 		super(ProjectAdminForm, self).__init__(*args, **kwargs)
+		self.fields["application_identifier"].label = ProjectsAccountsCustomization.get("project_application_identifier_name")
 		if self.instance.pk:
 			self.fields["members"].initial = self.instance.user_set.all()
 			self.fields["principal_investigators"].initial = self.instance.manager_set.all()
 
 
 class ProjectDocumentsInline(admin.TabularInline):
 	model = ProjectDocuments
 	extra = 1
 
 
 @register(Project)
 class ProjectAdmin(admin.ModelAdmin):
-	fields = (
-		"name",
-		"application_identifier",
-		"account",
-		"start_date",
-		"allow_consumable_withdrawals",
-		"active",
-		"members",
-		"principal_investigators",
-		"only_allow_tools",
-	)
-	list_display = ("name", "id", "application_identifier", "account", "active", "start_date")
+	list_display = ("name", "id", "get_application_identifier", "account", "active", "start_date")
 	filter_horizontal = ("only_allow_tools",)
 	search_fields = ("name", "application_identifier", "account__name")
-	list_filter = ("active", "account", "start_date")
-	inlines = (ProjectDocumentsInline,)
+	list_filter = ("active", ("account", admin.RelatedOnlyFieldListFilter), "start_date")
+	inlines = [ProjectDocumentsInline]
 	form = ProjectAdminForm
 
+	@display(ordering="application_identifier")
+	def get_application_identifier(self, project: Project):
+		return project.application_identifier
+
 	def save_model(self, request, obj, form, change):
 		"""
 		Audit project creation and modification. Also save any project membership changes explicitly.
 		"""
 		record_remote_many_to_many_changes_and_save(
 			request, obj, form, change, "members", super(ProjectAdmin, self).save_model
 		)
@@ -575,15 +538,15 @@
 		"end",
 		"duration",
 		"cancelled",
 		"missed",
 		"shortened",
 	)
 	readonly_fields = ("descendant",)
-	list_filter = ("cancelled", "missed", "tool", "area")
+	list_filter = ("cancelled", "missed", ("tool", admin.RelatedOnlyFieldListFilter), ("area", TreeRelatedFieldListFilter), ("user", admin.RelatedOnlyFieldListFilter))
 	date_hierarchy = "start"
 
 
 class ReservationQuestionsForm(forms.ModelForm):
 	class Meta:
 		model = ReservationQuestions
 		fields = "__all__"
@@ -664,43 +627,44 @@
 				rendered_form, form_validity_div
 			)
 		)
 
 
 @register(UsageEvent)
 class UsageEventAdmin(admin.ModelAdmin):
-	list_display = ("id", "tool", "user", "operator", "project", "start", "end", "duration")
-	list_filter = ("start", "end", "tool")
+	list_display = ("id", "tool", "user", "operator", "project", "start", "end", "duration", "remote_work")
+	list_filter = ("remote_work", "start", "end", ("tool", admin.RelatedOnlyFieldListFilter))
 	date_hierarchy = "start"
 
 
 @register(Consumable)
 class ConsumableAdmin(admin.ModelAdmin):
 	list_display = ("name", "quantity", "category", "visible", "reusable", "reminder_threshold", "reminder_email", "id")
-	list_filter = ("visible", "category", "reusable")
+	list_filter = ("visible", ("category", admin.RelatedOnlyFieldListFilter), "reusable")
 	search_fields = ("name",)
 	readonly_fields = ("reminder_threshold_reached",)
 
 
 @register(ConsumableCategory)
 class ConsumableCategoryAdmin(admin.ModelAdmin):
 	list_display = ("name",)
 
 
 @register(ConsumableWithdraw)
 class ConsumableWithdrawAdmin(admin.ModelAdmin):
 	list_display = ("id", "customer", "merchant", "consumable", "quantity", "project", "date")
-	list_filter = ("date", "consumable")
+	list_filter = ("date", ("consumable", admin.RelatedOnlyFieldListFilter))
 	date_hierarchy = "date"
 
 
 @register(RecurringConsumableCharge)
 class RecurringConsumableChargeAdmin(admin.ModelAdmin):
 	form = RecurringConsumableChargeForm
 	list_display = ("name", "customer", "project", "get_recurrence_display", "last_charge", "next_charge")
+	list_filter = (("customer", admin.RelatedOnlyFieldListFilter),)
 	readonly_fields = ("last_charge", "last_updated", "last_updated_by")
 
 	def save_model(self, request, obj: RecurringConsumableCharge, form, change):
 		obj.save_with_user(request.user)
 
 
 class InterlockCardAdminForm(forms.ModelForm):
@@ -752,16 +716,16 @@
 		"channel",
 		"unit_id",
 		"state",
 		"tool",
 		"door",
 		"most_recent_reply_time"
 	)
-	list_filter = ("card__enabled", "card", "state")
-	actions = [lock_selected_interlocks, unlock_selected_interlocks, synchronize_with_tool_usage]
+	list_filter = ("card__enabled", ("card", admin.RelatedOnlyFieldListFilter), "state", ("tool", admin.RelatedOnlyFieldListFilter), ("door", admin.RelatedOnlyFieldListFilter))
+	actions = [lock_selected_interlocks, unlock_selected_interlocks, synchronize_with_tool_usage, create_next_interlock]
 	readonly_fields = ["state", "most_recent_reply", "most_recent_reply_time"]
 
 	@display(boolean=True, ordering='card__enabled', description='Card Enabled')
 	def get_card_enabled(self, obj):
 		return obj.card.enabled
 
 
@@ -780,15 +744,15 @@
 		"creation_time",
 		"last_updated",
 		"problem_category",
 		"cancelled",
 		"resolved",
 		"resolution_category",
 	)
-	list_filter = ("urgency", "resolved", "cancelled", "safety_hazard", "creation_time", "tool")
+	list_filter = ("urgency", "resolved", "cancelled", "safety_hazard", "creation_time", ("tool", admin.RelatedOnlyFieldListFilter), ("creator", admin.RelatedOnlyFieldListFilter))
 	date_hierarchy = "creation_time"
 
 
 @register(TaskCategory)
 class TaskCategoryAdmin(admin.ModelAdmin):
 	list_display = ("name", "stage")
 
@@ -811,75 +775,86 @@
 	date_hierarchy = "time"
 
 
 @register(TaskImages)
 class TaskImagesAdmin(admin.ModelAdmin):
 	list_display = ("id", "get_tool", "task", "uploaded_at")
 
+	@admin.display(ordering="tool", description="Tool Name")
 	def get_tool(self, task_image: TaskImages):
 		return task_image.task.tool.name
 
-	get_tool.admin_order_field = "tool"  # Allows column order sorting
-	get_tool.short_description = "Tool Name"  # Renames column head
-
 
 @register(Comment)
 class CommentAdmin(admin.ModelAdmin):
 	list_display = (
 		"id",
 		"tool",
 		"author",
 		"creation_date",
 		"expiration_date",
 		"visible",
 		"staff_only",
 		"hidden_by",
 		"hide_date",
 	)
-	list_filter = ("visible", "creation_date", "tool", "staff_only")
+	list_filter = ("visible", "creation_date", ("tool", admin.RelatedOnlyFieldListFilter), "staff_only")
 	date_hierarchy = "creation_date"
 	search_fields = ("content",)
 
 
 @register(Resource)
 class ResourceAdmin(admin.ModelAdmin):
 	list_display = ("name", "category", "available")
 	list_filter = ("available", "category")
 	filter_horizontal = ("fully_dependent_tools", "partially_dependent_tools", "dependent_areas")
 
 
 @register(ActivityHistory)
 class ActivityHistoryAdmin(admin.ModelAdmin):
-	list_display = ("__str__", "content_type", "object_id", "action", "date", "authorizer")
+	list_display = ("__str__", "get_item", "action", "date", "authorizer")
+	list_filter = ("action", ("content_type", admin.RelatedOnlyFieldListFilter),)
 	date_hierarchy = "date"
 
+	@admin.display(description="Item")
+	def get_item(self, obj: ActivityHistory):
+		return admin_get_item(obj.content_type, obj.object_id)
+
 
 @register(MembershipHistory)
 class MembershipHistoryAdmin(admin.ModelAdmin):
 	list_display = (
 		"__str__",
-		"parent_content_type",
-		"parent_object_id",
+		"get_parent",
 		"action",
-		"child_content_type",
-		"child_object_id",
+		"get_child",
 		"date",
 		"authorizer",
 	)
+	list_filter = (("parent_content_type", admin.RelatedOnlyFieldListFilter), ("child_content_type", admin.RelatedOnlyFieldListFilter),)
 	date_hierarchy = "date"
 
+	@admin.display(description="Parent")
+	def get_parent(self, obj: MembershipHistory):
+		return admin_get_item(obj.parent_content_type, obj.parent_object_id)
+
+	@admin.display(description="Child")
+	def get_child(self, obj: MembershipHistory):
+		return admin_get_item(obj.child_content_type, obj.child_object_id)
+
 
 @register(UserType)
 class UserTypeAdmin(admin.ModelAdmin):
 	list_display = ("name",)
 
 
 @register(UserPreferences)
 class UserPreferencesAdmin(admin.ModelAdmin):
 	list_display = ("user",)
+	search_fields = ["user_preferences__user__first_name", "user_preferences__user__last_name", "user_preferences__user__username"]
 	form = UserPreferencesForm
 
 
 class UserAdminForm(forms.ModelForm):
 	class Meta:
 		model = User
 		fields = "__all__"
@@ -906,38 +881,24 @@
 	def __init__(self, *args, **kwargs):
 		super().__init__(*args, **kwargs)
 		if self.instance.pk:
 			self.fields["tool_qualifications"].initial = self.instance.qualifications.all()
 			self.fields["backup_owner_on_tools"].initial = self.instance.backup_for_tools.all()
 			self.fields["superuser_on_tools"].initial = self.instance.superuser_for_tools.all()
 
-	def clean(self):
-		cleaned_data = super().clean()
-		staff_status = cleaned_data.get("is_staff")
-		service_personnel_status = cleaned_data.get("is_service_personnel")
-
-		if staff_status and service_personnel_status:
-			raise forms.ValidationError(
-				{
-					"is_staff": "A user cannot be both staff and service personnel. Please choose one or the other.",
-					"is_service_personnel": "A user cannot be both staff and service personnel. Please choose one or the other.",
-				}
-			)
-		return cleaned_data
-
 
 class UserDocumentsInline(admin.TabularInline):
 	model = UserDocuments
 	extra = 1
 
 
 @register(User)
 class UserAdmin(admin.ModelAdmin):
 	form = UserAdminForm
-	inlines = (UserDocumentsInline,)
+	inlines = [UserDocumentsInline]
 	filter_horizontal = (
 		"groups",
 		"user_permissions",
 		"projects",
 		"managed_projects",
 		"physical_access_levels",
 		"onboarding_phases",
@@ -999,17 +960,17 @@
 					"safety_trainings",
 				)
 			},
 		),
 	)
 	search_fields = ("first_name", "last_name", "username", "email")
 	list_display = (
+		"username",
 		"first_name",
 		"last_name",
-		"username",
 		"email",
 		"is_active",
 		"domain",
 		"is_staff",
 		"is_user_office",
 		"is_accounting_officer",
 		"is_technician",
@@ -1047,15 +1008,15 @@
 		if "superuser_on_tools" in form.changed_data:
 			obj.superuser_for_tools.set(form.cleaned_data["superuser_on_tools"])
 
 
 @register(PhysicalAccessLog)
 class PhysicalAccessLogAdmin(admin.ModelAdmin):
 	list_display = ("user", "door", "time", "result")
-	list_filter = ("door", "result")
+	list_filter = (("door", admin.RelatedOnlyFieldListFilter), "result")
 	search_fields = ("user__first_name", "user__last_name", "user__username", "door__name")
 	date_hierarchy = "time"
 
 	def has_delete_permission(self, request, obj=None):
 		return False
 
 	def has_add_permission(self, request):
@@ -1064,15 +1025,15 @@
 	def has_change_permission(self, request, obj=None):
 		return False
 
 
 @register(SafetyIssue)
 class SafetyIssueAdmin(admin.ModelAdmin):
 	list_display = ("id", "reporter", "creation_time", "visible", "resolved", "resolution_time", "resolver")
-	list_filter = ("resolved", "visible", "creation_time", "resolution_time")
+	list_filter = ("resolved", "visible", "creation_time", "resolution_time", ("reporter", admin.RelatedOnlyFieldListFilter))
 	readonly_fields = ("creation_time", "resolution_time")
 	search_fields = ("location", "concern", "progress", "resolution")
 
 
 @register(SafetyCategory)
 class SafetyCategoryAdmin(admin.ModelAdmin):
 	list_display = ("name", "display_order")
@@ -1083,25 +1044,31 @@
 	extra = 1
 
 
 @register(SafetyItem)
 class SafetyItemAdmin(admin.ModelAdmin):
 	inlines = [SafetyItemDocumentsInline]
 	list_display = ("name", "category", "get_documents_number")
-	list_filter = ("category",)
+	list_filter = (("category", admin.RelatedOnlyFieldListFilter),)
 
 	@display(description='Documents')
 	def get_documents_number(self, obj: SafetyItem):
 		return SafetyItemDocuments.objects.filter(safety_item=obj).count()
 
 
 @register(Door)
 class DoorAdmin(admin.ModelAdmin):
 	list_display = ("name", "area", "interlock", "get_absolute_url", "id")
 
+	def formfield_for_foreignkey(self, db_field, request, **kwargs):
+		# Limit interlock selection to ones not already linked
+		if db_field.name == "interlock":
+			kwargs["queryset"] = Interlock.objects.filter(tool__isnull=True, door__isnull=True)
+		return super().formfield_for_foreignkey(db_field, request, **kwargs)
+
 
 @register(AlertCategory)
 class AlertCategoryAdmin(admin.ModelAdmin):
 	list_display = ("name",)
 
 
 class AlertAdminForm(forms.ModelForm):
@@ -1230,15 +1197,15 @@
 
 @register(Closure)
 class ClosureAdmin(admin.ModelAdmin):
 	inlines = [ClosureTimeInline]
 	form = ClosureAdminForm
 	list_display = ("name", "alert_days_before", "get_times_display", "staff_absent", "notify_managers_last_occurrence")
 	filter_horizontal = ("physical_access_levels",)
-	list_filter = ("physical_access_levels__area", "staff_absent", "notify_managers_last_occurrence")
+	list_filter = (("physical_access_levels__area", TreeRelatedFieldListFilter), "staff_absent", "notify_managers_last_occurrence")
 	readonly_fields = ("alert_preview",)
 	fieldsets = (
 		(
 			None,
 			{
 				"fields": (
 					"name",
@@ -1259,56 +1226,42 @@
 				alert_style = "width: 350px; color: #a94442; background-color: #f2dede; border-color: #dca7a7;padding: 15px; margin-bottom: 10px; border: 1px solid transparent; border-radius: 4px;"
 				display_title = f'<span style="font-weight:bold">{obj.name}</span><br>' if obj.name else ''
 				return iframe_content(f'<div style="{alert_style}">{display_title}{linebreaksbr(obj.closuretime_set.first().alert_contents())}</div>', extra_style="padding-bottom: 20%")
 			except Exception:
 				pass
 		return ""
 
+	@admin.display(description="Times")
 	def get_times_display(self, closure: Closure) -> str:
 		return mark_safe("<br>".join([format_daterange(ct.start_time, ct.end_time, dt_format="SHORT_DATETIME_FORMAT", d_format="SHORT_DATE_FORMAT", date_separator=" ", time_separator=" - ") for ct in ClosureTime.objects.filter(closure=closure)]))
 
-	get_times_display.short_description = 'Times'
-
 
 class TemporaryPhysicalAccessAdminForm(forms.ModelForm):
 	class Meta:
 		model = TemporaryPhysicalAccess
 		fields = "__all__"
 
 	class Media:
 		js = ("admin/time_options_override.js",)
 
-	def clean(self):
-		if any(self.errors):
-			return
-		cleaned_data = super().clean()
-		start_time = cleaned_data.get("start_time")
-		end_time = cleaned_data.get("end_time")
-		if end_time <= start_time:
-			self.add_error("end_time", "The end time must be later than the start time")
-		return cleaned_data
-
 
 @register(TemporaryPhysicalAccess)
 class TemporaryPhysicalAccessAdmin(admin.ModelAdmin):
 	list_display = ("id", "user", "start_time", "end_time", "get_area_name", "get_schedule_display_with_times")
-	list_filter = ("physical_access_level", "physical_access_level__area", "end_time", "start_time")
+	list_filter = (("physical_access_level", admin.RelatedOnlyFieldListFilter), ("physical_access_level__area", TreeRelatedFieldListFilter), "end_time", "start_time", ("user", admin.RelatedOnlyFieldListFilter))
 	form = TemporaryPhysicalAccessAdminForm
 
+	@admin.display(ordering="physical_access_level__area", description="Area")
 	def get_area_name(self, tpa: TemporaryPhysicalAccess) -> str:
 		return tpa.physical_access_level.area.name
 
-	get_area_name.admin_order_field = 'physical_access_level__area'
-	get_area_name.short_description = 'Area'
-
+	@admin.display(description="Schedule")
 	def get_schedule_display_with_times(self, tpa: TemporaryPhysicalAccess) -> str:
 		return tpa.physical_access_level.get_schedule_display_with_times()
 
-	get_schedule_display_with_times.short_description = 'Schedule'
-
 
 class TemporaryPhysicalAccessRequestFormAdmin(forms.ModelForm):
 	class Meta:
 		model = TemporaryPhysicalAccessRequest
 		fields = "__all__"
 
 
@@ -1322,29 +1275,26 @@
 		"start_time",
 		"end_time",
 		"physical_access_level",
 		"status_display",
 		"reviewer",
 		"deleted"
 	)
-	list_filter = ("status", "deleted")
+	list_filter = ("status", "deleted", ("creator", admin.RelatedOnlyFieldListFilter), ("physical_access_level", admin.RelatedOnlyFieldListFilter))
 	filter_horizontal = ("other_users",)
+	actions = [access_requests_export_csv]
 
+	@admin.display(ordering="other_users", description="Buddies")
 	def other_users_display(self, access_request: TemporaryPhysicalAccessRequest):
 		return mark_safe("<br>".join([u.username for u in access_request.other_users.all()]))
 
-	other_users_display.admin_order_field = "other_users"
-	other_users_display.short_description = "Buddies"
-
+	@admin.display(ordering="status", description="Status")
 	def status_display(self, access_request: TemporaryPhysicalAccessRequest):
 		return access_request.get_status_display()
 
-	status_display.admin_order_field = "status"
-	status_display.short_description = "Status"
-
 
 @register(ContactInformationCategory)
 class ContactInformationCategoryAdmin(admin.ModelAdmin):
 	list_display = ("name", "display_order")
 
 
 @register(ContactInformation)
@@ -1375,26 +1325,31 @@
 class ScheduledOutageCategoryAdmin(admin.ModelAdmin):
 	list_display = ("name",)
 
 
 @register(ScheduledOutage)
 class ScheduledOutageAdmin(admin.ModelAdmin):
 	list_display = ("id", "tool", "area", "resource", "creator", "title", "start", "end")
+	list_filter = (("tool", admin.RelatedOnlyFieldListFilter), ("area", TreeRelatedFieldListFilter), ("resource", admin.RelatedOnlyFieldListFilter), ("creator", admin.RelatedOnlyFieldListFilter))
 
 
 @register(News)
 class NewsAdmin(admin.ModelAdmin):
 	list_display = ("id", "title", "created", "last_updated", "archived", "pinned")
 	list_filter = ("archived", "pinned")
 
 
 @register(Notification)
 class NotificationAdmin(admin.ModelAdmin):
-	list_display = ("id", "user", "expiration", "content_type", "object_id")
-	list_filter = (("content_type", admin.RelatedOnlyFieldListFilter),)
+	list_display = ("id", "user", "get_item", "notification_type", "expiration")
+	list_filter = (("content_type", admin.RelatedOnlyFieldListFilter), "notification_type", )
+
+	@admin.display(description="Item")
+	def get_item(self, obj: Notification):
+		return admin_get_item(obj.content_type, obj.object_id)
 
 
 @register(BadgeReader)
 class BadgeReaderAdmin(admin.ModelAdmin):
 	list_display = ("id", "name", "send_key", "record_key")
 
 
@@ -1439,69 +1394,83 @@
 		"tool_usage_question",
 		"value",
 		"warning_threshold",
 		"last_reset",
 		"last_reset_by",
 		"is_active",
 	)
-	list_filter = ("tool",)
+	list_filter = (("tool", admin.RelatedOnlyFieldListFilter), "last_reset")
 	readonly_fields = ("warning_threshold_reached",)
 	form = CounterAdminForm
 
 
+class RequestMessageInlines(GenericStackedInline):
+	model = RequestMessage
+	extra = 1
+
+
 @register(BuddyRequest)
 class BuddyRequestAdmin(admin.ModelAdmin):
+	inlines = [RequestMessageInlines]
 	form = BuddyRequestForm
 	list_display = ("user", "start", "end", "area", "reply_count", "expired", "deleted")
-	list_filter = ("expired", "deleted")
+	list_filter = ("expired", "deleted", ("user", admin.RelatedOnlyFieldListFilter), ("area", TreeRelatedFieldListFilter))
 
+	@admin.display(ordering="replies", description="Replies")
 	def reply_count(self, buddy_request: BuddyRequest):
 		return buddy_request.replies.count()
 
-	reply_count.admin_order_field = "replies"
-	reply_count.short_description = "Replies"
-
-
-@register(BuddyRequestMessage)
-class BuddyRequestMessageAdmin(admin.ModelAdmin):
-	list_display = ("id", "link_to_buddy_request", "author", "creation_date")
-
-	def link_to_buddy_request(self, obj):
-		link = reverse("admin:NEMO_buddyrequest_change", args=[obj.buddy_request.id])  # model name has to be lowercase
-		return format_html('<a href="%s">%s</a>' % (link, obj.buddy_request))
 
-	link_to_buddy_request.short_description = "BUDDY REQUEST"
+@register(AdjustmentRequest)
+class AdjustmentRequestAdmin(admin.ModelAdmin):
+	inlines = [RequestMessageInlines]
+	list_display = ("creator", "last_updated", "get_item", "get_time_difference", "get_status_display", "reply_count", "deleted")
+	list_filter = ("status", "deleted", ("creator", admin.RelatedOnlyFieldListFilter), ("reviewer", admin.RelatedOnlyFieldListFilter))
+	date_hierarchy = "last_updated"
+	actions = [adjustment_requests_export_csv]
+
+	@admin.display(description="Diff")
+	def get_time_difference(self, adjustment_request: AdjustmentRequest):
+		return adjustment_request.get_time_difference()
+
+	@admin.display(ordering="replies", description="Replies")
+	def reply_count(self, adjustment_request: AdjustmentRequest):
+		return adjustment_request.replies.count()
+
+	@admin.display(description="Item")
+	def get_item(self, adjustment_request: AdjustmentRequest):
+		return admin_get_item(adjustment_request.item_type, adjustment_request.item_id)
 
 
 @register(StaffAbsenceType)
 class StaffAbsenceTypeAdmin(admin.ModelAdmin):
 	list_display = ("name", "description")
 
 
 @register(StaffAvailabilityCategory)
 class StaffAvailabilityCategoryAdmin(admin.ModelAdmin):
 	list_display = ("name", "display_order")
 
 
 @register(StaffAvailability)
 class StaffAvailabilityAdmin(admin.ModelAdmin):
-	list_display = ("staff_member", "category", "start_time", "end_time", *StaffAvailability.DAYS)
+	list_display = ("staff_member", "category", "visible", "start_time", "end_time", *StaffAvailability.DAYS)
 	list_filter = ("category", *StaffAvailability.DAYS)
 
 	def formfield_for_foreignkey(self, db_field, request, **kwargs):
 		""" We only want active users here """
 		if db_field.name == "staff_member":
 			kwargs["queryset"] = User.objects.filter(is_active=True)
 		return super().formfield_for_foreignkey(db_field, request, **kwargs)
 
 
 @register(StaffAbsence)
 class StaffAbsenceAdmin(admin.ModelAdmin):
 	list_display = ("creation_time", "staff_member", "absence_type", "full_day", "start_date", "end_date")
-	list_filter = ("staff_member", "absence_type", "start_date", "end_date", "creation_time")
+	list_filter = (("staff_member", admin.RelatedOnlyFieldListFilter), "absence_type", "start_date", "end_date", "creation_time")
 
 
 class ChemicalHazardAdminForm(forms.ModelForm):
 	class Meta:
 		model = ChemicalHazard
 		fields = "__all__"
 
@@ -1538,14 +1507,15 @@
 		if "chemicals" in form.changed_data:
 			obj.chemical_set.set(form.cleaned_data["chemicals"])
 
 
 @register(Chemical)
 class ChemicalAdmin(admin.ModelAdmin):
 	filter_horizontal = ("hazards",)
+	list_filter = ("hazards",)
 
 
 @register(SafetyTraining)
 class SafetyTrainingAdmin(admin.ModelAdmin):
 	list_display = ("name", "display_order")
 
 
@@ -1586,18 +1556,18 @@
 	"""
 	Return True if the given HttpRequest has permission to view
 	*at least one* page in the admin site.
 	In our case, anyone with a staff permission should be able
 	to access the admin site
 	"""
 	user: User = request.user
-	return user.is_active and user.is_any_part_of_staff
+	return user.is_active and (user.is_superuser or user.get_all_permissions())
 
 
 # Register our new admin permission
 admin.site.has_permission = has_admin_site_permission
 
 # Register other models
-admin.site.register(Discipline)
+admin.site.register(ProjectDiscipline)
 admin.site.register(AccountType)
 admin.site.register(ResourceCategory)
 admin.site.register(Permission)
```

### Comparing `NEMO-4.4.1/NEMO/apps/area_access/templates/area_access/already_logged_in.html` & `NEMO-4.5.0/NEMO/apps/area_access/templates/area_access/already_logged_in.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/apps/area_access/templates/area_access/base.html` & `NEMO-4.5.0/NEMO/apps/area_access/templates/area_access/base.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/apps/area_access/templates/area_access/choose_project.html` & `NEMO-4.5.0/NEMO/apps/area_access/templates/area_access/choose_project.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/apps/area_access/templates/area_access/logout_warning.html` & `NEMO-4.5.0/NEMO/apps/area_access/templates/area_access/logout_warning.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/apps/area_access/templates/area_access/resource_unavailable.html` & `NEMO-4.5.0/NEMO/apps/area_access/templates/area_access/resource_unavailable.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/apps/area_access/urls.py` & `NEMO-4.5.0/NEMO/apps/area_access/urls.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/apps/area_access/views.py` & `NEMO-4.5.0/NEMO/apps/area_access/views.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 	PhysicalAccessExpiredUserError,
 	ProjectChargeException,
 	ReservationRequiredUserError,
 	ScheduledOutageInProgressError,
 	UnavailableResourcesUserError,
 )
 from NEMO.models import (BadgeReader, Door, PhysicalAccessLog, PhysicalAccessType, Project, UsageEvent, User)
+from NEMO.policy import policy_class as policy
 from NEMO.views.area_access import log_in_user_to_area, log_out_user
 from NEMO.views.customization import ApplicationCustomization, InterlockCustomization
-from NEMO.views.policy import check_billing_to_project, check_policy_to_enter_any_area, check_policy_to_enter_this_area
 from NEMO.views.tool_control import interlock_bypass_allowed
 
 
 @login_required
 @permission_required("NEMO.add_areaaccessrecord")
 @require_GET
 def welcome_screen(request, door_id):
@@ -73,15 +73,15 @@
 	log.time = timezone.now()
 	log.result = PhysicalAccessType.DENY  # Assume the user does not have access
 
 	facility_name = ApplicationCustomization.get("facility_name")
 
 	# Check policy for entering an area
 	try:
-		check_policy_to_enter_any_area(user=user)
+		policy.check_to_enter_any_area(user=user)
 	except InactiveUserError:
 		log.details = "This user is not active, preventing them from entering any access controlled areas."
 		log.save()
 		return render(request, "area_access/inactive.html")
 
 	except NoActiveProjectsForUserError:
 		log.details = "The user has no active projects, preventing them from entering an access controlled area."
@@ -101,15 +101,15 @@
 		return render(request, "area_access/physical_access_denied.html", {"message": message})
 
 	max_capacity_reached = False
 	reservation_requirement_failed = False
 	scheduled_outage_in_progress = False
 	# Check policy to enter this area
 	try:
-		check_policy_to_enter_this_area(area=door.area, user=user)
+		policy.check_to_enter_area(area=door.area, user=user)
 	except NoAccessiblePhysicalAccessUserError as error:
 		if error.closure_time:
 			log.details = (
 				f"The user was blocked from entering this area because of a closure: {error.closure_time.closure.name}."
 			)
 			message = f"You do not have access to this area of the {facility_name} due to the following closure: {error.closure_time.closure.name}. The closure ends on {localize(error.closure_time.end_time.astimezone(timezone.get_current_timezone()))}"
 		else:
@@ -182,15 +182,15 @@
 			if not project_id:
 				# No log entry necessary here because all validation checks passed, and the user must indicate which project
 				# the wish to login under. The log entry is captured when the subsequent choice is made by the user.
 				return render(request, "area_access/choose_project.html", {"area": door.area, "user": user})
 			else:
 				project = get_object_or_404(Project, id=project_id)
 				try:
-					check_billing_to_project(project, user, door.area)
+					policy.check_billing_to_project(project, user, door.area)
 				except ProjectChargeException as e:
 					log.details = "The user attempted to bill the project named {} but got error: {}".format(project.name, e.msg)
 					log.save()
 					return render(request, "area_access/physical_access_denied.html", {"message": e.msg})
 
 		log.result = PhysicalAccessType.ALLOW
 		log.save()
@@ -198,21 +198,22 @@
 		# Automatically log the user out of any previous area before logging them in to the new area.
 		previous_area = None
 		if user.in_area():
 			previous_area = user.area_access_record().area
 			log_out_user(user)
 
 		# All policy checks passed so open the door for the user.
-		if not door.interlock.unlock():
-			if bypass_interlock and interlock_bypass_allowed(user):
-				pass
-			else:
-				return interlock_error("Login", user)
+		if door.interlock:
+			if not door.interlock.unlock():
+				if bypass_interlock and interlock_bypass_allowed(user):
+					pass
+				else:
+					return interlock_error("Login", user)
 
-		delay_lock_door(door.id)
+			delay_lock_door(door.id)
 
 		log_in_user_to_area(door.area, user, project)
 
 		return render(
 			request,
 			"area_access/login_success.html",
 			{"area": door.area, "name": user.first_name, "project": project, "previous_area": previous_area},
@@ -276,18 +277,20 @@
 			user=user,
 			door=door,
 			time=timezone.now(),
 			result=PhysicalAccessType.ALLOW,
 			details="The user was permitted to enter this area, and already had an active area access record for this area.",
 		)
 		log.save()
-		# If we cannot open the door, display message and let them try again or exit since there is nothing else to do (user is already logged in).
-		if not door.interlock.unlock():
-			return interlock_error(bypass_allowed=False)
-		delay_lock_door(door.id)
+		# If we cannot open the door, display message and let them try again,
+		# or exit since there is nothing else to do (user is already logged in).
+		if door.interlock:
+			if not door.interlock.unlock():
+				return interlock_error(bypass_allowed=False)
+			delay_lock_door(door.id)
 		return render(request, "area_access/door_is_open.html")
 	return render(request, "area_access/not_logged_in.html", {"area": door.area})
 
 
 def interlock_error(action: str = None, user: User = None, bypass_allowed: bool = None):
 	error_message = InterlockCustomization.get('door_interlock_failure_message')
 	bypass_allowed = interlock_bypass_allowed(user) if bypass_allowed is None else bypass_allowed
```

### Comparing `NEMO-4.4.1/NEMO/apps/kiosk/templates/kiosk/category_choices.html` & `NEMO-4.5.0/NEMO/apps/kiosk/templates/kiosk/category_choices.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/apps/kiosk/templates/kiosk/choices.html` & `NEMO-4.5.0/NEMO/apps/kiosk/templates/kiosk/choices.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/apps/kiosk/templates/kiosk/error.html` & `NEMO-4.5.0/NEMO/apps/kiosk/templates/kiosk/error.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/apps/kiosk/templates/kiosk/individual_reservation.html` & `NEMO-4.5.0/NEMO/apps/kiosk/templates/kiosk/individual_reservation.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/apps/kiosk/templates/kiosk/kiosk.html` & `NEMO-4.5.0/NEMO/apps/kiosk/templates/kiosk/kiosk.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/apps/kiosk/templates/kiosk/success.html` & `NEMO-4.5.0/NEMO/apps/kiosk/templates/kiosk/success.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/apps/kiosk/templates/kiosk/tool_information.html` & `NEMO-4.5.0/NEMO/apps/kiosk/templates/kiosk/tool_information.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/apps/kiosk/templates/kiosk/tool_project_selection_snippet.html` & `NEMO-4.5.0/NEMO/apps/kiosk/templates/kiosk/tool_project_selection_snippet.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/apps/kiosk/templates/kiosk/tool_reservation.html` & `NEMO-4.5.0/NEMO/apps/kiosk/templates/kiosk/tool_reservation.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/apps/kiosk/urls.py` & `NEMO-4.5.0/NEMO/apps/kiosk/urls.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/apps/kiosk/views.py` & `NEMO-4.5.0/NEMO/apps/kiosk/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,27 +7,23 @@
 from django.utils import timezone
 from django.utils.dateparse import parse_date, parse_time
 from django.views.decorators.http import require_GET, require_POST
 
 from NEMO.decorators import synchronized
 from NEMO.exceptions import RequiredUnansweredQuestionsException
 from NEMO.models import BadgeReader, Project, Reservation, ReservationItemType, Tool, UsageEvent, User
+from NEMO.policy import policy_class as policy
 from NEMO.utilities import localize, quiet_int
 from NEMO.views.calendar import (
 	cancel_the_reservation,
 	extract_configuration,
 	extract_reservation_questions,
 	render_reservation_questions,
 	shorten_reservation,
 )
-from NEMO.views.policy import (
-	check_policy_to_disable_tool,
-	check_policy_to_enable_tool,
-	check_policy_to_save_reservation,
-)
 from NEMO.views.status_dashboard import create_tool_summary
 from NEMO.views.tool_control import (
 	email_managers_required_questions_disable_tool,
 	interlock_bypass_allowed,
 	interlock_error,
 )
 from NEMO.widgets.dynamic_form import DynamicForm
@@ -43,15 +39,15 @@
 @synchronized("tool_id")
 def do_enable_tool(request, tool_id):
 	tool = Tool.objects.get(id=tool_id)
 	customer = User.objects.get(id=request.POST["customer_id"])
 	project = Project.objects.get(id=request.POST["project_id"])
 	bypass_interlock = request.POST.get("bypass", "False") == "True"
 
-	response = check_policy_to_enable_tool(tool, operator=customer, user=customer, project=project, staff_charge=False)
+	response = policy.check_to_enable_tool(tool, operator=customer, user=customer, project=project, staff_charge=False)
 	if response.status_code != HTTPStatus.OK:
 		dictionary = {
 			"message": "You are not authorized to enable this tool. {}".format(response.content.decode()),
 			"delay": 10,
 		}
 		return render(request, "kiosk/acknowledgement.html", dictionary)
 
@@ -83,15 +79,15 @@
 
 @synchronized("tool_id")
 def do_disable_tool(request, tool_id):
 	tool = Tool.objects.get(id=tool_id)
 	customer = User.objects.get(id=request.POST["customer_id"])
 	downtime = timedelta(minutes=quiet_int(request.POST.get("downtime")))
 	bypass_interlock = request.POST.get("bypass", "False") == "True"
-	response = check_policy_to_disable_tool(tool, customer, downtime)
+	response = policy.check_to_disable_tool(tool, customer, downtime)
 	if response.status_code != HTTPStatus.OK:
 		dictionary = {"message": response.content, "delay": 10}
 		return render(request, "kiosk/acknowledgement.html", dictionary)
 
 	# All policy checks passed so try to disable the tool for the user.
 	if tool.interlock and not tool.interlock.lock():
 		if bypass_interlock and interlock_bypass_allowed(customer):
@@ -158,15 +154,15 @@
 	reservation.project = project
 	reservation.user = customer
 	reservation.creator = customer
 	reservation.reservation_item = tool
 	reservation.start = start
 	reservation.end = end
 	reservation.short_notice = tool.determine_insufficient_notice(start)
-	policy_problems, overridable = check_policy_to_save_reservation(
+	policy_problems, overridable = policy.check_to_save_reservation(
 		cancelled_reservation=None,
 		new_reservation=reservation,
 		user_creating_reservation=customer,
 		explicit_policy_override=False,
 	)
 
 	# If there was a problem in saving the reservation then return the error...
@@ -357,14 +353,14 @@
 		reader_id = request.GET.get("reader_id")
 		dictionary = {
 			"location": location,
 			"badge_reader": BadgeReader.objects.get(id=reader_id) if reader_id else BadgeReader.default(),
 		}
 		return render(request, "kiosk/kiosk.html", dictionary)
 	else:
-		locations = sorted(list(set([tool.location for tool in Tool.objects.filter(visible=True)])))
+		locations = sorted(list(set([tool.location for tool in Tool.objects.filter(visible=True) if tool.location])))
 		dictionary = {
 			"locations": [
 				{"url": reverse("kiosk", kwargs={"location": location}), "name": location} for location in locations
 			]
 		}
 		return render(request, "kiosk/location_directory.html", dictionary)
```

### Comparing `NEMO-4.4.1/NEMO/apps/sensors/admin.py` & `NEMO-4.5.0/NEMO/apps/sensors/admin.py`

 * *Files 4% similar despite different names*

```diff
@@ -143,15 +143,15 @@
 		if not category.parent:
 			return ""
 		return mark_safe(
 			f'<a href="{reverse("admin:sensors_sensorcategory_change", args=[category.parent.id])}">{category.parent.name}</a>'
 		)
 
 	def formfield_for_foreignkey(self, db_field, request, **kwargs):
-		""" Filter list of potential parents """
+		"""Filter list of potential parents"""
 		if db_field.name == "parent":
 			kwargs["queryset"] = SensorCategory.objects.filter()
 		return super().formfield_for_foreignkey(db_field, request, **kwargs)
 
 
 @register(Sensor)
 class SensorAdmin(admin.ModelAdmin):
@@ -166,14 +166,20 @@
 		"unit_id",
 		"read_address",
 		"number_of_values",
 		"get_read_frequency",
 		"get_last_read",
 		"get_last_read_at",
 	)
+	list_filter = (
+		"visible",
+		"sensor_card__enabled",
+		("sensor_card", admin.RelatedOnlyFieldListFilter),
+		("sensor_category", admin.RelatedOnlyFieldListFilter),
+	)
 	actions = [duplicate_sensor_configuration, read_selected_sensors]
 
 	@display(boolean=True, ordering="sensor_card__enabled", description="Card Enabled")
 	def get_card_enabled(self, obj: Sensor):
 		return obj.card.enabled
 
 	@display(description="Last read")
@@ -196,15 +202,18 @@
 	list_display = ("name", "key")
 
 
 @register(SensorData)
 class SensorDataAdmin(admin.ModelAdmin):
 	list_display = ("created_date", "sensor", "value", "get_display_value")
 	date_hierarchy = "created_date"
-	list_filter = ("sensor", "sensor__sensor_category")
+	list_filter = (
+		("sensor", admin.RelatedOnlyFieldListFilter),
+		("sensor__sensor_category", admin.RelatedOnlyFieldListFilter),
+	)
 
 	@display(ordering="sensor__data_prefix", description="Display value")
 	def get_display_value(self, obj: SensorData):
 		return obj.display_value()
 
 
 @register(SensorAlertEmail)
@@ -212,15 +221,15 @@
 	list_display = ("sensor", "enabled", "trigger_condition", "trigger_no_data", "additional_emails", "triggered_on")
 	readonly_fields = ("triggered_on",)
 
 
 @register(SensorAlertLog)
 class SensorAlertLogAdmin(admin.ModelAdmin):
 	list_display = ["id", "time", "sensor", "reset", "value"]
-	list_filter = ["sensor", "value", "reset"]
+	list_filter = [("sensor", admin.RelatedOnlyFieldListFilter), "value", "reset"]
 	date_hierarchy = "time"
 
 	def has_delete_permission(self, request, obj=None):
 		return False
 
 	def has_add_permission(self, request):
 		return False
```

### Comparing `NEMO-4.4.1/NEMO/apps/sensors/customizations.py` & `NEMO-4.5.0/NEMO/apps/sensors/customizations.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/apps/sensors/evaluators.py` & `NEMO-4.5.0/NEMO/apps/sensors/evaluators.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/apps/sensors/migrations/0001_initial.py` & `NEMO-4.5.0/NEMO/apps/sensors/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/apps/sensors/models.py` & `NEMO-4.5.0/NEMO/apps/sensors/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 import datetime
 import random
 from logging import getLogger
 from typing import List, Optional
 
-from django.conf import settings
 from django.contrib.contenttypes.models import ContentType
 from django.core.exceptions import ValidationError
 from django.core.validators import MaxValueValidator, MinValueValidator
 from django.db import models
 from django.db.models import QuerySet
 from django.utils import timezone
 from django.utils.safestring import mark_safe
 
 from NEMO.apps.sensors.customizations import SensorCustomization
 from NEMO.apps.sensors.evaluators import evaluate_boolean_expression
 from NEMO.fields import MultiEmailField
 from NEMO.models import BaseModel, InterlockCard
-from NEMO.utilities import EmailCategory, format_datetime, send_mail
+from NEMO.utilities import EmailCategory, format_datetime, get_email_from_settings, send_mail
 
 models_logger = getLogger(__name__)
 
 
 class SensorCardCategory(BaseModel):
 	name = models.CharField(max_length=200, help_text="The name for this sensor card category")
 	key = models.CharField(max_length=100, help_text="The key to identify this sensor card category by in sensors.py")
@@ -334,15 +333,15 @@
 		recipients = [e for e in email_to.split(",") if e]
 		if self.additional_emails:
 			recipients.extend(self.additional_emails)
 		if recipients:
 			send_mail(
 				subject=subject,
 				content=message,
-				from_email=settings.SERVER_EMAIL,
+				from_email=get_email_from_settings(),
 				to=recipients,
 				email_category=EmailCategory.SENSORS,
 			)
 
 
 def get_alert_description(time, reset: bool, condition: str, no_data: bool, value: float):
 	if condition and value:
```

### Comparing `NEMO-4.4.1/NEMO/apps/sensors/sensors.py` & `NEMO-4.5.0/NEMO/apps/sensors/sensors.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,22 +91,25 @@
 		if not number_of_values:
 			error["number_of_values"] = _("This field is required.")
 		if error:
 			raise ValidationError(error)
 
 	def do_read_values(self, sensor: Sensor_model) -> List:
 		client = ModbusTcpClient(sensor.card.server, port=sensor.card.port)
-		valid_connection = client.connect()
-		if not valid_connection:
-			raise Exception(f"Connection to server {sensor.card.server}:{sensor.card.port} could not be established")
-		kwargs = {"slave": sensor.unit_id} if sensor.unit_id is not None else {}
-		read_response = client.read_holding_registers(sensor.read_address, sensor.number_of_values, **kwargs)
-		if read_response.isError():
-			raise Exception(str(read_response))
-		return read_response.registers
+		try:
+			valid_connection = client.connect()
+			if not valid_connection:
+				raise Exception(f"Connection to server {sensor.card.server}:{sensor.card.port} could not be established")
+			kwargs = {"slave": sensor.unit_id} if sensor.unit_id is not None else {}
+			read_response = client.read_holding_registers(sensor.read_address, sensor.number_of_values, **kwargs)
+			if read_response.isError():
+				raise Exception(f"Error with sensor {sensor.name}: {str(read_response)}")
+			return read_response.registers
+		finally:
+			client.close()
 
 	def evaluate_expression(self, formula, registers):
 		# Here we are using an expanded evaluator which includes modbus specific functions
 		return evaluate_modbus_expression(formula, registers=registers)
 
 
 class NoOpSensor(Sensor):
```

### Comparing `NEMO-4.4.1/NEMO/apps/sensors/static/sensors/chart.js` & `NEMO-4.5.0/NEMO/apps/sensors/static/sensors/chart.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/apps/sensors/static/sensors/chart.min.js` & `NEMO-4.5.0/NEMO/apps/sensors/static/sensors/chart.min.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/apps/sensors/static/sensors/chartjs-adapter-moment.js` & `NEMO-4.5.0/NEMO/apps/sensors/static/sensors/chartjs-adapter-moment.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/apps/sensors/static/sensors/daterangepicker.css` & `NEMO-4.5.0/NEMO/apps/sensors/static/sensors/daterangepicker.css`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/apps/sensors/static/sensors/daterangepicker.js` & `NEMO-4.5.0/NEMO/apps/sensors/static/sensors/daterangepicker.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/apps/sensors/static/sensors/sensors.css` & `NEMO-4.5.0/NEMO/apps/sensors/static/sensors/sensors.css`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/apps/sensors/templates/customizations/customizations_sensors.html` & `NEMO-4.5.0/NEMO/apps/sensors/templates/customizations/customizations_sensors.html`

 * *Files 2% similar despite different names*

```diff
@@ -37,12 +37,13 @@
                     <option value="5000" {% if sensor_default_refresh_rate == "5000" %}selected{% endif %}>every 5 seconds</option>
                     <option value="30000" {% if sensor_default_refresh_rate == "30000" %}selected{% endif %}>every 30 seconds</option>
                     <option value="60000" {% if sensor_default_refresh_rate == "60000" %}selected{% endif %}>every minute</option>
                     <option value="300000" {% if sensor_default_refresh_rate == "300000" %}selected{% endif %}>every 5 minutes</option>
                 </select>
             </div>
         </div>
-        <div class="col-md-offset-2">
-            {% button value="Save settings" type="save" %}
+        <div class="customization-separation" style="margin-bottom: 15px"></div>
+        <div class="text-center">
+            {% button type="save" value="Save settings" %}
         </div>
     </form>
 </div>
```

### Comparing `NEMO-4.4.1/NEMO/apps/sensors/templates/sensors/sensor_data.html` & `NEMO-4.5.0/NEMO/apps/sensors/templates/sensors/sensor_data.html`

 * *Files 2% similar despite different names*

```diff
@@ -67,29 +67,29 @@
             </ul>
             <div id="no-sensor-data" class="tab-content panel panel-default panel-tab-content" style="display: none;">
                 <div class="panel-body">
                     <i>There is no data to display. Try selecting a different date range</i>
                 </div>
             </div>
             <div id="sensor-data" class="tab-content panel panel-default panel-tab-content" style="margin-bottom: 0;">
-                <div class="tab-pane {% if tab == 'chart' %}active{% endif %}" id="chart-tab">
+                <div class="tab-pane{% if tab == 'chart' %} active{% endif %}" id="chart-tab">
                     <div class="panel-body">
                         <div class="text-right">
                             <div class="form-inline">
                                 <label class="control-label" for="chart-step">Display every</label>
                                 <input class="form-control input-sm" id="chart-step" type="number" value="{{ chart_step }}" onchange="refresh_page()" min="1" max="1440"/>
                                 <label class="control-label"> data point</label>
                             </div>
                         </div>
                         <div>
                             <canvas id="sensor-chart"></canvas>
                         </div>
                     </div>
                 </div>
-                <div class="tab-pane {% if tab == 'data' %}active{% endif %}" id="data-tab">
+                <div class="tab-pane{% if tab == 'data' %} active{% endif %}" id="data-tab">
                     <div class="panel-body">
                         <div class="text-right">
                             <div>
                                 {% url 'export_sensor_data' sensor.id as export_url %}
                                 {% button type="export" value="Export" onclick="refresh_page();window.open(get_base_url('"|concat:export_url|concat:"'))" %}
                             </div>
                         </div>
@@ -101,15 +101,15 @@
                                         <th>{{ sensor.data_label|default_if_none:'Value' }}</th>
                                     </tr>
                                 </tbody>
                             </table>
                         </div>
                     </div>
                 </div>
-                <div class="tab-pane {% if tab == 'alert' %}active{% endif %}" id="alert-tab">
+                <div class="tab-pane{% if tab == 'alert' %} active{% endif %}" id="alert-tab">
                     <div id="alert-div" class="panel-body">
                     </div>
                 </div>
             </div>
         </div>
     </div>
```

### Comparing `NEMO-4.4.1/NEMO/apps/sensors/templates/sensors/sensors.html` & `NEMO-4.5.0/NEMO/apps/sensors/templates/sensors/sensors.html`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 {% extends "base.html" %}
 {% load static %}
+{% load custom_tags_and_filters %}
 {% block extrahead %}
     <link rel="stylesheet" type="text/css" href="{% static "sensors/sensors.css" %}"/>
 {% endblock %}
 {% block title %}Sensors{% endblock %}
 {% block content %}
     <div class="well well-sensors-dashboard">
         <ol class="breadcrumb breadcrumb-sensors-dashboard">
@@ -33,15 +34,15 @@
                         {{ sensor.last_data_point.display_value }}
                     </li>
                 {% endfor %}
             {% endif %}
             {% if not sensors and not categories %}
                 <div class="dashboard-no-group-items">
                     no items to display.
-                    {% if user.is_superuser and not selected_category %}
+                    {% if user.is_superuser and not selected_category and "django.contrib.admin"|app_installed %}
                         <br/><br/>You can add sensors, categories and alerts by navigating to<br>
                         <a href="{% url 'admin:app_list' 'sensors' %}">
                             Administration -> Detailed Administration -> Sensors
                         </a>
                     {% endif %}
                 </div>
             {% endif %}
```

#### html2text {}

```diff
@@ -1,8 +1,9 @@
-{% extends "base.html" %} {% load static %} {% block extrahead %}
+{% extends "base.html" %} {% load static %} {% load custom_tags_and_filters %}
+{% block extrahead %}
 ensors.css" %}"/> {% endblock %} {% block title %}Sensors{% endblock %} {%
 block content %}
    1. {% if not selected_category %}
    2. Sensor Dashboard
    3. {% else %}
    4. Dashboard
    5. {% for ancestor in selected_category.ancestors %}
@@ -14,14 +15,14 @@
     * {{ category.name }}
     * {% endfor %} {% endif %} {% if sensors %} {% for sensor in sensors %}
     * {{ sensor.name }}
 
       {{ sensor.last_data_point.created_date|date:"SHORT_DATETIME_FORMAT" }}
       {{ sensor.last_data_point.display_value }}
     * {% endfor %} {% endif %} {% if not sensors and not categories %}
-      no items to display. {% if user.is_superuser and not selected_category %}
-
+      no items to display. {% if user.is_superuser and not selected_category
+      and "django.contrib.admin"|app_installed %}
 
       You can add sensors, categories and alerts by navigating to
       Administration_->_Detailed_Administration_->_Sensors {% endif %}
     * {% endif %}
 {% endblock %}
```

### Comparing `NEMO-4.4.1/NEMO/apps/sensors/urls.py` & `NEMO-4.5.0/NEMO/apps/sensors/urls.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/apps/sensors/views.py` & `NEMO-4.5.0/NEMO/apps/sensors/views.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/decorators.py` & `NEMO-4.5.0/NEMO/decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,15 +94,15 @@
 facility_manager_required = permission_decorator(lambda u: u.is_active and (u.is_facility_manager or u.is_superuser))
 staff_member_required = permission_decorator(lambda u: u.is_active and (u.is_staff or u.is_superuser))
 user_office_required = permission_decorator(lambda u: u.is_active and (u.is_user_office or u.is_superuser))
 accounting_required = permission_decorator(lambda u: u.is_active and (u.is_accounting_officer or u.is_superuser))
 staff_member_or_tool_superuser_required = permission_decorator(lambda u: u.is_active and (u.is_staff or u.is_tool_superuser or u.is_superuser))
 staff_member_or_user_office_required = permission_decorator(lambda u: u.is_active and (u.is_staff or u.is_user_office or u.is_superuser))
 accounting_or_user_office_or_manager_required = permission_decorator(lambda u: u.is_active and (u.is_accounting_officer or u.is_user_office or u.is_facility_manager or u.is_superuser))
-user_office_or_facility_manager_required = permission_decorator(lambda u: u.is_active and (u.is_user_office or u.is_facility_manager or u.is_superuser))
+user_office_or_manager_required = permission_decorator(lambda u: u.is_active and (u.is_user_office or u.is_facility_manager or u.is_superuser))
 any_staff_required = permission_decorator(lambda u: u.is_active and (u.is_any_part_of_staff))
 accounting_or_manager_required = permission_decorator(lambda u: u.is_active and (u.is_accounting_officer or u.is_facility_manager or u.is_superuser))
 
 
 # Use this decorator annotation to replace another existing function. The first parameter of
 # the new function should be "old_function" which will contain the function being replaced
 # For example, to replace NEMO.views.policy.check_policy_to_save_reservation(arg1, arg2)
```

### Comparing `NEMO-4.4.1/NEMO/exceptions.py` & `NEMO-4.5.0/NEMO/exceptions.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/fields.py` & `NEMO-4.5.0/NEMO/fields.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/forms.py` & `NEMO-4.5.0/NEMO/forms.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from datetime import date, datetime
+from datetime import datetime
 
 from django.core.exceptions import NON_FIELD_ERRORS, ValidationError
 from django.forms import (
 	BaseForm,
 	BooleanField,
 	CharField,
 	ChoiceField,
@@ -12,17 +12,17 @@
 	IntegerField,
 	ModelChoiceField,
 	ModelForm,
 )
 from django.forms.utils import ErrorDict, ErrorList
 from django.utils import timezone
 
-from NEMO.exceptions import ProjectChargeException
 from NEMO.models import (
 	Account,
+	AdjustmentRequest,
 	Alert,
 	AlertCategory,
 	BuddyRequest,
 	Comment,
 	Consumable,
 	ConsumableWithdraw,
 	Project,
@@ -36,15 +36,14 @@
 	TaskImages,
 	TemporaryPhysicalAccessRequest,
 	User,
 	UserPreferences,
 )
 from NEMO.utilities import bootstrap_primary_color, format_datetime, quiet_int
 from NEMO.views.customization import UserRequestsCustomization
-from NEMO.views.policy import check_billing_to_project
 
 
 class UserForm(ModelForm):
 	class Meta:
 		model = User
 		exclude = [
 			"is_staff",
@@ -183,14 +182,15 @@
 	class Meta:
 		model = SafetyIssue
 		fields = ["reporter", "concern", "location"]
 
 	def __init__(self, user, *args, **kwargs):
 		super(SafetyIssueCreationForm, self).__init__(*args, **kwargs)
 		self.user = user
+		self.fields["location"].required = True
 
 	def clean_update(self):
 		return self.cleaned_data["concern"].strip()
 
 	def clean_location(self):
 		return self.cleaned_data["location"].strip()
 
@@ -245,64 +245,14 @@
 		model = ConsumableWithdraw
 		fields = ["customer", "project", "consumable", "quantity"]
 
 	def __init__(self, *args, **kwargs):
 		super().__init__(*args, **kwargs)
 		self.fields["consumable"].queryset = Consumable.objects.filter(visible=True)
 
-	def clean_customer(self):
-		customer = self.cleaned_data["customer"]
-		if not customer.is_active:
-			raise ValidationError(
-				"A consumable withdraw was requested for an inactive user. Only active users may withdraw consumables."
-			)
-		if customer.access_expiration and customer.access_expiration < date.today():
-			raise ValidationError(f"This user's access expired on {format_datetime(customer.access_expiration)}")
-		return customer
-
-	def clean_project(self):
-		project = self.cleaned_data["project"]
-		if not project.active:
-			raise ValidationError(
-				"A consumable may only be billed to an active project. The user's project is inactive."
-			)
-		if not project.account.active:
-			raise ValidationError(
-				"A consumable may only be billed to a project that belongs to an active account. The user's account is inactive."
-			)
-		return project
-
-	def clean_quantity(self):
-		quantity = self.cleaned_data["quantity"]
-		if quantity < 1:
-			raise ValidationError("Please specify a valid quantity of items to withdraw.")
-		return quantity
-
-	def clean(self):
-		if any(self.errors):
-			return
-		cleaned_data = super().clean()
-		quantity = cleaned_data["quantity"]
-		consumable = cleaned_data["consumable"]
-		if not consumable.reusable and quantity > consumable.quantity:
-			raise ValidationError(
-				'There are not enough "'
-				+ consumable.name
-				+ '". (The current quantity in stock is '
-				+ str(consumable.quantity)
-				+ "). Please order more as soon as possible."
-			)
-		customer = cleaned_data["customer"]
-		project = cleaned_data["project"]
-		try:
-			check_billing_to_project(project, customer, consumable)
-		except ProjectChargeException as e:
-			raise ValidationError({"project": e.msg})
-		return cleaned_data
-
 
 class RecurringConsumableChargeForm(ModelForm):
 	class Meta:
 		model = RecurringConsumableCharge
 		exclude = ("last_charge", "last_updated", "last_updated_by")
 
 	def __init__(self, *args, **kwargs):
@@ -439,15 +389,15 @@
 			self.add_error("end", "The end must be later than the start")
 		return cleaned_data
 
 
 class TemporaryPhysicalAccessRequestForm(ModelForm):
 	class Meta:
 		model = TemporaryPhysicalAccessRequest
-		fields = ["start_time", "end_time", "physical_access_level", "other_users", "description"]
+		exclude = ["creation_time", "creator", "last_updated", "last_updated_by", "status", "reviewer", "deleted"]
 
 	def clean(self):
 		if any(self.errors):
 			return
 		cleaned_data = super().clean()
 		other_users = len(cleaned_data.get("other_users")) if "other_users" in cleaned_data else 0
 		minimum_total_users = quiet_int(UserRequestsCustomization.get("access_requests_minimum_users"), 2)
@@ -455,14 +405,20 @@
 			self.add_error(
 				"other_users",
 				f"You need at least {minimum_total_users - 1} other {'buddy' if minimum_total_users == 2 else 'buddies'} for this request",
 			)
 		return cleaned_data
 
 
+class AdjustmentRequestForm(ModelForm):
+	class Meta:
+		model = AdjustmentRequest
+		exclude = ["creation_time", "creator", "last_updated", "last_updated_by", "status", "reviewer", "deleted"]
+
+
 class StaffAbsenceForm(ModelForm):
 	class Meta:
 		model = StaffAbsence
 		fields = "__all__"
 
 
 def nice_errors(obj, non_field_msg="General form errors") -> ErrorDict:
```

### Comparing `NEMO-4.4.1/NEMO/interlocks.py` & `NEMO-4.5.0/NEMO/interlocks.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,21 +34,21 @@
 
 	def clean_interlock_card(self, interlock_card_form: InterlockCardAdminForm):
 		pass
 
 	def clean_interlock(self, interlock_form: InterlockAdminForm):
 		pass
 
-	def lock(self, interlock: Interlock_model) -> {True, False}:
+	def lock(self, interlock: Interlock_model) -> bool:
 		return self.__issue_command(interlock, Interlock_model.State.LOCKED)
 
-	def unlock(self, interlock: Interlock_model) -> {True, False}:
+	def unlock(self, interlock: Interlock_model) -> bool:
 		return self.__issue_command(interlock, Interlock_model.State.UNLOCKED)
 
-	def __issue_command(self, interlock: Interlock_model, command_type: Interlock_model.State):
+	def __issue_command(self, interlock: Interlock_model, command_type: Interlock_model.State) -> bool:
 		interlocks_enabled = getattr(settings, "INTERLOCKS_ENABLED", False)
 		now = timezone.now()
 		if not interlocks_enabled or not interlock.card.enabled:
 			interlock.most_recent_reply = "Interlock interface mocked out because settings.INTERLOCKS_ENABLED = False or interlock card is disabled. Interlock last set on " + format_datetime(now) + "."
 			interlock.most_recent_reply_time = now
 			interlock.state = command_type
 			interlock.save()
@@ -109,14 +109,19 @@
 
 class NoOpInterlock(Interlock):
 	def _send_command(self, interlock: Interlock_model, command_type: Interlock_model.State) -> Interlock_model.State:
 		pass
 
 
 class StanfordInterlock(Interlock):
+	MAX_ENABLE_VALUE = 3800
+	MIN_ENABLE_VALUE = 3200
+	MAX_DISABLE_VALUE = 1000
+	MIN_DISABLE_VALUE = 700
+
 	def clean_interlock_card(self, interlock_card_form: InterlockCardAdminForm):
 		even_port = interlock_card_form.cleaned_data["even_port"]
 		odd_port = interlock_card_form.cleaned_data["odd_port"]
 		number = interlock_card_form.cleaned_data["number"]
 		error = {}
 		if not even_port and even_port != 0:
 			error["even_port"] = _("This field is required.")
@@ -125,30 +130,34 @@
 		if not number and number != 0:
 			error["number"] = _("This field is required.")
 		if error:
 			raise ValidationError(error)
 
 	def clean_interlock(self, interlock_form: InterlockAdminForm):
 		channel = interlock_form.cleaned_data["channel"]
+		num_interlocks = interlock_form.cleaned_data["unit_id"]
 		error = {}
 		if not channel:
 			error["channel"] = _("This field is required.")
+		if num_interlocks is not None and num_interlocks < 1:
+			error["unit_id"] = _("The multiplier must be greater or equal to 1.")
 		if error:
 			raise ValidationError(error)
 
 	def _send_command(self, interlock: Interlock_model, command_type: Interlock_model.State) -> Interlock_model.State:
 		# The string in this next function call identifies the format of the interlock message.
 		# '!' means use network byte order (big endian) for the contents of the message.
 		# '20s' means that the message begins with a 20 character string.
+		# Each 'I' is an unsigned integer field (4 bytes).
 		# Each 'i' is an integer field (4 bytes).
-		# Each 'b' is a byte field (1 byte).
-		# '18s' means that the message ends with a 18 character string.
+		# Each 'B' is an unsigned char field (1 byte).
+		# '18s' means that the message ends with an 18 character string.
 		# More information on Python structs can be found at:
 		# http://docs.python.org/library/struct.html
-		command_schema = struct.Struct("!20siiiiiiiiibbbbb18s")
+		command_schema = struct.Struct("!20sIIIIIIIIIBBBBi18s")
 		command_message = command_schema.pack(
 			b"EQCNTL_BEGIN_COMMAND",
 			1,  # Instruction count
 			interlock.card.number,
 			interlock.card.even_port,
 			interlock.card.odd_port,
 			interlock.channel,
@@ -168,40 +177,62 @@
 		sock = socket.socket()
 		try:
 			sock.settimeout(3.0)  # Set the send/receive timeout to be 3 seconds.
 			server_address = (interlock.card.server, interlock.card.port)
 			sock.connect(server_address)
 			sock.send(command_message)
 			# The reply schema is the same as the command schema except there are no start and end strings.
-			reply_schema = struct.Struct("!iiiiiiiiibbbbb")
+			reply_schema = struct.Struct("!IIIIIIIIIBBBBi")
 			reply = sock.recv(reply_schema.size)
 			reply = reply_schema.unpack(reply)
 
-			# Update the state of the interlock in the database if the command succeeded.
-			if reply[5]:
-				interlock_state = command_type
-				return interlock_state
-			else:
+			num_interlocks = interlock.unit_id or 1
+
+			# Check for any interlock errors
+			error = ""
+			if not reply[5]:
+				error = "Stanford Interlock exception"
+			elif reply[9]:
+				error = "Signal driver overload"
+			elif reply[10]:
+				error = "Return driver overload"
+			elif not reply[11]:
+				error = "ADC not done"
+			elif reply[12]:
+				error = "Relay not ready"
+			elif not (
+				command_type == Interlock_model.State.UNLOCKED
+				and self.MIN_ENABLE_VALUE * num_interlocks <= reply[13] <= self.MAX_ENABLE_VALUE * num_interlocks
+				or command_type == Interlock_model.State.LOCKED
+				and self.MIN_DISABLE_VALUE * num_interlocks <= reply[13] <= self.MAX_DISABLE_VALUE * num_interlocks
+			):
+				error = "Enable return value exceeds limits"
+
+			if error:
 				# raise an exception if it failed
-				reply_message = "Stanford Interlock exception:\nResponse information: " +\
-								"Instruction count = " + str(reply[0]) + ", " +\
-								"card number = " + str(reply[1]) + ", " +\
-								"even port = " + str(reply[2]) + ", " +\
-								"odd port = " + str(reply[3]) + ", " +\
-								"channel = " + str(reply[4]) + ", " +\
-								"command return value = " + str(reply[5]) + ", " +\
-								"instruction type = " + str(reply[6]) + ", " +\
-								"instruction = " + str(reply[7]) + ", " +\
-								"delay = " + str(reply[8]) + ", " +\
-								"SD overload = " + str(reply[9]) + ", " +\
-								"RD overload = " + str(reply[10]) + ", " +\
-								"ADC done = " + str(reply[11]) + ", " +\
-								"busy = " + str(reply[12]) + ", " +\
+				reply_message = f"{error}:\nResponse information: " + \
+								"Instruction count = " + str(reply[0]) + ", " + \
+								"card number = " + str(reply[1]) + ", " + \
+								"even port = " + str(reply[2]) + ", " + \
+								"odd port = " + str(reply[3]) + ", " + \
+								"channel = " + str(reply[4]) + ", " + \
+								"command return value = " + str(reply[5]) + ", " + \
+								"instruction type = " + str(reply[6]) + ", " + \
+								"instruction = " + str(reply[7]) + ", " + \
+								"delay = " + str(reply[8]) + ", " + \
+								"SD overload = " + str(reply[9]) + ", " + \
+								"RD overload = " + str(reply[10]) + ", " + \
+								"ADC done = " + str(reply[11]) + ", " + \
+								"busy = " + str(reply[12]) + ", " + \
 								"instruction return value = " + str(reply[13]) + "."
 				raise InterlockError(interlock=interlock, msg=reply_message)
+			# Update the state of the interlock in the database if the command succeeded.
+			else:
+				interlock_state = command_type
+				return interlock_state
 
 		# Log any errors that occurred during the operation into the database.
 		except OSError as error:
 			reply_message = "Socket error"
 			if error.errno:
 				reply_message += " " + str(error.errno)
 			reply_message += ": " + str(error)
@@ -381,29 +412,34 @@
 			raise Exception("General exception: " + str(error))
 		return state
 
 	@classmethod
 	def setRelayState(cls, interlock: Interlock_model, state: {0, 1}) -> Interlock_model.State:
 		coil = interlock.channel
 		client = ModbusTcpClient(interlock.card.server, port=interlock.card.port)
-		client.connect()
-		kwargs = {"slave": interlock.unit_id} if interlock.unit_id is not None else {}
-		write_reply = client.write_coil(coil, state, **kwargs)
-		if write_reply.isError():
-			raise Exception(str(write_reply))
-		sleep(0.3)
-		read_reply = client.read_coils(coil, 1, **kwargs)
-		if read_reply.isError():
-			raise Exception(str(read_reply))
-		state = read_reply.bits[0]
-		client.close()
-		if state == cls.MODBUS_OFF:
-			return Interlock_model.State.LOCKED
-		elif state == cls.MODBUS_ON:
-			return Interlock_model.State.UNLOCKED
+		try:
+			valid_connection = client.connect()
+			if not valid_connection:
+				raise Exception(
+					f"Connection to server {interlock.card.server}:{interlock.card.port} could not be established")
+			kwargs = {"slave": interlock.unit_id} if interlock.unit_id is not None else {}
+			write_reply = client.write_coil(coil, state, **kwargs)
+			if write_reply.isError():
+				raise Exception(str(write_reply))
+			sleep(0.3)
+			read_reply = client.read_coils(coil, 1, **kwargs)
+			if read_reply.isError():
+				raise Exception(str(read_reply))
+			state = read_reply.bits[0]
+			if state == cls.MODBUS_OFF:
+				return Interlock_model.State.LOCKED
+			elif state == cls.MODBUS_ON:
+				return Interlock_model.State.UNLOCKED
+		finally:
+			client.close()
 
 
 def get(category: InterlockCardCategory, raise_exception=True):
 	"""	Returns the corresponding interlock implementation, and raises an exception if not found. """
 	interlock_impl = interlocks.get(category.key, False)
 	if not interlock_impl:
 		if raise_exception:
```

### Comparing `NEMO-4.4.1/NEMO/management/commands/send_email_usage_reminders.py` & `NEMO-4.5.0/NEMO/management/commands/send_email_usage_reminders.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/middleware.py` & `NEMO-4.5.0/NEMO/middleware.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import re
 from logging import getLogger
 from typing import Optional
 
 from django.conf import settings
 from django.contrib.auth.middleware import RemoteUserMiddleware
 from django.http import Http404, HttpResponseForbidden
-from django.shortcuts import redirect
 from django.urls import NoReverseMatch, resolve, reverse
 from django.utils.deprecation import MiddlewareMixin
 
 from NEMO.exceptions import InactiveUserError
 from NEMO.models import User
 from NEMO.utilities import is_ajax
 
@@ -39,15 +38,17 @@
 				middleware_logger.debug(f"Header: {self.header} not present or invalid")
 			super().process_request(request)
 		except (User.DoesNotExist, InactiveUserError):
 			from NEMO.views.authentication import all_auth_backends_are_pre_auth
 
 			# Only raise error if all we have are pre_authentication backends and they failed
 			if all_auth_backends_are_pre_auth():
-				return redirect("authorization_failed")
+				# We cannot use redirect here otherwise we create an infinite loop (calling the middleware again)
+				from NEMO.views.authentication import authorization_failed
+				return authorization_failed(request)
 
 
 class HTTPHeaderAuthenticationMiddleware(RemoteUserAuthenticationMiddleware):
 	header = "HTTP_" + getattr(settings, "AUTHENTICATION_HEADER", "AUTHORIZATION")
 
 
 class SessionTimeout:
```

### Comparing `NEMO-4.4.1/NEMO/migrations/0001_version_1_0_0.py` & `NEMO-4.5.0/NEMO/migrations/0001_version_1_0_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/migrations/0002_version_1_0_0_squashed.py` & `NEMO-4.5.0/NEMO/migrations/0002_version_1_0_0_squashed.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/migrations/0012_version_2_0_0_squashed.py` & `NEMO-4.5.0/NEMO/migrations/0012_version_2_0_0_squashed.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/migrations/0020_version_3_0_0.py` & `NEMO-4.5.0/NEMO/migrations/0020_version_3_0_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/migrations/0021_version_3_1_0.py` & `NEMO-4.5.0/NEMO/migrations/0021_version_3_1_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/migrations/0022_version_3_3_0.py` & `NEMO-4.5.0/NEMO/migrations/0022_version_3_3_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/migrations/0023_badgereader.py` & `NEMO-4.5.0/NEMO/migrations/0023_badgereader.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/migrations/0024_contactinformation_user.py` & `NEMO-4.5.0/NEMO/migrations/0024_contactinformation_user.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/migrations/0025_version_3_6_0.py` & `NEMO-4.5.0/NEMO/migrations/0025_version_3_6_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/migrations/0026_version_3_7_0.py` & `NEMO-4.5.0/NEMO/migrations/0026_version_3_7_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/migrations/0028_version_3_9_0.py` & `NEMO-4.5.0/NEMO/migrations/0028_version_3_9_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/migrations/0030_version_3_9_2.py` & `NEMO-4.5.0/NEMO/migrations/0030_version_3_9_2.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/migrations/0031_version_3_10_0.py` & `NEMO-4.5.0/NEMO/migrations/0031_version_3_10_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/migrations/0032_version_3_11_0.py` & `NEMO-4.5.0/NEMO/migrations/0032_version_3_11_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/migrations/0035_version_3_14_0.py` & `NEMO-4.5.0/NEMO/migrations/0035_version_3_14_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/migrations/0036_version_3_15_0.py` & `NEMO-4.5.0/NEMO/migrations/0036_version_3_15_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/migrations/0037_version_3_16_0.py` & `NEMO-4.5.0/NEMO/migrations/0037_version_3_16_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/migrations/0038_version_4_0_0.py` & `NEMO-4.5.0/NEMO/migrations/0038_version_4_0_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/migrations/0039_version_4_1_0.py` & `NEMO-4.5.0/NEMO/migrations/0039_version_4_1_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/migrations/0040_version_4_2_0.py` & `NEMO-4.5.0/NEMO/migrations/0040_version_4_2_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/migrations/0042_version_4_3_0.py` & `NEMO-4.5.0/NEMO/migrations/0042_version_4_3_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/migrations/0043_version_4_3_2.py` & `NEMO-4.5.0/NEMO/migrations/0043_version_4_3_2.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/migrations/0044_version_4_4_0.py` & `NEMO-4.5.0/NEMO/migrations/0044_version_4_4_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/migrations_utils.py` & `NEMO-4.5.0/NEMO/migrations_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,10 +32,18 @@
         story.last_updated = now
         story.last_update_content = content
         story.update_count = 0
         story.save()
         users = User.objects.filter(is_active=True)
         expiration = now + timedelta(days=30)  # Unread news story notifications always expire after 30 days
         for u in users:
-            Notification.objects.create(
-                user=u, expiration=expiration, content_type=news_content_type, object_id=story.id
+            notification = Notification(
+                user=u,
+                expiration=expiration,
+                content_type=news_content_type,
+                object_id=story.id,
             )
+            # This cannot be added directly because it didn't exist prior to 4.5.0
+            # and this code is used by ALL migrations, so anyone migrating before
+            # (4.2.0 to 4.3.0 for example) would get an exception and get completely stuck.
+            notification.notification_type = "news"
+            notification.save()
```

### Comparing `NEMO-4.4.1/NEMO/model_tree.py` & `NEMO-4.5.0/NEMO/model_tree.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/models.py` & `NEMO-4.5.0/NEMO/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,45 @@
+from __future__ import annotations
+
 import datetime
 import os
 import sys
 from copy import deepcopy
 from datetime import timedelta
 from enum import Enum
 from html import escape
 from json import loads
 from logging import getLogger
 from re import match
-from typing import List, Set, Union
+from typing import List, Optional, Set, Union
 
 from dateutil import rrule
 from django.conf import settings
 from django.contrib import auth
-from django.contrib.auth.models import BaseUserManager, Group, Permission
+from django.contrib.auth.models import BaseUserManager, Group, Permission, PermissionsMixin
 from django.contrib.contenttypes.fields import GenericForeignKey
 from django.contrib.contenttypes.models import ContentType
 from django.core.exceptions import NON_FIELD_ERRORS, ValidationError
 from django.core.validators import MinValueValidator
 from django.db import connections, models, transaction
 from django.db.models import Q, QuerySet
 from django.db.models.manager import Manager
 from django.db.models.signals import pre_delete
 from django.dispatch import receiver
 from django.template import loader
 from django.template.defaultfilters import linebreaksbr
 from django.urls import reverse
 from django.utils import timezone
 from django.utils.safestring import mark_safe
+from django.utils.translation import gettext_lazy as _
 from mptt.fields import TreeForeignKey
 from mptt.models import MPTTModel
 
 from NEMO import fields
+from NEMO.mixins import BillableItemMixin, CalendarDisplayMixin
 from NEMO.utilities import (
 	EmailCategory,
 	RecurrenceFrequency,
 	as_timezone,
 	beginning_of_the_day,
 	bootstrap_primary_color,
 	distinct_qs_value_list,
@@ -80,14 +84,21 @@
 		return [f.name for f in self.model._meta.fields if isinstance(f, models.TextField)]
 
 
 class BaseManager(Manager.from_queryset(BaseQuerySet)):
 	pass
 
 
+class DeserializationByNameManager(BaseManager):
+	""" Deserialization manager using name field """
+
+	def get_by_natural_key(self, name):
+		return self.get(name=name)
+
+
 class UserManager(BaseUserManager.from_queryset(BaseQuerySet)):
 
 	def create_user(self, username, first_name, last_name, email):
 		user = User()
 		user.username = username
 		user.first_name = first_name
 		user.last_name = last_name
@@ -108,15 +119,27 @@
 class BaseModel(models.Model):
 	objects = BaseManager()
 
 	class Meta:
 		abstract = True
 
 
-class BaseCategory(BaseModel):
+class SerializationByNameModel(BaseModel):
+	""" Serialization model using name field """
+
+	objects = DeserializationByNameManager()
+
+	class Meta:
+		abstract = True
+
+	def natural_key(self):
+		return (self.name,)
+
+
+class BaseCategory(SerializationByNameModel):
 	name = models.CharField(max_length=200, unique=True, help_text="The unique name for this item")
 	display_order = models.IntegerField(help_text="The display order is used to sort these items. The lowest value category is displayed first.")
 
 	class Meta:
 		abstract = True
 		ordering = ["display_order", "name"]
 
@@ -166,45 +189,44 @@
 	)
 
 	@classmethod
 	def on_choices(cls):
 		return [(choice[0], choice[1]) for choice in cls.Choices if choice[0] not in [cls.OFF, cls.ALTERNATE_EMAIL]]
 
 
-class CalendarDisplay(BaseModel):
-	"""
-	Inherit from this class to express that a class type can be displayed in the NEMO calendar.
-	Calling get_visual_end() will artificially lengthen the end time so the event is large enough to
-	be visible and clickable.
-	"""
-	start = None
-	end = None
-
-	def get_visual_end(self):
-		if self.end is None:
-			return max(self.start + timedelta(minutes=15), timezone.now())
-		else:
-			return max(self.start + timedelta(minutes=15), self.end)
+class RequestStatus(object):
+	PENDING = 0
+	APPROVED = 1
+	DENIED = 2
+	EXPIRED = 3
+	Choices = (
+		(PENDING, "Pending"),
+		(APPROVED, "Approved"),
+		(DENIED, "Denied"),
+		(EXPIRED, "Expired"),
+	)
 
-	class Meta:
-		abstract = True
+	@classmethod
+	def choices_without_expired(cls):
+		return [(choice[0], choice[1]) for choice in cls.Choices if choice[0] not in [cls.EXPIRED]]
 
 
 class UserPreferences(BaseModel):
 	attach_created_reservation = models.BooleanField('created_reservation_invite', default=False, help_text='Whether or not to send a calendar invitation when creating a new reservation')
 	attach_cancelled_reservation = models.BooleanField('cancelled_reservation_invite', default=False, help_text='Whether or not to send a calendar invitation when cancelling a reservation')
 	display_new_buddy_request_notification = models.BooleanField('new_buddy_request_notification', default=True, help_text='Whether or not to notify the user of new buddy requests (via unread badges)')
-	display_new_buddy_request_reply_notification = models.BooleanField('new_buddy_request_reply_notification', default=True, help_text='Whether or not to notify the user of replies on buddy request he commented on (via unread badges)')
 	email_new_buddy_request_reply = models.BooleanField('email_new_buddy_request_reply', default=True, help_text='Whether or not to email the user of replies on buddy request he commented on')
+	email_new_adjustment_request_reply = models.BooleanField('email_new_adjustment_request_reply', default=True, help_text='Whether or not to email the user of replies on adjustment request he commented on')
 	staff_status_view = models.CharField('staff_status_view', max_length=100, default='day', choices=[('day', 'Day'), ('week', 'Week'), ('month', 'Month')], help_text='Preferred view for staff status page')
 	email_alternate = models.EmailField(null=True, blank=True)
 	# Sort by the notifications that cannot be turned off first
 	email_send_reservation_emails = models.PositiveIntegerField(default=EmailNotificationType.BOTH_EMAILS, choices=EmailNotificationType.on_choices(), help_text="Reservation emails")
 	email_send_buddy_request_replies = models.PositiveIntegerField(default=EmailNotificationType.BOTH_EMAILS, choices=EmailNotificationType.on_choices(), help_text="Buddy request replies")
 	email_send_access_request_updates = models.PositiveIntegerField(default=EmailNotificationType.BOTH_EMAILS, choices=EmailNotificationType.on_choices(), help_text="Access request updates")
+	email_send_adjustment_request_updates = models.PositiveIntegerField(default=EmailNotificationType.BOTH_EMAILS, choices=EmailNotificationType.on_choices(), help_text="Adjustment request updates")
 	email_send_broadcast_emails = models.PositiveIntegerField(default=EmailNotificationType.BOTH_EMAILS, choices=EmailNotificationType.on_choices(), help_text="Broadcast emails")
 	email_send_task_updates = models.PositiveIntegerField(default=EmailNotificationType.BOTH_EMAILS, choices=EmailNotificationType.on_choices(), help_text="Task updates")
 	email_send_access_expiration_emails = models.PositiveIntegerField(default=EmailNotificationType.BOTH_EMAILS, choices=EmailNotificationType.on_choices(), help_text="Access expiration reminders")
 	email_send_tool_qualification_expiration_emails = models.PositiveIntegerField(default=EmailNotificationType.BOTH_EMAILS, choices=EmailNotificationType.on_choices(), help_text="Tool qualification expiration reminders")
 	email_send_usage_reminders = models.PositiveIntegerField(default=EmailNotificationType.BOTH_EMAILS, choices=EmailNotificationType.Choices, help_text="Usage reminders")
 	email_send_reservation_reminders = models.PositiveIntegerField(default=EmailNotificationType.BOTH_EMAILS, choices=EmailNotificationType.Choices, help_text="Reservation reminders")
 	email_send_reservation_ending_reminders = models.PositiveIntegerField(default=EmailNotificationType.BOTH_EMAILS, choices=EmailNotificationType.Choices, help_text="Reservation ending reminders")
@@ -218,33 +240,21 @@
 		return f"{self.user.username}'s preferences"
 
 	class Meta:
 		verbose_name = 'User preferences'
 		verbose_name_plural = 'User preferences'
 
 
-class UserType(BaseModel):
-	name = models.CharField(max_length=50, unique=True)
-
-	def __str__(self):
-		return self.name
-
-	class Meta:
-		ordering = ["name"]
+class UserType(BaseCategory):
+	pass
 
 
-class Discipline(BaseModel):
+class ProjectDiscipline(BaseCategory):
 	name = models.CharField(max_length=200, unique=True, help_text="The name of the discipline")
 
-	def __str__(self):
-		return self.name
-
-	class Meta:
-		ordering = ["name"]
-
 
 class PhysicalAccessLevel(BaseModel):
 	class Schedule(object):
 		ALWAYS = 0
 		WEEKDAYS = 1
 		WEEKENDS = 2
 		Choices = (
@@ -340,42 +350,34 @@
 
 	def ongoing_closure_time(self, time: datetime = None):
 		return self.physical_access_level.ongoing_closure_time(time)
 
 	def display(self):
 		return f"Temporary physical access of the '{self.physical_access_level.name}' for {self.user.get_full_name()} {format_daterange(self.start_time, self.end_time)}"
 
+	def clean(self):
+		if self.end_time and self.start_time and self.end_time <= self.start_time:
+			raise ValidationError({"end_time": "The end time must be later than the start time"})
+
 	class Meta:
 		ordering = ['-end_time']
+		verbose_name_plural = "TemporaryPhysicalAccess"
 
 
 class TemporaryPhysicalAccessRequest(BaseModel):
-
-	class Status(object):
-		PENDING = 0
-		APPROVED = 1
-		DENIED = 2
-		EXPIRED = 3
-		Choices = (
-			(PENDING, "Pending"),
-			(APPROVED, "Approved"),
-			(DENIED, "Denied"),
-			(EXPIRED, "Expired"),
-		)
-
 	creation_time = models.DateTimeField(auto_now_add=True, help_text="The date and time when the request was created.")
 	creator = models.ForeignKey("User", related_name='access_requests_created', on_delete=models.CASCADE)
 	last_updated = models.DateTimeField(auto_now=True, help_text="The last time this request was modified.")
 	last_updated_by = models.ForeignKey("User", null=True, blank=True, related_name="access_requests_updated", help_text="The last user who modified this request.", on_delete=models.SET_NULL)
 	physical_access_level = models.ForeignKey(PhysicalAccessLevel, on_delete=models.CASCADE)
 	description = models.TextField(null=True, blank=True, help_text="The description of the request.")
 	start_time = models.DateTimeField(help_text="The requested time for the access to start.")
 	end_time = models.DateTimeField(help_text="The requested time for the access to end.")
 	other_users = models.ManyToManyField("User", blank=True, help_text="Select the other users requesting access.")
-	status = models.IntegerField(choices=Status.Choices, default=Status.PENDING)
+	status = models.IntegerField(choices=RequestStatus.Choices, default=RequestStatus.PENDING)
 	reviewer = models.ForeignKey("User", null=True, blank=True, related_name='access_requests_reviewed', on_delete=models.CASCADE)
 	deleted = models.BooleanField(default=False, help_text="Indicates the request has been deleted and won't be shown anymore.")
 
 	def creator_and_other_users(self) -> Set:
 		result = {self.creator}
 		result.update(self.other_users.all())
 		return result
@@ -458,15 +460,15 @@
 	pass
 
 
 class OnboardingPhase(BaseCategory):
 	pass
 
 
-class User(BaseModel):
+class User(BaseModel, PermissionsMixin):
 	# Personal information:
 	username = models.CharField(max_length=100, unique=True)
 	first_name = models.CharField(max_length=100)
 	last_name = models.CharField(max_length=100)
 	email = models.EmailField(verbose_name='email address')
 	type = models.ForeignKey(UserType, null=True, blank=True, on_delete=models.SET_NULL)
 	domain = models.CharField(max_length=100, blank=True, help_text="The Active Directory domain that the account resides on")
@@ -504,24 +506,34 @@
 	# Preferences
 	preferences: UserPreferences = models.OneToOneField(UserPreferences, null=True, on_delete=models.SET_NULL)
 
 	USERNAME_FIELD = 'username'
 	REQUIRED_FIELDS = ['first_name', 'last_name', 'email']
 	objects = UserManager()
 
+	def natural_key(self):
+		return self.get_username(),
+
 	def clean(self):
 		username_pattern = getattr(settings, "USERNAME_REGEX", None)
 		if self.username:
 			if username_pattern and not match(username_pattern, self.username):
 				raise ValidationError({"username": "Invalid username format"})
 			username_taken = User.objects.filter(username__iexact=self.username)
 			if self.pk:
 				username_taken = username_taken.exclude(pk=self.pk)
 			if username_taken.exists():
 				raise ValidationError({'username': 'This username has already been taken'})
+		if self.is_staff and self.is_service_personnel:
+			raise ValidationError(
+				{
+					"is_staff": "A user cannot be both staff and service personnel. Please choose one or the other.",
+					"is_service_personnel": "A user cannot be both staff and service personnel. Please choose one or the other.",
+				}
+			)
 
 	def has_perm(self, perm, obj=None):
 		"""
 		Returns True if the user has each of the specified permissions. If
 		object is passed, it checks if the user has all required perms for this object.
 		"""
 
@@ -630,15 +642,15 @@
 	def accessible_areas(self):
 		""" Returns accessible leaf node areas for this user, including descendants """
 		return Area.objects.filter(id__in=[leaf_descendant.id for access in self.accessible_access_levels() for leaf_descendant in access.area.get_descendants(include_self=True) if leaf_descendant.is_leaf_node()]).distinct()
 
 	def in_area(self) -> bool:
 		return AreaAccessRecord.objects.filter(customer=self, staff_charge=None, end=None).exists()
 
-	def area_access_record(self):
+	def area_access_record(self) -> Optional[AreaAccessRecord]:
 		try:
 			return AreaAccessRecord.objects.get(customer=self, staff_charge=None, end=None)
 		except AreaAccessRecord.DoesNotExist:
 			return None
 
 	def is_logged_in_area_without_reservation(self) -> bool:
 		access_record = self.area_access_record()
@@ -752,15 +764,15 @@
 
 	new_file = instance.document
 	if not old_file == new_file:
 		if os.path.isfile(old_file.path):
 			os.remove(old_file.path)
 
 
-class Tool(BaseModel):
+class Tool(SerializationByNameModel):
 	name = models.CharField(max_length=100, unique=True)
 	parent_tool = models.ForeignKey('Tool', related_name="tool_children_set", null=True, blank=True, help_text='Select a parent tool to allow alternate usage', on_delete=models.CASCADE)
 	visible = models.BooleanField(default=True, help_text="Specifies whether this tool is visible to users.")
 	_description = models.TextField(db_column="description", null=True, blank=True, help_text="HTML syntax could be used")
 	_serial = models.CharField(db_column="serial", null=True, blank=True, max_length=100, help_text="Serial Number")
 	_image = models.ImageField(db_column="image", upload_to=get_tool_image_filename, blank=True, help_text="An image that represent the tool. Maximum width and height are 500px")
 	_tool_calendar_color = models.CharField(db_column="tool_calendar_color", max_length=9, default="#33ad33", help_text="Color for tool reservations in calendar overviews")
@@ -1242,14 +1254,58 @@
 	def tool_documents(self):
 		return ToolDocuments.objects.filter(tool=self).order_by()
 
 	def get_tool_info_html(self):
 		content = escape(loader.render_to_string("snippets/tool_info.html", {"tool": self}))
 		return f'<a href="javascript:;" data-title="{content}" data-tooltip-id="tooltip-tool-{self.id}" data-placement="bottom" class="tool-info-tooltip info-tooltip-container"><span class="glyphicon glyphicon-send small-icon"></span>{self.name_or_child_in_use_name()}</a>'
 
+	def clean(self):
+		errors = {}
+		if self.parent_tool_id:
+			if self.parent_tool_id == self.id:
+				errors["parent_tool"] = "You cannot select the parent to be the tool itself."
+		else:
+			from NEMO.views.customization import ToolCustomization
+			from NEMO.widgets.dynamic_form import DynamicForm
+			if not self._category:
+				errors["_category"] = "This field is required."
+			if not self._location and ToolCustomization.get_bool("tool_location_required"):
+				errors["_location"] = "This field is required."
+			if not self._phone_number and ToolCustomization.get_bool("tool_phone_number_required"):
+				errors["_phone_number"] = "This field is required."
+			if not self._primary_owner_id:
+				errors["_primary_owner"] = "This field is required."
+
+			# Validate _post_usage_questions JSON format
+			if self._post_usage_questions:
+				try:
+					loads(self._post_usage_questions)
+				except ValueError:
+					errors["_post_usage_questions"] = "This field needs to be a valid JSON string"
+				try:
+					DynamicForm(self._post_usage_questions).validate("tool_usage_group_question", self.id)
+				except Exception:
+					error_info = sys.exc_info()
+					errors["_post_usage_questions"] = error_info[0].__name__ + ": " + str(error_info[1])
+
+			if self._policy_off_between_times and (not self._policy_off_start_time or not self._policy_off_end_time):
+				if not self._policy_off_start_time:
+					errors["_policy_off_start_time"] = "Start time must be specified"
+				if not self._policy_off_end_time:
+					errors["_policy_off_end_time"] = "End time must be specified"
+		if errors:
+			raise ValidationError(errors)
+
+	def save(self, force_insert=False, force_update=False, using=None, update_fields=None):
+		if self.parent_tool_id:
+			# in case of alternate tool, recreate a new tool with only parent_tool and name (never visible)
+			fresh_tool = Tool(id=self.id, parent_tool=self.parent_tool, name=self.name, visible=False)
+			self.__dict__.update(fresh_tool.__dict__)
+		super().save(force_insert, force_update, using, update_fields)
+
 
 class ToolDocuments(BaseModel):
 	tool = models.ForeignKey(Tool, on_delete=models.CASCADE)
 	document = models.FileField(null=True, blank=True, upload_to=get_tool_document_filename, verbose_name='Document')
 	url = models.CharField(null=True, blank=True, max_length=200, verbose_name='URL')
 	name = models.CharField(null=True, blank=True, max_length=200, help_text="The optional name to display for this document")
 	uploaded_at = models.DateTimeField(auto_now_add=True)
@@ -1296,14 +1352,22 @@
 
 	new_file = instance.document
 	if not old_file == new_file:
 		if os.path.isfile(old_file.path):
 			os.remove(old_file.path)
 
 
+class ToolQualificationGroup(BaseModel):
+	name = models.CharField(max_length=200, unique=True, help_text="The name of this tool group")
+	tools = models.ManyToManyField(Tool, blank=False)
+
+	def __str__(self):
+		return self.name
+
+
 class Qualification(BaseModel):
 	user = models.ForeignKey(User, on_delete=models.CASCADE)
 	tool = models.ForeignKey(Tool, on_delete=models.CASCADE)
 	qualified_on = models.DateField(default=datetime.date.today)
 
 	class Meta:
 		# For db consistency and compatibility with previous queries
@@ -1360,15 +1424,15 @@
 	class Meta:
 		ordering = ["tool", "name"]
 
 	def __str__(self):
 		return str(self.tool.name) + ': ' + str(self.name)
 
 
-class TrainingSession(BaseModel):
+class TrainingSession(BaseModel, BillableItemMixin):
 	class Type(object):
 		INDIVIDUAL = 0
 		GROUP = 1
 		Choices = (
 			(INDIVIDUAL, 'Individual'),
 			(GROUP, 'Group')
 		)
@@ -1377,23 +1441,24 @@
 	trainee = models.ForeignKey(User, related_name="student_set", on_delete=models.CASCADE)
 	tool = models.ForeignKey(Tool, on_delete=models.CASCADE)
 	project = models.ForeignKey('Project', on_delete=models.CASCADE)
 	duration = models.PositiveIntegerField(help_text="The duration of the training session in minutes.")
 	type = models.IntegerField(choices=Type.Choices)
 	date = models.DateTimeField(default=timezone.now)
 	qualified = models.BooleanField(default=False, help_text="Indicates that after this training session the user was qualified to use the tool.")
+	validated = models.BooleanField(default=False)
 
 	class Meta:
 		ordering = ['-date']
 
 	def __str__(self):
 		return str(self.id)
 
 
-class StaffCharge(CalendarDisplay):
+class StaffCharge(BaseModel, CalendarDisplayMixin, BillableItemMixin):
 	staff_member = models.ForeignKey(User, related_name='staff_charge_actor', on_delete=models.CASCADE)
 	customer = models.ForeignKey(User, related_name='staff_charge_customer', on_delete=models.CASCADE)
 	project = models.ForeignKey('Project', on_delete=models.CASCADE)
 	start = models.DateTimeField(default=timezone.now)
 	end = models.DateTimeField(null=True, blank=True)
 	note = models.TextField(null=True, blank=True)
 	validated = models.BooleanField(default=False)
@@ -1526,21 +1591,22 @@
 	def abuse_email_list(self):
 		return [email for area in self.get_ancestors(ascending=True, include_self=True) for email in area.abuse_email]
 
 	def reservation_email_list(self):
 		return [email for area in self.get_ancestors(ascending=True, include_self=True) for email in area.reservation_email]
 
 
-class AreaAccessRecord(CalendarDisplay):
+class AreaAccessRecord(BaseModel, CalendarDisplayMixin, BillableItemMixin):
 	area = TreeForeignKey(Area, on_delete=models.CASCADE)
 	customer = models.ForeignKey(User, on_delete=models.CASCADE)
 	project = models.ForeignKey('Project', on_delete=models.CASCADE)
 	start = models.DateTimeField(default=timezone.now)
 	end = models.DateTimeField(null=True, blank=True)
 	staff_charge = models.ForeignKey(StaffCharge, blank=True, null=True, on_delete=models.CASCADE)
+	validated = models.BooleanField(default=False)
 
 	class Meta:
 		indexes = [
 			models.Index(fields=['end']),
 		]
 
 	def __str__(self):
@@ -1558,25 +1624,19 @@
 		ordering = ['-modification_time']
 		verbose_name_plural = "Configuration histories"
 
 	def __str__(self):
 		return str(self.id)
 
 
-class AccountType(BaseModel):
-	name = models.CharField(max_length=100, unique=True)
-
-	class Meta:
-		ordering = ["name"]
-
-	def __str__(self):
-		return str(self.name)
+class AccountType(BaseCategory):
+	pass
 
 
-class Account(BaseModel):
+class Account(SerializationByNameModel):
 	name = models.CharField(max_length=100, unique=True)
 	type = models.ForeignKey(AccountType, null=True, blank=True, on_delete=models.SET_NULL)
 	start_date = models.DateField(null=True, blank=True)
 	active = models.BooleanField(default=True, help_text="Users may only charge to an account if it is active. Deactivate the account to block future billable activity (such as tool usage and consumable check-outs) of all the projects that belong to it.")
 
 	class Meta:
 		ordering = ["name"]
@@ -1584,21 +1644,21 @@
 	def sorted_projects(self):
 		return self.project_set.all().order_by("-active", "name")
 
 	def __str__(self):
 		return str(self.name)
 
 
-class Project(BaseModel):
+class Project(SerializationByNameModel):
 	name = models.CharField(max_length=100, unique=True)
 	application_identifier = models.CharField(max_length=100)
 	start_date = models.DateField(null=True, blank=True)
 	account = models.ForeignKey(Account, help_text="All charges for this project will be billed to the selected account.", on_delete=models.CASCADE)
+	discipline = models.ForeignKey(ProjectDiscipline, null=True, blank=True, on_delete=models.SET_NULL)
 	active = models.BooleanField(default=True, help_text="Users may only charge to a project if it is active. Deactivate the project to block billable activity (such as tool usage and consumable check-outs).")
-	discipline = models.ForeignKey(Discipline, null=True, blank=True, on_delete=models.SET_NULL)
 	only_allow_tools = models.ManyToManyField(Tool, blank=True, help_text="Selected tools will be the only ones allowed for this project.")
 	allow_consumable_withdrawals = models.BooleanField(default=True, help_text="Uncheck this box if consumable withdrawals are forbidden under this project")
 
 	class Meta:
 		ordering = ["name"]
 
 	def __str__(self):
@@ -1669,15 +1729,15 @@
 # Call the function "pre_delete_entity" every time an account, project, tool, or user is deleted:
 pre_delete.connect(pre_delete_entity, sender=Account)
 pre_delete.connect(pre_delete_entity, sender=Project)
 pre_delete.connect(pre_delete_entity, sender=Tool)
 pre_delete.connect(pre_delete_entity, sender=User)
 
 
-class Reservation(CalendarDisplay):
+class Reservation(BaseModel, CalendarDisplayMixin, BillableItemMixin):
 	user = models.ForeignKey(User, related_name="reservation_user", on_delete=models.CASCADE)
 	creator = models.ForeignKey(User, related_name="reservation_creator", on_delete=models.CASCADE)
 	creation_time = models.DateTimeField(default=timezone.now)
 	tool = models.ForeignKey(Tool, null=True, blank=True, on_delete=models.CASCADE)
 	area = TreeForeignKey(Area, null=True, blank=True, on_delete=models.CASCADE)
 	project = models.ForeignKey(Project, null=True, blank=True, help_text="Indicates the intended project for this reservation. A missed reservation would be billed to this project.", on_delete=models.CASCADE)
 	start = models.DateTimeField('start')
@@ -1689,14 +1749,15 @@
 	missed = models.BooleanField(default=False, help_text="Indicates that the tool was not enabled by anyone before the tool's \"missed reservation threshold\" passed.")
 	shortened = models.BooleanField(default=False, help_text="Indicates that the user finished using the tool and relinquished the remaining time on their reservation. The reservation will no longer be visible on the calendar and a descendant reservation will be created in place of the existing one.")
 	descendant = models.OneToOneField('Reservation', related_name='ancestor', null=True, blank=True, on_delete=models.SET_NULL, help_text="Any time a reservation is moved or resized, the old reservation is cancelled and a new reservation with updated information takes its place. This field links the old reservation to the new one, so the history of reservation moves & changes can be easily tracked.")
 	additional_information = models.TextField(null=True, blank=True)
 	self_configuration = models.BooleanField(default=False, help_text="When checked, indicates that the user will perform their own tool configuration (instead of requesting that the staff configure it for them).")
 	title = models.TextField(default='', blank=True, max_length=200, help_text="Shows a custom title for this reservation on the calendar. Leave this field blank to display the reservation's user name as the title (which is the default behaviour).")
 	question_data = models.TextField(null=True, blank=True)
+	validated = models.BooleanField(default=False)
 
 	@property
 	def reservation_item(self) -> Union[Tool, Area]:
 		if self.tool:
 			return self.tool
 		elif self.area:
 			return self.area
@@ -1773,22 +1834,23 @@
 		ordering = ["name"]
 		verbose_name_plural = 'Reservation questions'
 
 	def __str__(self):
 		return self.name
 
 
-class UsageEvent(CalendarDisplay):
+class UsageEvent(BaseModel, CalendarDisplayMixin, BillableItemMixin):
 	user = models.ForeignKey(User, related_name="usage_event_user", on_delete=models.CASCADE)
 	operator = models.ForeignKey(User, related_name="usage_event_operator", on_delete=models.CASCADE)
 	project = models.ForeignKey(Project, on_delete=models.CASCADE)
 	tool = models.ForeignKey(Tool, related_name='+', on_delete=models.CASCADE)  # The related_name='+' disallows reverse lookups. Helper functions of other models should be used instead.
 	start = models.DateTimeField(default=timezone.now)
 	end = models.DateTimeField(null=True, blank=True)
 	validated = models.BooleanField(default=False)
+	remote_work = models.BooleanField(default=False)
 	run_data = models.TextField(null=True, blank=True)
 
 	def duration(self):
 		return calculate_duration(self.start, self.end, "In progress")
 
 	class Meta:
 		ordering = ['-start']
@@ -1849,25 +1911,53 @@
 		ordering = ["name"]
 		verbose_name_plural = 'Consumable categories'
 
 	def __str__(self):
 		return self.name
 
 
-class ConsumableWithdraw(BaseModel):
+class ConsumableWithdraw(BaseModel, BillableItemMixin):
 	customer = models.ForeignKey(User, related_name="consumable_user", help_text="The user who will use the consumable item.", on_delete=models.CASCADE)
 	merchant = models.ForeignKey(User, related_name="consumable_merchant", help_text="The staff member that performed the withdraw.", on_delete=models.CASCADE)
 	consumable = models.ForeignKey(Consumable, on_delete=models.CASCADE)
 	quantity = models.PositiveIntegerField()
 	project = models.ForeignKey(Project, help_text="The withdraw will be billed to this project.", on_delete=models.CASCADE)
 	date = models.DateTimeField(default=timezone.now, help_text="The date and time when the user withdrew the consumable.")
+	validated = models.BooleanField(default=False)
 
 	class Meta:
 		ordering = ['-date']
 
+	def clean(self):
+		errors = {}
+		if self.customer_id:
+			if not self.customer.is_active:
+				errors["customer"] = "A consumable withdraw was requested for an inactive user. Only active users may withdraw consumables."
+			if self.customer.access_expiration and self.customer.access_expiration < datetime.date.today():
+				errors["customer"] = f"This user's access expired on {format_datetime(self.customer.access_expiration)}"
+		if self.project_id:
+			if not self.project.active:
+				errors["project"] = "A consumable may only be billed to an active project. The user's project is inactive."
+			if not self.project.account.active:
+				errors["project"] = "A consumable may only be billed to a project that belongs to an active account. The user's account is inactive."
+		if self.quantity is not None and self.quantity < 1:
+			errors["quantity"] = "Please specify a valid quantity of items to withdraw."
+		if self.consumable_id:
+			if not self.consumable.reusable and self.quantity > self.consumable.quantity:
+				errors[NON_FIELD_ERRORS] = f'There are not enough "{self.consumable.name}". (The current quantity in stock is {str(self.consumable.quantity)}). Please order more as soon as possible.'
+		if self.customer_id and self.consumable_id and self.project_id:
+			from NEMO.exceptions import ProjectChargeException
+			from NEMO.policy import policy_class as policy
+			try:
+				policy.check_billing_to_project(self.project, self.customer, self.consumable)
+			except ProjectChargeException as e:
+				errors["project"] = e.msg
+		if errors:
+			raise ValidationError(errors)
+
 	def __str__(self):
 		return str(self.id)
 
 
 class RecurringConsumableCharge(BaseModel):
 	name = models.CharField(max_length=200, help_text="The name/identifier for this recurring charge.")
 	customer = models.ForeignKey(User, null=True, blank=True, related_name="recurring_charge_customer", help_text="The user who will be charged.", on_delete=models.CASCADE)
@@ -1954,15 +2044,15 @@
 			from NEMO.views.consumables import make_withdrawal
 			self.full_clean()
 			make_withdrawal(self.consumable.id, self.quantity, self.project.id, self.last_updated_by, self.customer.id)
 			self.last_charge = timezone.now()
 			self.save()
 
 	def is_empty(self):
-		return not any([self.customer, self.project])
+		return not any([self.customer_id, self.project_id])
 
 	def clear(self):
 		self.customer = None
 		self.project = None
 		self.last_charge = None
 		self.save()
 
@@ -1982,15 +2072,15 @@
 			# Validate needed fields are present
 			if errors:
 				raise ValidationError(errors)
 			# Validate if we have everything to charge
 			from NEMO.forms import ConsumableWithdrawForm
 			from NEMO.views.customization import RecurringChargesCustomization
 			skip_customer = RecurringChargesCustomization.get_bool("recurring_charges_skip_customer_validation")
-			charge_form = ConsumableWithdrawForm({"customer": self.customer.id, "project": self.project.id, "consumable": self.consumable.id, "quantity": self.quantity})
+			charge_form = ConsumableWithdrawForm({"customer": self.customer_id, "project": self.project_id, "consumable": self.consumable_id, "quantity": self.quantity})
 			if not charge_form.is_valid():
 				if not skip_customer or list(charge_form.errors.keys()) != ["customer"]:
 					raise ValidationError(charge_form.errors)
 
 	def save_with_user(self, user: User, *args, **kwargs):
 		self.last_updated_by = user
 		self.last_updated = timezone.now()
@@ -2043,33 +2133,33 @@
 			(UNKNOWN, 'Unknown'),
 			(UNLOCKED, 'Unlocked'),  # The 'unlocked' and 'locked' constants match the hardware command types to control the interlocks.
 			(LOCKED, 'Locked'),
 		)
 
 	card = models.ForeignKey(InterlockCard, on_delete=models.CASCADE)
 	channel = models.PositiveIntegerField(blank=True, null=True, verbose_name="Channel/Relay/Coil")
-	unit_id = models.PositiveIntegerField(null=True, blank=True)
+	unit_id = models.PositiveIntegerField(null=True, blank=True, verbose_name="Multiplier/Unit id")
 	state = models.IntegerField(choices=State.Choices, default=State.UNKNOWN)
 	most_recent_reply = models.TextField(default="None")
 	most_recent_reply_time = models.DateTimeField(null=True, blank=True)
 
-	def unlock(self):
+	def unlock(self) -> bool:
 		from NEMO import interlocks
 		return interlocks.get(self.card.category).unlock(self)
 
-	def lock(self):
+	def lock(self) -> bool:
 		from NEMO import interlocks
 		return interlocks.get(self.card.category).lock(self)
 
 	class Meta:
 		unique_together = ('card', 'channel')
 		ordering = ['card__server', 'card__number', 'channel']
 
 	def __str__(self):
-		return str(self.card) + ", channel " + str(self.channel)
+		return str(self.card) + (", channel " + str(self.channel) if self.channel else "")
 
 
 class InterlockCardCategory(BaseModel):
 	name = models.CharField(max_length=200, help_text="The name for this interlock category")
 	key = models.CharField(max_length=100, help_text="The key to identify this interlock category by in interlocks.py")
 
 	class Meta:
@@ -2207,15 +2297,15 @@
 		verbose_name_plural = "Task categories"
 		ordering = ["name"]
 
 	def __str__(self):
 		return str(self.name)
 
 
-class TaskStatus(BaseModel):
+class TaskStatus(SerializationByNameModel):
 	name = models.CharField(max_length=200, unique=True)
 	notify_primary_tool_owner = models.BooleanField(default=False, help_text="Notify the primary tool owner when a task transitions to this status")
 	notify_backup_tool_owners = models.BooleanField(default=False, help_text="Notify the backup tool owners when a task transitions to this status")
 	notify_tool_notification_email = models.BooleanField(default=False, help_text="Send an email to the tool notification email address when a task transitions to this status")
 	custom_notification_email_address = models.EmailField(blank=True, help_text="Notify a custom email address when a task transitions to this status. Leave this blank if you don't need it.")
 	notification_message = models.TextField(blank=True)
 
@@ -2383,28 +2473,28 @@
 	else:
 		return end - start
 
 
 class Door(BaseModel):
 	name = models.CharField(max_length=100)
 	area = TreeForeignKey(Area, related_name='doors', on_delete=models.PROTECT)
-	interlock = models.OneToOneField(Interlock, on_delete=models.PROTECT)
+	interlock = models.OneToOneField(Interlock, null=True, blank=True, on_delete=models.PROTECT)
 
 	def __str__(self):
 		return str(self.name)
 
 	def get_absolute_url(self):
 		from django.urls import reverse
 		return reverse('welcome_screen', args=[self.id])
 	get_absolute_url.short_description = 'URL'
 
 
 class SafetyIssue(BaseModel):
 	reporter = models.ForeignKey(User, blank=True, null=True, related_name='reported_safety_issues', on_delete=models.SET_NULL)
-	location = models.CharField(max_length=200)
+	location = models.CharField(null=True, blank=True, max_length=200)
 	creation_time = models.DateTimeField(auto_now_add=True)
 	visible = models.BooleanField(default=True, help_text='Should this safety issue be visible to all users? When unchecked, the issue is only visible to staff.')
 	concern = models.TextField()
 	progress = models.TextField(blank=True, null=True)
 	resolution = models.TextField(blank=True, null=True)
 	resolved = models.BooleanField(default=False)
 	resolution_time = models.DateTimeField(blank=True, null=True)
@@ -2543,34 +2633,39 @@
 		ordering = ["name"]
 
 	def __str__(self):
 		return str(self.name)
 
 
 class Notification(BaseModel):
-	user = models.ForeignKey(User, related_name='notifications', on_delete=models.CASCADE)
-	expiration = models.DateTimeField()
-	content_type = models.ForeignKey(ContentType, on_delete=models.CASCADE)
-	object_id = models.PositiveIntegerField()
-	content_object = GenericForeignKey('content_type', 'object_id')
-
 	class Types:
 		NEWS = 'news'
 		SAFETY = 'safetyissue'
 		BUDDY_REQUEST = 'buddyrequest'
 		BUDDY_REQUEST_REPLY = 'buddyrequestmessage'
+		ADJUSTMENT_REQUEST = 'adjustmentrequest'
+		ADJUSTMENT_REQUEST_REPLY = 'adjustmentrequestmessage'
 		TEMPORARY_ACCESS_REQUEST = 'temporaryphysicalaccessrequest'
 		Choices = (
 			(NEWS, 'News creation and updates - notifies all users'),
 			(SAFETY, 'New safety issues - notifies staff only'),
 			(BUDDY_REQUEST, 'New buddy request - notifies all users'),
 			(BUDDY_REQUEST_REPLY, 'New buddy request reply - notifies request creator and users who have replied'),
+			(ADJUSTMENT_REQUEST, 'New adjustment request - notifies facility managers only'),
+			(ADJUSTMENT_REQUEST_REPLY, 'New adjustment request reply - notifies request creator and users who have replied'),
 			(TEMPORARY_ACCESS_REQUEST, 'New access request - notifies other users on request and reviewers')
 		)
 
+	user = models.ForeignKey(User, related_name='notifications', on_delete=models.CASCADE)
+	expiration = models.DateTimeField()
+	notification_type = models.CharField(max_length=100, choices=Types.Choices)
+	content_type = models.ForeignKey(ContentType, on_delete=models.CASCADE)
+	object_id = models.PositiveIntegerField()
+	content_object = GenericForeignKey('content_type', 'object_id')
+
 
 class LandingPageChoice(BaseModel):
 	image = models.ImageField(help_text='An image that symbolizes the choice. It is automatically resized to 128x128 pixels when displayed, so set the image to this size before uploading to optimize bandwidth usage and landing page load time')
 	name = models.CharField(max_length=40, help_text='The textual name that will be displayed underneath the image')
 	url = models.CharField(max_length=200, verbose_name='URL', help_text='The URL that the choice leads to when clicked. Relative paths such as /calendar/ are used when linking within the site. Use fully qualified URL paths such as https://www.google.com/ to link to external sites.')
 	display_order = models.IntegerField(help_text="The order in which choices are displayed on the landing page, from left to right, top to bottom. Lower values are displayed first.")
 	open_in_new_tab = models.BooleanField(default=False, help_text="Open the URL in a new browser tab when it's clicked")
@@ -2720,22 +2815,23 @@
 		ordering = ["tool__name"]
 
 
 # This method is used to check when a tool usage counter value gets over the threshold
 @receiver(models.signals.pre_save, sender=ToolUsageCounter)
 def check_tool_usage_counter_threshold(sender, instance: ToolUsageCounter, **kwargs):
 	try:
-		if instance.is_active and not instance.warning_threshold_reached and instance.value >= instance.warning_threshold:
-			# value is over threshold. set flag and send email
-			instance.warning_threshold_reached = True
-			from NEMO.views.tool_control import send_tool_usage_counter_email
-			send_tool_usage_counter_email(instance)
-		if instance.warning_threshold_reached and instance.value < instance.warning_threshold:
-			# it has been reset. reset flag
-			instance.warning_threshold_reached = False
+		if instance.warning_threshold:
+			if instance.is_active and not instance.warning_threshold_reached and instance.value >= instance.warning_threshold:
+				# value is over threshold. set flag and send email
+				instance.warning_threshold_reached = True
+				from NEMO.views.tool_control import send_tool_usage_counter_email
+				send_tool_usage_counter_email(instance)
+			if instance.warning_threshold_reached and instance.value < instance.warning_threshold:
+				# it has been reset. reset flag
+				instance.warning_threshold_reached = False
 	except Exception as e:
 		models_logger.exception(e)
 		pass
 
 
 class BuddyRequest(BaseModel):
 	creation_time = models.DateTimeField(default=timezone.now, help_text="The date and time when the request was created.")
@@ -2743,26 +2839,91 @@
 	end = models.DateField(help_text="The end date the user is requesting a buddy.")
 	description = models.TextField(help_text="The description of the request.")
 	area = models.ForeignKey(Area, on_delete=models.CASCADE)
 	user = models.ForeignKey(User, help_text="The user who is submitting the request.", on_delete=models.CASCADE)
 	expired = models.BooleanField(default=False, help_text="Indicates the request has expired and won't be shown anymore.")
 	deleted = models.BooleanField(default=False, help_text="Indicates the request has been deleted and won't be shown anymore.")
 
+	@property
+	def creator(self) -> User:
+		return self.user
+
+	@property
+	def replies(self) -> QuerySet:
+		return RequestMessage.objects.filter(object_id=self.id, content_type=ContentType.objects.get_for_model(self))
+
 	def creator_and_reply_users(self) -> List[User]:
 		result = {self.user}
-		for reply in self.replies.all():
+		for reply in self.replies:
 			result.add(reply.author)
 		return list(result)
 
 	def __str__(self):
 		return f"BuddyRequest [{self.id}]"
 
 
-class BuddyRequestMessage(BaseModel):
-	buddy_request = models.ForeignKey(BuddyRequest, related_name="replies", help_text="The request that this message relates to.", on_delete=models.CASCADE)
+class AdjustmentRequest(BaseModel):
+	creation_time = models.DateTimeField(auto_now_add=True, help_text="The date and time when the request was created.")
+	creator = models.ForeignKey("User", related_name='adjustment_requests_created', on_delete=models.CASCADE)
+	last_updated = models.DateTimeField(auto_now=True, help_text="The last time this request was modified.")
+	last_updated_by = models.ForeignKey("User", null=True, blank=True, related_name="adjustment_requests_updated", help_text="The last user who modified this request.", on_delete=models.SET_NULL)
+	item_type = models.ForeignKey(ContentType, null=True, blank=True, on_delete=models.CASCADE)
+	item_id = models.PositiveIntegerField(null=True, blank=True)
+	item = GenericForeignKey('item_type', 'item_id')
+	description = models.TextField(null=True, blank=True, help_text="The description of the request.")
+	manager_note = models.TextField(null=True, blank=True, help_text="A manager's note to send to the user when a request is denied or to the user office when it is approved.")
+	new_start = models.DateTimeField(null=True, blank=True)
+	new_end = models.DateTimeField(null=True, blank=True)
+	status = models.IntegerField(choices=RequestStatus.choices_without_expired(), default=RequestStatus.PENDING)
+	reviewer = models.ForeignKey("User", null=True, blank=True, related_name='adjustment_requests_reviewed', on_delete=models.CASCADE)
+	deleted = models.BooleanField(default=False, help_text="Indicates the request has been deleted and won't be shown anymore.")
+
+	@property
+	def replies(self) -> QuerySet:
+		return RequestMessage.objects.filter(object_id=self.id, content_type=ContentType.objects.get_for_model(self))
+
+	def get_new_start(self) -> Optional[datetime]:
+		# Returns the new start if different from the item's start (not counting seconds and microseconds)
+		return self.new_start if self.new_start and self.item and self.item.start and self.item.start.replace(microsecond=0, second=0) != self.new_start else None
+
+	def get_new_end(self) -> Optional[datetime]:
+		# Returns the new end if different from the item's end (not counting seconds and microseconds)
+		return self.new_end if self.new_end and self.item and self.item.end and self.item.end.replace(microsecond=0, second=0) != self.new_end else None
+
+	def get_time_difference(self) -> str:
+		if self.item and self.new_start and self.new_end:
+			previous_duration = self.item.end.replace(microsecond=0, second=0) - self.item.start.replace(microsecond=0, second=0)
+			new_duration = self.new_end - self.new_start
+			return f"+{(new_duration - previous_duration)}" if new_duration >= previous_duration else f"- {(previous_duration - new_duration)}"
+
+	def creator_and_reply_users(self) -> List[User]:
+		result = {self.creator}
+		for reply in self.replies:
+			result.add(reply.author)
+		for manager in User.objects.filter(is_active=True, is_facility_manager=True):
+			result.add(manager)
+		return list(result)
+
+	def clean(self):
+		if not self.description:
+			raise ValidationError({"description": _("This field is required.")})
+		if self.item:
+			if self.new_start and self.new_end and self.new_start > self.new_end:
+				raise ValidationError({"new_end": "The end must be later than the start"})
+			if self.new_start and format_datetime(self.new_start) == format_datetime(self.item.start) and self.new_end and format_datetime(self.new_end) == format_datetime(self.item.end):
+				raise ValidationError({NON_FIELD_ERRORS: "One of the dates must be different from the original charge"})
+
+	class Meta:
+		ordering = ['-creation_time']
+
+
+class RequestMessage(BaseModel):
+	content_type = models.ForeignKey(ContentType, on_delete=models.CASCADE)
+	object_id = models.PositiveIntegerField()
+	content_object = GenericForeignKey('content_type', 'object_id')
 	author = models.ForeignKey(User, on_delete=models.CASCADE)
 	creation_date = models.DateTimeField(default=timezone.now)
 	content = models.TextField()
 
 	class Meta:
 		ordering = ['creation_date']
 
@@ -2783,14 +2944,15 @@
 	class Meta(BaseCategory.Meta):
 		verbose_name_plural = "Staff availability categories"
 
 
 class StaffAvailability(BaseModel):
 	DAYS = ["monday", "tuesday", "wednesday", "thursday", "friday", "saturday", "sunday"]
 	staff_member = models.ForeignKey("User", help_text="The staff member to display on the staff status page.", on_delete=models.CASCADE)
+	visible = models.BooleanField(default=True, help_text="Specifies whether this staff member should be displayed on the staff status page.")
 	category = models.ForeignKey(StaffAvailabilityCategory, null=True, blank=True, help_text="The category for this staff member.", on_delete=models.CASCADE)
 	start_time = models.TimeField(null=True, blank=True, help_text="The usual start time for this staff member.")
 	end_time = models.TimeField(null=True, blank=True, help_text="The usual end time for this staff member.")
 	monday = models.BooleanField(default=True, help_text="Check this box if the staff member usually works on Mondays.")
 	tuesday = models.BooleanField(default=True, help_text="Check this box if the staff member usually works on Tuesdays.")
 	wednesday = models.BooleanField(default=True, help_text="Check this box if the staff member usually works on Wednesdays.")
 	thursday = models.BooleanField(default=True, help_text="Check this box if the staff member usually works on Thursdays.")
@@ -2857,25 +3019,25 @@
 	def link(self):
 		return self.document.url if self.document else self.url
 
 	def __str__(self):
 		return str(self.name)
 
 
-# These two auto-delete tool images from filesystem when they are unneeded:
+# These two auto-delete hazard images from filesystem when they are unneeded:
 @receiver(models.signals.post_delete, sender=ChemicalHazard)
-def auto_delete_file_on_tool_delete(sender, instance: ChemicalHazard, **kwargs):
+def auto_delete_file_on_hazard_delete(sender, instance: ChemicalHazard, **kwargs):
 	"""	Deletes file from filesystem when corresponding `ChemicalHazard` object is deleted.	"""
 	if instance.logo:
 		if os.path.isfile(instance.logo.path):
 			os.remove(instance.logo.path)
 
 
 @receiver(models.signals.pre_save, sender=ChemicalHazard)
-def auto_delete_file_on_tool_change(sender, instance: ChemicalHazard, **kwargs):
+def auto_delete_file_on_hazard_change(sender, instance: ChemicalHazard, **kwargs):
 	"""	Deletes old file from filesystem when corresponding `ChemicalHazard` object is updated with new file. """
 	if not instance.pk:
 		return False
 
 	try:
 		old_file = ChemicalHazard.objects.get(pk=instance.pk).logo
 	except ChemicalHazard.DoesNotExist:
@@ -2884,25 +3046,25 @@
 	if old_file:
 		new_file = instance.logo
 		if not old_file == new_file:
 			if os.path.isfile(old_file.path):
 				os.remove(old_file.path)
 
 
-# These two auto-delete tool images from filesystem when they are unneeded:
+# These two auto-delete chemical document from filesystem when they are unneeded:
 @receiver(models.signals.post_delete, sender=Chemical)
-def auto_delete_file_on_tool_delete(sender, instance: Chemical, **kwargs):
+def auto_delete_file_on_chemical_delete(sender, instance: Chemical, **kwargs):
 	"""	Deletes file from filesystem when corresponding `Chemical` object is deleted.	"""
 	if instance.document:
 		if os.path.isfile(instance.document.path):
 			os.remove(instance.document.path)
 
 
 @receiver(models.signals.pre_save, sender=Chemical)
-def auto_delete_file_on_tool_change(sender, instance: Chemical, **kwargs):
+def auto_delete_file_on_chemical_change(sender, instance: Chemical, **kwargs):
 	"""	Deletes old file from filesystem when corresponding `Chemical` object is updated with new file. """
 	if not instance.pk:
 		return False
 
 	try:
 		old_file = Chemical.objects.get(pk=instance.pk).document
 	except Chemical.DoesNotExist:
@@ -2927,14 +3089,15 @@
 
 	class Meta:
 		ordering = ['-when']
 
 
 def record_remote_many_to_many_changes_and_save(request, obj, form, change, many_to_many_field, save_function_pointer):
 	"""
+	TODO: This should be done through pre/post save
 	Record the changes in a many-to-many field that the model does not own. Then, save the many-to-many field.
 	"""
 	# If the model object is being changed then we can get the list of previous members.
 	if change:
 		original_members = set(obj.user_set.all())
 	else:  # The model object is being created (instead of changed) so we can assume there are no members (initially).
 		original_members = set()
@@ -2978,14 +3141,15 @@
 		ex_member.child_content_object = user
 		ex_member.action = MembershipHistory.Action.REMOVED
 		ex_member.save()
 
 
 def record_local_many_to_many_changes(request, obj, form, many_to_many_field, form_field=None):
 	"""
+	TODO: This should be done through pre/post save
 	Record the changes in a many-to-many field that the model owns.
 	"""
 	data_field = form_field or many_to_many_field
 	if data_field in form.changed_data:
 		original_members = set(getattr(obj, many_to_many_field).all())
 		current_members = set(form.cleaned_data[data_field])
 		added_members = set(current_members) - set(original_members)
@@ -3005,14 +3169,15 @@
 			p.parent_content_object = a
 			p.save()
 
 
 def record_active_state(request, obj, form, field_name, is_initial_creation):
 	"""
 	Record whether the account, project, or user is active when the active state is changed.
+	TODO: this should be done in post_save rather than save_model
 	"""
 	if field_name in form.changed_data or is_initial_creation:
 		activity_entry = ActivityHistory()
 		activity_entry.authorizer = request.user
 		activity_entry.action = getattr(obj, field_name)
 		activity_entry.content_object = obj
 		activity_entry.save()
```

### Comparing `NEMO-4.4.1/NEMO/permissions.py` & `NEMO-4.5.0/NEMO/permissions.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/provisioning.py` & `NEMO-4.5.0/NEMO/provisioning.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/rates.py` & `NEMO-4.5.0/NEMO/rates.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-import importlib
 import json
 from abc import ABC, abstractmethod
 from logging import getLogger
 from typing import Dict, List, Union
 
 from django.conf import settings
 
 from NEMO.models import Consumable, Tool
+from NEMO.utilities import get_class_from_settings
 
 rates_logger = getLogger(__name__)
 
+
 class Rates(ABC):
 
 	rates = None
 
 	@abstractmethod
 	def load_rates(self, force_reload=False):
 		pass
@@ -112,25 +113,16 @@
 		table_row += "</tr>"
 		html_rate += table_header
 		html_rate += table_header_2
 		html_rate += table_row
 		html_rate += "</tr></table></div></div></div>"
 		return html_rate
 
-
 	def _get_rate_by_table_id_and_class(self, item: Union[Consumable, Tool], table_id, rate_claz) -> float:
 		if self.rates:
 			matching_rates = list(filter(lambda rate: rate['table_id'] == table_id and rate['rate_class'] == rate_claz and rate['item_id'] == item.id, self.rates))
 			if matching_rates:
 				return matching_rates[0]['rate']
 
 
-def get_rate_class():
-	rates_class = getattr(settings, "RATES_CLASS", "NEMO.rates.NISTRates")
-	assert isinstance(rates_class, str)
-	pkg, attr = rates_class.rsplit(".", 1)
-	ret = getattr(importlib.import_module(pkg), attr)
-	return ret()
-
-
 # ONLY import this LOCALLY to avoid potential issues
-rate_class = get_rate_class()
+rate_class: Rates = get_class_from_settings("RATES_CLASS", "NEMO.rates.NISTRates")
```

### Comparing `NEMO-4.4.1/NEMO/rest_filter_backend.py` & `NEMO-4.5.0/NEMO/rest_filter_backend.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/static/admin/physical_access_level/access_level.js` & `NEMO-4.5.0/NEMO/static/admin/physical_access_level/access_level.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/static/admin/questions_preview/questions_preview.css` & `NEMO-4.5.0/NEMO/static/admin/questions_preview/questions_preview.css`

 * *Files 3% similar despite different names*

```diff
@@ -140,15 +140,15 @@
     min-height: 20px;
     padding-left: 20px;
     margin-bottom: 0;
     font-weight: normal;
     cursor: pointer;
 }
 
-.questions_preview .form-group .radio input[type="radio"], .questions_preview .form-group .radio-inline input[type="radio"], .post_usage_preview .form-group .checkbox input[type="checkbox"], .post_usage_preview .form-group .checkbox-inline input[type="checkbox"]
+.questions_preview .form-group .radio input[type="radio"], .questions_preview .form-group .radio-inline input[type="radio"], .questions_preview .form-group .checkbox input[type="checkbox"], .questions_preview .form-group .checkbox-inline input[type="checkbox"]
 {
     position: absolute;
     margin-top: 4px \9;
     margin-left: -20px;
 }
 
 .questions_preview .form-group input[type="radio"], .questions_preview .form-group input[type="checkbox"]
```

### Comparing `NEMO-4.4.1/NEMO/static/admin/questions_preview/questions_preview.js` & `NEMO-4.5.0/NEMO/static/admin/questions_preview/questions_preview.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/static/admin/time_options_override.js` & `NEMO-4.5.0/NEMO/static/admin/time_options_override.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/static/admin/tool/tool.js` & `NEMO-4.5.0/NEMO/static/admin/tool/tool.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/static/badge_reader.js` & `NEMO-4.5.0/NEMO/static/badge_reader.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/static/bootstrap/css/bootstrap-theme.css` & `NEMO-4.5.0/NEMO/static/bootstrap/css/bootstrap-theme.css`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/static/bootstrap/css/bootstrap-theme.css.map` & `NEMO-4.5.0/NEMO/static/bootstrap/css/bootstrap-theme.css.map`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/static/bootstrap/css/bootstrap-theme.min.css` & `NEMO-4.5.0/NEMO/static/bootstrap/css/bootstrap-theme.min.css`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/static/bootstrap/css/bootstrap.css` & `NEMO-4.5.0/NEMO/static/bootstrap/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/static/bootstrap/css/bootstrap.css.map` & `NEMO-4.5.0/NEMO/static/bootstrap/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/static/bootstrap/css/bootstrap.min.css` & `NEMO-4.5.0/NEMO/static/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.eot` & `NEMO-4.5.0/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.svg` & `NEMO-4.5.0/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.ttf` & `NEMO-4.5.0/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.woff` & `NEMO-4.5.0/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.woff2` & `NEMO-4.5.0/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/static/bootstrap/js/bootstrap.js` & `NEMO-4.5.0/NEMO/static/bootstrap/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/static/bootstrap/js/bootstrap.min.js` & `NEMO-4.5.0/NEMO/static/bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/static/datetimepicker/bootstrap-datetimepicker.css` & `NEMO-4.5.0/NEMO/static/datetimepicker/bootstrap-datetimepicker.css`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/static/datetimepicker/bootstrap-datetimepicker.js` & `NEMO-4.5.0/NEMO/static/datetimepicker/bootstrap-datetimepicker.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/static/favicon.ico` & `NEMO-4.5.0/NEMO/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/static/fullcalendar/fullcalendar.css` & `NEMO-4.5.0/NEMO/static/fullcalendar/fullcalendar.css`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/static/fullcalendar/fullcalendar.js` & `NEMO-4.5.0/NEMO/static/fullcalendar/fullcalendar.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/static/fullcalendar/fullcalendar.min.css` & `NEMO-4.5.0/NEMO/static/fullcalendar/fullcalendar.min.css`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/static/fullcalendar/fullcalendar.min.js` & `NEMO-4.5.0/NEMO/static/fullcalendar/fullcalendar.min.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/static/icons/agreement.png` & `NEMO-4.5.0/NEMO/static/icons/agreement.png`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/static/icons/caution.png` & `NEMO-4.5.0/NEMO/static/icons/caution.png`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/static/icons/preferences.png` & `NEMO-4.5.0/NEMO/static/icons/preferences.png`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/static/jquery.js` & `NEMO-4.5.0/NEMO/static/jquery.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/static/jquery.min.js` & `NEMO-4.5.0/NEMO/static/jquery.min.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/static/jumbotron_watermark.bmp` & `NEMO-4.5.0/NEMO/static/jumbotron_watermark.bmp`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/static/mobile.js` & `NEMO-4.5.0/NEMO/static/mobile.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/static/moment.js` & `NEMO-4.5.0/NEMO/static/moment.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/static/moment.min.js` & `NEMO-4.5.0/NEMO/static/moment.min.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/static/moment.min.js.map` & `NEMO-4.5.0/NEMO/static/moment.min.js.map`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/static/nemo.css` & `NEMO-4.5.0/NEMO/static/nemo.css`

 * *Files 9% similar despite different names*

```diff
@@ -365,14 +365,101 @@
 .customization-input-file
 {
 	color: transparent;
 	display: inline-block !important;
 	margin-right: -170px;
 }
 
+/* Navbar customization, mainly size when switching */
+@media (max-width: 991px)
+{
+	.navbar-header
+	{
+		float: none;
+	}
+	.navbar-left,.navbar-right
+	{
+		float: none !important;
+	}
+	.navbar-toggle
+	{
+		display: block;
+	}
+	.navbar-collapse
+	{
+		border-top: 1px solid transparent;
+		box-shadow: inset 0 1px 0 rgba(255,255,255,0.1);
+	}
+	.navbar-fixed-top
+	{
+		top: 0;
+		border-width: 0 0 1px;
+	}
+	.navbar-collapse.collapse
+	{
+		display: none!important;
+	}
+	.navbar-nav
+	{
+		float: none!important;
+		margin: 7.5px -15px;
+	}
+	.navbar-nav>li
+	{
+		float: none;
+	}
+	.navbar-nav>li>a
+	{
+		padding-top: 10px;
+		padding-bottom: 10px;
+	}
+	.collapse.in
+	{
+		display:block !important;
+	}
+	/* sub-menu */
+	.navbar-nav .open .dropdown-menu
+	{
+		position: static;
+		float: none;
+		width: auto;
+		margin-top: 0;
+		background-color: transparent;
+		border: 0;
+		-webkit-box-shadow: none;
+		box-shadow: none;
+	}
+	.navbar-nav .open .dropdown-menu > li > a,
+	.navbar-nav .open .dropdown-menu .dropdown-header
+	{
+		padding: 5px 15px 5px 25px;
+	}
+	.navbar-nav .open .dropdown-menu > li > a
+	{
+		line-height: 20px;
+	}
+	.navbar-nav .open .dropdown-menu > li > a:hover,
+	.navbar-nav .open .dropdown-menu > li > a:focus
+	{
+		background-image: none;
+	}
+	.navbar-default .navbar-nav .open .dropdown-menu > li > a
+	{
+		color: #777;
+	}
+}
+
+@media (min-width: 768px)
+{
+	.navbar-toggle
+	{
+		margin-right: 0;
+	}
+}
+
 .navbar-preferences > a
 {
 	padding-left: 0 !important;
 	padding-right: 0 !important;
 }
 
 .navbar-preferences > a > img
@@ -705,22 +792,28 @@
 
 .buddy-list-item-reply, .buddy-list-item-message
 {
 	float: right;
 	width: 90%;
 }
 
-.buddy-list-item-message-user
+.request-item-message-user
 {
 	position: absolute;
 	top: 5px;
 	right: 5px;
 	font-size: x-small;
 }
 
+.request-item-message-new-reply
+{
+	position: absolute;
+	top: 5px;
+}
+
 .buddy-list-item-reply-buttons
 {
 	margin: 15px 0;
 	padding: 0 10px;
 }
 
 .buddy-list-day
@@ -890,14 +983,15 @@
     padding-top: 6px;
     margin-bottom: 0;
     background-color: transparent;
     border: solid transparent;
     border-width: 1px 0;
 }
 
+/* Media queries for popups in safety and other media items */
 @media (max-width: 768px)
 {
 	.modal-lg .media-popup
 	{
 		max-height: calc(100vh - 115px);
 	}
 }
@@ -925,7 +1019,23 @@
 @media (min-width: 992px)
 {
 	.modal-lg .media-popup
 	{
 		max-width: 870px;
 	}
 }
+
+.adjustment-request-message, .adjustment-request-reply-textarea
+{
+	border-top: 1px solid #eae9e9 !important;
+}
+
+.adjustment-request-message
+{
+	position: relative;
+	padding-top: 20px;
+}
+
+.adjustment-request-reply-textarea
+{
+	padding-top: 5px;
+}
```

### Comparing `NEMO-4.4.1/NEMO/static/nemo.js` & `NEMO-4.5.0/NEMO/static/nemo.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -337,16 +337,19 @@
     ajax_message(url, "GET", contents, success_callback, failure_callback, always_callback, traditional_serialization)
 }
 
 function ajax_post(url, contents, success_callback, failure_callback, always_callback, traditional_serialization) {
     if (contents === undefined) {
         contents = {};
     }
+    if (contents.constructor === Object) {
+        contents = $.param(contents)
+    }
     //noinspection JSUnresolvedFunction
-    contents.csrfmiddlewaretoken = csrf_token();
+    contents += "&csrfmiddlewaretoken=" + csrf_token();
     ajax_message(url, "POST", contents, success_callback, failure_callback, always_callback, traditional_serialization)
 }
 
 function ajax_message(url, type, contents, success_callback, failure_callback, always_callback, traditional_serialization) {
     let options = {
         "data": contents,
         "type": type,
```

### Comparing `NEMO-4.4.1/NEMO/static/numpad/custom_numpad.jquery.js` & `NEMO-4.5.0/NEMO/static/numpad/custom_numpad.jquery.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/static/pickadate/default.css` & `NEMO-4.5.0/NEMO/static/pickadate/default.css`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/static/pickadate/default.date.css` & `NEMO-4.5.0/NEMO/static/pickadate/default.date.css`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/static/pickadate/default.time.css` & `NEMO-4.5.0/NEMO/static/pickadate/default.time.css`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/static/pickadate/picker.date.js` & `NEMO-4.5.0/NEMO/static/pickadate/picker.date.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/static/pickadate/picker.js` & `NEMO-4.5.0/NEMO/static/pickadate/picker.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/static/pickadate/picker.time.js` & `NEMO-4.5.0/NEMO/static/pickadate/picker.time.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/static/typeahead.jquery.js` & `NEMO-4.5.0/NEMO/static/typeahead.jquery.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/static/typeahead.jquery.min.js` & `NEMO-4.5.0/NEMO/static/typeahead.jquery.min.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/static/virtualkeyboard/jquery.keyboard.js` & `NEMO-4.5.0/NEMO/static/virtualkeyboard/jquery.keyboard.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/static/virtualkeyboard/jquery.keyboard.min.js` & `NEMO-4.5.0/NEMO/static/virtualkeyboard/jquery.keyboard.min.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/static/virtualkeyboard/keyboard-basic.css` & `NEMO-4.5.0/NEMO/static/virtualkeyboard/keyboard-basic.css`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/static/virtualkeyboard/keyboard-basic.min.css` & `NEMO-4.5.0/NEMO/static/virtualkeyboard/keyboard-basic.min.css`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/abuse/abuse.html` & `NEMO-4.5.0/NEMO/templates/abuse/abuse.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/abuse/user_drill_down.html` & `NEMO-4.5.0/NEMO/templates/abuse/user_drill_down.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/accounts_and_projects/account_and_projects.html` & `NEMO-4.5.0/NEMO/templates/accounts_and_projects/account_and_projects.html`

 * *Files 4% similar despite different names*

```diff
@@ -44,15 +44,15 @@
                                 </a>
                             </form>
                         </div>
                         <div style="margin-left:34px">
                             {% if selected_project %}<label class="control-label">Account:</label> <a href="{% url 'account' project.account.id %}">{{ project.account }}</a>{% endif %}
                             <div id="project_{{ project.id }}_details" class="collapse {% if selected_project %}in{% endif %}">
                                 <div>
-                                    <label class="control-label">Identifier:</label>
+                                    <label class="control-label">{{ "projects_and_accounts"|customization:"project_application_identifier_name" }}:</label>
                                     <span class="grey">{{ project.application_identifier }}</span>
                                 </div>
 								{% if project.discipline %}
 									<div>
 										<label class="control-label">Discipline:</label>
 										<span class="grey">{{ project.discipline }}</span>
 									</div>
@@ -106,26 +106,26 @@
             $("#project_" + project_id + "_documents").load_multipart(form.action, form, complete_callback);
 		}
         function remove_document_from_project(url, project_id)
 		{
 			let complete_callback = ajax_complete_callback('Unable to remove document from project');
 			$("#project_" + project_id + "_documents").load(url, {'csrfmiddlewaretoken': '{{ csrf_token }}'}, complete_callback);
 		}
+        function reset_autocomplete()
+        {
+			$('.user_search').autocomplete('users', add_user_to_project, {{ users|json_search_base }});
+        }
 		function on_load()
 		{
 			$('#search').autocomplete('accounts_and_projects', get_account, {% json_search_base_with_extra_fields accounts_and_projects 'application_identifier' %});
-			$('.user_search').autocomplete('users', add_user_to_project, {{ users|json_search_base }});
+            reset_autocomplete();
 		}
 		window.addEventListener('load', on_load, true);
 	</script>
 	<style>
-        .set-pi .twitter-typeahead
-        {
-            display: inline-block !important;
-        }
 		#search_container .tt-dropdown-menu
 		{
 			min-width: 400px;
 			max-height: 600px;
 		}
 	</style>
 {% endblock %}
```

#### html2text {}

```diff
@@ -15,15 +15,16 @@
 selected_project or project == selected_project %}
  {{ project }}
 {% csrf_token %} {# Using an 'input submit' element would be preferable to an
 anchor on the following line, but Bootstrap can't style a 'submit' as a label
 so you have to use an anchor. #} {% if project.active %}Active{% else
 %}Inactive{% endif %}
 {% if selected_project %}Account: {{_project.account_}}{% endif %}
-Identifier: {{ project.application_identifier }}
+{{ "projects_and_accounts"|customization:"project_application_identifier_name"
+}}: {{ project.application_identifier }}
 {% if project.discipline %}
 Discipline: {{ project.discipline }}
 {% endif %} {% if project.start_date %}
 Start Date: {{ project.start_date }}
 {% endif %}
 {% include 'accounts_and_projects/users_for_project.html' with
 users=project.user_set.all %}
```

### Comparing `NEMO-4.4.1/NEMO/templates/accounts_and_projects/accounts_and_projects.html` & `NEMO-4.5.0/NEMO/templates/accounts_and_projects/accounts_and_projects.html`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 {% endblock %}
 {% block pagination_content %}
 	<table class="table table-bordered table-condensed table-hover table-align-middle thead-light">
 			<thead>
 				<tr>
 					<th>{% include 'pagination/pagination_column.html' with order_by='name' name='Name' %}</th>
 					{% if account_types %}<th>{% include 'pagination/pagination_column.html' with order_by='type' name='Account type' %}</th>{% endif %}
-					<th>Project identifier</th>
+					<th>{{ "projects_and_accounts"|customization:"project_application_identifier_name" }}</th>
 					<th class="button-column-minimum">{% include 'pagination/pagination_column.html' with order_by='active' name='Active' %}</th>
 					<th class="button-column-minimum"></th>
 				</tr>
 			</thead>
 			<tbody>
 				{% for account in page %}
 					<tr style="background-color: #f9f9f9">
```

#### html2text {}

```diff
@@ -2,41 +2,42 @@
 %} {% block title %}Accounts and projects{% endblock %} {% block
 before_pagination %}
 Accounts and projects
 {% button type="add" value="New project" url="create_project" %} {% button
 type="add" value="New account" url="create_account" %}
 [                    ]
 {% endblock %} {% block pagination_content %}
-{% include 'pagination/ {% include 'pagination/                                      {% include 'pagination/
-pagination_column.html' pagination_column.html' with  Project identifier             pagination_column.html'
-with order_by='name'    order_by='type' name='Account                                with order_by='active'
-name='Name' %}          type' %}                                                     name='Active' %}
-                                                                                     {% csrf_token %} {% if  {% url
-                                                                                     account.active %} {%    "account"
-                                                                                     button type="save"      account.id as
-                                                                                     size="small"            account_url %}
-                        {                                                            title="Deactivate"      {% button
-                        {                                                            icon="glyphicon-ok"     type="view"
- {{ account.name }}     account.type|default_if_none:                                value="" %} {% else %}  size="small"
-                        "" }}                                                        {% button type="delete" value="View"
-                                                                                     submit=True             title="View
-                                                                                     size="small"            account"
-                                                                                     title="Reactivate"      url=account_url
-                                                                                     icon="glyphicon-remove" %}
-                                                                                     value="" %} {% endif %}
+{% include 'pagination/ {% include 'pagination/       {                                      {% include 'pagination/
+pagination_column.html' pagination_column.html' with  {                                      pagination_column.html'
+with order_by='name'    order_by='type' name='Account "projects_and_accounts"|customization: with order_by='active'
+name='Name' %}          type' %}                      "project_application_identifier_name"  name='Active' %}
+                                                      }}
+                                                                                             {% csrf_token %} {% if  {% url
+                                                                                             account.active %} {%    "account"
+                                                                                             button type="save"      account.id as
+                                                                                             size="small"            account_url %}
+                        {                                                                    title="Deactivate"      {% button
+                        {                                                                    icon="glyphicon-ok"     type="view"
+ {{ account.name }}     account.type|default_if_none:                                        value="" %} {% else %}  size="small"
+                        "" }}                                                                {% button type="delete" value="View"
+                                                                                             submit=True             title="View
+                                                                                             size="small"            account"
+                                                                                             title="Reactivate"      url=account_url
+                                                                                             icon="glyphicon-remove" %}
+                                                                                             value="" %} {% endif %}
 This account does not have any active projects
-                                                                                     {% csrf_token %} {% if  {% url
-                                                                                     project.active %} {%    "project"
-                                                                                     button type="save"      project.id as
-                                                                                     size="small"            project_url %}
-                                                      {                              title="Deactivate"      {% button
-                                                      {                              icon="glyphicon-ok"     type="view"
-{{ project.name }}                                    project.application_identifier value="" %} {% else %}  size="small"
-                                                      }}                             {% button type="delete" value="View"
-                                                                                     submit=True             title="View
-                                                                                     size="small"            project"
-                                                                                     title="Reactivate"      url=project_url
-                                                                                     icon="glyphicon-remove" %}
-                                                                                     value="" %} {% endif %}
+                                                                                             {% csrf_token %} {% if  {% url
+                                                                                             project.active %} {%    "project"
+                                                                                             button type="save"      project.id as
+                                                                                             size="small"            project_url %}
+                                                                                             title="Deactivate"      {% button
+                                                                                             icon="glyphicon-ok"     type="view"
+{{ project.name }}                                    {{ project.application_identifier }}   value="" %} {% else %}  size="small"
+                                                                                             {% button type="delete" value="View"
+                                                                                             submit=True             title="View
+                                                                                             size="small"            project"
+                                                                                             title="Reactivate"      url=project_url
+                                                                                             icon="glyphicon-remove" %}
+                                                                                             value="" %} {% endif %}
 This account does not have any projects
 {% endblock %} {% block after_pagination %}
  {% endblock %}
```

### Comparing `NEMO-4.4.1/NEMO/templates/accounts_and_projects/create_account.html` & `NEMO-4.5.0/NEMO/templates/accounts_and_projects/create_account.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/accounts_and_projects/create_project.html` & `NEMO-4.5.0/NEMO/templates/accounts_and_projects/create_project.html`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 				<input type="button" id="selected_account" class="btn btn-default" onclick="clear_account_selection()" style="display:none">
 			</div>
 			<div class="col-sm-6 form-control-static danger-highlight">
 				{{ form.account.errors|striptags }}
 			</div>
 		</div>
 		<div class="form-group">
-            <label for="application_identifier" class="control-label col-sm-2"><b>Application identifier</b></label>
+            <label for="application_identifier" class="control-label col-sm-2"><b>{{ "projects_and_accounts"|customization:"project_application_identifier_name" }}</b></label>
 			<div class="col-sm-4">
 				<input type="text" name="application_identifier" id="application_identifier" maxlength="100" class="form-control" value="{{ form.application_identifier.value|default_if_none:'' }}" required>
 			</div>
 			<div class="col-sm-6 form-control-static danger-highlight">
 				{{ form.application_identifier.errors|striptags }}
 			</div>
 		</div>
```

#### html2text {}

```diff
@@ -10,15 +10,16 @@
 {% csrf_token %}
 Name
 [{{ form.name.value|default_if_none:'' }}]
 {{ form.name.errors|striptags }}
 Account
 [account             ] [Unknown INPUT type]
 {{ form.account.errors|striptags }}
-Application identifier
+{{ "projects_and_accounts"|customization:"project_application_identifier_name"
+}}
 [{{ form.application_identifier.value|default_if_none:'' }}]
 {{ form.application_identifier.errors|striptags }}
 {% if form.fields.discipline.choices.queryset %}
 Discipline
 {% for discipline_id, discipline_name in form.fields.discipline.choices %}
 % if discipline_id == form.discipline.value|to_int %}selected{% endif %}>{
 { discipline_name|default_if_none:'' }}
```

### Comparing `NEMO-4.4.1/NEMO/templates/accounts_and_projects/documents_for_project.html` & `NEMO-4.5.0/NEMO/templates/accounts_and_projects/documents_for_project.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/accounts_and_projects/users_for_project.html` & `NEMO-4.5.0/NEMO/templates/accounts_and_projects/users_for_project.html`

 * *Files 9% similar despite different names*

```diff
@@ -43,12 +43,16 @@
 000002a0: 7b7b 2075 207d 7d3c 2f73 7061 6e3e 7b25  {{ u }}</span>{%
 000002b0: 2065 6e64 6966 2025 7d3c 6272 3e0a 097b   endif %}<br>..{
 000002c0: 2520 656d 7074 7920 257d 0a09 0954 6869  % empty %}...Thi
 000002d0: 7320 7072 6f6a 6563 7420 646f 6573 206e  s project does n
 000002e0: 6f74 2068 6176 6520 616e 7920 6d65 6d62  ot have any memb
 000002f0: 6572 732e 0a09 7b25 2065 6e64 666f 7220  ers...{% endfor 
 00000300: 257d 0a3c 2f64 6976 3e0a 0a3c 7363 7269  %}.</div>..<scri
-00000310: 7074 3e0a 0924 2822 2373 6561 7263 685f  pt>..$("#search_
-00000320: 7573 6572 5f66 6f72 5f70 726f 6a65 6374  user_for_project
-00000330: 5f22 202b 2022 7b7b 2070 726f 6a65 6374  _" + "{{ project
-00000340: 2e69 6420 7d7d 2229 2e66 6f63 7573 2829  .id }}").focus()
-00000350: 3b0a 3c2f 7363 7269 7074 3e              ;.</script>
+00000310: 7074 3e0a 2020 2020 2428 6675 6e63 7469  pt>.    $(functi
+00000320: 6f6e 2829 0a20 2020 207b 0a20 2020 2020  on().    {.     
+00000330: 2020 2072 6573 6574 5f61 7574 6f63 6f6d     reset_autocom
+00000340: 706c 6574 6528 293b 0a09 2020 2020 2428  plete();..    $(
+00000350: 2223 7365 6172 6368 5f75 7365 725f 666f  "#search_user_fo
+00000360: 725f 7072 6f6a 6563 745f 2220 2b20 227b  r_project_" + "{
+00000370: 7b20 7072 6f6a 6563 742e 6964 207d 7d22  { project.id }}"
+00000380: 292e 666f 6375 7328 293b 0a20 2020 207d  ).focus();.    }
+00000390: 293b 0a3c 2f73 6372 6970 743e            );.</script>
```

### Comparing `NEMO-4.4.1/NEMO/templates/alerts.html` & `NEMO-4.5.0/NEMO/templates/alerts.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/area_access/area_access.html` & `NEMO-4.5.0/NEMO/templates/area_access/area_access.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/area_access/calendar_self_login.html` & `NEMO-4.5.0/NEMO/templates/area_access/calendar_self_login.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/area_access/change_project.html` & `NEMO-4.5.0/NEMO/templates/area_access/change_project.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/area_access/login_areas.html` & `NEMO-4.5.0/NEMO/templates/area_access/login_areas.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/area_access/new_area_access_record.html` & `NEMO-4.5.0/NEMO/templates/area_access/new_area_access_record.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/area_access/new_area_access_record_details.html` & `NEMO-4.5.0/NEMO/templates/area_access/new_area_access_record_details.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/area_access/self_login.html` & `NEMO-4.5.0/NEMO/templates/area_access/self_login.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/authorization_failed.html` & `NEMO-4.5.0/NEMO/templates/authorization_failed.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/base.html` & `NEMO-4.5.0/NEMO/templates/base.html`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 <html lang="en">
 <head>
 	{# This meta-tag forcefully disables 'compatibility mode' in Internet Explorer because it causes rendering problems. #}
 	<meta http-equiv="X-UA-Compatible" content="IE=edge"/>
 	<meta charset="UTF-8">
 	<meta name="application-name" content="NEMO">
 	<meta name="author" content="Center for Nanoscale Science and Technology">
-	<meta name="description" content="NEMO allows facility users to make tool reservations, control access to tools in their facilty, and streamline logistics and communication">
+	<meta name="description" content="NEMO allows facility users to make tool reservations, control access to tools in their facility, and streamline logistics and communication">
 	<meta name="keywords" content="logistics, operations, nano-technology, nano-fabrication, reservation, tool control, status">
 	<meta name="viewport" content="width=device-width, initial-scale=1, user-scalable=no">
 
 	{# Snippet to prevent clickjacking. Taken from https://www.codemagi.com/blog/post/194 #}
 	<style id="antiClickjack">
 		body
 		{
@@ -117,18 +117,25 @@
         $('#loading-div-page').hide();
     }
 	function show_alerts()
 	{
 		let alert_users = $(".alert.show-on-load");
 		alert_users.each(function(index, element) {
 		    let speed = 4500;
-		    if ($(element).data('speed')) speed = $(element).data('speed')
-			$(element).fadeTo(speed, 500).slideUp(500, function () {
-				$(element).slideUp(500);
-			});
+		    if ($(element).data('speed')) { speed = $(element).data('speed'); }
+            let manual_only = $(element).data("trigger") === "manual";
+            if (manual_only)
+            {
+                {# Manual dismissal only #}
+                $(element).fadeTo(speed, 500);
+            }
+            else
+            {
+                $(element).fadeTo(speed, 500).slideUp(500, function () { $(element).slideUp(500); });
+            }
 		});
 	}
 	{# Add an event listener on load for scripts. UseCapture is False so this is executed a bit later #}
 	window.addEventListener("load", function ()
     {
         show_alerts();
```

### Comparing `NEMO-4.4.1/NEMO/templates/calendar/calendar.html` & `NEMO-4.5.0/NEMO/templates/calendar/calendar.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/calendar/configuration.html` & `NEMO-4.5.0/NEMO/templates/calendar/configuration.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/calendar/configuration_helper.html` & `NEMO-4.5.0/NEMO/templates/calendar/configuration_helper.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/calendar/policy_dialog.html` & `NEMO-4.5.0/NEMO/templates/calendar/policy_dialog.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/calendar/project_choice.html` & `NEMO-4.5.0/NEMO/templates/calendar/project_choice.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/calendar/proxy_reservation.html` & `NEMO-4.5.0/NEMO/templates/calendar/proxy_reservation.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/calendar/reservation_event_feed.html` & `NEMO-4.5.0/NEMO/templates/calendar/reservation_event_feed.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/calendar/reservation_questions.html` & `NEMO-4.5.0/NEMO/templates/calendar/reservation_questions.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/calendar/reservation_warning.html` & `NEMO-4.5.0/NEMO/templates/calendar/reservation_warning.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/calendar/scheduled_outage_information.html` & `NEMO-4.5.0/NEMO/templates/calendar/scheduled_outage_information.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/calendar/specific_user_feed.html` & `NEMO-4.5.0/NEMO/templates/calendar/specific_user_feed.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/calendar/usage_event_feed.html` & `NEMO-4.5.0/NEMO/templates/calendar/usage_event_feed.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/configuration_agenda.html` & `NEMO-4.5.0/NEMO/templates/configuration_agenda.html`

 * *Files 8% similar despite different names*

```diff
@@ -43,14 +43,19 @@
 										{{ reservation.start }}<br>
 										{{ reservation.end }}<br>
 										{{ reservation.additional_information|linebreaksbr }}
 									</p>
 									{% if not reservation.tool.in_use and reservation.project %}
                                         {% url 'enable_tool' tool_id=reservation.tool.id user_id=reservation.user.id project_id=reservation.project.id staff_charge='false' as enable_tool_for_user_url %}
                                         {% button type="info" icon="glyphicon-play" value="Enable the tool on behalf of "|concat:reservation.user.first_name onclick="enable_tool('"|concat:enable_tool_for_user_url|concat:"');" %}
+                                        {% if "remote_work"|customization:"remote_work_ask_explicitly" %}
+                                            <div style="margin-top: 5px">
+                                                {% button type="info" icon="glyphicon-play" value="Enable the tool on behalf of "|concat:reservation.user.first_name|concat:" for remote work" onclick="enable_tool('"|concat:enable_tool_for_user_url|concat:"', true);" %}
+                                            </div>
+                                        {% endif %}
 									{% endif %}
 								</td>
 								{% if forloop.first %}
 									<td style="width:50%;border:2px solid black" rowspan="100">
 										{% for id, widget in configuration_widgets.items %}
 											{% if tool.id == id %}
 												{{ widget }}
@@ -84,18 +89,18 @@
 							</tr>
 						{% endfor %}
 					{% endif %}
 				{% endfor %}
 			</table>
 		{% endfor %}
 		<script>
-			function enable_tool(url)
+			function enable_tool(url, remote_work)
 			{
 				let failure_dialog = ajax_failure_callback("Unable to enable tool");
-				ajax_post(url, undefined, reload_page, failure_dialog);
+				ajax_post(url, {"remote_work": remote_work || ""}, reload_page, failure_dialog);
 			}
 
 			function disable_tool(url)
 			{
 				let failure_dialog = ajax_failure_callback("Unable to disable tool");
 				ajax_post(url, undefined, reload_page, failure_dialog);
 			}
```

### Comparing `NEMO-4.4.1/NEMO/templates/consumables/consumables.html` & `NEMO-4.5.0/NEMO/templates/consumables/consumables.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/consumables/consumables_order.html` & `NEMO-4.5.0/NEMO/templates/consumables/consumables_order.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/consumables/recurring_charge.html` & `NEMO-4.5.0/NEMO/templates/consumables/recurring_charge.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/consumables/recurring_charges.html` & `NEMO-4.5.0/NEMO/templates/consumables/recurring_charges.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/contact/contact_staff.html` & `NEMO-4.5.0/NEMO/templates/contact/contact_staff.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/customizations/customizations.html` & `NEMO-4.5.0/NEMO/templates/customizations/customizations.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/customizations/customizations_application.html` & `NEMO-4.5.0/NEMO/templates/customizations/customizations_application.html`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,13 @@
 {% load custom_tags_and_filters %}
 <div class="panel-body">
     <h3 class="customization-section-title">Application settings</h3>
     <form method="POST" action="{% url 'customize' 'application' %}" class="form-horizontal">
         {% csrf_token %}
         <div class="form-group">
-            <label class="control-label col-md-2">Area login/logout</label>
-            <div class="col-md-10">
-                <div class="checkbox">
-                    <label><input type="checkbox" name="self_log_in" {% if self_log_in %}checked{% endif %} value="enabled">Allow users to log themselves into access controlled areas from the landing page</label><br/>
-                    <label><input type="checkbox" name="self_log_out" {% if self_log_out %}checked{% endif %} value="enabled">Allow users to log themselves out of access controlled areas from the landing page</label><br/>
-                    <label><input type="checkbox" name="calendar_login_logout" {% if calendar_login_logout %}checked{% endif %} value="enabled">Show access controlled area login/logout button on calendar view (requires login and/or logout feature enabled above)</label>
-                </div>
-            </div>
-        </div>
-        <div class="form-group">
             <label class="control-label col-md-2" for="facility_name">Facility name</label>
             <div class="col-md-5">
                 <input type="text" id="facility_name" name="facility_name" class="form-control" value="{{ facility_name }}">
             </div>
             <div class="col-md-5 help-block light-grey">
                 The name of the facility to use in all templates.
             </div>
@@ -27,20 +17,23 @@
             <div class="col-md-5">
                 <input type="text" id="site_title" name="site_title" class="form-control" value="{{ site_title }}">
             </div>
             <div class="col-md-5 help-block light-grey">
                 The name of the site to use in all templates/headers.
             </div>
         </div>
-        <div class="col-md-offset-2">
+        <div class="form-group">
+            <label class="control-label col-md-2">Area login/logout</label>
+            <div class="col-md-10">
+                <div class="checkbox">
+                    <label><input type="checkbox" name="self_log_in" {% if self_log_in %}checked{% endif %} value="enabled">Allow users to log themselves into access controlled areas from the landing page</label><br/>
+                    <label><input type="checkbox" name="self_log_out" {% if self_log_out %}checked{% endif %} value="enabled">Allow users to log themselves out of access controlled areas from the landing page</label><br/>
+                    <label><input type="checkbox" name="calendar_login_logout" {% if calendar_login_logout %}checked{% endif %} value="enabled">Show access controlled area login/logout button on calendar view (requires login and/or logout feature enabled above)</label>
+                </div>
+            </div>
+        </div>
+        <div class="customization-separation" style="margin-bottom: 15px"></div>
+        <div class="text-center">
             {% button type="save" value="Save settings" %}
         </div>
     </form>
-    <script type="text/javascript">
-        $("#application-tab-link").click(function() {setTimeout(on_application_tab_show, 50)});
-        function on_application_tab_show()
-        {
-            auto_size_textarea(document.getElementById('project_selection_template'))
-        }
-        on_application_tab_show();
-    </script>
 </div>
```

### Comparing `NEMO-4.4.1/NEMO/templates/customizations/customizations_calendar.html` & `NEMO-4.5.0/NEMO/templates/customizations/customizations_calendar.html`

 * *Files 1% similar despite different names*

```diff
@@ -107,12 +107,13 @@
                     <label style="padding-right: 20px;"><input type="checkbox" id="calendar_all_tools" name="calendar_all_tools" {% if calendar_all_tools  %}checked{% endif %} value="enabled"> Enable all tools option</label>
                     <label style="padding-right: 20px;"><input type="checkbox" id="calendar_all_areas" name="calendar_all_areas" {% if calendar_all_areas %}checked{% endif %} value="enabled"> Enable all areas option</label>
                     <label style="padding-right: 20px;"><input type="checkbox" id="calendar_all_areastools" name="calendar_all_areastools" {% if calendar_all_areastools %}checked{% endif %} value="enabled"> Enable all tools & areas option</label>
                     <label style="padding-right: 20px;"><input type="checkbox" id="calendar_qualified_tools" name="calendar_qualified_tools" {% if calendar_qualified_tools %}checked{% endif %} value="enabled"> Show qualified tools button</label>
                 </div>
             </div>
         </div>
-        <div class="col-md-offset-2">
+        <div class="customization-separation" style="margin-bottom: 15px"></div>
+        <div class="text-center">
             {% button type="save" value="Save settings" %}
         </div>
     </form>
 </div>
```

### Comparing `NEMO-4.4.1/NEMO/templates/customizations/customizations_dashboard.html` & `NEMO-4.5.0/NEMO/templates/customizations/customizations_dashboard.html`

 * *Files 2% similar despite different names*

```diff
@@ -84,12 +84,13 @@
                 <div class="radio">
                     <label><input type="radio" id="dashboard_staff_status_staff_view" name="dashboard_staff_status_staff_view" {% if not dashboard_staff_status_staff_view %}checked{% endif %} value=""> Day/Week/Month</label>
                     <label><input type="radio" id="dashboard_staff_status_staff_view" name="dashboard_staff_status_staff_view" {% if dashboard_staff_status_staff_view == 'week' %}checked{% endif %} value="week"> Day/Week</label>
                     <label><input type="radio" id="dashboard_staff_status_staff_view" name="dashboard_staff_status_staff_view" {% if dashboard_staff_status_staff_view == 'day' %}checked{% endif %} value="day"> Day</label>
                 </div>
             </div>
         </div>
-        <div class="col-md-offset-2">
+        <div class="customization-separation" style="margin-bottom: 15px"></div>
+        <div class="text-center">
             {% button type="save" value="Save settings" %}
         </div>
     </form>
 </div>
```

### Comparing `NEMO-4.4.1/NEMO/templates/customizations/customizations_emails.html` & `NEMO-4.5.0/NEMO/templates/customizations/customizations_emails.html`

 * *Files 5% similar despite different names*

```diff
@@ -51,12 +51,13 @@
                 {% if errors.user_office_email_address %}
                     {{ errors.user_office_email_address.error }}
                 {% else %}
                     The main point of contact for users to obtain {{ facility_name }} information. Automated emails sent from {{ site_title }} are typically 'from' this address.
                 {% endif %}
             </div>
         </div>
-        <div class="col-md-offset-2">
+        <div class="customization-separation" style="margin-bottom: 15px"></div>
+        <div class="text-center">
             {% button type="save" value="Save settings" %}
         </div>
     </form>
 </div>
```

### Comparing `NEMO-4.4.1/NEMO/templates/customizations/customizations_interlock.html` & `NEMO-4.5.0/NEMO/templates/customizations/customizations_interlock.html`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,16 @@
             <label class="control-label col-md-2">Bypass on error</label>
             <div class="col-md-10">
                 <div class="checkbox">
                     <label><input type="checkbox" name="allow_bypass_interlock_on_failure" {% if allow_bypass_interlock_on_failure %}checked{% endif %} value="enabled">Check this box to offer users the option to bypass lock/unlock command when there is an interlock error.</label><br/>
                 </div>
             </div>
         </div>
-        <div class="col-md-offset-2">
+        <div class="customization-separation" style="margin-bottom: 15px"></div>
+        <div class="text-center">
             {% button type="save" value="Save settings" %}
         </div>
     </form>
     <script type="text/javascript">
         $("#interlock-tab-link").click(function() {setTimeout(on_interlock_tab_show, 50)});
         function on_interlock_tab_show()
         {
```

### Comparing `NEMO-4.4.1/NEMO/templates/customizations/customizations_projects_and_accounts.html` & `NEMO-4.5.0/NEMO/templates/customizations/customizations_projects_and_accounts.html`

 * *Files 23% similar despite different names*

```diff
@@ -1,70 +1,95 @@
 {% load custom_tags_and_filters %}
 <div class="panel-body">
     <h3 class="customization-section-title">Projects & accounts</h3>
     <form method="POST" action="{% url 'customize' 'projects_and_accounts' %}" class="form-horizontal">
         {% csrf_token %}
         <div class="form-group" style="margin-bottom: 0">
-            <label class="control-label col-md-2" for="account_list_active_only">Account list</label>
-            <div class="col-md-3">
+            <label class="control-label col-md-3" for="account_list_active_only">Account list</label>
+            <div class="col-md-9">
                 <div class="checkbox">
                     <label><input type="checkbox" id="account_list_active_only" name="account_list_active_only" {% if account_list_active_only %}checked{% endif %} value="enabled"> Hide inactive accounts</label>
                 </div>
             </div>
-            <div class="col-md-7 help-block light-grey">
+            <div class="col-md-offset-3 col-md-9 help-block light-grey">
                 Check this box to only show active accounts in the user list.
             </div>
         </div>
         <div class="form-group" style="margin-bottom: 0">
-            <div class="col-md-offset-2 col-md-3">
+            <div class="col-md-offset-3 col-md-9">
                 <div class="checkbox">
                     <label><input type="checkbox" id="project_list_active_only" name="project_list_active_only" {% if project_list_active_only %}checked{% endif %} value="enabled"> Hide inactive projects</label>
                 </div>
             </div>
-            <div class="col-md-7 help-block light-grey">
+            <div class="col-md-offset-3 col-md-9 help-block light-grey">
                 Check this box to only show active projects in the user list.
             </div>
         </div>
         <div class="form-group">
-            <div class="col-md-offset-2 col-md-4">
+            <div class="col-md-offset-3 col-md-9">
                 <div class="checkbox">
                     <label><input type="checkbox" id="account_list_collapse" name="account_list_collapse" {% if account_list_collapse %}checked{% endif %} value="enabled"> Collapse project list by default</label>
                 </div>
             </div>
-            <div class="col-md-6 help-block light-grey">
+            <div class="col-md-offset-3 col-md-9 help-block light-grey">
                 Check this box to collapse account projects by default.
             </div>
         </div>
+		<div class="form-group">
+			<label class="control-label col-md-3" for="project_allow_pi_manage_users">Project PIs</label>
+            <div class="col-md-8">
+                <div class="checkbox">
+                    <label><input type="checkbox" id="project_allow_pi_manage_users" name="project_allow_pi_manage_users" {% if project_allow_pi_manage_users %}checked{% endif %} value="enabled"> Allow project PIs to manage users</label>
+                </div>
+            </div>
+            <div class="col-md-offset-3 col-md-8 help-block light-grey">
+                Check this box to allow project PIs to add/remove users to/from projects.
+            </div>
+        </div>
+        <div class="form-group {% if errors.project_application_identifier_name %}has-error{% endif %}">
+            <label class="control-label col-md-3" for="project_application_identifier_name">Project identifier name</label>
+            <div class="col-md-8">
+                <input type="text" id="project_application_identifier_name" name="project_application_identifier_name" class="form-control" value="{{ project_application_identifier_name }}">
+            </div>
+            <div class="col-md-offset-3 col-md-8 help-block light-grey">
+                {% if errors.project_application_identifier_name %}
+                    {{ errors.project_application_identifier_name.error }}
+                {% else %}
+                    The name of the project identifier property (Application, ID, Reference, PO etc.).
+                {% endif %}
+            </div>
+        </div>
         <div class="form-group {% if errors.project_selection_template %}has-error{% endif %}">
-            <label class="control-label col-md-2" for="project_selection_template">Project selection template</label>
-            <div class="col-md-5">
+            <label class="control-label col-md-3" for="project_selection_template">Project selection template</label>
+            <div class="col-md-8">
                 <textarea oninput="auto_size_textarea(this);" id="project_selection_template" name="project_selection_template" class="form-control">{% if errors.project_selection_template %}{{ errors.project_selection_template.value }}{% else %}{{ project_selection_template }}{% endif %}</textarea>
             </div>
-            <div class="col-md-5 help-block light-grey">
+            <div class="col-md-offset-3 col-md-8 help-block light-grey">
                 {% if errors.project_selection_template %}
                     {{ errors.project_selection_template.error }}
                 {% else %}
                     The django template used for rendering project selection when enabling tools and making reservations. The context variable <b>project</b> is provided.
                 {% endif %}
             </div>
         </div>
 		<div class="form-group">
-			<label class="control-label col-md-2">Document upload</label>
+			<label class="control-label col-md-3">Document upload</label>
 			<div class="col-md-5">
 				<div class="checkbox">
 					<label><input type="checkbox" name="project_allow_document_upload" {% if project_allow_document_upload %}checked{% endif %} value="enabled">Enable project document upload</label>
 				</div>
 			</div>
 		</div>
-        <div class="col-md-offset-2">
+        <div class="customization-separation" style="margin-bottom: 15px"></div>
+        <div class="text-center">
             {% button type="save" value="Save settings" %}
         </div>
     </form>
     <script type="text/javascript">
-        $("#application-tab-link").click(function() {setTimeout(on_application_tab_show, 50)});
-        function on_application_tab_show()
+        $("#projects_and_accounts-tab-link").click(function() {setTimeout(on_project_tab_show, 50)});
+        function on_project_tab_show()
         {
             auto_size_textarea(document.getElementById('project_selection_template'))
         }
-        on_application_tab_show();
+        on_project_tab_show();
     </script>
 </div>
```

### Comparing `NEMO-4.4.1/NEMO/templates/customizations/customizations_rates.html` & `NEMO-4.5.0/NEMO/templates/customizations/customizations_rates.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 {% load custom_tags_and_filters %}
-<div class="panel-body">
+<div class="panel-body" style="padding-bottom: 0">
     <h3 class="customization-section-title" id="rate">Rates settings</h3>
     <form method="POST" action="{% url 'customize' 'rates' %}" class="form-horizontal">
         {% csrf_token %}
         <div class="form-group">
             <label class="control-label col-md-2">Rates table</label>
             <div class="col-md-10">
                 <div class="checkbox">
                     <label><input type="checkbox" name="rates_expand_table" {% if rates_expand_table %}checked{% endif %} value="enabled">Expand rates table in tool control</label><br/>
                 </div>
             </div>
         </div>
-        <div class="form-group">
-            <div class="col-md-2"></div>
-			<div class="col-md-5">
-                {% button type="save" value="Save settings" %}
-            </div>
+        <div class="customization-separation" style="margin-bottom: 15px"></div>
+        <div class="text-center">
+            {% button type="save" value="Save settings" %}
         </div>
     </form>
-    <div class="customization-separation" style="clear: both"></div>
-    <div class="form-group form-horizontal" style="margin-top: 15px">
+    <div class="customization-separation" style="margin-top: 15px; margin-bottom: 15px"></div>
+    <div class="form-group form-horizontal">
         <h3 class="customization-section-title" id="rate">Tool Rates</h3>
         <p>
             You can upload a json file to display tool rates. An example of a valid rates file can be found on <a target="_blank" href="https://github.com/usnistgov/NEMO/raw/master/resources/splash_pad_rates.json">Github</a>.
             <br><br>It should be a JSON array of elements, and the following key/values are supported for each element:
         </p>
         <ul>
             <li><b>item_id</b> - the id of the tool or supply</li>
```

### Comparing `NEMO-4.4.1/NEMO/templates/customizations/customizations_recurring_charges.html` & `NEMO-4.5.0/NEMO/templates/customizations/customizations_recurring_charges.html`

 * *Files 2% similar despite different names*

```diff
@@ -47,12 +47,13 @@
             <div class="col-md-3">
                 <input type="number" step="1" id="recurring_charges_force_quantity" name="recurring_charges_force_quantity" class="form-control" value="{{ recurring_charges_force_quantity }}">
             </div>
             <div class="col-md-7 help-block light-grey">
                 [Optional] Define a quantity to be automatically set for every {{ recurring_charges_name|lower }}.
             </div>
         </div>
-        <div class="col-md-offset-2">
+        <div class="customization-separation" style="margin-bottom: 15px"></div>
+        <div class="text-center">
             {% button type="save" value="Save settings" %}
         </div>
     </form>
 </div>
```

### Comparing `NEMO-4.4.1/NEMO/templates/customizations/customizations_safety.html` & `NEMO-4.5.0/NEMO/templates/customizations/customizations_safety.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 {% load custom_tags_and_filters %}
 <div class="panel-body">
     <h3 class="customization-section-title">Safety settings</h3>
     <form method="POST" action="{% url 'customize' 'safety' %}" class="form-horizontal">
         {% csrf_token %}
         <div class="form-group">
-            <label class="control-label col-sm-4 col-md-3" >Main menu item</label>
+            <label class="control-label col-sm-4 col-md-3">Main menu item</label>
             <div class="col-sm-8 col-md-9">
                 <div class="checkbox">
                     <input type="hidden" name="safety_main_menu" value="off"/>
                     <label for="safety_main_menu"><input type="checkbox" id="safety_main_menu" name="safety_main_menu" {% if safety_main_menu != "off" %}checked{% endif %} value=""> Show</label>
                 </div>
             </div>
         </div>
         <div class="form-group">
-            <label class="control-label col-sm-4 col-md-3" >Safety page items</label>
+            <label class="control-label col-sm-4 col-md-3">Safety page items</label>
             <div class="col-sm-8 col-md-9">
                 <div class="checkbox">
                     <div class="row col-sm-12">
                         <input type="hidden" name="safety_show_safety" value="off"/>
                         <label for="safety_show_safety"><input type="checkbox" id="safety_show_safety" name="safety_show_safety" {% if safety_show_safety != "off" %}checked{% endif %} value=""> Safety</label>
                     </div>
                     <div class="row col-sm-12">
@@ -28,28 +28,29 @@
                         <input type="hidden" name="safety_show_safety_data_sheets" value="off"/>
                         <label for="safety_show_safety_data_sheets"><input type="checkbox" id="safety_show_safety_data_sheets" name="safety_show_safety_data_sheets" {% if safety_show_safety_data_sheets != "off" %}checked{% endif %} value=""> Safety data sheets</label>
                     </div>
                 </div>
             </div>
         </div>
         <div class="form-group">
-            <label class="control-label col-sm-4 col-md-3" >Safety items view</label>
+            <label class="control-label col-sm-4 col-md-3">Safety items view</label>
             <div class="col-sm-8 col-md-9">
                 <div class="radio">
                     <label><input type="radio" id="safety_items_expand_categories" name="safety_items_expand_categories" {% if not safety_items_expand_categories %}checked{% endif %} value=""> Side category panel</label>
                     <label><input type="radio" name="safety_items_expand_categories" {% if safety_items_expand_categories %}checked{% endif %} value="enabled"> All expanded categories</label>
                 </div>
             </div>
         </div>
         <div class="form-group">
-            <label class="control-label col-sm-4 col-md-3" >Safety data sheets</label>
+            <label class="control-label col-sm-4 col-md-3">Safety data sheets</label>
             <div class="col-sm-8 col-md-9">
                 <div class="checkbox">
                     <label for="safety_data_sheets_keywords_default"><input type="checkbox" id="safety_data_sheets_keywords_default" name="safety_data_sheets_keywords_default" {% if safety_data_sheets_keywords_default %}checked{% endif %} value="enabled"> Search with keywords by default</label>
                 </div>
             </div>
         </div>
-        <div class="col-sm-offset-4 col-md-offset-3">
+        <div class="customization-separation" style="margin-bottom: 15px"></div>
+        <div class="text-center">
             {% button type="save" value="Save settings" %}
         </div>
     </form>
 </div>
```

### Comparing `NEMO-4.4.1/NEMO/templates/customizations/customizations_templates.html` & `NEMO-4.5.0/NEMO/templates/customizations/customizations_templates.html`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,31 @@
             <li><b>access_requests_url</b> - the URL to the access requests page</li>
         </ul>
         {% include 'customizations/customizations_upload.html' with element=access_request_notification_email name='access request notification email' key='templates' %}
         <div class="customization-separation"></div>
     </div>
 
     <div class="panel-body">
+        <h3 class="customization-section-title" id="adjustment_request_notification_email_id">Adjustment request notification email</h3>
+        <p>This email is sent to the person who created the request when an adjustment request is created or updated. Facility managers are cc'ed.</p>
+        <p>When an adjustment request is approved it is also sent to the User Office</p>
+        <p>The following context variables are provided when the email is rendered:</p>
+        <ul>
+            <li><b>template_color</b> - the color: green if approved, red if denied, blue otherwise</li>
+            <li><b>adjustment_request</b> - the user's adjustment request that was created or updated</li>
+            <li><b>status</b> - the status of the request: received, updated, approved or denied</li>
+            <li><b>adjustment_requests_url</b> - the URL to the adjustment requests page</li>
+            <li><b>manager_note</b> - an extra (optional) note from the manager sent to the user when the request is denied or to the user office when it is approved</li>
+            <li><b>user_office</b> - a flag that is true when the email is addressed to the User Office</li>
+        </ul>
+        {% include 'customizations/customizations_upload.html' with element=adjustment_request_notification_email name='adjustment request notification email' key='templates' %}
+        <div class="customization-separation"></div>
+    </div>
+
+    <div class="panel-body">
         <h3 class="customization-section-title" id="cancellation_email_id">Cancellation email</h3>
         <p>This email is sent to a user when a staff member cancels the user's reservation. The following context variables are provided when the email is rendered:</p>
         <ul>
             <li><b>reservation</b> - the user's reservation that was cancelled</li>
             <li><b>staff_member</b> - the user object of the staff member who cancelled the reservation</li>
             <li><b>reason</b> - the reason the staff member provided for cancelling the reservation</li>
         </ul>
```

#### html2text {}

```diff
@@ -50,14 +50,32 @@
       otherwise
     * access_request - the user's access request that was created or updated
     * status - the status of the request: received, updated, approved or denied
     * access_requests_url - the URL to the access requests page
 {% include 'customizations/customizations_upload.html' with
 element=access_request_notification_email name='access request notification
 email' key='templates' %}
+**** Adjustment request notification email ****
+This email is sent to the person who created the request when an adjustment
+request is created or updated. Facility managers are cc'ed.
+When an adjustment request is approved it is also sent to the User Office
+The following context variables are provided when the email is rendered:
+    * template_color - the color: green if approved, red if denied, blue
+      otherwise
+    * adjustment_request - the user's adjustment request that was created or
+      updated
+    * status - the status of the request: received, updated, approved or denied
+    * adjustment_requests_url - the URL to the adjustment requests page
+    * manager_note - an extra (optional) note from the manager sent to the user
+      when the request is denied or to the user office when it is approved
+    * user_office - a flag that is true when the email is addressed to the User
+      Office
+{% include 'customizations/customizations_upload.html' with
+element=adjustment_request_notification_email name='adjustment request
+notification email' key='templates' %}
 **** Cancellation email ****
 This email is sent to a user when a staff member cancels the user's
 reservation. The following context variables are provided when the email is
 rendered:
     * reservation - the user's reservation that was cancelled
     * staff_member - the user object of the staff member who cancelled the
       reservation
```

### Comparing `NEMO-4.4.1/NEMO/templates/customizations/customizations_upload.html` & `NEMO-4.5.0/NEMO/templates/customizations/customizations_upload.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/customizations/customizations_user.html` & `NEMO-4.5.0/NEMO/templates/customizations/customizations_user.html`

 * *Files 17% similar despite different names*

```diff
@@ -1,76 +1,74 @@
 {% load custom_tags_and_filters %}
 <form method="POST" action="{% url 'customize' 'user' %}" class="form-horizontal">
     <div class="panel-body">
         {% csrf_token %}
         <h3 class="customization-section-title">General</h3>
         <div class="form-group">
-            <label class="control-label col-md-2" for="default_user_training_not_required">New user facility tutorial</label>
-            <div class="col-md-4">
+            <label class="control-label col-md-4 col-lg-3" for="default_user_training_not_required">New user facility tutorial</label>
+            <div class="col-md-8 col-lg-9">
                 <div class="radio">
                     <label><input type="radio" id="default_user_training_not_required" name="default_user_training_not_required" {% if not default_user_training_not_required %}checked{% endif %} value=""> Required</label>
                     <label><input type="radio" name="default_user_training_not_required" {% if default_user_training_not_required %}checked{% endif %} value="enabled"> Not required</label>
                 </div>
             </div>
-            <div class="col-md-6 help-block light-grey">
+            <div class="col-lg-offset-3 col-md-offset-4 col-md-8 col-lg-9 help-block light-grey">
                 Whether the facility rules tutorial is required for new users by default.
             </div>
         </div>
         <div class="form-group">
-            <label class="control-label col-md-2" for="user_list_active_only">User list</label>
-            <div class="col-md-4">
+            <label class="control-label col-md-4 col-lg-3" for="user_list_active_only">User list</label>
+            <div class="col-md-8 col-lg-9">
                 <div class="checkbox">
                     <label><input type="checkbox" id="user_list_active_only" name="user_list_active_only" {% if user_list_active_only %}checked{% endif %} value="enabled"> Hide inactive</label>
                 </div>
             </div>
-            <div class="col-md-6 help-block light-grey">
+            <div class="col-lg-offset-3 col-md-offset-4 col-md-8 col-lg-9 help-block light-grey">
                 Check this box to only show active users in the user list.
             </div>
         </div>
         <div class="form-group">
-            <label class="control-label col-md-2" for="user_list_active_only">User document upload</label>
-            <div class="col-md-4">
+            <label class="control-label col-md-4 col-lg-3" for="user_list_active_only">User document upload</label>
+            <div class="col-md-8 col-lg-9">
                 <div class="checkbox">
 					<label><input type="checkbox" name="user_allow_document_upload" {% if user_allow_document_upload %}checked{% endif %} value="enabled">Enable</label>
 				</div>
             </div>
-            <div class="col-md-6 help-block light-grey">
+            <div class="col-lg-offset-3 col-md-offset-4 col-md-8 col-lg-9 help-block light-grey">
                 Check this box to allow uploading documents to users.
             </div>
         </div>
-    </div>
-    <div class="panel-body">
+        <div class="customization-separation" style="margin-bottom: 15px"></div>
         <h3 class="customization-section-title">Access expiration reminder</h3>
 		<div class="form-group {% if errors.user_access_expiration_reminder_days %}has-error{% endif %}">
-            <label class="control-label col-md-2" for="user_access_expiration_reminder_days">Reminder days</label>
-            <div class="col-md-4">
+            <label class="control-label col-md-4 col-lg-3" for="user_access_expiration_reminder_days">Reminder days</label>
+            <div class="col-md-8 col-lg-9">
                 <input type="text" id="user_access_expiration_reminder_days" name="user_access_expiration_reminder_days" class="form-control" value="{% if errors.user_access_expiration_reminder_days %}{{ errors.user_access_expiration_reminder_days.value }}{% else %}{{ user_access_expiration_reminder_days }}{% endif %}"/>
             </div>
-            <div class="col-md-6 help-block light-grey">
+            <div class="col-lg-offset-3 col-md-offset-4 col-md-8 col-lg-9 help-block light-grey">
                 {% if errors.user_access_expiration_reminder_days %}
                     {{ errors.user_access_expiration_reminder_days.error }}
                 {% else %}
                     The number of days to send a reminder prior to the user's access expiration. A comma-separated list can be used for multiple reminders.
                     This setting and the <a href="{% url 'customization' 'templates' %}?#user_access_expiration_reminder_email_id">user access expiration reminder email</a> need to be set to enable this feature.
                 {% endif %}
             </div>
         </div>
 		<div class="form-group {% if errors.user_access_expiration_reminder_cc %}has-error{% endif %}">
-            <label class="control-label col-md-2" for="user_access_expiration_reminder_cc">Reminder email CC</label>
-            <div class="col-md-4">
+            <label class="control-label col-md-4 col-lg-3" for="user_access_expiration_reminder_cc">Reminder email CC</label>
+            <div class="col-md-8 col-lg-9">
                 <input type="text" id="user_access_expiration_reminder_cc" name="user_access_expiration_reminder_cc" class="form-control" value="{% if errors.user_access_expiration_reminder_cc %}{{ errors.user_access_expiration_reminder_cc.value }}{% else %}{{ user_access_expiration_reminder_cc }}{% endif %}" placeholder="information@example.org"/>
             </div>
-            <div class="col-md-6 help-block light-grey">
+            <div class="col-lg-offset-3 col-md-offset-4 col-md-8 col-lg-9 help-block light-grey">
                 {% if errors.user_access_expiration_reminder_cc %}
                     {{ errors.user_access_expiration_reminder_cc.error }}
                 {% else %}
                     Extra email address to copy when a user access expiration reminder is sent. A comma-separated list can be used.
                 {% endif %}
             </div>
         </div>
-    </div>
-    <div class="panel-body">
-        <div class="col-md-offset-2">
+        <div class="customization-separation" style="margin-bottom: 15px"></div>
+        <div class="text-center">
             {% button type="save" value="Save settings" %}
         </div>
     </div>
 </form>
```

### Comparing `NEMO-4.4.1/NEMO/templates/email/compose_email.html` & `NEMO-4.5.0/NEMO/templates/email/compose_email.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/email/email_broadcast.html` & `NEMO-4.5.0/NEMO/templates/email/email_broadcast.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/email/email_form.html` & `NEMO-4.5.0/NEMO/templates/email/email_form.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/event_details/area_access_details.html` & `NEMO-4.5.0/NEMO/templates/event_details/area_access_details.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/event_details/outage_details.html` & `NEMO-4.5.0/NEMO/templates/event_details/outage_details.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/event_details/reservation_details.html` & `NEMO-4.5.0/NEMO/templates/event_details/reservation_details.html`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
                 {# You must provide a reason if you are cancelling someone else's reservation. #}
                 {% if reservation.user == user %}
                     <button type="button" class="btn btn-danger" data-dismiss="modal" onclick="{% if popup_view %}$('#dialog').one('hidden.bs.modal', function() { {% endif %}cancel_reservation('{% url 'cancel_reservation' reservation.id %}', 'Reservation {{ reservation.id }}') {% if popup_view %}}){% endif %}" title="Cancel this reservation"><i class="glyphicon glyphicon-trash"></i> Cancel this reservation</button>
                 {% else %}
                     <div class="input-group">
                         <input type="text" id="reason" class="form-control" placeholder="Reason for cancellation (required)" aria-label="Reason for cancellation (required)" maxlength="3000">
                         <span class="input-group-btn">
-                            <button type="button" class="btn btn-danger" data-dismiss="modal" onclick="{% if popup_view %}$('#dialog').one('hidden.bs.modal', function() { {% endif %}cancel_reservation('{% url 'cancel_reservation' reservation.id %}', 'Reservation {{ reservation.id }}', $('#reason').val()) {% if popup_view %} }) {% endif %}" title="Cancel this reservation"><i class="glyphicon glyphicon-trash"></i>Cancel this reservation</button>
+                            <button type="button" class="btn btn-danger" data-dismiss="modal" onclick="{% if popup_view %}$('#dialog').one('hidden.bs.modal', function() { {% endif %}cancel_reservation('{% url 'cancel_reservation' reservation.id %}', 'Reservation {{ reservation.id }}', $('#reason').val()) {% if popup_view %} }) {% endif %}" title="Cancel this reservation"><i class="glyphicon glyphicon-trash"></i> Cancel this reservation</button>
                         </span>
                     </div>
                     <script>
                         autofocus("#reason");
                     </script>
                 {% endif %}
             </div>
```

#### html2text {}

```diff
@@ -34,12 +34,12 @@
 Additional information: {{ reservation.additional_information|linebreaksbr }}
 {# Allow the user to cancel the reservation if they have that priviledge. #} {%
 if not reservation.missed and not reservation.cancelled %} {% if
 reservation.user.id == user.id and reservation.has_not_ended or user.is_staff
 %}
 {# You must provide a reason if you are cancelling someone else's reservation.
 #} {% if reservation.user == user %}  Cancel this reservation {% else %}
-[                    ]  Cancel this reservation
+[                    ]   Cancel this reservation
  {% endif %}
 {% endif %} {% endif %} {% if popup_view and
 reservation.question_data_json.items %}
  {% endif %} {% endblock %}
```

### Comparing `NEMO-4.4.1/NEMO/templates/event_details/usage_details.html` & `NEMO-4.5.0/NEMO/templates/event_details/usage_details.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/feedback.html` & `NEMO-4.5.0/NEMO/templates/feedback.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/history.html` & `NEMO-4.5.0/NEMO/templates/history.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/impersonate.html` & `NEMO-4.5.0/NEMO/templates/impersonate.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/jumbotron/jumbotron.html` & `NEMO-4.5.0/NEMO/templates/jumbotron/jumbotron.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/jumbotron/jumbotron_content.html` & `NEMO-4.5.0/NEMO/templates/jumbotron/jumbotron_content.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/landing.html` & `NEMO-4.5.0/NEMO/templates/landing.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 {% extends 'base.html' %}
 {% load static %}
+{% load custom_tags_and_filters %}
 
 {% block title %}{{ site_title }}{% endblock %}
 {% block content %}
 	{% if user.training_required %}
 		<div class="row">
 			<div class="col-lg-12">
 				<a href="{% url 'facility_rules' %}">
@@ -119,23 +120,25 @@
 					</a>
 				</div>
 			{% if forloop.counter|divisibleby:4 or forloop.last %}</div>{% endif %}
 		{% empty %}
 			<span style="font-size:xx-large">
 				Welcome! This is {{ site_title }}'s landing page - the first page users see when visiting the site. There's nothing here yet...<br>&nbsp;<br>
 
-				Add landing page choices by navigating to<br>
-				<a href="{% url 'admin:NEMO_landingpagechoice_add' %}">
-					Administration -> Detailed Administration -><br>
-					Landing page choices -> Add landing page choice
-				</a>
-				<br>&nbsp;<br>
+                {% if user.is_superuser and "django.contrib.admin"|app_installed %}
+                    Add landing page choices by navigating to<br>
+                    <a href="{% url 'admin:NEMO_landingpagechoice_add' %}">
+                        Administration -> Detailed Administration -><br>
+                        Landing page choices -> Add landing page choice
+                    </a>
+                    <br>&nbsp;<br>
 
-				Customize {{ site_title }} further by navigating to<br>
-				<a href="{% url 'customization' %}">Administration -> Customization</a>
+                    Customize {{ site_title }} further by navigating to<br>
+                    <a href="{% url 'customization' %}">Administration -> Customization</a>
+                {% endif %}
 			</span>
 		{% endfor %}
     <script>
         let facility_usage_height = document.getElementById('facility-usage') ? document.getElementById('facility-usage').scrollHeight : 0;
         let reservations_height = document.getElementById('upcoming-reservations') ? document.getElementById('upcoming-reservations').scrollHeight : 0;
         if (document.getElementById('alerts-outages'))
         {
```

#### html2text {}

```diff
@@ -1,9 +1,10 @@
-{% extends 'base.html' %} {% load static %} {% block title %}{{ site_title }}{%
-endblock %} {% block content %} {% if user.training_required %}
+{% extends 'base.html' %} {% load static %} {% load custom_tags_and_filters %}
+{% block title %}{{ site_title }}{% endblock %} {% block content %} {% if
+user.training_required %}
 [Caution_image]
 *****_{{_facility_name_}}_Rules_Tutorial_*****
 You_must_complete_your_{{_facility_name_}}_rules_tutorial_before_you_can_make
 reservations_or_use_{{_facility_name_}}_tools._Click_here_to_begin_the
 tutorial.
 [Agreement_icon]
 {% endif %}
@@ -60,15 +61,16 @@
 **** {{ choice.name }} {% if choice.notifications %} {% for type, count in
 notification_counts.items %} {% if choice.notifications == type and count %} {
 { count }} {% endif %} {% endfor %} {% endif %} ****
 {% if forloop.counter|divisibleby:4 or forloop.last %}
 {% endif %} {% empty %}  Welcome! This is {{ site_title }}'s landing page - the
 first page users see when visiting the site. There's nothing here yet...
  
-Add landing page choices by navigating to
+{% if user.is_superuser and "django.contrib.admin"|app_installed %} Add landing
+page choices by navigating to
 Administration_->_Detailed_Administration_->
 Landing_page_choices_->_Add_landing_page_choice
  
 Customize {{ site_title }} further by navigating to
-Administration_->_Customization  {% endfor %}
+Administration_->_Customization {% endif %}  {% endfor %}
  {% endblock %} {% block extra_whitespace %}{# Hide extra whitespace #}{%
 endblock %}
```

### Comparing `NEMO-4.4.1/NEMO/templates/login.html` & `NEMO-4.5.0/NEMO/templates/login.html`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 			{{ site_title }} relies on cookies to work properly. Please modify your web browser settings
 			to allow this site to use cookies. Reload this page after modifying the settings
 			and you will be able to log in.
 		</div>
 
 		{% if user_name_or_password_incorrect %}
 			<div class="alert alert-danger">
-				<span class="glyphicon icon-info"></span> The user name or password was not valid.
+				<span class="glyphicon icon-info"></span> The username or password was not valid.
 			</div>
 		{% endif %}
 
 		{% if login_banner %}
 			<div class="alert alert-info">
 				{{ login_banner|safe }}
 			</div>
```

#### html2text {}

```diff
@@ -16,11 +16,11 @@
 [********************]
 {% button style="width: 100%;" type="save" value="Log in" icon="glyphicon-log-
 in" %}
 {{ site_title }} relies on cookies to work properly. Please modify your web
 browser settings to allow this site to use cookies. Reload this page after
 modifying the settings and you will be able to log in.
 {% if user_name_or_password_incorrect %}
- The user name or password was not valid.
+ The username or password was not valid.
 {% endif %} {% if login_banner %}
 {{ login_banner|safe }}
 {% endif %} {% include 'base/footer.html' %}
```

### Comparing `NEMO-4.4.1/NEMO/templates/maintenance/closed_task_details.html` & `NEMO-4.5.0/NEMO/templates/maintenance/closed_task_details.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/maintenance/maintenance.html` & `NEMO-4.5.0/NEMO/templates/maintenance/maintenance.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/maintenance/pending_task_details.html` & `NEMO-4.5.0/NEMO/templates/maintenance/pending_task_details.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/mobile/cancellation_result.html` & `NEMO-4.5.0/NEMO/templates/mobile/cancellation_result.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/mobile/choose_item.html` & `NEMO-4.5.0/NEMO/templates/mobile/choose_item.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/mobile/individual_outage.html` & `NEMO-4.5.0/NEMO/templates/mobile/individual_outage.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/mobile/individual_reservation.html` & `NEMO-4.5.0/NEMO/templates/mobile/individual_reservation.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/mobile/new_reservation.html` & `NEMO-4.5.0/NEMO/templates/mobile/new_reservation.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/mobile/reservation_success.html` & `NEMO-4.5.0/NEMO/templates/mobile/reservation_success.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/mobile/view_calendar.html` & `NEMO-4.5.0/NEMO/templates/mobile/view_calendar.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/news/archived_news.html` & `NEMO-4.5.0/NEMO/templates/news/archived_news.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/news/new_news_form.html` & `NEMO-4.5.0/NEMO/templates/news/new_news_form.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/news/news_update_form.html` & `NEMO-4.5.0/NEMO/templates/news/news_update_form.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/news/recent_news.html` & `NEMO-4.5.0/NEMO/templates/news/recent_news.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/occupancy/occupancy_content.html` & `NEMO-4.5.0/NEMO/templates/occupancy/occupancy_content.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/occupancy/occupancy_count.html` & `NEMO-4.5.0/NEMO/templates/occupancy/occupancy_count.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/pagination/pagination_base.html` & `NEMO-4.5.0/NEMO/templates/pagination/pagination_base.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/pagination/pagination_column.html` & `NEMO-4.5.0/NEMO/templates/pagination/pagination_column.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/pagination/pagination_pages.html` & `NEMO-4.5.0/NEMO/templates/pagination/pagination_pages.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/pagination/pagination_selector.html` & `NEMO-4.5.0/NEMO/templates/pagination/pagination_selector.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/qualifications.html` & `NEMO-4.5.0/NEMO/templates/qualifications.html`

 * *Files 18% similar despite different names*

```diff
@@ -32,39 +32,42 @@
 			</div>
 			<div class="col-md-6">
 				<div class="form-group">
 					<label for="tool_search">Search for tool</label>
 					<input id='tool_search' class="form-control"/>
 				</div>
 				<div id="chosen_tools" class="form-group"></div>
+				<div id="chosen_toolqualificationgroups" class="form-group"></div>
 			</div>
 		</div>
 	</form>
 
 	<script type="text/javascript">
 		function create_entry(jquery_event, search_selection, dataset_name)
 		{
 			$('#user_search').typeahead('val', '');
 			$('#tool_search').typeahead('val', '');
-			let id = dataset_name + "_" + search_selection.id;
+            {# Use type if provided otherwise the name of the dataset #}
+            let input_name = search_selection.type || dataset_name;
+			let id = input_name + "_" + search_selection.id;
 			if($("#" + id).length)
 				return;
-			$("#chosen_" + dataset_name + "s").append
+			$("#chosen_" + input_name + "s").append
 			(
 					"<div class='form-group'>" +
 					"<button class='btn btn-default' onclick='$(this).closest(\"div\").remove()'>" + search_selection.name + "</button>" +
-					"<input type='hidden' name='chosen_" + dataset_name + "[]' value='" + search_selection.id + "' id='" + dataset_name + "_" + search_selection.id + "'>" +
+					"<input type='hidden' name='chosen_" + input_name + "[]' value='" + search_selection.id + "' id='" + input_name + "_" + search_selection.id + "'>" +
 					"</div>"
 			);
 		}
 
 		function on_load()
 		{
 			$('#user_search').autocomplete('user', create_entry, {{ users|json_search_base }}).focus();
-			$('#tool_search').autocomplete('tool', create_entry, {{ tools|json_search_base }});
+			$('#tool_search').autocomplete('tool', create_entry, {% json_search_base_with_extra_fields tools|add:tool_groups %}, {% if tool_groups %}false{% else %}true{% endif %});
 		}
 
 		$(on_load);
 
 	</script>
 
 {% endblock %}
```

### Comparing `NEMO-4.4.1/NEMO/templates/refresh_sidebar_icons.html` & `NEMO-4.5.0/NEMO/templates/refresh_sidebar_icons.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/remote_work.html` & `NEMO-4.5.0/NEMO/templates/remote_work/remote_work.html`

 * *Files 13% similar despite different names*

```diff
@@ -1,78 +1,80 @@
-{% extends 'base.html' %}
+{% extends 'remote_work/remote_work_base.html' %}
 {% load static %}
 {% load custom_tags_and_filters %}
-{% block title %}Remote work{% endblock %}
+{% block title %}Previous work{% endblock %}
+{% block remote_work_title %}Previous work{% endblock %}
+{% block remote_work_tab_class %}active{% endblock %}
 {% block extrahead %}
 	<script type="text/javascript" src="{% static "datetimepicker/bootstrap-datetimepicker.js" %}"></script>
 	<link rel="stylesheet" type="text/css" href="{% static "datetimepicker/bootstrap-datetimepicker.css" %}"/>
 {% endblock %}
-{% block content %}
-	<h1>Remote work</h1>
-
+{% block tab_content %}
 	<p>This page displays remote work done by {{ facility_name }} staff on behalf of users. You can filter by which staff member performed the work, and
 	when, by using the dropdown boxes below.</p>
 
 	<p>Each charge can be validated, which means that you have confirmed that the charge is legitimate and correct, and no adjustment needs to
 	be made to it. Press the green 'Validate' button on an individual row to validate a charge. Charges that have already been validated are
 	highlighted in <span class="success-highlight">green</span>.</p>
 
 	<p>Do not validate a charge if part or all of it is incorrect. Instead, visit the user office so an adjustment can be entered
 	into the billing system. Furthermore, please visit the user office if there is a charge that you forgot to enter.</p>
 
 	<form id="remote_work_form" class="form-horizontal" role="form" style="margin-top: 20px">
 		<input type="hidden" name="csv" id="hidden_data_csv"/>
 		<div class="form-group">
 			<label class="control-label col-md-2" for="operator">View charges for</label>
-			<div class="col-md-3">
+			<div class="col-md-4">
 				<select id="operator" name="operator" class="form-control">
 					<option {% if selected_staff == "all staff" %}selected{% endif %}>all staff</option>
 					{% for s in staff_list %}
 						<option value="{{ s.id }}" {% if s.id == selected_staff %}selected{% endif %}>{{ s }}</option>
 					{% endfor %}
 				</select>
 			</div>
 			<div class="control-label col-md-2">
 				<label class="text-center" style="width: 100%" for="project">and for</label>
 			</div>
-			<div class="col-md-3">
+			<div class="col-md-4">
 				<select id="project" name="project" class="form-control">
 					<option {% if selected_project == "all projects" %}selected{% endif %}>all projects</option>
 					{% for p in project_list %}
 						<option value="{{ p.id }}" {% if p.id == selected_project %}selected{% endif %}>{{ p }}</option>
 					{% endfor %}
 				</select>
 			</div>
 		</div>
 		<div class="form-group">
 			<label for="month_list" class="control-label col-md-2">during</label>
-			<div class="col-md-2">
+			<div class="col-md-3">
 				<select id="month_list" class="form-control" style="margin-right: 5px;" onchange="set_dates_from_month(this.value)">
 					<option selected></option>
 					{% for month in month_list %}
 						<option>{{ month|date:"F, Y" }}</option>
 					{% endfor %}
 				</select>
 			</div>
-			<div class="control-label col-md-1" style="padding-left: 0;padding-right: 0">
+			<div class="control-label col-md-2" style="padding-left: 0;padding-right: 0">
 				<label for="start_date" class="text-center" style="width: 100%">or between</label>
 			</div>
 			<div class="col-md-2">
 				<input type="text" id="start_date" name="start" class="form-control text-center" placeholder="Choose a date" value="{{ start_date.date|input_date_format }}">
 			</div>
 			<div class="control-label col-md-1">
 				<label for="end_date" class="text-center" style="width: 100%">and</label>
 			</div>
 			<div class="col-md-2">
 				<input type="text" id="end_date" name="end" class="form-control text-center" placeholder="Choose a date" value="{{ end_date.date|input_date_format }}">
 			</div>
 		</div>
 		<div class="form-group" style="margin-top: 25px">
-			<div class="col-sm-12 text-center">
+			<div class="col-md-offset-2 col-md-5 col-xs-6">
                 {% button type="save" submit=False value="Update" icon="glyphicon-refresh" onclick="$('#hidden_data_csv').val('');$('#remote_work_form').submit();" %}
+            </div>
+			<div class="col-md-5 col-xs-6 text-right">
                 {% button type="export" submit=False value="Export" onclick="$('#hidden_data_csv').val('true');$('#remote_work_form').submit();" %}
 			</div>
 		</div>
 	</form>
 
 	<h3>Staff charges</h3>
 	<table class="table">
@@ -80,42 +82,52 @@
 		<tr>
 			<th>ID</th>
 			<th>Staff member</th>
 			<th>Customer</th>
 			<th>Project</th>
 			<th>Start</th>
 			<th>End</th>
-			<th>Validate</th>
+			{% if remote_work_validation %}<th>Validate</th>{% endif %}
 		</tr>
 		</thead>
 		<tbody>
 		{% for c in staff_charges %}
-			<tr class="staff_charge_row_{{ c.id }} {% if c.validated %}success-highlight{% endif %}">
-				<td>{{ c.id }}</td>
+			<tr class="staff_charge_row_{{ c.id }} {% if remote_work_validation and  c.validated %}success-highlight{% endif %}">
+				{% if "django.contrib.admin"|app_installed and perms.NEMO.change_staffcharge %}
+                    <td><a href="{% url 'admin:NEMO_staffcharge_change' c.id %}">{{ c.id }}</a></td>
+                {% else %}
+                    <td>{{ c.id }}</td>
+                {% endif %}
 				<td>{{ c.staff_member }}</td>
 				<td>{{ c.customer }}</td>
 				<td>{{ c.project }}</td>
 				<td>{{ c.start }}</td>
 				<td>{{ c.end|default_if_none:'' }}</td>
-				<td {% if c.note and c.areaaccessrecord_set.exists %}rowspan="3" {% elif c.note or c.areaaccessrecord_set.exists %}rowspan="2"{% endif %} style="vertical-align: middle">
-                    {% url 'validate_staff_charge' c.id as validate_staff_charge_url %}
-                    {% if not c.validated %}
-                        {% button type="save" submit=False onclick="validate_charge('"|concat:validate_staff_charge_url|concat:"', this, '.staff_charge_row_"|concat:c.id|concat:"')" icon="glyphicon-ok-circle" value="Validate" %}
-                    {% endif %}
-                </td>
+				{% if remote_work_validation %}
+                    <td {% if c.note and c.areaaccessrecord_set.exists %}rowspan="3" {% elif c.note or c.areaaccessrecord_set.exists %}rowspan="2"{% endif %} style="vertical-align: middle">
+                        {% url 'validate_staff_charge' c.id as validate_staff_charge_url %}
+                        {% if not c.validated %}
+                            {% button type="save" submit=False onclick="validate_charge('"|concat:validate_staff_charge_url|concat:"', this, '.staff_charge_row_"|concat:c.id|concat:"')" icon="glyphicon-ok-circle" value="Validate" %}
+                        {% endif %}
+                    </td>
+                {% endif %}
 			</tr>
             {% if c.note %}
-                <tr class="staff_charge_row_{{ c.id }} {% if c.validated %}success-highlight{% endif %}">
+                <tr class="staff_charge_row_{{ c.id }} {% if remote_work_validation and c.validated %}success-highlight{% endif %}">
                     <td style="border: none; padding-top: 0"></td>
                     <td colspan="5" style="border:none; padding-top: 0">Charge note: {{ c.note|linebreaksbr }}<br></td>
                 </tr>
             {% endif %}
 			{% for area_access_record in c.areaaccessrecord_set.all %}
-				<tr class="staff_charge_row_{{ c.id }} {% if c.validated %}success-highlight{% endif %}" style="font-size: smaller">
-					<td style="border-top: none"></td>
+				<tr class="staff_charge_row_{{ c.id }} {% if remote_work_validation and c.validated %}success-highlight{% endif %}" style="font-size: smaller">
+					{% if "django.contrib.admin"|app_installed and perms.NEMO.change_areaaccessrecord %}
+                        <td><a href="{% url 'admin:NEMO_areaaccessrecord_change' area_access_record.id %}">{{ area_access_record.id }}</a></td>
+                    {% else %}
+                        <td>{{ area_access_record.id }}</td>
+                    {% endif %}
 					<td colspan="3" style="border-top-style: dotted">{{ area_access_record.area.name }} access</td>
 					<td style="border-top-style: dotted">{{ area_access_record.start }}</td>
 					<td style="border-top-style: dotted">{{ area_access_record.end|default_if_none:'' }}</td>
 				</tr>
 			{%  endfor %}
         {% empty %}
             <tr><td colspan="7">
@@ -134,33 +146,39 @@
 			<th>ID</th>
 			<th>Operator</th>
 			<th>User</th>
 			<th>Project</th>
 			<th>Start</th>
 			<th>End</th>
 			<th>Tool</th>
-			<th>Validate</th>
+			{% if remote_work_validation %}<th>Validate</th>{% endif %}
 		</tr>
 		</thead>
 		<tbody>
 		{% for u in usage %}
-			<tr {% if u.validated %}class="success-highlight"{% endif %} id="usage_event_row_{{ forloop.counter }}">
-				<td>{{ u.id }}</td>
+			<tr {% if remote_work_validation and u.validated %}class="success-highlight"{% endif %} id="usage_event_row_{{ forloop.counter }}">
+				{% if "django.contrib.admin"|app_installed and perms.NEMO.change_usageevent %}
+                    <td><a href="{% url 'admin:NEMO_usageevent_change' u.id %}">{{ u.id }}</a></td>
+                {% else %}
+                    <td>{{ u.id }}</td>
+                {% endif %}
 				<td>{{ u.operator }}</td>
 				<td>{{ u.user }}</td>
 				<td>{{ u.project }}</td>
 				<td>{{ u.start }}</td>
 				<td>{{ u.end|default_if_none:'' }}</td>
 				<td>{{ u.tool }}</td>
-				<td>
-                    {% url 'validate_usage_event' u.id as validate_usage_url %}
-                    {% if not u.validated %}
-                        {% button type="save" submit=False onclick="validate_charge('"|concat:validate_usage_url|concat:"', this, '#usage_event_row_"|concat:forloop.counter|concat:"')" icon="glyphicon-ok-circle" value="Validate" %}
-                    {% endif %}
-                </td>
+				{% if remote_work_validation %}
+                    <td>
+                        {% url 'validate_usage_event' u.id as validate_usage_url %}
+                        {% if not u.validated %}
+                            {% button type="save" submit=False onclick="validate_charge('"|concat:validate_usage_url|concat:"', this, '#usage_event_row_"|concat:forloop.counter|concat:"')" icon="glyphicon-ok-circle" value="Validate" %}
+                        {% endif %}
+                    </td>
+                {% endif %}
 			</tr>
         {% empty %}
             <tr><td colspan="8">
                 {% if start_date or end_date %}
                     No tool usage exist {% if start_date and end_date %}between {{ start_date }} and {{ end_date }}{% elif start_date %}after {{ start_date }}{% else %}before {{ end_date }}{% endif %}.
                 {% endif %}
             </td></tr>
```

#### html2text {}

```diff
@@ -1,12 +1,13 @@
-{% extends 'base.html' %} {% load static %} {% load custom_tags_and_filters %}
-{% block title %}Remote work{% endblock %} {% block extrahead %}
+{% extends 'remote_work/remote_work_base.html' %} {% load static %} {% load
+custom_tags_and_filters %} {% block title %}Previous work{% endblock %} {%
+block remote_work_title %}Previous work{% endblock %} {% block
+remote_work_tab_class %}active{% endblock %} {% block extrahead %}
 ootstrap-datetimepicker.js" %}">
-ootstrap-datetimepicker.css" %}"/> {% endblock %} {% block content %}
-****** Remote work ******
+ootstrap-datetimepicker.css" %}"/> {% endblock %} {% block tab_content %}
 This page displays remote work done by {{ facility_name }} staff on behalf of
 users. You can filter by which staff member performed the work, and when, by
 using the dropdown boxes below.
 Each charge can be validated, which means that you have confirmed that the
 charge is legitimate and correct, and no adjustment needs to be made to it.
 Press the green 'Validate' button on an individual row to validate a charge.
 Charges that have already been validated are highlighted in green.
@@ -29,31 +30,30 @@
 {{ month|date:"F, Y" }}
 {% endfor %}
 or between
 [{{ start_date.date|input_date_format }}]
 and
 [{{ end_date.date|input_date_format }}]
 {% button type="save" submit=False value="Update" icon="glyphicon-refresh"
-onclick="$('#hidden_data_csv').val('');$('#remote_work_form').submit();" %} {%
-button type="export" submit=False value="Export" onclick="$
+onclick="$('#hidden_data_csv').val('');$('#remote_work_form').submit();" %}
+{% button type="export" submit=False value="Export" onclick="$
 ('#hidden_data_csv').val('true');$('#remote_work_form').submit();" %}
 **** Staff charges ****
-ID   Staff member   Customer   Project   Start                    End                                     Validate
-{    {              {          {
-{    {              {          {         {{ c.start }}            {{ c.end|default_if_none:'' }}
-c.id c.staff_member c.customer c.project
-}}   }}             }}         }}
-     Charge note: {{ c.note|linebreaksbr }}
-                                         {                        {
-     {{ area_access_record.area.name }}  {                        {
-     access                              area_access_record.start area_access_record.end|default_if_none:
-                                         }}                       '' }}
-{% if start_date or end_date %} No staff charges exist {% if start_date and end_date %}between {{ start_date }}
-and {{ end_date }}{% elif start_date %}after {{ start_date }}{% else %}before {{ end_date }}{% endif %}. {% endif
-%}
+ID                    Staff member          Customer       Project    Start     End                      Validate
+                                            {              {          {
+{{_c.id_}}            {{ c.id }}            {              {          {         {{ c.start }}            {{ c.end|default_if_none:'' }}
+                                            c.staff_member c.customer c.project
+                                            }}             }}         }}
+                      Charge note: {{ c.note|linebreaksbr }}
+{                     {                                                         {                        {
+{                     {                     {{ area_access_record.area.name }}  {                        {
+area_access_record.id area_access_record.id access                              area_access_record.start area_access_record.end|default_if_none:
+}}                    }}                                                        }}                       '' }}
+{% if start_date or end_date %} No staff charges exist {% if start_date and end_date %}between {{ start_date }} and {{ end_date }}{% elif
+start_date %}after {{ start_date }}{% else %}before {{ end_date }}{% endif %}. {% endif %}
 
 **** Tool usage ****
 ID Operator User Project Start End Tool Validate
 {% if start_date or end_date %} No tool usage exist {% if start_date and
 end_date %}between {{ start_date }} and {{ end_date }}{% elif start_date
 %}after {{ start_date }}{% else %}before {{ end_date }}{% endif %}. {%
 endif %}
```

### Comparing `NEMO-4.4.1/NEMO/templates/requests/access_requests/access_request.html` & `NEMO-4.5.0/NEMO/templates/requests/access_requests/access_request.html`

 * *Files 3% similar despite different names*

```diff
@@ -43,24 +43,30 @@
                     {% else %}
                         {% for physical_access_level in physical_access_levels %}
                             <option value="{{ physical_access_level.id }}" {% if form.physical_access_level.value|to_int == physical_access_level.id %}selected{% endif %}>{{ physical_access_level.display_value_for_select }}</option>
                         {% endfor %}
                     {% endif %}
                     </select>
                 </div>
+                {% if form.instance.id and user.is_facility_manager %}
+                    <div class="col-sm-6">
+                        <label for="creator_readonly" class="control-label">Creator</label>
+                        <input id="creator_readonly" class="form-control" style="min-width: 250px;" disabled value="{{ form.instance.creator }}">
+                    </div>
+                {% endif %}
             </div>
 		</div>
 		<div class="form-group">
             <div class="row">
                 <div class="col-sm-6">
                     <label for="search_other_users" class="control-label">Buddies</label>
                     <input id="search_other_users" type="text" class="form-control" placeholder="Search for other users to add as your buddies" style="min-width: 250px;">
                 </div>
                 <div class="col-sm-6" id="other_users_label" style="display: none">
-                    <div style="margin-bottom: 5px;">Selected users</div>
+                    <div style="margin-bottom: 5px;">Selected buddies</div>
                     <ul id="other_users" class="form-control form-control-static" style="height: 100%">
                     </ul>
                 </div>
             </div>
             {% if form.other_users.errors %}
                 <div class="row">
                     <div class="col-sm-6"><span style="color:red">{{ form.other_users.errors|striptags }}</span></div>
@@ -68,15 +74,15 @@
             {% endif %}
 		</div>
 		<div class="form-group">
 			<label for="description" class="control-label">Description</label>{% if form.description.errors %} - <span style="color:red">{{ form.description.errors|striptags }}</span>{% endif %}
 			<textarea class="form-control" rows="3" name="description" id="description" maxlength="{{ form.fields.description.max_length }}" placeholder="Provide additional details if needed">{{ form.description.value|default_if_none:"" }}</textarea>
 		</div>
 		<div class="text-right">
-            {% if form.instance.status == form.instance.Status.PENDING %}
+            {% if form.instance.get_status_display == "Pending" %}
                 {% if form.instance.id and user.is_facility_manager %}
                     {% button type="save" submit=False name="approve_request" title="Approve request" icon="glyphicon-ok-circle" value="Approve" onclick="if (confirm('Are you sure you want to approve this request?')) {submit_and_disable(this)}" %}
                     {% button type="delete" submit=False name="deny_request" title="Deny request" icon="glyphicon-ban-circle" value="Deny" onclick="if (confirm('Are you sure you want to deny this request?')) {submit_and_disable(this)}" %}
                 {% else %}
                     {% button type="save" value=form.instance.id|yesno:"Save changes,Create access request" %}
                 {% endif %}
             {% endif %}
```

#### html2text {}

```diff
@@ -17,26 +17,29 @@
 {% endif %}
 {% if physical_access_levels|length_is:1 %}
 {{ physical_access_levels.0.display_value_for_select }}
 {% else %} {% for physical_access_level in physical_access_levels %}
 % if form.physical_access_level.value|to_int == physical_access_level.id
 %}selected{% endif %}>{{ physical_access_level.display_value_for_select }}
 {% endfor %} {% endif %}
+{% if form.instance.id and user.is_facility_manager %}
+Creator [{{ form.instance.creator }}]
+{% endif %}
 Buddies [                    ]
-Selected users
+Selected buddies
 {% if form.other_users.errors %}
 {{ form.other_users.errors|striptags }}
 {% endif %}
 Description{% if form.description.errors %} - {
 { form.description.errors|striptags }}{% endif %}
 {{ form.description.value|default_if_none:"" }}
-{% if form.instance.status == form.instance.Status.PENDING %} {% if
-form.instance.id and user.is_facility_manager %} {% button type="save"
-submit=False name="approve_request" title="Approve request" icon="glyphicon-ok-
-circle" value="Approve" onclick="if (confirm('Are you sure you want to approve
-this request?')) {submit_and_disable(this)}" %} {% button type="delete"
-submit=False name="deny_request" title="Deny request" icon="glyphicon-ban-
-circle" value="Deny" onclick="if (confirm('Are you sure you want to deny this
+{% if form.instance.get_status_display == "Pending" %} {% if form.instance.id
+and user.is_facility_manager %} {% button type="save" submit=False
+name="approve_request" title="Approve request" icon="glyphicon-ok-circle"
+value="Approve" onclick="if (confirm('Are you sure you want to approve this
+request?')) {submit_and_disable(this)}" %} {% button type="delete" submit=False
+name="deny_request" title="Deny request" icon="glyphicon-ban-circle"
+value="Deny" onclick="if (confirm('Are you sure you want to deny this
 request?')) {submit_and_disable(this)}" %} {% else %} {% button type="save"
 value=form.instance.id|yesno:"Save changes,Create access request" %} {% endif
 %} {% endif %}
  {% endblock %}
```

### Comparing `NEMO-4.4.1/NEMO/templates/requests/access_requests/access_requests.html` & `NEMO-4.5.0/NEMO/templates/requests/access_requests/access_requests.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 {% load custom_tags_and_filters %}
 <div style="margin: 15px 0">
     <div style="display: table-cell; width: 100%">
         {% if access_requests_description %}
             <div class="well" style="display: table; margin-right: 15px">
                 <span class="requests-description-info glyphicon glyphicon-info-sign primary-highlight"></span>
-                <div class="requests-description">{{ access_requests_description|linebreaksbr }}</div>
+                <div class="requests-description">{{ access_requests_description|safe|linebreaksbr }}</div>
             </div>
         {% endif %}
     </div>
-    <div class="align-right" style="display: table-cell; vertical-align: top">{% button type="add" url="create_access_request" value="New request" %}</div>
+    <div class="text-right" style="display: table-cell; vertical-align: top">{% button type="add" url="create_access_request" value="New request" %}</div>
 </div>
 {% if pending_access_requests or approved_access_requests or denied_access_requests or expired_access_requests %}
+    {% if user.is_superuser or user.is_facility_manager or user.is_user_office %}
+        <div class="text-right" style="margin-bottom: -20px">
+            {% button type="export" value="Export" url="export_access_requests" target="_blank" %}
+        </div>
+    {% endif %}
     <div>
         {% if pending_access_requests %}
             <h3><a onclick="toggle_details(this)" data-toggle="collapse" data-target="#pending_access_requests" class="pointer">
                 <span class="glyphicon glyphicon-chevron-down pull-left chevron"></span>Pending ({{ pending_access_requests|length }})
             </a></h3>
             <div id="pending_access_requests" class="collapse in">
                 {% include 'requests/access_requests/access_requests_table.html' with request_status='pending' access_request_list=pending_access_requests %}
```

### Comparing `NEMO-4.4.1/NEMO/templates/requests/access_requests/access_requests_table.html` & `NEMO-4.5.0/NEMO/templates/requests/access_requests/access_requests_table.html`

 * *Files 2% similar despite different names*

```diff
@@ -29,28 +29,28 @@
                     <ul style="padding-inline-start: 25px; margin-bottom: 0">
                         <li><b>{{ a_request.creator }}</b></li>
                         {% for other_user in a_request.other_users.all %}
                             <li>{{ other_user }}</li>
                         {% endfor %}
                     </ul>
                 </td>
-                <td class="text-center" style="vertical-align: middle">
+                <td class="text-center text-nowrap" style="vertical-align: middle">
                     {% if request_status == 'pending' and user.is_facility_manager %}
                         <a class="btn btn-sm btn-default" title="Approve/Deny" href="{% url 'edit_access_request' a_request.id %}"><i class="glyphicon glyphicon-ok-circle success-highlight"></i>&nbsp;&nbsp;<i class="glyphicon glyphicon-ban-circle danger-highlight"></i> Review</a>
                     {% elif request_status == 'pending' and a_request.creator == user %}
                         {% url 'edit_access_request' a_request.id as edit_request_url %}
                         {% url 'delete_access_request' a_request.id as delete_request_url %}
                         {% button type="edit" size="small" value="Edit" title="Edit request" url=edit_request_url %}
                         {% button type="delete" size="small" value="Delete" title="Delete request" url=delete_request_url onclick="return confirm('Are you sure you want to delete this request?');" %}
                     {% elif request_status == 'approved' or request_status == 'denied' %}
                         {{ a_request.reviewer.get_name }}
                     {% endif %}
                 </td>
             </tr>
             <tr>
                 {% if a_request.description %}
-                    <td colspan="{% if user.is_facility_manager %}7{% else %}6{% endif %}" style="border: none">{% if a_request.description %}<u>Description:</u><br>{{ a_request.description|linebreaksbr }}{% endif %}</td>
+                    <td colspan="6" style="border: none">{% if a_request.description %}<u>Description:</u><br>{{ a_request.description|linebreaksbr }}{% endif %}</td>
                 {% endif %}
             </tr>
         {% endfor %}
     </tbody>
 </table>
```

#### html2text {}

```diff
@@ -1,48 +1,44 @@
 {% load custom_tags_and_filters %}
-                                                                                                                                                                                {% if request_status ==
-                                                                                                                                                                                'pending' and
-                                                                                                                                                                                user.is_facility_manager %}
-                                                                                                                                                                                Action {% elif
-Created                            Access                                                   Requested start            Requested end            Users                           request_status ==
-                                                                                                                                                                                'approved' %} Approved by
-                                                                                                                                                                                {% elif request_status ==
-                                                                                                                                                                                'denied' %} Denied by {%
-                                                                                                                                                                                endif %}
-                                                                                                                                                                                {% if request_status ==
-                                                                                                                                                                                'pending' and
-                                                                                                                                                                                user.is_facility_manager %}
-                                                                                                                                                                                  _Review
-                                                                                                                                                                                 {% elif request_status ==
-                                                                                                                                                                                'pending' and
-                                                                                                                                                                                a_request.creator == user
-                                                                                                                                                                                %} {% url
-                                                                                                                                                                                'edit_access_request'
-                                                                                                                                                                                a_request.id as
-                                                                                                                                                                                edit_request_url %} {% url
-                                                                                                                                                                                'delete_access_request'
-                                                                                                                                                                                a_request.id as
-{% if a_request.id in                                                                                                  {                            * {{ a_request.creator }}   delete_request_url %} {%
-access_request_notifications %}New {                                                        {                          {                            * {% for other_user in      button type="edit"
-{% endif %}{                       {                                                        {                          a_request.end_time|date:       a_request.other_users.all size="small" value="Edit"
-{ a_request.creation_time|date:    a_request.physical_access_level.display_value_for_select a_request.start_time|date: 'SHORT_DATETIME_FORMAT'        %}                        title="Edit request"
-'SHORT_DATETIME_FORMAT' }}         }}                                                       'SHORT_DATETIME_FORMAT' }} }}                           * {{ other_user }}          url=edit_request_url %} {%
-                                                                                                                                                    * {% endfor %}              button type="delete"
-                                                                                                                                                                                size="small" value="Delete"
-                                                                                                                                                                                title="Delete request"
-                                                                                                                                                                                url=delete_request_url
-                                                                                                                                                                                onclick="return confirm
-                                                                                                                                                                                ('Are you sure you want to
-                                                                                                                                                                                delete this request?');" %}
-                                                                                                                                                                                {% elif request_status ==
-                                                                                                                                                                                'approved' or
-                                                                                                                                                                                request_status == 'denied'
-                                                                                                                                                                                %} {
-                                                                                                                                                                                {
-                                                                                                                                                                                a_request.reviewer.get_name
-                                                                                                                                                                                }} {% endif %}
-{% if a_request.description
-%}Description:
-{
-{
-a_request.description|linebreaksbr
-}}{% endif %}
+                                                                                                                                                                           {% if request_status ==
+                                                                                                                                                                           'pending' and
+                                                                                                                                                                           user.is_facility_manager %}
+                                                                                                                                                                           Action {% elif
+Created                       Access                                                   Requested start            Requested end            Users                           request_status ==
+                                                                                                                                                                           'approved' %} Approved by
+                                                                                                                                                                           {% elif request_status ==
+                                                                                                                                                                           'denied' %} Denied by {%
+                                                                                                                                                                           endif %}
+                                                                                                                                                                           {% if request_status ==
+                                                                                                                                                                           'pending' and
+                                                                                                                                                                           user.is_facility_manager %}
+                                                                                                                                                                             _Review
+                                                                                                                                                                            {% elif request_status ==
+                                                                                                                                                                           'pending' and
+                                                                                                                                                                           a_request.creator == user
+                                                                                                                                                                           %} {% url
+                                                                                                                                                                           'edit_access_request'
+                                                                                                                                                                           a_request.id as
+                                                                                                                                                                           edit_request_url %} {% url
+                                                                                                                                                                           'delete_access_request'
+                                                                                                                                                                           a_request.id as
+{% if a_request.id in                                                                                             {                            * {{ a_request.creator }}   delete_request_url %} {%
+access_request_notifications  {                                                        {                          {                            * {% for other_user in      button type="edit"
+%}New {% endif %}{            {                                                        {                          a_request.end_time|date:       a_request.other_users.all size="small" value="Edit"
+{                             a_request.physical_access_level.display_value_for_select a_request.start_time|date: 'SHORT_DATETIME_FORMAT'        %}                        title="Edit request"
+a_request.creation_time|date: }}                                                       'SHORT_DATETIME_FORMAT' }} }}                           * {{ other_user }}          url=edit_request_url %} {%
+'SHORT_DATETIME_FORMAT' }}                                                                                                                     * {% endfor %}              button type="delete"
+                                                                                                                                                                           size="small" value="Delete"
+                                                                                                                                                                           title="Delete request"
+                                                                                                                                                                           url=delete_request_url
+                                                                                                                                                                           onclick="return confirm
+                                                                                                                                                                           ('Are you sure you want to
+                                                                                                                                                                           delete this request?');" %}
+                                                                                                                                                                           {% elif request_status ==
+                                                                                                                                                                           'approved' or
+                                                                                                                                                                           request_status == 'denied'
+                                                                                                                                                                           %} {
+                                                                                                                                                                           {
+                                                                                                                                                                           a_request.reviewer.get_name
+                                                                                                                                                                           }} {% endif %}
+{% if a_request.description %}Description:
+{{ a_request.description|linebreaksbr }}{% endif %}
```

### Comparing `NEMO-4.4.1/NEMO/templates/requests/buddy_requests/buddy_request.html` & `NEMO-4.5.0/NEMO/templates/requests/buddy_requests/buddy_request.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/requests/buddy_requests/buddy_requests.html` & `NEMO-4.5.0/NEMO/templates/requests/buddy_requests/buddy_requests.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 {% load custom_tags_and_filters %}
 <div style="margin: 15px 0">
     <div style="display: table-cell; width: 100%">
         {% if buddy_board_description %}
             <div class="well" style="display: table; margin-right: 15px">
                 <span class="requests-description-info glyphicon glyphicon-info-sign primary-highlight"></span>
-                <div class="requests-description">{{ buddy_board_description|linebreaksbr }}</div>
+                <div class="requests-description">{{ buddy_board_description|safe|linebreaksbr }}</div>
             </div>
         {% endif %}
     </div>
-    <div class="align-right" style="display: table-cell; vertical-align: top">{% button type="add" value="New request" url="create_buddy_request" %}</div>
+    <div class="text-right" style="display: table-cell; vertical-align: top">{% button type="add" value="New request" url="create_buddy_request" %}</div>
 </div>
 {% if buddy_requests %}
     <div class="table-responsive buddy-system-requests">
         {% regroup buddy_requests by start as requests_by_date %}
         {% for date in requests_by_date %}
             <h3>{{ date.grouper|date }}</h3>
             <ul class="buddy-list-day">
@@ -32,20 +32,20 @@
                                             {% button type="edit" size="small" url=edit_buddy_request_url value="Edit" %}
                                             {% url 'delete_buddy_request' br.id as delete_buddy_request_url %}
                                             {% button type="delete" size="small" url=delete_buddy_request_url value="Delete" %}
                                         </div>
                                     {% endif %}
                                 </div>
                             </li>
-                            {% for message in br.replies.all %}
+                            {% for message in br.replies %}
                                 <li class="buddy-list-item" id="{{ message.id }}">
                                     {% if message.id in reply_notifications %}<span class="label label-success">New reply</span>{% endif %}
                                     <div class="list-group-item buddy-list-item-message">
                                         {{ message.content|linebreaksbr }}
-                                        <div class="buddy-list-item-message-user">{{ message.author.get_name }}, {{ message.creation_date }}</div>
+                                        <div class="request-item-message-user">{{ message.author.get_name }}, {{ message.creation_date }}</div>
                                     </div>
                                 </li>
                             {% endfor %}
                             <li class="buddy-list-item" style="display: none">
                                 <div class="buddy-list-item-reply list-group-item-text">
                                     <form id="buddy_request_reply_{{ br.id }}" action="{% url 'buddy_request_reply' br.id %}" method="post">
                                         {% csrf_token %}
```

### Comparing `NEMO-4.4.1/NEMO/templates/requests/user_requests.html` & `NEMO-4.5.0/NEMO/templates/requests/user_requests.html`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 {% extends 'base.html' %}
 {% block title %}Requests{% endblock %}
 {% block content %}
     <div class="clearfix" style="margin-top: 0;">
-        <span class="h1" style="margin-top: 0;margin-right: 15px">{% if tab == 'access' %}{{ access_requests_title }}{% elif tab == 'buddy' %}{{ buddy_requests_title }}{% else %}Requests{% endif %}</span>
         <ul class="nav nav-pills nav-pills-spacer" id="tabs" style="display: inline-block;float: right; margin-bottom: 15px">
             {% if access_user_request_allowed_exist and facility_managers_exist %}
                 <li class="{% if tab == 'access' %}active{% endif %}">
                     <a href="#access-requests" onclick="location.href = '{% url "user_requests" "access" %}'">{{ access_requests_title }}
                         {% if temporary_access_notification_count %}
                             <span class="badge badge-tab-top">{{ temporary_access_notification_count }}</span>
                         {% endif %}
@@ -18,24 +17,39 @@
                     <a href="#buddy-requests" onclick="location.href = '{% url "user_requests" "buddy" %}'">{{ buddy_requests_title }}
                         {% if buddy_notification_count %}
                             <span class="badge badge-tab-top">{{ buddy_notification_count }}</span>
                         {% endif %}
                     </a>
                 </li>
             {% endif %}
+            {% if adjustment_request_allowed and facility_managers_exist %}
+                <li class="{% if tab == 'adjustment' %}active{% endif %}">
+                    <a href="#adjustment-requests" onclick="location.href = '{% url "user_requests" "adjustment" %}'">{{ adjustment_requests_title }}
+                        {% if adjustment_notification_count %}
+                            <span class="badge badge-tab-top">{{ adjustment_notification_count }}</span>
+                        {% endif %}
+                    </a>
+                </li>
+            {% endif %}
         </ul>
+        <h1 class="pull-left" style="margin-top: 0;margin-right: 20px">{% if tab == 'access' %}{{ access_requests_title }}{% elif tab == 'buddy' %}{{ buddy_requests_title }}{% elif tab == 'adjustment' %}{{ adjustment_requests_title }}{% else %}Requests{% endif %}</h1>
     </div>
     <div class="tab-content">
         {% if access_user_request_allowed_exist and facility_managers_exist %}
-            <div class="tab-pane {% if tab == 'access' %}active{% endif %}" id="access-requests">
+            <div class="tab-pane{% if tab == 'access' %} active{% endif %}" id="access-requests">
                 {# This will be loaded asynchronously #}
             </div>
         {% endif %}
         {% if buddy_system_areas_exist %}
-	        <div class="tab-pane {% if tab == 'buddy' %}active{% endif %}" id="buddy-requests">
+	        <div class="tab-pane{% if tab == 'buddy' %} active{% endif %}" id="buddy-requests">
+                {# This will be loaded asynchronously #}
+            </div>
+        {% endif %}
+        {% if adjustment_request_allowed and facility_managers_exist %}
+            <div class="tab-pane{% if tab == 'adjustment' %} active{% endif %}" id="adjustment-requests">
                 {# This will be loaded asynchronously #}
             </div>
         {% endif %}
     </div>
     <script>
         $("#tabs").find("a").click(switch_tab);
 
@@ -45,11 +59,17 @@
             $("#buddy-requests").load("{% url 'buddy_requests' %}", undefined, failure_dialog);
         }
         function load_access_requests()
         {
             let failure_dialog = ajax_complete_callback("Unable to load access requests", "There was a problem loading access requests.");
             $("#access-requests").load("{% url 'access_requests' %}", undefined, failure_dialog);
         }
+        function load_adjustment_requests()
+        {
+            let failure_dialog = ajax_complete_callback("Unable to load adjustment requests", "There was a problem loading adjustment requests.");
+            $("#adjustment-requests").load("{% url 'adjustment_requests' %}", undefined, failure_dialog);
+        }
         {% if tab == 'buddy' %}load_buddy_board();{% endif %}
         {% if tab == 'access' %}load_access_requests();{% endif %}
+        {% if tab == 'adjustment' %}load_adjustment_requests();{% endif %}
     </script>
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,18 +1,25 @@
 {% extends 'base.html' %} {% block title %}Requests{% endblock %} {% block
 content %}
-{% if tab == 'access' %}{{ access_requests_title }}{% elif tab == 'buddy' %}{
-{ buddy_requests_title }}{% else %}Requests{% endif %}
     * {% if access_user_request_allowed_exist and facility_managers_exist %}
     *  "access" %}'">{{ access_requests_title }} {% if
       temporary_access_notification_count %} {
       { temporary_access_notification_count }} {% endif %}
 {% endif %} {% if buddy_system_areas_exist %}
  "buddy" %}'">{{ buddy_requests_title }} {% if buddy_notification_count %} {
 { buddy_notification_count }} {% endif %}
+{% endif %} {% if adjustment_request_allowed and facility_managers_exist %}
+ "adjustment" %}'">{{ adjustment_requests_title }} {% if
+adjustment_notification_count %} {{ adjustment_notification_count }} {% endif
+%}
 {% endif %}
+****** {% if tab == 'access' %}{{ access_requests_title }}{% elif tab ==
+'buddy' %}{{ buddy_requests_title }}{% elif tab == 'adjustment' %}{
+{ adjustment_requests_title }}{% else %}Requests{% endif %} ******
 {% if access_user_request_allowed_exist and facility_managers_exist %}
 {# This will be loaded asynchronously #}
 {% endif %} {% if buddy_system_areas_exist %}
 {# This will be loaded asynchronously #}
+{% endif %} {% if adjustment_request_allowed and facility_managers_exist %}
+{# This will be loaded asynchronously #}
 {% endif %}
  {% endblock %}
```

### Comparing `NEMO-4.4.1/NEMO/templates/resources/modify_resource.html` & `NEMO-4.5.0/NEMO/templates/resources/modify_resource.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/resources/resource_details.html` & `NEMO-4.5.0/NEMO/templates/resources/resource_details.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/resources/resources.html` & `NEMO-4.5.0/NEMO/templates/resources/resources.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 {% extends 'base.html' %}
+{% load custom_tags_and_filters %}
 {% block title %}Resources{% endblock %}
 {% block content %}
 	<h1>Resources</h1>
 	<p>
 		Below is a list of resources, grouped by category.
 		<br>Resources in <span class="success-highlight">green</span> are currently
 		available while resources in <span class="danger-highlight">red</span> are unavailable. Click on a resource to modify its
@@ -19,11 +20,11 @@
 					{% if not resource.available %}
 						- {{ resource.restriction_message }}
 					{% endif %}
 					<br>
 				{% endfor %}
 			</div>
 		{% endfor %}
-	{% else %}
+	{% elif user.is_superuser and "django.contrib.admin"|app_installed %}
 		<h3>No resources exist yet. You can <a href="{% url 'admin:NEMO_resource_changelist' %}">create some in the Resources section of 'Detailed Administration'</a>.</h3>
 	{% endif %}
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,20 +1,21 @@
-{% extends 'base.html' %} {% block title %}Resources{% endblock %} {% block
-content %}
+{% extends 'base.html' %} {% load custom_tags_and_filters %} {% block title
+%}Resources{% endblock %} {% block content %}
 ****** Resources ******
 Below is a list of resources, grouped by category.
 Resources in green are currently available while resources in red are
 unavailable. Click on a resource to modify its availability, status message or
 to schedule an outage.
 When a resource is unavailable, users are blocked from using tools or login to
 areas that fully depend on that resource.
 {% if resources %} {% regroup resources by category as category_list %} {% for
 category in category_list %} {% if category.grouper %}
 **** {{ category.grouper }} ****
 {% endif %}
 {% for resource in category.list %} {{_resource_}} {% if not resource.available
 %} - {{ resource.restriction_message }} {% endif %}
 {% endfor %}
-{% endfor %} {% else %}
+{% endfor %} {% elif user.is_superuser and "django.contrib.admin"|app_installed
+%}
 **** No resources exist yet. You can create_some_in_the_Resources_section_of
 'Detailed_Administration'. ****
 {% endif %} {% endblock %}
```

### Comparing `NEMO-4.4.1/NEMO/templates/resources/scheduled_outage.html` & `NEMO-4.5.0/NEMO/templates/resources/scheduled_outage.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/safety/safety.html` & `NEMO-4.5.0/NEMO/templates/safety/safety.html`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 {% extends 'safety/safety_base.html' %}
+{% load custom_tags_and_filters %}
 {% block title %}Safety{% endblock %}
 {% block safety_title %}Safety{% endblock %}
 {% block tab_content %}
     {% if safety_categories or safety_items %}
         <div class="row" style="margin-bottom: 25px">
             <div class="col-sm-6">
                 <input id="search" type="text" aria-label="Search" placeholder="Search" class="form-control">
@@ -38,15 +39,15 @@
                         {% include 'safety/safety_items.html' with safety_items=safety_category.safetyitem_set.all %}
                     {% endfor %}
                 </div>
             {% endif %}
         </div>
     {% else %}
         <p>There are currently no safety items.</p>
-        {% if user.is_superuser %}
+        {% if user.is_superuser and "django.contrib.admin"|app_installed %}
             <p>Please go to <a href="{% url 'admin:NEMO_safetyitem_changelist' %}">Administration -> Detailed Administration -> SafetyItems</a>
             </p>
         {% endif %}
     {% endif %}
     <script>
         function get_safety_item(jquery_event, search_selection, dataset_name)
 		{
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-{% extends 'safety/safety_base.html' %} {% block title %}Safety{% endblock %}
-{% block safety_title %}Safety{% endblock %} {% block tab_content %} {% if
-safety_categories or safety_items %}
+{% extends 'safety/safety_base.html' %} {% load custom_tags_and_filters %} {%
+block title %}Safety{% endblock %} {% block safety_title %}Safety{% endblock %}
+{% block tab_content %} {% if safety_categories or safety_items %}
 [                    ]
 {% if not safety_items_expand_categories %} {% if safety_categories %}
     * {% if safety_general %}
     * General
     * {% endif %} {% for safety_category in safety_categories %}
     * {{_safety_category.name_}}
     * {% endfor %}
@@ -14,11 +14,11 @@
 {% if safety_general %} {% include 'safety/safety_items.html' with
 safety_items=safety_general safety_category="General" %} {% endif %} {% for
 safety_category in safety_categories %} {% include 'safety/safety_items.html'
 with safety_items=safety_category.safetyitem_set.all %} {% endfor %}
 {% endif %}
 {% else %}
 There are currently no safety items.
-{% if user.is_superuser %}
+{% if user.is_superuser and "django.contrib.admin"|app_installed %}
 Please go to Administration_->_Detailed_Administration_->_SafetyItems
 {% endif %} {% endif %}
  {% endblock %}
```

### Comparing `NEMO-4.4.1/NEMO/templates/safety/safety_base.html` & `NEMO-4.5.0/NEMO/templates/safety/safety_base.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 {% extends 'base.html' %}
 {% load custom_tags_and_filters %}
 {% block content %}
     <div id="safety_tabs" class="clearfix" style="margin-top: 0;margin-bottom: 15px">
-        <span class="h1" style="margin-top: 0;margin-right: 15px">{% block safety_title %}Safety{% endblock %}</span>
+        <h1 class="pull-left" style="margin-top: 0;margin-right: 20px">{% block safety_title %}Safety{% endblock %}</h1>
         {% if show_tabs > 1 %}
             <ul class="nav nav-pills nav-pills-spacer" id="tabs" style="display: inline-block;float: right;">
                 {% if show_safety %}
                     <li class="{% if tab == 'safety' %}active{% endif %}">
                         <a href="#safety" onclick="location.href = '{% url "safety" %}'">Safety</a>
                     </li>
                 {% endif %}
```

#### html2text {}

```diff
@@ -1,10 +1,11 @@
 {% extends 'base.html' %} {% load custom_tags_and_filters %} {% block content
 %}
-{% block safety_title %}Safety{% endblock %} {% if show_tabs > 1 %}
+****** {% block safety_title %}Safety{% endblock %} ******
+{% if show_tabs > 1 %}
     * {% if show_safety %}
     *  %}'">Safety
 {% endif %} {% if show_safety_issues %}
  %}'">Safety issues {% if safety_notification_count %} {
 { safety_notification_count }} {% endif %}
 {% endif %} {% if show_safety_data_sheets %}
  %}'">Safety data sheets
```

### Comparing `NEMO-4.4.1/NEMO/templates/safety/safety_data_sheets.html` & `NEMO-4.5.0/NEMO/templates/safety/safety_data_sheets.html`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
                     {% endfor %}
                 </tbody>
             </table>
         </div>
     {% else %}
         <div>
             There are no chemicals to display.
-            {% if user.is_superuser %}
+            {% if user.is_superuser and "django.contrib.admin"|app_installed %}
                 <br/><br/>You can add some by navigating to<br>
                 <a href="{% url 'admin:NEMO_chemical_changelist' %}">
                     Administration -> Detailed Administration -> Chemicals
                 </a>
             {% endif %}
         </div>
     {% endif %}
```

### Comparing `NEMO-4.4.1/NEMO/templates/safety/safety_issues.html` & `NEMO-4.5.0/NEMO/templates/safety/safety_issues.html`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 							{% endif %}
 							Concern
 						</h4>
 						{{ ticket.concern|linebreaksbr }}
 					</div>
 					<div class="form-group">
 						{% if not ticket.visible %}<span class="glyphicon glyphicon-eye-close"></span> This issue is hidden from users<br>{% endif %}
-						Location: {{ ticket.location }}<br>
+						{% if ticket.location %}Location: {{ ticket.location }}<br>{% endif %}
 						{% if ticket.reporter %}
 							Reported on {{ ticket.creation_time }}{% if user.is_staff %} by {{ ticket.reporter }}{% endif %}<br>
 						{% else %}
 							Reported anonymously on {{ ticket.creation_time }}<br>
 						{% endif %}
 					</div>
 					{% if ticket.progress %}
```

#### html2text {}

```diff
@@ -9,17 +9,17 @@
 url="resolved_safety_issues" value="Past safety issues" icon="glyphicon-list"
 %}
 {% if tickets %} {% for ticket in tickets %} {% if user.is_staff %}
 {%_endif_%}
 ***_{%_if_ticket.id_in_notifications_%}_New_{%_endif_%}_Concern_***
 {{_ticket.concern|linebreaksbr_}}
 {%_if_not_ticket.visible_%}_This_issue_is_hidden_from_users
-{%_endif_%}_Location:_{{_ticket.location_}}
-{%_if_ticket.reporter_%}_Reported_on_{{_ticket.creation_time_}}{%_if
-user.is_staff_%}_by_{{_ticket.reporter_}}{%_endif_%}
+{%_endif_%}_{%_if_ticket.location_%}Location:_{{_ticket.location_}}
+{%_endif_%}_{%_if_ticket.reporter_%}_Reported_on_{{_ticket.creation_time_}}{%
+if_user.is_staff_%}_by_{{_ticket.reporter_}}{%_endif_%}
 {%_else_%}_Reported_anonymously_on_{{_ticket.creation_time_}}
 {%_endif_%}
 {%_if_ticket.progress_%}
 ***_Progress_***
 {{_ticket.progress|linebreaksbr_}}
 {%_endif_%}
 {%_if_user.is_staff_%}
```

### Comparing `NEMO-4.4.1/NEMO/templates/safety/safety_issues_create.html` & `NEMO-4.5.0/NEMO/templates/safety/safety_issues_create.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/safety/safety_issues_resolved.html` & `NEMO-4.5.0/NEMO/templates/safety/safety_issues_resolved.html`

 * *Files 10% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 			<div class="panel-body">
 				<div class="form-group">
 					<h4>Concern</h4>
 					{{ ticket.concern|linebreaksbr }}
 				</div>
 				<div class="form-group">
 					{% if not ticket.visible %}<span class="glyphicon glyphicon-eye-close"></span> This issue is hidden from users<br>{% endif %}
-					Location: {{ ticket.location }}<br>
+					{% if ticket.location %}Location: {{ ticket.location }}<br>{% endif %}
 					{% if ticket.reporter %}
 						Reported on {{ ticket.creation_time }}{% if user.is_staff %} by {{ ticket.reporter }}{% endif %}<br>
 					{% else %}
 						Reported anonymously on {{ ticket.creation_time }}<br>
 					{% endif %}
 					Resolved on {{ ticket.resolution_time }} by {{ ticket.resolver }}
 				</div>
```

### Comparing `NEMO-4.4.1/NEMO/templates/safety/safety_issues_update.html` & `NEMO-4.5.0/NEMO/templates/safety/safety_issues_update.html`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 	<div class="form-group" style="margin-top:50px">
 		<h4>Concern</h4>
 		{{ ticket.concern|linebreaksbr }}
 	</div>
 	<div class="form-group">
 		{% if not ticket.visible %}<span class="glyphicon glyphicon-eye-close"></span> This issue is hidden from users<br>{% endif %}
-		Location: {{ ticket.location }}<br>
+		{% if ticket.location %}Location: {{ ticket.location }}<br>{% endif %}
 		{% if ticket.reporter %}
 			Reported on {{ ticket.creation_time }}{% if user.is_staff %} by {{ ticket.reporter }}{% endif %}<br>
 		{% else %}
 			Reported anonymously on {{ ticket.creation_time }}<br>
 		{% endif %}
 	</div>
 	{% if ticket.progress %}
```

### Comparing `NEMO-4.4.1/NEMO/templates/safety/safety_items.html` & `NEMO-4.5.0/NEMO/templates/safety/safety_items.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/snippets/button.html` & `NEMO-4.5.0/NEMO/templates/snippets/button.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/snippets/contact_person.html` & `NEMO-4.5.0/NEMO/templates/snippets/contact_person.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/snippets/embedded_document.html` & `NEMO-4.5.0/NEMO/templates/snippets/embedded_document.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/snippets/tool_info.html` & `NEMO-4.5.0/NEMO/templates/snippets/tool_info.html`

 * *Files 8% similar despite different names*

```diff
@@ -23,9 +23,9 @@
         <li><a href="{% url 'get_email_form_for_user' superuser.id %}">{{ superuser.get_name }}</a></li>
     {% endfor %}
     </ul>
 {% endif %}
 {% if tool.notification_email_address %}
     Email: <a href="{% url 'get_email_form' %}?recipient={{ tool.notification_email_address }}" title="Email {{ tool.notification_email_address }}">{{ tool.notification_email_address }}</a><br/>
 {% endif %}
-Location: {{ tool.location }}<br/>
-Phone number: <a href="tel:{{ tool.phone_number }}">{{ tool.phone_number }}</a>
+{% if tool.location %}Location: {{ tool.location }}<br/>{% endif %}
+{% if tool.phone_number %}Phone number: <a href="tel:{{ tool.phone_number }}">{{ tool.phone_number }}</a>{% endif %}
```

#### html2text {}

```diff
@@ -10,9 +10,10 @@
 tool.superusers.all|first as superuser %} Superuser: {{_superuser.get_name_}}
 {% endwith %} {% elif tool.superusers.all.count > 1 %} Superusers:
     * {% for superuser in tool.superusers.all %}
     * {{_superuser.get_name_}}
     * {% endfor %}
 {% endif %} {% if tool.notification_email_address %} Email: {
 {_tool.notification_email_address_}}
-{% endif %} Location: {{ tool.location }}
-Phone number: {{_tool.phone_number_}}
+{% endif %} {% if tool.location %}Location: {{ tool.location }}
+{% endif %} {% if tool.phone_number %}Phone number: {{_tool.phone_number_}}{%
+endif %}
```

### Comparing `NEMO-4.4.1/NEMO/templates/staff_charges/change_status.html` & `NEMO-4.5.0/NEMO/templates/staff_charges/change_status.html`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 {% extends 'staff_charges/staff_charges_base.html' %}
 {% load custom_tags_and_filters %}
 {% load mptt_tags %}
+{% block remote_work_title %}Current staff charge{% endblock %}
 {% block staff_charges_content %}
 	<form action="{% url 'end_staff_charge' %}" class="form-horizontal" method="post">
 		{% csrf_token %}
 		<input type="submit" class="btn btn-primary" value="I have finished working on this project">
 	</form>
 	{% if areas %}
 		<div style="height:30px"></div>
```

### Comparing `NEMO-4.4.1/NEMO/templates/staff_charges/choose_project.html` & `NEMO-4.5.0/NEMO/templates/staff_charges/choose_project.html`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 {% extends 'staff_charges/staff_charges_base.html' %}
 {% load custom_tags_and_filters %}
+{% block remote_work_title %}Project selection{% endblock %}
 {% block staff_charges_content %}
 	<div class="col-sm-12">
 		<form action="{% url 'begin_staff_charge' %}" class="form-horizontal" method="post">
 			{% csrf_token %}
 			<div class="form-group">
 				Customer: {{ customer }}<br>
 				<input type="hidden" name="customer" value="{{ customer.id }}">
```

### Comparing `NEMO-4.4.1/NEMO/templates/staff_charges/new_staff_charge.html` & `NEMO-4.5.0/NEMO/templates/staff_charges/new_staff_charge.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 {% extends 'staff_charges/staff_charges_base.html' %}
 {% load custom_tags_and_filters %}
+{% block remote_work_title %}New staff charge{% endblock %}
 {% block staff_charges_content %}
 	<p>Use this form to charge a user for staff time and area access time when you are working on a project on their behalf. You may only work on one user project at a time for a customer.</p>
 	{% if error %}
 		<div class="alert alert-danger">
 			{{ error }}
 		</div>
 	{% endif %}
 	<form id="new_staff_charge" action="{% url 'staff_charges' %}" class="form-horizontal" method="get">
 		<div class="form-group">
-			<label for="customer_search" class="control-label col-sm-1">Customer</label>
+			<label for="customer_search" class="control-label col-sm-1" style="margin-right: 5px">Customer</label>
 			<div class="col-sm-4">
 				<input id="customer_search" type="text" class="form-control" placeholder="Search for a customer">
 				<input id="customer" name="customer" type="hidden">
 			</div>
 		</div>
 	</form>
 	<script>
```

#### html2text {}

```diff
@@ -1,9 +1,10 @@
 {% extends 'staff_charges/staff_charges_base.html' %} {% load
-custom_tags_and_filters %} {% block staff_charges_content %}
+custom_tags_and_filters %} {% block remote_work_title %}New staff charge{%
+endblock %} {% block staff_charges_content %}
 Use this form to charge a user for staff time and area access time when you are
 working on a project on their behalf. You may only work on one user project at
 a time for a customer.
 {% if error %}
 {{ error }}
 {% endif %}
 Customer
```

### Comparing `NEMO-4.4.1/NEMO/templates/staff_charges/reminder.html` & `NEMO-4.5.0/NEMO/templates/staff_charges/reminder.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/staff_charges/staff_charges_base.html` & `NEMO-4.5.0/NEMO/templates/staff_charges/staff_charges_base.html`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-{% extends 'base.html' %}
+{% extends 'remote_work/remote_work_base.html' %}
 {% load custom_tags_and_filters %}
-{% block title %}Staff charges{% endblock %}
-{% block content %}
-	<h1>Staff charges</h1>
+{% block title %}Staff charge{% endblock %}
+{% block staff_charges_tab_class %}active{% endblock %}
+{% block tab_content %}
 	{% if staff_charge %}
 		<p>You are charging staff time to {{ staff_charge.customer }} for the project named {{ staff_charge.project }} since {{ staff_charge.start }}.</p>
         <div style="display: table-row">
             <label for="staff_charge_note" style="vertical-align: top;display: table-cell">Charge note: </label>
             <div style="display: table-cell; padding: 0 10px; width: 75%">
                 <textarea oninput="auto_size_textarea(this)" class="form-control" id="staff_charge_note">{{ staff_charge.note|default_if_none:"" }}</textarea>
             </div>
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-{% extends 'base.html' %} {% load custom_tags_and_filters %} {% block title
-%}Staff charges{% endblock %} {% block content %}
-****** Staff charges ******
-{% if staff_charge %}
+{% extends 'remote_work/remote_work_base.html' %} {% load
+custom_tags_and_filters %} {% block title %}Staff charge{% endblock %} {% block
+staff_charges_tab_class %}active{% endblock %} {% block tab_content %} {% if
+staff_charge %}
 You are charging staff time to {{ staff_charge.customer }} for the project
 named {{ staff_charge.project }} since {{ staff_charge.start }}.
 Charge note:
 {{ staff_charge.note|default_if_none:"" }}
 {% url "edit_staff_charge_note" as edit_staff_charge_note_url %} {% button
 type="save" size="small" submit=False value=staff_charge.note|yesno:
 "Update,Save" onclick="ajax_post('"|concat:edit_staff_charge_note_url|concat:
```

### Comparing `NEMO-4.4.1/NEMO/templates/status_dashboard/occupancy.html` & `NEMO-4.5.0/NEMO/templates/status_dashboard/occupancy.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/status_dashboard/staff.html` & `NEMO-4.5.0/NEMO/templates/status_dashboard/staff.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/status_dashboard/staff_absence.html` & `NEMO-4.5.0/NEMO/templates/status_dashboard/staff_absence.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/status_dashboard/status_dashboard.html` & `NEMO-4.5.0/NEMO/templates/status_dashboard/status_dashboard.html`

 * *Files 2% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 <ul class="nav nav-pills" id="tabs" {% if no_header %}style="display:none"{% endif %}>
     {% if areas_exist %}<li {% if tab == 'occupancy' %}class="active"{% endif %}><a href="#occupancy">Area occupancy</a></li>{% endif %}
     {% if tools_exist %}<li {% if tab == 'tools' %}class="active"{% endif %}><a href="#tools">Tool status & usage</a></li>{% endif %}
     {% if show_staff_status %}<li {% if tab == 'staff' %}class="active"{% endif %}><a href="#staff">Staff status</a></li>{% endif %}
 </ul>
 
 <div id="content" class="tab-content" style="padding-top:10px">
-	<div class="tab-pane {% if areas_exist and tab == 'occupancy' %}active{% endif %}" id="occupancy">
+	<div class="tab-pane{% if areas_exist and tab == 'occupancy' %} active{% endif %}" id="occupancy">
 		{% include 'status_dashboard/occupancy.html' %}
 	</div>
-	<div class="tab-pane {% if tools_exist and tab == 'tools' %}active{% endif %} info-tooltip-container" id="tools">
+	<div class="tab-pane{% if tools_exist and tab == 'tools' %} active{% endif %} info-tooltip-container" id="tools">
 		<div class="btn-group sidebar-item">
 			<button id="filter" type="button" class="btn btn-default dropdown-toggle" data-toggle="dropdown" {% if no_header %}style="display:none;"{% endif %}>
 				Showing tools in use
 				<span class="caret"></span>
 			</button>
 			<ul class="dropdown-menu">
 				<li class="dropdown-header">Filter by...</li>
@@ -35,15 +35,15 @@
 		</div>
 		<p>
 		<div id="tool_status_table">
 			{% include 'status_dashboard/tools.html' %}
 		</div>
 	</div>
     {% if show_staff_status %}
-        <div class="tab-pane {% if tab == 'staff' %}active{% endif %}" id="staff">
+        <div class="tab-pane{% if tab == 'staff' %} active{% endif %}" id="staff">
             {% include 'status_dashboard/staff.html' %}
         </div>
     {% endif %}
 </div>
 
 <script>
 	function on_load()
```

### Comparing `NEMO-4.4.1/NEMO/templates/status_dashboard/tools.html` & `NEMO-4.5.0/NEMO/templates/status_dashboard/tools.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/tasks/resolve.html` & `NEMO-4.5.0/NEMO/templates/tasks/resolve.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/tasks/update.html` & `NEMO-4.5.0/NEMO/templates/tasks/update.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/tool_control/get_projects.html` & `NEMO-4.5.0/NEMO/templates/tool_control/get_projects.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/tool_control/interlock_error.html` & `NEMO-4.5.0/NEMO/templates/tool_control/interlock_error.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/tool_control/past_tasks_and_comments.html` & `NEMO-4.5.0/NEMO/templates/tool_control/past_tasks_and_comments.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/tool_control/qualified_users.html` & `NEMO-4.5.0/NEMO/templates/tool_control/qualified_users.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/tool_control/tool_control.html` & `NEMO-4.5.0/NEMO/templates/tool_control/tool_control.html`

 * *Files 2% similar despite different names*

```diff
@@ -178,31 +178,32 @@
 			let url = "{% url 'enable_tool' tool_id=111 user_id=22222222 project_id=33333333 staff_charge='false' %}".replace('111', tool_id).replace('22222222', user_id.toString()).replace('33333333', project_id.toString()).replace('false', staff_charge.toString())
 			let success_callbacks;
 			if(staff_charge === true)
 				success_callbacks = [reload_page]; {# If there's a new staff charge then we need to reload the whole page so it's displayed in the menu bar. #}
 			else
 				success_callbacks = [refresh_tool_status, ajax_success_callback];
 			let enable_start_button = function() { $("#start button").prop("disabled", false); };
-			try_post_catch_interlock_error(url, undefined, success_callbacks, enable_start_button);
+			try_post_catch_interlock_error(url, {"remote_work": $("#remote_work").val()}, success_callbacks, enable_start_button);
 		}
 
 		function disable_tool(url)
 		{
 			$("#stop").prop("disabled", true);
-			let contents = serialize("#tool_control");
+			let contents = $("#tool_control").serialize();
 			let enable_stop_button = function() { $("#stop").prop("disabled", false); };
 			try_post_catch_interlock_error(url, contents, [refresh_tool_status, ajax_success_callback], enable_stop_button);
 		}
 
 		{% if user.is_staff %}
 
 			{# Only staff can perform the functions in this if-block. #}
 
-			function use_tool_for_other()
+			function use_tool_for_other(remote_work)
 			{
+                $("#remote_work").val(remote_work || "");
 				$("#start").hide();
 				$("#project_choice").html("Fetching user list...").show().load("{% url 'use_tool_for_other' %}", undefined, load_projects_completion_callback);
 			}
 
 			function clear_customer()
 			{
 				$("#customer").text("").hide();
```

### Comparing `NEMO-4.4.1/NEMO/templates/tool_control/tool_status.html` & `NEMO-4.5.0/NEMO/templates/tool_control/tool_status.html`

 * *Files 17% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 {% load custom_tags_and_filters %}
 <div>
-	{% if device == 'mobile' %}
-		<h1>{{ tool.name_or_child_in_use_name }}</h1>
-		<ul class="nav nav-pills" id="tabs" style="margin-bottom:10px">
-			<li style="width:48%; text-align:center" class="active"><a href="#summary" style="padding: 10px 5px">Summary</a></li>
-			<li style="width:48%; text-align:center"><a href="#details" style="padding: 10px 5px">Details</a></li>
-			{% if configs %}<li style="width:48%; text-align:center"><a href="#config" style="padding: 10px 5px">Config History</a></li>{% endif %}
-			{% if tool.post_usage_questions %}<li><a href="#usage_data" style="padding: 10px 5px;" onclick="load_usage_data('{{ tool.id }}');">Usage Data History</a></li>{% endif %}
-			<li style="width:48%; text-align:center"><a href="#problem" style="padding: 10px 5px">Report a problem</a></li>
-			<li style="width:48%; text-align:center"><a href="#comment" style="padding: 10px 5px">Post a comment</a></li>
-		</ul>
-	{% else %}
-		<h1 class="pull-left" style="margin-right:20px; margin-top:0; margin-bottom:10px">{{ tool.name_or_child_in_use_name }}</h1>
-		<ul class="nav nav-pills" id="tabs">
-			<li class="active"><a href="#summary">Summary</a></li>
-			<li><a href="#details">Details</a></li>
-			{% if configs %}<li><a href="#config">Config History</a></li>{% endif %}
-			{% if tool.post_usage_questions %}<li><a href="#usage_data" onclick="load_usage_data('{{ tool.id }}');">Usage Data History</a></li>{% endif %}
-			<li><a href="#problem">Report a problem</a></li>
-			<li><a href="#comment">Post a comment</a></li>
-		</ul>
-	{% endif %}
+    {% with hide_data_history="tool"|customization:"tool_control_hide_data_history_users" %}
+        {% if device == 'mobile' %}
+            <h1>{{ tool.name_or_child_in_use_name }}</h1>
+            <ul class="nav nav-pills" id="tabs" style="margin-bottom:10px">
+                <li style="width:48%; text-align:center" class="active"><a href="#summary" style="padding: 10px 5px">Summary</a></li>
+                <li style="width:48%; text-align:center"><a href="#details" style="padding: 10px 5px">Details</a></li>
+                {% if configs %}<li style="width:48%; text-align:center"><a href="#config" style="padding: 10px 5px">Config History</a></li>{% endif %}
+                {% if tool.post_usage_questions and not hide_data_history or user.is_any_part_of_staff %}<li style="width: 48%; text-align: center"><a href="#usage_data" style="padding: 10px 5px;" onclick="load_usage_data('{{ tool.id }}');">Usage Data History</a></li>{% endif %}
+                <li style="width:48%; text-align:center"><a href="#problem" style="padding: 10px 5px">Report a problem</a></li>
+                <li style="width:48%; text-align:center"><a href="#comment" style="padding: 10px 5px">Post a comment</a></li>
+            </ul>
+        {% else %}
+            <h1 class="pull-left" style="margin-right:20px; margin-top:0; margin-bottom:10px">{{ tool.name_or_child_in_use_name }}</h1>
+            <ul class="nav nav-pills" id="tabs">
+                <li class="active"><a href="#summary">Summary</a></li>
+                <li><a href="#details">Details</a></li>
+                {% if configs %}<li><a href="#config">Config History</a></li>{% endif %}
+                {% if tool.post_usage_questions and not hide_data_history or user.is_any_part_of_staff %}<li><a href="#usage_data" onclick="load_usage_data('{{ tool.id }}');">Usage Data History</a></li>{% endif %}
+                <li><a href="#problem">Report a problem</a></li>
+                <li><a href="#comment">Post a comment</a></li>
+            </ul>
+        {% endif %}
+    {% endwith %}
 </div>
 
 <div class="tab-content">
 	<div class="tab-pane active" id="summary">
 		{% if tool.serial %}
-			<div style="float: right; font-size:x-small">s/n : {{tool.serial| safe }}</div>
+			<div style="float: right; font-size:x-small">s/n : {{ tool.serial| safe }}</div>
 		{% endif %}
 
 		{# Display tool status... #}
 		<div class="tool-status">
 			{% if tool.in_use %}
 				<div class="primary-highlight">
 					<span class="glyphicon glyphicon-user pull-left notification-icon"></span>
@@ -298,31 +300,37 @@
                         {% url 'disable_tool' tool.get_current_usage_event.tool.id as disable_tool_url %}
                         {% button type="delete" id="stop" icon="glyphicon-stop" onclick="disable_tool('"|concat:disable_tool_url|concat:"'); return false;" value="Stop using the "|concat:tool.name_or_child_in_use_name %}
                     </div>
 				{% endif %}
 			{% else %}
 				{% if user.is_staff or user.is_service_personnel and tool in user.qualifications.all %}
 					<h4>What would you like to do?</h4>
+                    <input type="hidden" id="remote_work" name="remote_work" value="">
 					<div class="radio"><label><input type="radio" onchange="use_tool_for_self()" name="staff_charge" value="false">Use this tool for my own project</label></div>
 					{% if user.is_staff %}
-						<div class="radio"><label><input type="radio" onchange="use_tool_for_other()" name="staff_charge" value="false">Use this tool on behalf of another user</label></div>
+						<div class="radio"><label><input type="radio" onchange="use_tool_for_other()" name="staff_charge" value="false">Use this tool on behalf of another user{% if "remote_work"|customization:"remote_work_ask_explicitly" %} (no remote){% endif %}</label></div>
+                        {% if "remote_work"|customization:"remote_work_ask_explicitly" %}
+						    <div class="radio">
+                                <label><input type="radio" onchange="use_tool_for_other(true)" name="staff_charge" value="false">Use this tool for a remote project</label>
+                            </div>
+                        {% endif %}
 						{% if user.charging_staff_time %}
 							{% with user.get_staff_charge as staff_charge %}
 								<div class="radio disabled">
 									<label id="staff_charge_tooltip_container" class="light-grey" data-toggle="tooltip" data-placement="right" title="This option is not available because you are already charging staff time to {{ staff_charge.customer }} for the project named {{ staff_charge.project }} since {{ staff_charge.start }}.">
 										<input type="radio" onchange="use_tool_for_other()" disabled>
-										<span id="staff_charge_tooltip_location">Use this tool for a remote project</span>
+										<span id="staff_charge_tooltip_location">Use this tool for a remote project{% if "remote_work"|customization:"remote_work_ask_explicitly" %} (charge staff time{% if tool.requires_area_access and "remote_work"|customization:"remote_work_start_area_access_automatically" == "enabled" %} & {{ tool.requires_area_access }} time{% endif %}){% endif %}</span>
 									</label>
 								</div>
 								<script>
 									$("#staff_charge_tooltip_container").tooltip();
 								</script>
 							{% endwith %}
 						{% else %}
-							<div class="radio"><label><input type="radio" onchange="use_tool_for_other()" name="staff_charge" value="true">Use this tool for a remote project</label></div>
+							<div class="radio"><label><input type="radio" onchange="use_tool_for_other()" name="staff_charge" value="true">Use this tool for a remote project{% if "remote_work"|customization:"remote_work_ask_explicitly" %} (charge staff time{% if tool.requires_area_access and "remote_work"|customization:"remote_work_start_area_access_automatically" == "enabled" %} & {{ tool.requires_area_access }} time{% endif %}){% endif %}</label></div>
 						{% endif %}
 					{% endif %}
 					<div id="project_choice"></div>
 				{% elif tool.operational and not tool.required_resource_is_unavailable and not tool.delayed_logoff_in_progress and not tool.scheduled_outage_in_progress %}
 					{% include 'tool_control/get_projects.html' with active_projects=user.active_projects user_id=user.id %}
 				{% endif %}
 				{% if user.is_staff or user.is_service_personnel and tool in user.qualifications.all or tool.ready_to_use %}
@@ -421,16 +429,16 @@
 						{% endif %}
 					{% endfor %}
 					</p>
 				{% endif %}
 				{% if tool.notification_email_address %}
 					<p>Problem reports for the {{ tool.name_or_child_in_use_name }} are automatically emailed to <a href="{% url 'get_email_form' %}?recipient={{ tool.notification_email_address }}" title="Email {{ tool.notification_email_address }}"><span class="glyphicon glyphicon-send small-icon"></span>{{ tool.notification_email_address }}</a>.</p>
 				{% endif %}
-				<p>The {{ tool.name_or_child_in_use_name }} is located in room <span class="glyphicon glyphicon-map-marker small-icon"></span>{{ tool.location }}.</p>
-				<p>You may dial the phone that is closest to the {{ tool.name_or_child_in_use_name }} at extension <span class="glyphicon glyphicon-phone small-icon"></span>{{ tool.phone_number }}.</p>
+				{% if tool.location %}<p>The {{ tool.name_or_child_in_use_name }} is located in room <span class="glyphicon glyphicon-map-marker small-icon"></span>{{ tool.location }}.</p>{% endif %}
+				{% if tool.phone_number %}<p>You may dial the phone that is closest to the {{ tool.name_or_child_in_use_name }} at extension <span class="glyphicon glyphicon-phone small-icon"></span>{{ tool.phone_number }}.</p>{% endif %}
 			</div>
 		</div>
 		{% if user.is_staff %}
 			<div id="qualified_users_container" class="media">
 				{% include 'tool_control/qualified_users.html' %}
 			</div>
 		{% endif %}
```

#### html2text {}

```diff
@@ -1,33 +1,36 @@
 {% load custom_tags_and_filters %}
-{% if device == 'mobile' %}
+{% with hide_data_history="tool"|customization:
+"tool_control_hide_data_history_users" %} {% if device == 'mobile' %}
 ****** {{ tool.name_or_child_in_use_name }} ******
     * Summary
     * Details
     * {% if configs %}
     * Config_History
-    * {% endif %} {% if tool.post_usage_questions %}
+    * {% endif %} {% if tool.post_usage_questions and not hide_data_history or
+      user.is_any_part_of_staff %}
     * Usage_Data_History
     * {% endif %}
     * Report_a_problem
     * Post_a_comment
 {% else %}
 ****** {{ tool.name_or_child_in_use_name }} ******
     * Summary
     * Details
     * {% if configs %}
     * Config_History
-    * {% endif %} {% if tool.post_usage_questions %}
+    * {% endif %} {% if tool.post_usage_questions and not hide_data_history or
+      user.is_any_part_of_staff %}
     * Usage_Data_History
     * {% endif %}
     * Report_a_problem
     * Post_a_comment
-{% endif %}
+{% endif %} {% endwith %}
 {% if tool.serial %}
-s/n : {{tool.serial| safe }}
+s/n : {{ tool.serial| safe }}
 {% endif %} {# Display tool status... #}
 {% if tool.in_use %}
  {% with tool.get_current_usage_event as current_usage_event %}
 ***** {% if current_usage_event.operator.id == user.id %} You are using this
 tool {% else %} {{_current_usage_event.operator_}} is using this tool {% endif
 %} {% if current_usage_event.operator.id != current_usage_event.user.id %} on
 behalf of {{ current_usage_event.user }} {% endif %} for the project named {
@@ -143,20 +146,31 @@
 onclick="disable_tool('"|concat:disable_tool_url|concat:"'); return false;"
 value="Stop using the "|concat:tool.name_or_child_in_use_name %}
 {% endif %} {% else %} {% if user.is_staff or user.is_service_personnel and
 tool in user.qualifications.all %}
 *** What would you like to do? ***
 oUse this tool for my own project
 {% if user.is_staff %}
-oUse this tool on behalf of another user
-{% if user.charging_staff_time %} {% with user.get_staff_charge as staff_charge
-%}
- o Use this tool for a remote project
- {% endwith %} {% else %}
+oUse this tool on behalf of another user{% if "remote_work"|customization:
+"remote_work_ask_explicitly" %} (no remote){% endif %}
+{% if "remote_work"|customization:"remote_work_ask_explicitly" %}
 oUse this tool for a remote project
+{% endif %} {% if user.charging_staff_time %} {% with user.get_staff_charge as
+staff_charge %}
+ o Use this tool for a remote project{% if "remote_work"|customization:
+"remote_work_ask_explicitly" %} (charge staff time{% if
+tool.requires_area_access and "remote_work"|customization:
+"remote_work_start_area_access_automatically" == "enabled" %} & {
+{ tool.requires_area_access }} time{% endif %}){% endif %}
+ {% endwith %} {% else %}
+oUse this tool for a remote project{% if "remote_work"|customization:
+"remote_work_ask_explicitly" %} (charge staff time{% if
+tool.requires_area_access and "remote_work"|customization:
+"remote_work_start_area_access_automatically" == "enabled" %} & {
+{ tool.requires_area_access }} time{% endif %}){% endif %}
 {% endif %} {% endif %}
 {% elif tool.operational and not tool.required_resource_is_unavailable and not
 tool.delayed_logoff_in_progress and not tool.scheduled_outage_in_progress %} {%
 include 'tool_control/get_projects.html' with
 active_projects=user.active_projects user_id=user.id %} {% endif %} {% if
 user.is_staff or user.is_service_personnel and tool in user.qualifications.all
 or tool.ready_to_use %}
@@ -211,19 +225,21 @@
 For equipment training, you can contact the primary, backup or one of the
 superusers {% for x in tool.superusers.all %} {% if not forloop.last %} {
 { x.get_contact_info_html|safe }}, {% else %} or {
 { x.get_contact_info_html|safe }}. {% endif %} {% endfor %}
 {% endif %} {% if tool.notification_email_address %}
 Problem reports for the {{ tool.name_or_child_in_use_name }} are automatically
 emailed to {{_tool.notification_email_address_}}.
-{% endif %}
+{% endif %} {% if tool.location %}
 The {{ tool.name_or_child_in_use_name }} is located in room {{ tool.location
 }}.
+{% endif %} {% if tool.phone_number %}
 You may dial the phone that is closest to the {{ tool.name_or_child_in_use_name
 }} at extension {{ tool.phone_number }}.
+{% endif %}
 {% if user.is_staff %}
 {% include 'tool_control/qualified_users.html' %}
 {% endif %} {% if tool.required_resource_set.exists %}
 
 *** Resources that are required for this tool to operate ***
     * {% for u in tool.required_resource_set.all %}
     * {{ u.name }} {% if u.category %}({{ u.category }}){% endif %}
```

### Comparing `NEMO-4.4.1/NEMO/templates/tool_control/usage_data.html` & `NEMO-4.5.0/NEMO/templates/tool_control/usage_data.html`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 				{% endfor %}
 			</tr>
 		</thead>
 		<tbody>
 			{% for row in usage_data_table.flat_rows %}
 				<tr>
 					{% for item in row %}
-						<td>{{ item }}</td>
+						<td>{% if item|class_name == "list" %}{{ item|join:", " }}{% else %}{{ item }}{% endif %}</td>
 					{% endfor %}
 				</tr>
 			{% endfor %}
 		</tbody>
 	</table>
 {% else %}
 	<span class="italic">No usage data was found between these dates</span>
```

### Comparing `NEMO-4.4.1/NEMO/templates/training/get_projects.html` & `NEMO-4.5.0/NEMO/templates/training/get_projects.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/training/training.html` & `NEMO-4.5.0/NEMO/templates/training/training.html`

 * *Files 8% similar despite different names*

```diff
@@ -47,29 +47,31 @@
 		}
 
 		function enable_autocompletion(entry_number)
 		{
 			let id = "#user_textbox__" + entry_number;
 			$(id).autocomplete('user', on_autocomplete_selection, {{ users|json_search_base }}).prop('required', true).focus();
 			id = "#tool_textbox__" + entry_number;
-			$(id).autocomplete('tool', on_autocomplete_selection, {{ tools|json_search_base }}).prop('required', true);
+			$(id).autocomplete('tool', on_autocomplete_selection, {% json_search_base_with_extra_fields tools|add:tool_groups %}, {% if tool_groups %}false{% else %}true{% endif %}).prop('required', true);
 		}
 
 		function remove_row(number)
 		{
 			$("#row_" + number).remove();
 		}
 
 		function on_autocomplete_selection(jquery_event, search_selection, dataset_name)
 		{
 			$(this).typeahead('val', search_selection.id).hide();
 			let row = $(this).data('row');
 			let button_id = "#" + dataset_name + "_button__" + row;
 			let textbox_id = "#" + dataset_name + "_textbox__" + row;
+			let textbox_type_id = "#" + dataset_name + "_textbox_type__" + row;
 			$(textbox_id).prop('required', false);
+			$(textbox_type_id).val(search_selection.type);
 			$(button_id).val(search_selection.name).show();
 
 			if(dataset_name === "user")
 				fetch_projects(row, search_selection.id);
 
 			advance_focus(dataset_name, row);
 		}
@@ -116,14 +118,15 @@
 			$("#user_textbox__" + row).typeahead('val', '').prop('required', true).show().focus();
 		}
 
 		function purge_tool(row)
 		{
 			$("#tool_button__" + row).hide();
 			$("#tool_textbox__" + row).typeahead('val', '').prop('required', true).show().focus();
+			$("#tool_textbox_type__" + row).typeahead('val', '');
 		}
 
 		function on_submit()
 		{
 			let failure_dialog = ajax_failure_callback("Could not record training sessions");
 			ajax_post("{% url 'charge_training' %}", serialize("#training_session_form"), ajax_success_callback, failure_dialog);
 			return false;
```

### Comparing `NEMO-4.4.1/NEMO/templates/training/training_entry.html` & `NEMO-4.5.0/NEMO/templates/training/training_entry.html`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 	<td style="vertical-align: middle"><span class="glyphicon glyphicon-remove-circle grey pointer" onclick="remove_row({{ entry_number }})"></span></td>
 	<td>
 		<input type="text" class="form-control" id="user_textbox__{{ entry_number }}" name="chosen_user__{{ entry_number }}" data-row="{{ entry_number }}">
 		<input type="button" class="btn btn-default" style="display:none" id="user_button__{{ entry_number }}" onclick="purge_trainee({{ entry_number }})">
 	</td>
 	<td>
 		<input type="text" class="form-control" id="tool_textbox__{{ entry_number }}" name="chosen_tool__{{ entry_number }}" data-row="{{ entry_number }}">
+		<input type="hidden" id="tool_textbox_type__{{ entry_number }}" name="chosen_type__{{ entry_number }}" data-row="{{ entry_number }}">
 		<input type="button" class="btn btn-default" style="display:none" id="tool_button__{{ entry_number }}" onclick="purge_tool({{ entry_number }})">
 	</td>
 	<td id="project__{{ entry_number }}" style="vertical-align: middle">
 
 	</td>
 	<td><input type="number" class="form-control" name="duration__{{ entry_number }}" id="duration__{{ entry_number }}" min="1" inputmode="numeric" pattern="[0-9]*" required></td>
 	<td>
```

### Comparing `NEMO-4.4.1/NEMO/templates/usage/billing.html` & `NEMO-4.5.0/NEMO/templates/usage/billing.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/usage/usage_base.html` & `NEMO-4.5.0/NEMO/templates/usage/usage_base.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/users/create_or_modify_user.html` & `NEMO-4.5.0/NEMO/templates/users/create_or_modify_user.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/users/preferences.html` & `NEMO-4.5.0/NEMO/templates/users/preferences.html`

 * *Files 3% similar despite different names*

```diff
@@ -22,18 +22,25 @@
 				<div class="panel-body">
 					<h3>Buddy System</h3>
 					<div class="form-group col-sm-12">
 						<div class="checkbox">
 							<label><input name="display_new_buddy_request_notification" type="checkbox" {% if user_preferences.display_new_buddy_request_notification %}checked{% endif %}>Check this box to see notification badges for new buddy requests</label>
 						</div>
 						<div class="checkbox">
-							<label><input name="display_new_buddy_request_reply_notification" type="checkbox" {% if user_preferences.display_new_buddy_request_reply_notification %}checked{% endif %}>Check this box to see notification badges when users reply to buddy requests you replied to</label>
+							<label><input name="email_new_buddy_request_reply" type="checkbox" {% if user_preferences.email_new_buddy_request_reply %}checked{% endif %}>Check this box to receive an email notification when users reply to buddy requests you replied to</label>
 						</div>
+					</div>
+				</div>
+			</div>
+            <div class="panel panel-default">
+				<div class="panel-body">
+					<h3>Adjustment Requests</h3>
+					<div class="form-group col-sm-12">
 						<div class="checkbox">
-							<label><input name="email_new_buddy_request_reply" type="checkbox" {% if user_preferences.email_new_buddy_request_reply %}checked{% endif %}>Check this box to receive an email notification when users reply to buddy requests you replied to</label>
+							<label><input name="email_new_adjustment_request_reply" type="checkbox" {% if user_preferences.email_new_adjustment_request_reply %}checked{% endif %}>Check this box to receive an email notification for replies to your adjustment requests</label>
 						</div>
 					</div>
 				</div>
 			</div>
             {% if not form.fields.staff_status_view.disabled %}
                 <div class="panel panel-default">
                     <div class="panel-body">
```

### Comparing `NEMO-4.4.1/NEMO/templates/users/safe_deactivation.html` & `NEMO-4.5.0/NEMO/templates/users/safe_deactivation.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templates/users/users.html` & `NEMO-4.5.0/NEMO/templates/users/users.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/templatetags/custom_tags_and_filters.py` & `NEMO-4.5.0/NEMO/templatetags/custom_tags_and_filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 import datetime
 from datetime import timedelta
 from importlib.metadata import PackageNotFoundError, version
 
 from django import template
+from django.contrib.contenttypes.models import ContentType
 from django.shortcuts import resolve_url
 from django.template import Context, Template
 from django.template.defaultfilters import date, time
 from django.urls import NoReverseMatch, reverse
 from django.utils import timezone
 from django.utils.formats import localize_input
 from django.utils.html import escape, escapejs, format_html
 from django.utils.safestring import mark_safe
 
+from NEMO.mixins import BillableItemMixin
+from NEMO.models import User
 from NEMO.views.customization import CustomizationBase, ProjectsAccountsCustomization
 
 register = template.Library()
 
 
 @register.filter
 def class_name(value):
 	return value.__class__.__name__
 
 
 @register.filter
 def is_soon(time):
-	""" 'Soon' is defined as within 10 minutes from now. """
+	"""'Soon' is defined as within 10 minutes from now."""
 	return time <= timezone.now() + timedelta(minutes=10)
 
 
 @register.filter
 def to_int(value):
 	return int(value)
 
@@ -75,15 +78,15 @@
 	for item in items_to_search:
 		object_type = item.__class__.__name__.lower()
 		attr = getattr(item, display, None)
 		item_display = attr() if callable(attr) else attr
 		# we need to escape the name and the extra fields in case they contain new lines etc. otherwise it breaks.
 		result += '{{"name":"{0}", "id":"{1}", "type":"{2}"'.format(escapejs(item_display), item.id, object_type)
 		# remove name just in case it's also given as extra fields (it would clash with search result name)
-		for x in [field for field in extra_fields if field != 'name']:
+		for x in [field for field in extra_fields if field != "name"]:
 			if hasattr(item, x):
 				result += ', "{0}":"{1}"'.format(x, escapejs(getattr(item, x)))
 		result += "},"
 	result = result.rstrip(",") + "]"
 	return mark_safe(result)
 
 
@@ -102,15 +105,17 @@
 	input_dict = dictionary[list(dictionary.keys())[0]]
 	headers = list(input_dict.keys())
 	header_cells = "".join([format_html("<th>{}</th>", h) for h in headers])
 	head_html = format_html("<thead><tr><th>#</th>{}</tr></thead>", mark_safe(header_cells))
 
 	rows = []
 	for i, (index, d) in enumerate(dictionary.items()):
-		data_cells_html = "".join([format_html("<td>{}</td>", ", ".join(d[h]) if isinstance(d[h], list) else d[h]) for h in headers])
+		data_cells_html = "".join(
+			[format_html("<td>{}</td>", ", ".join(d[h]) if isinstance(d[h], list) else d[h]) for h in headers]
+		)
 		row_html = format_html("<tr><th>{}</th>{}</tr>", i + 1, mark_safe(data_cells_html))
 		rows.append(row_html)
 	body_html = format_html("<tbody>{}</tbody>", mark_safe("".join(rows)))
 	return head_html + body_html
 
 
 @register.filter
@@ -160,14 +165,25 @@
 @register.filter
 def app_installed(app_name):
 	from django.apps import apps
 
 	return apps.is_installed(app_name)
 
 
+@register.filter
+def content_type(obj):
+	if obj:
+		return ContentType.objects.get_for_model(obj)
+
+
+@register.filter
+def billable_display(item: BillableItemMixin, user: User):
+	return item.get_display(user) if item else ""
+
+
 @register.inclusion_tag("snippets/button.html")
 def button(value, type="default", size="", icon=None, onclick=None, dismiss="", submit=None, title=None, url="", **kwargs):
 	"""
 	This tag is useful to provide a consistent button experience throughout the application.
 	Button types are "view", "save", "add", "edit", "delete", "export", "warn", "default".
 	Button sizes are "xsmall", "small", "medium", "large".
 	"""
```

### Comparing `NEMO-4.4.1/NEMO/urls.py` & `NEMO-4.5.0/NEMO/urls.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,16 +14,18 @@
 from rest_framework import routers
 
 from NEMO.models import ReservationItemType
 from NEMO.views import (
 	abuse,
 	access_requests,
 	accounts_and_projects,
+	adjustment_requests,
 	alerts,
 	api,
+	api_file_import,
 	area_access,
 	authentication,
 	buddy_requests,
 	calendar,
 	configuration_agenda,
 	consumables,
 	contact_staff,
@@ -40,38 +42,42 @@
 	mobile,
 	news,
 	qualifications,
 	remote_work,
 	resources,
 	safety,
 	sidebar,
-	staff_charges,
 	status_dashboard,
 	tasks,
 	tool_control,
 	training,
 	tutorials,
 	usage,
 	user_requests,
 	users,
 )
 
 logger = logging.getLogger(__name__)
 
-if apps.is_installed("django.contrib.admin"):
-	# Use our custom login page instead of Django's built-in one.
-	admin.site.login = login_required(admin.site.login)
-
 # REST API URLs
 router = routers.DefaultRouter()
+router.register(r"auth_groups", api.GroupViewSet)
+router.register(r"auth_permissions", api.PermissionViewSet)
+router.register(r"account_types", api.AccountTypeViewSet)
 router.register(r"accounts", api.AccountViewSet)
 router.register(r"area_access_records", api.AreaAccessRecordViewSet)
 router.register(r"areas", api.AreaViewSet)
 router.register(r"billing", api.BillingViewSet, basename="billing")
+router.register(r"consumable_categories", api.ConsumableCategoryViewSet)
+router.register(r"consumable_withdrawals", api.ConsumableWithdrawViewSet)
+router.register(r"consumables", api.ConsumableViewSet)
+router.register(r"content_types", api.ContentTypeViewSet)
+router.register(r"project_disciplines", api.ProjectDisciplineViewSet)
 router.register(r"projects", api.ProjectViewSet)
+router.register(r"qualifications", api.QualificationViewSet)
 router.register(r"reservations", api.ReservationViewSet)
 router.register(r"resources", api.ResourceViewSet)
 router.register(r"scheduled_outages", api.ScheduledOutageViewSet)
 router.register(r"staff_charges", api.StaffChargeViewSet)
 router.register(r"tasks", api.TaskViewSet)
 router.register(r"tools", api.ToolViewSet)
 router.register(r"training_sessions", api.TrainingSessionViewSet)
@@ -90,15 +96,15 @@
 	if app_name != "NEMO" and app_name.startswith("NEMO"):
 		try:
 			mod = import_module("%s.urls" % app_name)
 		except ModuleNotFoundError:
 			logger.warning(f"no urls found for NEMO plugin: {app_name}")
 			pass
 		except Exception as e:
-			logger.warning(f"could not import urls for NEMO plugin: {app_name} {str(e)}")
+			logger.exception(f"could not import urls for NEMO plugin: {app_name}")
 			pass
 		else:
 			urlpatterns += [path("", include("%s.urls" % app_name))]
 			logger.debug(f"automatically including urls for plugin: {app_name}")
 
 # The order matters for some tests to run properly
 urlpatterns += [
@@ -134,29 +140,40 @@
 	path("past_comments_and_tasks/", tool_control.past_comments_and_tasks, name="past_comments_and_tasks"),
 	path("ten_most_recent_past_comments_and_tasks/<int:tool_id>/", tool_control.ten_most_recent_past_comments_and_tasks, name="ten_most_recent_past_comments_and_tasks"),
 	path("tool_usage_group_question/<int:tool_id>/<str:group_name>/", tool_control.tool_usage_group_question, name="tool_usage_group_question"),
 	path("reset_tool_counter/<int:counter_id>/", tool_control.reset_tool_counter, name="reset_tool_counter"),
 
 	# User requests
 	path("user_requests/", user_requests.user_requests, name="user_requests"),
-	re_path(r"^user_requests/(?P<tab>buddy|access)/$", user_requests.user_requests, name="user_requests"),
+	re_path(r"^user_requests/(?P<tab>buddy|access|adjustment)/$", user_requests.user_requests, name="user_requests"),
 
 	# Access requests
 	path("access_requests/", access_requests.access_requests, name="access_requests"),
 	path("create_access_request/", access_requests.create_access_request, name="create_access_request"),
 	path("edit_access_request/<int:request_id>/", access_requests.create_access_request, name="edit_access_request"),
+	path("export_access_requests/", access_requests.csv_export, name="export_access_requests"),
 	path("delete_access_request/<int:request_id>/", access_requests.delete_access_request, name="delete_access_request"),
 
 	# Buddy System
 	path("buddy_requests/", buddy_requests.buddy_requests, name="buddy_requests"),
 	path("create_buddy_request/", buddy_requests.create_buddy_request, name="create_buddy_request"),
 	path("edit_buddy_request/<int:request_id>/", buddy_requests.create_buddy_request, name="edit_buddy_request"),
 	path("delete_buddy_request/<int:request_id>/", buddy_requests.delete_buddy_request, name="delete_buddy_request"),
 	path("buddy_request_reply/<int:request_id>/", buddy_requests.buddy_request_reply, name="buddy_request_reply"),
 
+	# Adjustment requests
+	path("adjustment_requests/", adjustment_requests.adjustment_requests, name="adjustment_requests"),
+	path("create_adjustment_request/", adjustment_requests.create_adjustment_request, name="create_adjustment_request"),
+	path("create_adjustment_request/<int:item_type_id>/<int:item_id>/", adjustment_requests.create_adjustment_request, name="create_adjustment_request"),
+	path("edit_adjustment_request/<int:request_id>/", adjustment_requests.create_adjustment_request, name="edit_adjustment_request"),
+	path("edit_adjustment_request/<int:request_id>/<int:item_type_id>/<int:item_id>/", adjustment_requests.create_adjustment_request, name="edit_adjustment_request"),
+	path("adjustment_request_reply/<int:request_id>/", adjustment_requests.adjustment_request_reply, name="adjustment_request_reply"),
+	path("export_adjustment_requests/", adjustment_requests.csv_export, name="export_adjustment_requests"),
+	path("delete_adjustment_request/<int:request_id>/", adjustment_requests.delete_adjustment_request, name="delete_adjustment_request"),
+
 	# Tasks:
 	path("create_task/", tasks.create, name="create_task"),
 	path("cancel_task/<int:task_id>/", tasks.cancel, name="cancel_task"),
 	path("update_task/<int:task_id>/", tasks.update, name="update_task"),
 	path("task_update_form/<int:task_id>/", tasks.task_update_form, name="task_update_form"),
 	path("task_resolution_form/<int:task_id>/", tasks.task_resolution_form, name="task_resolution_form"),
 
@@ -184,21 +201,24 @@
 	path("event_details/area_access/<int:event_id>/", event_details.area_access_details, name="area_access_details"),
 
 	# Qualifications:
 	path("qualifications/", qualifications.qualifications, name="qualifications"),
 	path("modify_qualifications/", qualifications.modify_qualifications, name="modify_qualifications"),
 	path("get_qualified_users/", qualifications.get_qualified_users, name="get_qualified_users"),
 
-	# Staff charges:
-	path("staff_charges/", staff_charges.staff_charges, name="staff_charges"),
-	path("begin_staff_charge/", staff_charges.begin_staff_charge, name="begin_staff_charge"),
-	path("begin_staff_area_charge/", staff_charges.begin_staff_area_charge, name="begin_staff_area_charge"),
-	path("end_staff_area_charge/", staff_charges.end_staff_area_charge, name="end_staff_area_charge"),
-	path("end_staff_charge/", staff_charges.end_staff_charge, name="end_staff_charge"),
-	path("edit_staff_charge_note/", staff_charges.edit_staff_charge_note, name="edit_staff_charge_note"),
+	# Remote work:
+	path("remote_work/", remote_work.remote_work, name="remote_work"),
+	path("staff_charges/", remote_work.staff_charges, name="staff_charges"),
+	path("begin_staff_charge/", remote_work.begin_staff_charge, name="begin_staff_charge"),
+	path("begin_staff_area_charge/", remote_work.begin_staff_area_charge, name="begin_staff_area_charge"),
+	path("end_staff_area_charge/", remote_work.end_staff_area_charge, name="end_staff_area_charge"),
+	path("end_staff_charge/", remote_work.end_staff_charge, name="end_staff_charge"),
+	path("edit_staff_charge_note/", remote_work.edit_staff_charge_note, name="edit_staff_charge_note"),
+	path("validate_staff_charge/<int:staff_charge_id>/", remote_work.validate_staff_charge, name="validate_staff_charge"),
+	path("validate_usage_event/<int:usage_event_id>/", remote_work.validate_usage_event, name="validate_usage_event"),
 
 	# Status dashboard:
 	path("status_dashboard/", status_dashboard.status_dashboard, name="status_dashboard"),
 	re_path(r"^status_dashboard/(?P<tab>tools|occupancy|staff)/$", status_dashboard.status_dashboard, name="status_dashboard_tab"),
 
 	# Jumbotron:
 	path("jumbotron/", jumbotron.jumbotron, name="jumbotron"),
@@ -321,19 +341,21 @@
 	re_path(r"^media_view/(?P<popup>(true|false))/(?P<document_type>\w+)/(?P<document_id>\d+)/$", documents.media_view, name="media_view"),
 
 	# User Preferences
 	path("user_preferences/", users.user_preferences, name="user_preferences"),
 ]
 
 if settings.ALLOW_CONDITIONAL_URLS:
-	urlpatterns += [
-		path("admin/", admin.site.urls),
+	if apps.is_installed("django.contrib.admin"):
+		urlpatterns += [path("admin/", admin.site.urls)]
 
+	urlpatterns += [
 		# REST API
 		path("api/", include(router.urls)),
+		path("api/file_import/", api_file_import.file_import, name="api_file_import"),
 
 		# Area access
 		path("area_access/", area_access.area_access, name="area_access"),
 		path("new_area_access_record/", area_access.new_area_access_record, name="new_area_access_record"),
 
 		# Reminders and periodic events
 		path("cancel_unused_reservations/", calendar.cancel_unused_reservations, name="cancel_unused_reservations"),
@@ -371,19 +393,14 @@
 		path("add_user_to_project/", accounts_and_projects.add_user_to_project, name="add_user_to_project"),
 		path("projects/<int:project_id>/remove_document/<int:document_id>/", accounts_and_projects.remove_document_from_project, name="remove_document_from_project"),
 		path("projects/<int:project_id>/add_document/", accounts_and_projects.add_document_to_project, name="add_document_to_project"),
 
 		# Account, project, and user history
 		re_path(r"^history/(?P<item_type>account|project|user)/(?P<item_id>\d+)/$", history.history, name="history"),
 
-		# Remote work:
-		path("remote_work/", remote_work.remote_work, name="remote_work"),
-		path("validate_staff_charge/<int:staff_charge_id>/", remote_work.validate_staff_charge, name="validate_staff_charge"),
-		path("validate_usage_event/<int:usage_event_id>/", remote_work.validate_usage_event, name="validate_usage_event"),
-
 		# Site customization:
 		path("customization/", customization.customization, name="customization"),
 		path("customization/<str:key>/", customization.customization, name="customization"),
 		path("customize/<str:key>/", customization.customize, name="customize"),
 		path("customize/<str:key>/<str:element>/", customization.customize, name="customize"),
 
 		# Project Usage:
```

### Comparing `NEMO-4.4.1/NEMO/utilities.py` & `NEMO-4.5.0/NEMO/utilities.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 import csv
+import importlib
 import os
 from calendar import monthrange
 from datetime import date, datetime, time
 from email import encoders
 from email.mime.base import MIMEBase
 from enum import Enum
 from io import BytesIO
 from logging import getLogger
 from typing import Dict, List, Optional, Sequence, Set, Tuple, Union
 from urllib.parse import urljoin
 
 from PIL import Image
 from dateutil import rrule
 from dateutil.parser import parse
-from django.conf import settings
+from django.apps import apps
+from django.conf import global_settings, settings
 from django.contrib.admin import ModelAdmin
+from django.contrib.contenttypes.models import ContentType
 from django.core.files.base import ContentFile
 from django.core.files.uploadedfile import InMemoryUploadedFile
 from django.core.mail import EmailMessage
 from django.db.models import QuerySet
 from django.http import HttpRequest, HttpResponse, QueryDict
 from django.shortcuts import render
 from django.template import Template
 from django.template.context import make_context
+from django.urls import NoReverseMatch, reverse
 from django.utils import timezone
 from django.utils.formats import date_format, get_format, time_format
+from django.utils.html import format_html
 from django.utils.timezone import is_naive, localtime
 
 utilities_logger = getLogger(__name__)
 
 # List of python to js formats
 py_to_js_date_formats = {
 	"%A": "dddd",
@@ -77,17 +82,18 @@
 	def __init__(self):
 		super().__init__()
 		self.session = QueryDict(mutable=True)
 		self.device = "desktop"
 
 
 class BasicDisplayTable(object):
-	""" Utility table to make adding headers and rows easier, and export to csv """
+	"""Utility table to make adding headers and rows easier, and export to csv"""
 
 	def __init__(self):
+		self.list_delimiter = ", "
 		# headers is a list of tuples (key, display)
 		self.headers: List[Tuple[str, str]] = []
 		# rows is a list of dictionaries. Each dictionary is a row, with keys corresponding to header keys
 		self.rows: List[Dict] = []
 
 	def add_header(self, header: Tuple[str, str]):
 		if not any(k[0] == header[0] for k in self.headers):
@@ -109,14 +115,16 @@
 		if value:
 			if isinstance(value, time):
 				return format_datetime(value, "SHORT_TIME_FORMAT")
 			elif isinstance(value, datetime):
 				return format_datetime(value, "SHORT_DATETIME_FORMAT")
 			elif isinstance(value, date):
 				return format_datetime(value, "SHORT_DATE_FORMAT")
+			elif isinstance(value, list):
+				return self.list_delimiter.join(value)
 		return value
 
 	def to_csv(self) -> HttpResponse:
 		response = HttpResponse(content_type="text/csv")
 		writer = csv.writer(response)
 		writer.writerow([capitalize(display_value) for key, display_value in self.headers])
 		for row in self.rows:
@@ -144,26 +152,28 @@
 	TIMED_SERVICES = 4
 	FEEDBACK = 5
 	ABUSE = 6
 	SAFETY = 7
 	TASKS = 8
 	ACCESS_REQUESTS = 9
 	SENSORS = 10
+	ADJUSTMENT_REQUESTS = 11
 	Choices = (
 		(GENERAL, "General"),
 		(SYSTEM, "System"),
 		(DIRECT_CONTACT, "Direct Contact"),
 		(BROADCAST_EMAIL, "Broadcast Email"),
 		(TIMED_SERVICES, "Timed Services"),
 		(FEEDBACK, "Feedback"),
 		(ABUSE, "Abuse"),
 		(SAFETY, "Safety"),
 		(TASKS, "Tasks"),
 		(ACCESS_REQUESTS, "Access Requests"),
 		(SENSORS, "Sensors"),
+		(ADJUSTMENT_REQUESTS, "Adjustment Requests"),
 	)
 
 
 class RecurrenceFrequency(Enum):
 	DAILY = 1, rrule.DAILY, "Day(s)", "day"
 	DAILY_WEEKDAYS = 2, rrule.DAILY, "Week Day(s)", "week day"
 	DAILY_WEEKENDS = 3, rrule.DAILY, "Weekend Day(s)", "weekend day"
@@ -323,15 +333,18 @@
 		return time_format(local_time, df or "TIME_FORMAT", use_l10n)
 	elif isinstance(local_time, datetime):
 		return date_format(local_time, df or "DATETIME_FORMAT", use_l10n)
 	return date_format(local_time, df or "DATE_FORMAT", use_l10n)
 
 
 def export_format_datetime(date_time=None, d_format=True, t_format=True, underscore=True, as_current_timezone=True) -> str:
-	""" This function returns a formatted date/time for export files. Default returns date + time format, with underscores """
+	"""
+	This function returns a formatted date/time for export files.
+	Default returns date + time format, with underscores
+	"""
 	this_time = date_time if date_time else timezone.now() if as_current_timezone else datetime.now()
 	export_date_format = getattr(settings, "EXPORT_DATE_FORMAT", "m_d_Y").replace("-", "_")
 	export_time_format = getattr(settings, "EXPORT_TIME_FORMAT", "h_i_s").replace("-", "_")
 	if not underscore:
 		export_date_format = export_date_format.replace("_", "-")
 		export_time_format = export_time_format.replace("_", "-")
 	separator = "-" if underscore else "_"
@@ -359,21 +372,21 @@
 
 
 def naive_local_current_datetime():
 	return localtime(timezone.now()).replace(tzinfo=None)
 
 
 def beginning_of_the_day(t: datetime, in_local_timezone=True) -> datetime:
-	""" Returns the BEGINNING of today's day (12:00:00.000000 AM of the current day) in LOCAL time. """
+	"""Returns the BEGINNING of today's day (12:00:00.000000 AM of the current day) in LOCAL time."""
 	zero = t.replace(hour=0, minute=0, second=0, microsecond=0, tzinfo=None)
 	return localize(zero) if in_local_timezone else zero
 
 
 def end_of_the_day(t: datetime, in_local_timezone=True) -> datetime:
-	""" Returns the END of today's day (11:59:59.999999 PM of the current day) in LOCAL time. """
+	"""Returns the END of today's day (11:59:59.999999 PM of the current day) in LOCAL time."""
 	midnight = t.replace(hour=23, minute=59, second=59, microsecond=999999, tzinfo=None)
 	return localize(midnight) if in_local_timezone else midnight
 
 
 def remove_duplicates(iterable: Union[List, Set, Tuple]) -> List:
 	if not iterable:
 		return []
@@ -442,14 +455,16 @@
 			email_record.attachments = ", ".join(email_attachments)
 	return email_record
 
 
 def create_email_attachment(stream, filename=None, maintype="application", subtype="octet-stream", **content_type_params) -> MIMEBase:
 	attachment = MIMEBase(maintype, subtype, **content_type_params)
 	attachment.set_payload(stream.read())
+	if maintype == "text":
+		attachment.set_charset('utf-8')
 	encoders.encode_base64(attachment)
 	if filename:
 		attachment.add_header("Content-Disposition", f'attachment; filename="{filename}"')
 	return attachment
 
 
 def get_task_image_filename(task_images, filename):
@@ -458,15 +473,18 @@
 
 	task: Task = task_images.task
 	tool_name = slugify(task.tool)
 	now = datetime.now()
 	date = export_format_datetime(now, t_format=False, as_current_timezone=False)
 	year = now.strftime("%Y")
 	number = "{:02d}".format(
-		TaskImages.objects.filter(task__tool=task.tool, uploaded_at__year=now.year, uploaded_at__month=now.month, uploaded_at__day=now.day).count()	+ 1
+		TaskImages.objects.filter(
+			task__tool=task.tool, uploaded_at__year=now.year, uploaded_at__month=now.month, uploaded_at__day=now.day
+		).count()
+		+ 1
 	)
 	ext = os.path.splitext(filename)[1]
 	return f"task_images/{year}/{tool_name}/{date}_{tool_name}_{number}{ext}"
 
 
 def get_tool_image_filename(tool, filename):
 	from django.template.defaultfilters import slugify
@@ -516,15 +534,15 @@
 	from django.template.defaultfilters import slugify
 
 	item_name = slugify(safety_documents.safety_item.name)
 	return f"safety_item/{item_name}/{filename}"
 
 
 def resize_image(image: InMemoryUploadedFile, max: int, quality=85) -> InMemoryUploadedFile:
-	""" Returns a resized image based on the given maximum size """
+	"""Returns a resized image based on the given maximum size"""
 	with Image.open(image) as img:
 		width, height = img.size
 		# no need to resize if width or height is already less than the max
 		if width <= max or height <= max:
 			return image
 		if width > height:
 			width_ratio = max / float(width)
@@ -545,23 +563,23 @@
 
 def distinct_qs_value_list(qs: QuerySet, field_name: str) -> Set:
 	return set(list(qs.values_list(field_name, flat=True)))
 
 
 # Useful function to render and combine 2 separate django templates
 def render_combine_responses(request, original_response: HttpResponse, template_name, context):
-	""" Combines contents of an original http response with a new one """
+	"""Combines contents of an original http response with a new one"""
 	additional_content = render(request, template_name, context)
 	original_response.content += additional_content.content
 	return original_response
 
 
 def render_email_template(template, dictionary: dict, request=None):
-	""" Use Django's templating engine to render the email template
-		If we don't have a request, create a empty one so context_processors (messages, customizations etc.) can be used
+	"""Use Django's templating engine to render the email template
+	If we don't have a request, create a empty one so context_processors (messages, customizations etc.) can be used
 	"""
 	return Template(template).render(make_context(dictionary, request or EmptyHttpRequest()))
 
 
 def queryset_search_filter(query_set: QuerySet, search_fields: Sequence, request, display="__str__") -> HttpResponse:
 	"""
 	This function reuses django admin search result to implement our own autocomplete.
@@ -572,14 +590,15 @@
 		query = request.GET.get("query", "")
 		admin_model = ModelAdmin(query_set.model, None)
 		admin_model.search_fields = search_fields
 		search_qs, search_use_distinct = admin_model.get_search_results(None, query_set, query)
 		if search_use_distinct:
 			search_qs = search_qs.distinct()
 		from NEMO.templatetags.custom_tags_and_filters import json_search_base_with_extra_fields
+
 		data = json_search_base_with_extra_fields(search_qs, *search_fields, display=display)
 	else:
 		data = "This request can only be made as an ajax call"
 	return HttpResponse(data, "application/json")
 
 
 def is_ajax(request):
@@ -592,26 +611,75 @@
 		by_week_day = (rrule.MO, rrule.TU, rrule.WE, rrule.TH, rrule.FR)
 	elif frequency == RecurrenceFrequency.DAILY_WEEKENDS:
 		by_week_day = (rrule.SA, rrule.SU)
 	return rrule.rrule(dtstart=start, freq=frequency.rrule_freq, interval=interval, until=until, count=count, byweekday=by_week_day)
 
 
 def get_full_url(location, request=None):
+	"""
+	Function used mainly in emails and places where the request might or might not be available.
+	If the request is available, use django's built in way to build the absolute URL, otherwise
+	use the SERVER_DOMAIN variable from settings, which defaults to the first ALLOWED_HOSTS value.
+	"""
 	# For lazy locations
 	location = str(location)
-	main_url = getattr(settings, "MAIN_URL", None)
-	if main_url:
-		return urljoin(main_url, location)
-	elif request:
+	if request:
 		return request.build_absolute_uri(location)
 	else:
-		return location
+		domain = getattr(settings, "SERVER_DOMAIN", "https://{}".format(settings.ALLOWED_HOSTS[0]))
+		return urljoin(domain, location)
 
 
 def capitalize(string: Optional[str]) -> str:
 	"""
 	This function capitalizes the first letter only. Built-in .capitalize() method does it, but also
 	makes the rest of the string lowercase, which is not what we want here
 	"""
 	if not string:
 		return string
 	return string[0].upper() + string[1:]
+
+
+def admin_get_item(content_type, object_id):
+	"""
+	This function can be used in django admin to display the item of a generic foreign key with a link
+	"""
+	if not content_type or not object_id:
+		return "-"
+	app_label, model = content_type.app_label, content_type.model
+	viewname = f"admin:{app_label}_{model}_change"
+	try:
+		args = [object_id]
+		link = reverse(viewname, args=args)
+	except NoReverseMatch:
+		return "-"
+	else:
+		return format_html('<a href="{}">{} - #{}</a>', link, get_model_name(content_type), object_id)
+
+
+def get_model_name(content_type: ContentType):
+	try:
+		model = apps.get_model(content_type.app_label, content_type.model)
+		return model._meta.verbose_name.capitalize()
+	except (LookupError, AttributeError):
+		return ""
+
+
+def get_email_from_settings() -> str:
+	"""
+	Return the default from email if it has been overriden, otherwise the server email
+	This allows admins to specify a different default from email (used for communication)
+	from the server email which is more meant for errors and such.
+	"""
+	return (
+		settings.DEFAULT_FROM_EMAIL
+		if settings.DEFAULT_FROM_EMAIL != global_settings.DEFAULT_FROM_EMAIL
+		else settings.SERVER_EMAIL
+	)
+
+
+def get_class_from_settings(setting_name: str, default_value: str):
+	setting_class = getattr(settings, setting_name, default_value)
+	assert isinstance(setting_class, str)
+	pkg, attr = setting_class.rsplit(".", 1)
+	ret = getattr(importlib.import_module(pkg), attr)
+	return ret()
```

### Comparing `NEMO-4.4.1/NEMO/views/abuse.py` & `NEMO-4.5.0/NEMO/views/abuse.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/views/access_requests.py` & `NEMO-4.5.0/NEMO/views/access_requests.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,22 +5,33 @@
 from django.contrib.auth.decorators import login_required, permission_required
 from django.db.models import Q
 from django.http import HttpResponse, HttpResponseBadRequest
 from django.shortcuts import get_object_or_404, redirect, render
 from django.urls import reverse
 from django.utils import timezone
 from django.utils.dateparse import parse_datetime
+from django.utils.text import slugify
 from django.views.decorators.http import require_GET, require_http_methods
 
+from NEMO.decorators import user_office_or_manager_required
 from NEMO.forms import TemporaryPhysicalAccessRequestForm
-from NEMO.models import PhysicalAccessLevel, TemporaryPhysicalAccess, TemporaryPhysicalAccessRequest, User
+from NEMO.models import (
+	Notification,
+	PhysicalAccessLevel,
+	RequestStatus,
+	TemporaryPhysicalAccess,
+	TemporaryPhysicalAccessRequest,
+	User,
+)
 from NEMO.utilities import (
+	BasicDisplayTable,
 	EmailCategory,
 	beginning_of_the_day,
 	bootstrap_primary_color,
+	export_format_datetime,
 	format_datetime,
 	get_full_url,
 	quiet_int,
 	render_email_template,
 	send_mail,
 )
 from NEMO.views.customization import (
@@ -36,30 +47,31 @@
 
 
 @login_required
 @require_GET
 def access_requests(request):
 	mark_requests_expired()
 	user: User = request.user
-	status = TemporaryPhysicalAccessRequest.Status
 	max_requests = quiet_int(UserRequestsCustomization.get("access_requests_display_max"), None)
 	physical_access_requests = TemporaryPhysicalAccessRequest.objects.filter(deleted=False)
 	physical_access_requests = physical_access_requests.order_by("-end_time")
-	if not user.is_facility_manager and not user.is_staff:
+	if not user.is_facility_manager and not user.is_staff and not user.is_user_office:
 		# For some reason doing an "or" filtering with manytomany field returns duplicates, and using distinct() returns nothing...
 		other_user_physical_access_requests = physical_access_requests.filter(other_users__in=[user]).distinct()
-		physical_access_requests = physical_access_requests.filter(Q(creator=user) | Q(id__in=other_user_physical_access_requests))
+		physical_access_requests = physical_access_requests.filter(
+			Q(creator=user) | Q(id__in=other_user_physical_access_requests)
+		)
 	dictionary = {
-		"pending_access_requests": physical_access_requests.filter(status=status.PENDING).order_by("start_time"),
-		"approved_access_requests": physical_access_requests.filter(status=status.APPROVED)[:max_requests],
-		"denied_access_requests": physical_access_requests.filter(status=status.DENIED)[:max_requests],
-		"expired_access_requests": physical_access_requests.filter(status=status.EXPIRED)[:max_requests],
+		"pending_access_requests": physical_access_requests.filter(status=RequestStatus.PENDING).order_by("start_time"),
+		"approved_access_requests": physical_access_requests.filter(status=RequestStatus.APPROVED)[:max_requests],
+		"denied_access_requests": physical_access_requests.filter(status=RequestStatus.DENIED)[:max_requests],
+		"expired_access_requests": physical_access_requests.filter(status=RequestStatus.EXPIRED)[:max_requests],
 		"access_requests_description": UserRequestsCustomization.get("access_requests_description"),
 		"access_request_notifications": get_notifications(
-			request.user, TemporaryPhysicalAccessRequest, delete=not user.is_facility_manager
+			request.user, Notification.Types.TEMPORARY_ACCESS_REQUEST, delete=not user.is_facility_manager
 		),
 	}
 	return render(request, "requests/access_requests/access_requests.html", dictionary)
 
 
 @login_required
 @require_http_methods(["GET", "POST"])
@@ -78,15 +90,15 @@
 	if request.method == "POST":
 		# some extra validation needs to be done here because it depends on the user
 		edit = bool(access_request)
 		errors = []
 		if edit:
 			if access_request.deleted:
 				errors.append("You are not allowed to edit expired or deleted requests.")
-			if access_request.status != TemporaryPhysicalAccessRequest.Status.PENDING:
+			if access_request.status != RequestStatus.PENDING:
 				errors.append("Only pending requests can be modified.")
 			if access_request.creator != user and not user.is_facility_manager:
 				errors.append("You are not allowed to edit a request you didn't create.")
 
 		form = TemporaryPhysicalAccessRequestForm(
 			request.POST, instance=access_request, initial={"creator": access_request.creator if edit else user}
 		)
@@ -102,29 +114,29 @@
 		if form.is_valid():
 			if not edit:
 				form.instance.creator = user
 			if edit and user.is_facility_manager:
 				decision = [state for state in ["approve_request", "deny_request"] if state in request.POST]
 				if decision:
 					if next(iter(decision)) == "approve_request":
-						access_request.status = TemporaryPhysicalAccessRequest.Status.APPROVED
+						access_request.status = RequestStatus.APPROVED
 						create_temporary_access(access_request)
 					else:
-						access_request.status = TemporaryPhysicalAccessRequest.Status.DENIED
+						access_request.status = RequestStatus.DENIED
 					access_request.reviewer = user
 
 			form.instance.last_updated_by = user
 			new_access_request = form.save()
 			create_access_request_notification(new_access_request)
 			if edit:
 				# remove notification for current user and other facility managers
-				delete_notification(TemporaryPhysicalAccessRequest, new_access_request.id, [user])
+				delete_notification(Notification.Types.TEMPORARY_ACCESS_REQUEST, new_access_request.id, [user])
 				if user.is_facility_manager:
 					managers = User.objects.filter(is_active=True, is_facility_manager=True)
-					delete_notification(TemporaryPhysicalAccessRequest, new_access_request.id, managers)
+					delete_notification(Notification.Types.TEMPORARY_ACCESS_REQUEST, new_access_request.id, managers)
 			send_request_received_email(request, new_access_request, edit)
 			return redirect("user_requests", "access")
 		else:
 			dictionary["form"] = form
 			return render(request, "requests/access_requests/access_request.html", dictionary)
 	else:
 		form = TemporaryPhysicalAccessRequestForm(instance=access_request)
@@ -135,20 +147,20 @@
 @login_required
 @require_GET
 def delete_access_request(request, request_id):
 	access_request = get_object_or_404(TemporaryPhysicalAccessRequest, id=request_id)
 
 	if access_request.creator != request.user:
 		return HttpResponseBadRequest("You are not allowed to delete a request you didn't create.")
-	if access_request and access_request.status != TemporaryPhysicalAccessRequest.Status.PENDING:
+	if access_request and access_request.status != RequestStatus.PENDING:
 		return HttpResponseBadRequest("You are not allowed to delete a request that is not pending.")
 
 	access_request.deleted = True
 	access_request.save(update_fields=["deleted"])
-	delete_notification(TemporaryPhysicalAccessRequest, access_request.id)
+	delete_notification(Notification.Types.TEMPORARY_ACCESS_REQUEST, access_request.id)
 	return redirect("user_requests", "access")
 
 
 def create_temporary_access(access_request: TemporaryPhysicalAccessRequest):
 	for user in access_request.creator_and_other_users():
 		TemporaryPhysicalAccess.objects.create(
 			user=user,
@@ -156,18 +168,18 @@
 			start_time=access_request.start_time,
 			end_time=access_request.end_time,
 		)
 
 
 def mark_requests_expired():
 	for expired_request in TemporaryPhysicalAccessRequest.objects.filter(
-			status=TemporaryPhysicalAccessRequest.Status.PENDING, deleted=False, end_time__lt=timezone.now()
+		status=RequestStatus.PENDING, deleted=False, end_time__lt=timezone.now()
 	):
-		delete_notification(TemporaryPhysicalAccessRequest, expired_request.id)
-		expired_request.status = TemporaryPhysicalAccessRequest.Status.EXPIRED
+		delete_notification(Notification.Types.TEMPORARY_ACCESS_REQUEST, expired_request.id)
+		expired_request.status = RequestStatus.EXPIRED
 		expired_request.save(update_fields=["status"])
 
 
 def send_request_received_email(request, access_request: TemporaryPhysicalAccessRequest, edit):
 	user_office_email = EmailsCustomization.get("user_office_email_address")
 	access_request_notification_email = get_media_file_contents("access_request_notification_email.html")
 	if user_office_email and access_request_notification_email:
@@ -179,17 +191,17 @@
 			email
 			for user in cc_users
 			for email in user.get_emails(user.get_preferences().email_send_access_request_updates)
 		]
 		ccs.append(user_office_email)
 		status = (
 			"approved"
-			if access_request.status == TemporaryPhysicalAccessRequest.Status.APPROVED
+			if access_request.status == RequestStatus.APPROVED
 			else "denied"
-			if access_request.status == TemporaryPhysicalAccessRequest.Status.DENIED
+			if access_request.status == RequestStatus.DENIED
 			else "updated"
 			if edit
 			else "received"
 		)
 		absolute_url = get_full_url(reverse("user_requests", kwargs={"tab": "access"}), request)
 		color_type = "success" if status == "approved" else "danger" if status == "denied" else "info"
 		message = render_email_template(
@@ -217,17 +229,17 @@
 @require_GET
 def email_weekend_access_notification(request):
 	return send_email_weekend_access_notification()
 
 
 def send_email_weekend_access_notification():
 	"""
-		Sends a weekend access email to the addresses set in customization with the template provided.
-		The email is sent when the first request (each week) that includes weekend access is approved.
-		If no weekend access requests are made by the given time on the cutoff day (if set), a no access email is sent.
+	Sends a weekend access email to the addresses set in customization with the template provided.
+	The email is sent when the first request (each week) that includes weekend access is approved.
+	If no weekend access requests are made by the given time on the cutoff day (if set), a no access email is sent.
 	"""
 	try:
 		user_office_email = EmailsCustomization.get("user_office_email_address")
 		email_to = UserRequestsCustomization.get("weekend_access_notification_emails")
 		access_contents = get_media_file_contents("weekend_access_email.html")
 		if user_office_email and email_to and access_contents:
 			process_weekend_access_notification(user_office_email, email_to, access_contents)
@@ -246,17 +258,16 @@
 	if cutoff_hour.isdigit() and cutoff_day and cutoff_day.isdigit():
 		cutoff_datetime = (beginning_of_the_week + timedelta(days=int(cutoff_day))).replace(hour=int(cutoff_hour))
 
 	end_of_the_week = beginning_of_the_week + timedelta(weeks=1)
 	beginning_of_the_weekend = beginning_of_the_week + timedelta(days=5)
 
 	# Approved access request that include weekend time do overlap with weekend date interval.
-	approved_status = TemporaryPhysicalAccessRequest.Status.APPROVED
 	approved_weekend_access_requests = TemporaryPhysicalAccessRequest.objects.filter(
-		deleted=False, status=approved_status
+		deleted=False, status=RequestStatus.APPROVED
 	)
 	approved_weekend_access_requests = approved_weekend_access_requests.exclude(start_time__gte=end_of_the_week)
 	approved_weekend_access_requests = approved_weekend_access_requests.exclude(end_time__lte=beginning_of_the_weekend)
 
 	cutoff_time_passed = cutoff_datetime and timezone.now() >= cutoff_datetime
 	last_sent = CustomizationBase.get("weekend_access_notification_last_sent")
 	last_sent_datetime = parse_datetime(last_sent) if last_sent else None
@@ -293,7 +304,49 @@
 		subject=subject,
 		content=message,
 		from_email=user_office_email,
 		to=recipients,
 		cc=ccs,
 		email_category=EmailCategory.ACCESS_REQUESTS,
 	)
+
+
+@user_office_or_manager_required
+@require_GET
+def csv_export(request):
+	return access_csv_export(TemporaryPhysicalAccessRequest.objects.filter(deleted=False))
+
+
+def access_csv_export(request_list: List[TemporaryPhysicalAccessRequest]) -> HttpResponse:
+	table_result = BasicDisplayTable()
+	table_result.add_header(("status", "Status"))
+	table_result.add_header(("created_date", "Created date"))
+	table_result.add_header(("last_updated", "Last updated"))
+	table_result.add_header(("creator", "Creator"))
+	table_result.add_header(("other_users", "Buddies"))
+	table_result.add_header(("area", "Area"))
+	table_result.add_header(("access_level", "Access level"))
+	table_result.add_header(("start", "Start"))
+	table_result.add_header(("end", "End"))
+	table_result.add_header(("reviewer", "Reviewer"))
+	for req in request_list:
+		req: TemporaryPhysicalAccessRequest = req
+		table_result.add_row(
+			{
+				"status": req.get_status_display(),
+				"created_date": req.creation_time,
+				"last_updated": req.last_updated,
+				"creator": req.creator,
+				"other_users": ", ".join([str(user) for user in req.other_users.all()]),
+				"area": req.physical_access_level.area,
+				"access_level": req.physical_access_level,
+				"start": req.start_time,
+				"end": req.end_time,
+				"reviewer": req.reviewer,
+			}
+		)
+
+	name = slugify(UserRequestsCustomization.get("access_requests_title")).replace("-", "_")
+	filename = f"{name}_{export_format_datetime()}.csv"
+	response = table_result.to_csv()
+	response["Content-Disposition"] = f'attachment; filename="{filename}"'
+	return response
```

### Comparing `NEMO-4.4.1/NEMO/views/accounts_and_projects.py` & `NEMO-4.5.0/NEMO/views/accounts_and_projects.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from django.contrib.auth.decorators import login_required
-from django.http import HttpResponseBadRequest
+from django.http import HttpResponseBadRequest, HttpResponseForbidden
 from django.shortcuts import get_object_or_404, redirect, render
 from django.views.decorators.http import require_GET, require_POST, require_http_methods
 
 from NEMO.decorators import accounting_or_user_office_or_manager_required
 from NEMO.forms import AccountForm, ProjectForm
 from NEMO.models import Account, AccountType, ActivityHistory, MembershipHistory, Project, ProjectDocuments, User
 from NEMO.views.customization import ProjectsAccountsCustomization
@@ -121,36 +121,38 @@
 	history.authorizer = request.user
 	history.action = account.active
 	history.content_object = account
 	history.save()
 	return redirect("account", account.id)
 
 
-@accounting_or_user_office_or_manager_required
 @require_POST
 def remove_user_from_project(request):
 	user = get_object_or_404(User, id=request.POST["user_id"])
 	project = get_object_or_404(Project, id=request.POST["project_id"])
+	if not is_user_allowed(request.user, project):
+		return HttpResponseForbidden()
 	if project.user_set.filter(id=user.id).exists():
 		history = MembershipHistory()
 		history.action = MembershipHistory.Action.REMOVED
 		history.authorizer = request.user
 		history.parent_content_object = project
 		history.child_content_object = user
 		history.save()
 		project.user_set.remove(user)
 	dictionary = {"users": project.user_set.all(), "project": project}
 	return render(request, "accounts_and_projects/users_for_project.html", dictionary)
 
 
-@accounting_or_user_office_or_manager_required
 @require_POST
 def add_user_to_project(request):
 	user = get_object_or_404(User, id=request.POST["user_id"])
 	project = get_object_or_404(Project, id=request.POST["project_id"])
+	if not is_user_allowed(request.user, project):
+		return HttpResponseForbidden()
 	if user not in project.user_set.all():
 		history = MembershipHistory()
 		history.action = MembershipHistory.Action.ADDED
 		history.authorizer = request.user
 		history.parent_content_object = project
 		history.child_content_object = user
 		history.save()
@@ -187,9 +189,20 @@
 	return render(request, "accounts_and_projects/documents_for_project.html", dictionary)
 
 
 @login_required
 @require_GET
 def projects(request):
 	user: User = request.user
-	dictionary = {"managed_projects": user.managed_projects.all()}
+	dictionary = {"managed_projects": user.managed_projects.all(), "users": User.objects.all()}
 	return render(request, "accounts_and_projects/projects.html", dictionary)
+
+
+def is_user_allowed(user: User, project):
+	is_active = user.is_active
+	accounting_or_user_office_or_manager = user.is_accounting_officer or user.is_user_office or user.is_facility_manager or user.is_superuser
+	allow_pi_manage = ProjectsAccountsCustomization.get_bool("project_allow_pi_manage_users")
+	if not allow_pi_manage:
+		return is_active and accounting_or_user_office_or_manager
+	else:
+		project_manager = user in project.manager_set.all()
+		return is_active and (project_manager or accounting_or_user_office_or_manager)
```

### Comparing `NEMO-4.4.1/NEMO/views/alerts.py` & `NEMO-4.5.0/NEMO/views/alerts.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/views/api_billing.py` & `NEMO-4.5.0/NEMO/views/api_billing.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/views/area_access.py` & `NEMO-4.5.0/NEMO/views/area_access.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,24 +23,24 @@
 	PhysicalAccessExpiredUserError,
 	ProjectChargeException,
 	ReservationRequiredUserError,
 	ScheduledOutageInProgressError,
 	UnavailableResourcesUserError,
 )
 from NEMO.models import Area, AreaAccessRecord, Project, User
+from NEMO.policy import policy_class as policy
 from NEMO.utilities import (
 	beginning_of_the_day,
 	date_input_format,
 	end_of_the_day,
 	extract_optional_beginning_and_end_dates,
 	quiet_int,
 )
 from NEMO.views.calendar import shorten_reservation
 from NEMO.views.customization import ApplicationCustomization
-from NEMO.views.policy import check_billing_to_project, check_policy_to_enter_any_area, check_policy_to_enter_this_area
 
 area_access_logger = getLogger(__name__)
 
 
 # Utility parser to find error messages in rendered self_login view
 class ParseSelfLoginErrorMessage(HTMLParser):
 
@@ -132,16 +132,16 @@
 			dictionary['error_message'] = 'Your request contained an invalid identifier.'
 			return render(request, 'area_access/new_area_access_record.html', dictionary)
 		try:
 			error_message = check_policy_for_user(customer=user)
 			if error_message:
 				dictionary['error_message'] = error_message
 				return render(request, 'area_access/new_area_access_record.html', dictionary)
-			check_billing_to_project(project, user, area)
-			check_policy_to_enter_this_area(area=area, user=user)
+			policy.check_billing_to_project(project, user, area)
+			policy.check_to_enter_area(area=area, user=user)
 		except ProjectChargeException as e:
 			dictionary['error_message'] = e.msg
 			return render(request, 'area_access/new_area_access_record.html', dictionary)
 		except NoAccessiblePhysicalAccessUserError as error:
 			if error.closure_time:
 				dictionary['error_message'] = '{} does not have access to the {} at this time due to the following closure: {}.'.format(user, area.name, error.closure_time.closure.name)
 			else:
@@ -173,15 +173,15 @@
 		dictionary['success'] = '{} is now logged in to the {}.'.format(user, area.name)
 		return render(request, 'area_access/new_area_access_record.html', dictionary)
 
 
 def check_policy_for_user(customer: User):
 	error_message = None
 	try:
-		check_policy_to_enter_any_area(user=customer)
+		policy.check_to_enter_any_area(user=customer)
 	except InactiveUserError:
 		error_message = '{} is inactive'.format(customer)
 	except NoActiveProjectsForUserError:
 		error_message = '{} does not have any active projects to bill area access'.format(customer)
 	except NoPhysicalAccessUserError:
 		error_message = '{} does not have access to any billable areas'.format(customer)
 	except PhysicalAccessExpiredUserError:
@@ -214,15 +214,15 @@
 		}
 		return render(request, 'area_access/change_project.html', dictionary)
 	# If we're already billing the requested project then there's nothing to do.
 	if old_project.id == new_project:
 		return redirect(reverse('landing'))
 	new_project = get_object_or_404(Project, id=new_project)
 	try:
-		check_billing_to_project(new_project, user, user.area_access_record().area)
+		policy.check_billing_to_project(new_project, user, user.area_access_record().area)
 	except ProjectChargeException as e:
 		dictionary = {
 			'error': e.msg
 		}
 		return render(request, 'area_access/change_project.html', dictionary)
 	# Stop billing the user's initial project
 	record = user.area_access_record()
@@ -277,15 +277,15 @@
 		'projects': user.active_projects(),
 	}
 	if request.GET.get('area_id'):
 		dictionary['area_id'] = quiet_int(request.GET['area_id'])
 
 	facility_name = ApplicationCustomization.get('facility_name')
 	try:
-		check_policy_to_enter_any_area(user)
+		policy.check_to_enter_any_area(user)
 	except InactiveUserError:
 		dictionary['error_message'] = f'Your account has been deactivated. Please visit the {facility_name} staff to resolve the problem.'
 		return render(request, 'area_access/self_login.html', dictionary)
 	except NoActiveProjectsForUserError:
 		dictionary['error_message'] = f"You are not a member of any active projects. You won't be able to use any interlocked {facility_name} tools. Please visit the {facility_name} user office for more information."
 		return render(request, 'area_access/self_login.html', dictionary)
 	except PhysicalAccessExpiredUserError:
@@ -303,16 +303,16 @@
 
 	if request.method == 'GET':
 		return render(request, 'area_access/self_login.html', dictionary)
 	if request.method == 'POST':
 		try:
 			a = Area.objects.get(id=request.POST['area'])
 			p = Project.objects.get(id=request.POST['project'])
-			check_policy_to_enter_this_area(a, request.user)
-			check_billing_to_project(p, user, a)
+			policy.check_to_enter_area(a, request.user)
+			policy.check_billing_to_project(p, user, a)
 			log_in_user_to_area(a, request.user, p)
 		except ProjectChargeException as e:
 			dictionary['area_error_message'] = e.msg
 			return render(request, 'area_access/self_login.html', dictionary)
 		except NoAccessiblePhysicalAccessUserError as error:
 			if error.closure_time:
 				dictionary['area_error_message'] = f"You do not have access to the {error.area.name} at this time due to the following closure: {error.closure_time.closure.name}. The closure ends on {localize(error.closure_time.end_time.astimezone(timezone.get_current_timezone()))}"
```

### Comparing `NEMO-4.4.1/NEMO/views/authentication.py` & `NEMO-4.5.0/NEMO/views/authentication.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,17 @@
 	if pieces[0] != "Basic":
 		return None
 	return b64decode(pieces[1]).decode().split(":")
 
 
 class RemoteUserAuthenticationBackend(ModelBackend):
 	""" The web server performs authentication and passes the username remotely. (header or env) """
+	create_unknown_user = False
 
+	# This override not matching is intended
 	def authenticate(self, request, remote_user):
 		if not remote_user:
 			return
 		username = self.clean_username(remote_user)
 		user = check_user_exists_and_active(self, username)
 		# All security checks passed so let the user in.
 		auth_logger.debug(
```

### Comparing `NEMO-4.4.1/NEMO/views/buddy_requests.py` & `NEMO-4.5.0/NEMO/views/buddy_requests.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,34 @@
-from datetime import date
+from datetime import date, datetime
 from typing import Optional
 
-from django.conf import settings
 from django.contrib.auth.decorators import login_required
 from django.http import HttpResponseBadRequest
 from django.shortcuts import get_object_or_404, redirect, render
 from django.template.defaultfilters import linebreaksbr
 from django.urls import reverse
 from django.views.decorators.http import require_GET, require_POST, require_http_methods
 
 from NEMO.exceptions import (
 	InactiveUserError,
 	NoActiveProjectsForUserError,
 	NoPhysicalAccessUserError,
 	PhysicalAccessExpiredUserError,
 )
 from NEMO.forms import BuddyRequestForm
-from NEMO.models import Area, BuddyRequest, BuddyRequestMessage, User
-from NEMO.utilities import get_full_url
+from NEMO.models import Area, BuddyRequest, Notification, RequestMessage, User
+from NEMO.policy import policy_class as policy
+from NEMO.utilities import end_of_the_day, get_email_from_settings, get_full_url
 from NEMO.views.customization import UserRequestsCustomization
 from NEMO.views.notifications import (
-	create_buddy_reply_notification,
 	create_buddy_request_notification,
+	create_request_message_notification,
 	delete_notification,
 	get_notifications,
 )
-from NEMO.views.policy import check_policy_to_enter_any_area
 
 
 @login_required
 @require_GET
 def buddy_requests(request):
 	mark_requests_expired()
 	buddy_requests = BuddyRequest.objects.filter(expired=False, deleted=False).order_by(
@@ -37,16 +36,16 @@
 	)
 	# extend buddy request to add whether the current user can reply
 	for buddy_request in buddy_requests:
 		buddy_request.user_reply_error = check_user_reply_error(buddy_request, request.user)
 	dictionary = {
 		"buddy_requests": buddy_requests,
 		"buddy_board_description": UserRequestsCustomization.get("buddy_board_description"),
-		"request_notifications": get_notifications(request.user, BuddyRequest),
-		"reply_notifications": get_notifications(request.user, BuddyRequestMessage),
+		"request_notifications": get_notifications(request.user, Notification.Types.BUDDY_REQUEST),
+		"reply_notifications": get_notifications(request.user, Notification.Types.BUDDY_REQUEST_REPLY),
 	}
 	return render(request, "requests/buddy_requests/buddy_requests.html", dictionary)
 
 
 @login_required
 @require_http_methods(["GET", "POST"])
 def create_buddy_request(request, request_id=None):
@@ -90,61 +89,64 @@
 	if buddy_request.replies.count() > 0:
 		return HttpResponseBadRequest("You are not allowed to delete a request that has replies.")
 	if buddy_request.user != request.user:
 		return HttpResponseBadRequest("You are not allowed to delete a request you didn't create.")
 
 	buddy_request.deleted = True
 	buddy_request.save(update_fields=["deleted"])
-	delete_notification(BuddyRequest, buddy_request.id)
+	delete_notification(Notification.Types.BUDDY_REQUEST, buddy_request.id)
 	return redirect("user_requests", "buddy")
 
 
 @login_required
 @require_POST
 def buddy_request_reply(request, request_id):
 	buddy_request = get_object_or_404(BuddyRequest, id=request_id)
 	user: User = request.user
 	message_content = request.POST["reply_content"]
 
 	error_message = check_user_reply_error(buddy_request, user)
 	if error_message:
 		return HttpResponseBadRequest(error_message)
 	elif message_content:
-		reply = BuddyRequestMessage()
-		reply.buddy_request = buddy_request
+		reply = RequestMessage()
+		reply.content_object = buddy_request
 		reply.content = message_content
 		reply.author = user
 		reply.save()
-		create_buddy_reply_notification(reply)
+		request_end = buddy_request.end
+		# Unread buddy request reply notifications expire after the request ends
+		expiration = end_of_the_day(datetime(request_end.year, request_end.month, request_end.day))
+		create_request_message_notification(reply, Notification.Types.BUDDY_REQUEST_REPLY, expiration)
 		email_interested_parties(
 			reply, get_full_url(f"{reverse('user_requests', kwargs={'tab': 'buddy'})}?#{reply.id}", request)
 		)
 	return redirect("user_requests", "buddy")
 
 
-def email_interested_parties(reply: BuddyRequestMessage, reply_url):
-	creator: User = reply.buddy_request.user
-	for user in reply.buddy_request.creator_and_reply_users():
+def email_interested_parties(reply: RequestMessage, reply_url):
+	creator: User = reply.content_object.user
+	for user in reply.content_object.creator_and_reply_users():
 		if user != reply.author and (user == creator or user.get_preferences().email_new_buddy_request_reply):
 			creator_display = f"{creator.get_name()}'s" if creator != user else "your"
 			creator_display_his = creator_display if creator != reply.author else "his"
 			subject = f"New reply on {creator_display} buddy request"
 			message = f"""{reply.author.get_name()} also replied to {creator_display_his} buddy request:
 <br><br>
 {linebreaksbr(reply.content)}
 <br><br>
 Please visit {reply_url} to reply"""
 			email_notification = user.get_preferences().email_send_buddy_request_replies
-			user.email_user(subject=subject, message=message, from_email=settings.SERVER_EMAIL, email_notification=email_notification)
+			user.email_user(subject=subject, message=message, from_email=get_email_from_settings(), email_notification=email_notification)
 
 
 def check_user_reply_error(buddy_request: BuddyRequest, user: User) -> Optional[str]:
 	error_message = None
 	try:
-		check_policy_to_enter_any_area(user)
+		policy.check_to_enter_any_area(user)
 	except InactiveUserError:
 		error_message = "You cannot reply to this request because your account has been deactivated"
 	except NoActiveProjectsForUserError:
 		error_message = "You cannot reply to this request because you don't have any active projects"
 	except PhysicalAccessExpiredUserError:
 		error_message = "You cannot reply to this request because your facility access has expired"
 	except NoPhysicalAccessUserError:
```

### Comparing `NEMO-4.4.1/NEMO/views/calendar.py` & `NEMO-4.5.0/NEMO/views/calendar.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,60 +38,54 @@
 	ScheduledOutage,
 	ScheduledOutageCategory,
 	StaffCharge,
 	Tool,
 	UsageEvent,
 	User,
 )
+from NEMO.policy import policy_class as policy
 from NEMO.utilities import (
 	EmailCategory,
 	RecurrenceFrequency,
 	as_timezone,
 	beginning_of_the_day,
 	bootstrap_primary_color,
 	create_email_attachment,
 	date_input_format,
 	extract_times,
 	format_datetime,
+	get_email_from_settings,
 	get_full_url,
 	get_recurring_rule,
 	localize,
 	parse_parameter_string,
 	quiet_int,
 	render_email_template,
 	send_mail,
 )
 from NEMO.views.constants import ADDITIONAL_INFORMATION_MAXIMUM_LENGTH
 from NEMO.views.customization import (
 	ApplicationCustomization,
 	CalendarCustomization,
 	EmailsCustomization,
 	RecurringChargesCustomization,
-	ToolQualificationCustomization,
+	ToolCustomization,
 	UserCustomization,
 	get_media_file_contents,
 )
-from NEMO.views.policy import (
-	check_billing_to_project,
-	check_policy_to_cancel_reservation,
-	check_policy_to_create_outage,
-	check_policy_to_save_reservation,
-	check_tool_reservation_requiring_area,
-	maximum_users_in_overlapping_reservations,
-)
 from NEMO.widgets.dynamic_form import DynamicForm, render_group_questions
 
 calendar_logger = getLogger(__name__)
 
 
 @login_required
 @require_GET
 def calendar(request, item_type=None, item_id=None):
 	""" Present the calendar view to the user. """
-	user:User = request.user
+	user: User = request.user
 	if request.device == 'mobile':
 		if item_type and item_type == 'tool' and item_id:
 			return redirect('view_calendar', item_id)
 		else:
 			return redirect('choose_item', 'view_calendar')
 
 	tools = Tool.objects.filter(visible=True).only('name', '_category', 'parent_tool_id').order_by('_category', 'name')
@@ -99,15 +93,15 @@
 
 	# We want to remove areas the user doesn't have access to
 	display_all_areas = CalendarCustomization.get_bool("calendar_display_not_qualified_areas")
 	if not display_all_areas and areas and user and not user.is_superuser:
 		areas = [area for area in areas if area in user.accessible_areas()]
 
 	from NEMO.widgets.item_tree import ItemTree
-	rendered_item_tree_html = ItemTree().render(None, {'tools': tools, 'areas':areas, 'user': request.user})
+	rendered_item_tree_html = ItemTree().render(None, {'tools': tools, 'areas': areas, 'user': request.user})
 
 	calendar_view = CalendarCustomization.get('calendar_view')
 	calendar_first_day_of_week = CalendarCustomization.get('calendar_first_day_of_week')
 	calendar_time_format = CalendarCustomization.get('calendar_time_format')
 	calendar_day_column_format = CalendarCustomization.get('calendar_day_column_format')
 	calendar_week_column_format = CalendarCustomization.get('calendar_week_column_format')
 	calendar_month_column_format = CalendarCustomization.get('calendar_month_column_format')
@@ -120,22 +114,22 @@
 
 	dictionary = {
 		'rendered_item_tree_html': rendered_item_tree_html,
 		'tools': list(tools),
 		'areas': list(areas),
 		'auto_select_item_id': item_id,
 		'auto_select_item_type': item_type,
-		'calendar_view' : calendar_view,
-		'calendar_first_day_of_week' : calendar_first_day_of_week,
-		'calendar_time_format' : calendar_time_format,
-		'calendar_day_column_format' : calendar_day_column_format,
-		'calendar_week_column_format' : calendar_week_column_format,
-		'calendar_month_column_format' : calendar_month_column_format,
-		'calendar_start_of_the_day' : calendar_start_of_the_day,
-		'calendar_now_indicator' : calendar_now_indicator,
+		'calendar_view': calendar_view,
+		'calendar_first_day_of_week': calendar_first_day_of_week,
+		'calendar_time_format': calendar_time_format,
+		'calendar_day_column_format': calendar_day_column_format,
+		'calendar_week_column_format': calendar_week_column_format,
+		'calendar_month_column_format': calendar_month_column_format,
+		'calendar_start_of_the_day': calendar_start_of_the_day,
+		'calendar_now_indicator': calendar_now_indicator,
 		'calendar_all_tools': calendar_all_tools,
 		'calendar_all_areas': calendar_all_areas,
 		'calendar_all_areastools': calendar_all_areastools,
 		'calendar_qualified_tools': calendar_qualified_tools,
 		'self_login': False,
 		'self_logout': False,
 	}
@@ -150,15 +144,15 @@
 	return render(request, 'calendar/calendar.html', dictionary)
 
 
 @login_required
 @require_GET
 @disable_session_expiry_refresh
 def event_feed(request):
-	""" Get all reservations for a specific time-window. Optionally: filter by tool, area or user name. """
+	""" Get all reservations for a specific time-window. Optionally: filter by tool, area or user. """
 	try:
 		start, end = extract_calendar_dates(request.GET)
 	except Exception as e:
 		return HttpResponseBadRequest('Invalid start or end time. ' + str(e))
 
 	# We don't want to let someone hammer the database with phony calendar feed lookups.
 	# Block any requests that have a duration of more than 8 weeks. The FullCalendar
@@ -388,15 +382,15 @@
 	new_reservation.user = user
 	new_reservation.creator = current_user
 	# set tool or area
 	setattr(new_reservation, item_type.value, item)
 	new_reservation.start = start
 	new_reservation.end = end
 	new_reservation.short_notice = item.determine_insufficient_notice(start) if item_type == ReservationItemType.TOOL else False
-	policy_problems, overridable = check_policy_to_save_reservation(cancelled_reservation=None, new_reservation=new_reservation, user_creating_reservation=request.user, explicit_policy_override=explicit_policy_override)
+	policy_problems, overridable = policy.check_to_save_reservation(cancelled_reservation=None, new_reservation=new_reservation, user_creating_reservation=request.user, explicit_policy_override=explicit_policy_override)
 
 	# If there was a policy problem with the reservation then return the error...
 	if policy_problems:
 		return render(request, 'calendar/policy_dialog.html', {
 			'policy_problems': policy_problems,
 			'overridable': overridable and request.user.is_staff,
 			'reservation_action': 'create'
@@ -417,15 +411,15 @@
 				return render(request, 'calendar/project_choice.html', {
 					'active_projects': active_projects,
 					'missed_reservation_threshold': new_reservation.reservation_item.missed_reservation_threshold
 				})
 
 		# Check if we are allowed to bill to project
 		try:
-			check_billing_to_project(new_reservation.project, user, new_reservation.reservation_item)
+			policy.check_billing_to_project(new_reservation.project, user, new_reservation.reservation_item)
 		except ProjectChargeException as e:
 			policy_problems.append(e.msg)
 			return render(request, 'calendar/policy_dialog.html', {'policy_problems': policy_problems, 'overridable': False, 'reservation_action': 'create'})
 
 	# Reservation questions if applicable
 	reservation_questions = render_reservation_questions(item_type, item_id, new_reservation.project)
 	if reservation_questions:
@@ -467,28 +461,28 @@
 		return HttpResponse()
 
 	return HttpResponseBadRequest("Reservation creation failed because invalid parameters were sent to the server.")
 
 
 def reservation_success(request, reservation: Reservation):
 	""" Checks area capacity and display warning message if capacity is high """
-	max_area_overlap, max_location_overlap = (0,0)
+	max_area_overlap, max_location_overlap = (0, 0)
 	max_area_time, max_location_time = (None, None)
 	area: Area = reservation.tool.requires_area_access if reservation.reservation_item_type == ReservationItemType.TOOL else reservation.area
 	location = reservation.tool.location if reservation.reservation_item_type == ReservationItemType.TOOL else None
 	if area and area.reservation_warning:
 		overlapping_reservations_in_same_area = Reservation.objects.filter(cancelled=False, missed=False, shortened=False, end__gte=reservation.start, start__lte=reservation.end)
 		if reservation.reservation_item_type == ReservationItemType.TOOL:
 			overlapping_reservations_in_same_area = overlapping_reservations_in_same_area.filter(tool__in=Tool.objects.filter(_requires_area_access=area))
 		elif reservation.reservation_item_type == ReservationItemType.AREA:
 			overlapping_reservations_in_same_area = overlapping_reservations_in_same_area.filter(area=area)
-		max_area_overlap, max_area_time = maximum_users_in_overlapping_reservations(overlapping_reservations_in_same_area)
+		max_area_overlap, max_area_time = policy.check_maximum_users_in_overlapping_reservations(overlapping_reservations_in_same_area)
 		if location:
 			overlapping_reservations_in_same_location = overlapping_reservations_in_same_area.filter(tool__in=Tool.objects.filter(_location=location))
-			max_location_overlap, max_location_time = maximum_users_in_overlapping_reservations(overlapping_reservations_in_same_location)
+			max_location_overlap, max_location_time = policy.check_maximum_users_in_overlapping_reservations(overlapping_reservations_in_same_location)
 	if max_area_overlap and max_area_overlap >= area.warning_capacity():
 		dictionary = {
 			'area': area,
 			'location': location,
 			'max_area_count': max_area_overlap,
 			'max_location_count': max_location_overlap,
 			'max_area_time': max(max_area_time, reservation.start),
@@ -531,29 +525,30 @@
 
 @staff_member_required
 @require_POST
 def create_outage(request):
 	""" Create an outage. """
 	try:
 		start, end = extract_times(request.POST)
+		duration = end - start
 		item_type = ReservationItemType(request.POST['item_type'])
 		item_id = request.POST.get('item_id')
 	except Exception as e:
 		return HttpResponseBadRequest(str(e))
 	item = get_object_or_404(item_type.get_object_class(), id=item_id)
-	# Create the new reservation:
+	# Create the new outage:
 	outage = ScheduledOutage()
 	outage.creator = request.user
 	outage.category = request.POST.get('category', '')[:200]
 	outage.outage_item = item
 	outage.start = start
 	outage.end = end
 
 	# If there is a policy problem for the outage then return the error...
-	policy_problem = check_policy_to_create_outage(outage)
+	policy_problem = policy.check_to_create_outage(outage)
 	if policy_problem:
 		return HttpResponseBadRequest(policy_problem)
 
 	# Make sure there is at least an outage title
 	if not request.POST.get('title'):
 		calendar_outage_recurrence_limit = CalendarCustomization.get("calendar_outage_recurrence_limit")
 		dictionary = {
@@ -570,29 +565,29 @@
 	if request.POST.get('recurring_outage') == 'on':
 		# we have to remove tz before creating rules otherwise 8am would become 7am after DST change for example.
 		start_no_tz = outage.start.replace(tzinfo=None)
 		end_no_tz = outage.end.replace(tzinfo=None)
 
 		submitted_frequency = request.POST.get('recurrence_frequency')
 		submitted_date_until = request.POST.get('recurrence_until', None)
-		date_until = end.replace(hour=0, minute=0, second=0)
+		date_until_no_tz = end_no_tz.replace(hour=0, minute=0, second=0)
 		if submitted_date_until:
-			date_until = localize(datetime.strptime(submitted_date_until, date_input_format))
-		date_until += timedelta(days=1, seconds=-1)  # set at the end of the day
+			date_until_no_tz = datetime.strptime(submitted_date_until, date_input_format)
+		date_until_no_tz += timedelta(days=1, seconds=-1)  # set at the end of the day
 		frequency = RecurrenceFrequency(quiet_int(submitted_frequency, RecurrenceFrequency.DAILY.index))
-		rules = get_recurring_rule(start, frequency, date_until, int(request.POST.get('recurrence_interval', 1)))
+		rules = get_recurring_rule(start_no_tz, frequency, date_until_no_tz, int(request.POST.get('recurrence_interval', 1)))
 		for rule in list(rules):
 			recurring_outage = ScheduledOutage()
 			recurring_outage.creator = outage.creator
 			recurring_outage.category = outage.category
 			recurring_outage.outage_item = outage.outage_item
 			recurring_outage.title = outage.title
 			recurring_outage.details = outage.details
 			recurring_outage.start = localize(start_no_tz.replace(year=rule.year, month=rule.month, day=rule.day))
-			recurring_outage.end = localize(end_no_tz.replace(year=rule.year, month=rule.month, day=rule.day))
+			recurring_outage.end = recurring_outage.start + duration
 			recurring_outage.save()
 	else:
 		outage.save()
 
 	return HttpResponse()
 
 
@@ -662,25 +657,25 @@
 	new_start = reservation_to_cancel.start + start_delta if start_delta else None
 	new_end = reservation_to_cancel.end + end_delta if end_delta else None
 	new_reservation = reservation_to_cancel.copy(new_start, new_end)
 	# Set new creator/time
 	new_reservation.creation_time = now
 	new_reservation.creator = current_user
 
-	response = check_policy_to_cancel_reservation(current_user, reservation_to_cancel, new_reservation)
+	response = policy.check_to_cancel_reservation(current_user, reservation_to_cancel, new_reservation)
 	# Do not move the reservation if the user was not authorized to cancel it.
 	if response.status_code != HTTPStatus.OK:
 		return response
 
 	# Cancel the user's original reservation.
 	reservation_to_cancel.cancelled = True
 	reservation_to_cancel.cancellation_time = now
 	reservation_to_cancel.cancelled_by = current_user
 
-	policy_problems, overridable = check_policy_to_save_reservation(cancelled_reservation=reservation_to_cancel, new_reservation=new_reservation, user_creating_reservation=request.user, explicit_policy_override=explicit_policy_override)
+	policy_problems, overridable = policy.check_to_save_reservation(cancelled_reservation=reservation_to_cancel, new_reservation=new_reservation, user_creating_reservation=request.user, explicit_policy_override=explicit_policy_override)
 	if policy_problems:
 		reservation_action = "resize" if start_delta is None else "move"
 		return render(request, 'calendar/policy_dialog.html', {'policy_problems': policy_problems, 'overridable': overridable and request.user.is_staff, 'reservation_action': reservation_action})
 	else:
 		# All policy checks passed, so save the reservation.
 		new_reservation.save_and_notify()
 		reservation_to_cancel.descendant = new_reservation
@@ -692,15 +687,15 @@
 	try:
 		outage = ScheduledOutage.objects.get(pk=request.POST.get('id'))
 	except ScheduledOutage.DoesNotExist:
 		return HttpResponseNotFound("The outage that you wish to modify doesn't exist!")
 	if start_delta:
 		outage.start += start_delta
 	outage.end += end_delta
-	policy_problem = check_policy_to_create_outage(outage)
+	policy_problem = policy.check_to_create_outage(outage)
 	if policy_problem:
 		return HttpResponseBadRequest(policy_problem)
 	else:
 		# All policy checks passed, so save the reservation.
 		outage.save()
 	return HttpResponse()
 
@@ -748,15 +743,15 @@
 @login_required
 @require_POST
 def change_reservation_project(request, reservation_id):
 	""" Change reservation project for a user. """
 	reservation = get_object_or_404(Reservation, id=reservation_id)
 	project = get_object_or_404(Project, id=request.POST['project_id'])
 	try:
-		check_billing_to_project(project, reservation.user, reservation.reservation_item)
+		policy.check_billing_to_project(project, reservation.user, reservation.reservation_item)
 	except ProjectChargeException as e:
 		return HttpResponseBadRequest(e.msg)
 
 	if (request.user.is_staff or request.user == reservation.user) and \
 		reservation.has_not_ended() and reservation.has_not_started() and \
 		project in reservation.user.active_projects():
 		reservation.project = project
@@ -987,15 +982,15 @@
 @permission_required('NEMO.trigger_timed_services', raise_exception=True)
 def email_out_of_time_reservation_notification(request):
 	return send_email_out_of_time_reservation_notification(request)
 
 
 def send_email_out_of_time_reservation_notification(request=None):
 	"""
-	Out of time reservation notification for areas is when a user is still logged in a area but his reservation expired.
+	Out of time reservation notification for areas is when a user is still logged in an area but his reservation expired.
 	"""
 	# Exit early if the out of time reservation email template has not been customized for the organization yet.
 	# This feature only sends emails, so if the template is not defined there nothing to do.
 	if not get_media_file_contents('out_of_time_reservation_email.html'):
 		return HttpResponseNotFound('The out of time reservation email template has not been customized for your organization yet. Please visit the customization page to upload a template, then out of time email notifications can be sent.')
 
 	out_of_time_user_area = []
@@ -1085,23 +1080,23 @@
 			current_reservation.save()
 	except Reservation.DoesNotExist:
 		pass
 
 
 def cancel_the_reservation(reservation: Reservation, user_cancelling_reservation: User, reason: Optional[str], request=None):
 	# Check policy to cancel reservation contains rules common to cancelling and modifying
-	response = check_policy_to_cancel_reservation(user_cancelling_reservation, reservation)
+	response = policy.check_to_cancel_reservation(user_cancelling_reservation, reservation)
 
 	# The following rules apply only for proper cancellation, not for modification
 	# Staff must provide a reason when cancelling a reservation they do not own.
 	if reservation.user != user_cancelling_reservation and not reason:
 		response = HttpResponseBadRequest("You must provide a reason when cancelling someone else's reservation.")
 
 	policy_problems = []
-	check_tool_reservation_requiring_area(policy_problems, user_cancelling_reservation, reservation, None)
+	policy.check_tool_reservation_requiring_area(policy_problems, user_cancelling_reservation, reservation, None)
 	if policy_problems:
 		return HttpResponseBadRequest(policy_problems[0])
 
 	if response.status_code == HTTPStatus.OK:
 		# All policy checks passed, so cancel the reservation.
 		reservation.cancelled = True
 		reservation.cancellation_time = timezone.now()
@@ -1146,15 +1141,15 @@
 		recipients.append(abuse_email)
 		recipients.append(user_office_email)
 		send_mail(subject=subject, content=message, from_email=user_office_email, to=recipients, email_category=EmailCategory.TIMED_SERVICES)
 	else:
 		calendar_logger.error("Missed reservation email couldn't be send because missed_reservation_email.html or user_office_email are not defined")
 
 
-def send_out_of_time_reservation_notification(reservation:Reservation, request=None):
+def send_out_of_time_reservation_notification(reservation: Reservation, request=None):
 	message = get_media_file_contents('out_of_time_reservation_email.html')
 	user_office_email = EmailsCustomization.get('user_office_email_address')
 	if message and user_office_email:
 		subject = "Out of time in the " + str(reservation.area.name)
 		message = render_email_template(message, {'reservation': reservation}, request)
 		recipients = reservation.user.get_emails(reservation.user.get_preferences().email_send_reservation_ending_reminders)
 		recipients.extend(reservation.area.abuse_email_list())
@@ -1268,15 +1263,15 @@
 Dear facility manager,<br>
 This email is to inform you that today was the last occurrence for the {closure_time.closure.name} facility closure.
 <br><br>Go to NEMO -> Detailed administration -> Closures to add more times if needed.
 """
 	send_mail(
 		subject=f"Last {closure_time.closure.name} occurrence",
 		content=message,
-		from_email=settings.SERVER_EMAIL,
+		from_email=get_email_from_settings(),
 		to=facility_manager_emails,
 		email_category=EmailCategory.SYSTEM,
 	)
 
 
 @login_required
 @require_GET
@@ -1314,17 +1309,17 @@
 @permission_required("NEMO.trigger_timed_services", raise_exception=True)
 def manage_tool_qualifications(request):
 	return do_manage_tool_qualifications(request)
 
 
 def do_manage_tool_qualifications(request=None):
 	user_office_email = EmailsCustomization.get("user_office_email_address")
-	qualification_reminder_days = ToolQualificationCustomization.get("tool_qualification_reminder_days")
-	qualification_expiration_days = ToolQualificationCustomization.get("tool_qualification_expiration_days")
-	qualification_expiration_never_used = ToolQualificationCustomization.get("tool_qualification_expiration_never_used_days")
+	qualification_reminder_days = ToolCustomization.get("tool_qualification_reminder_days")
+	qualification_expiration_days = ToolCustomization.get("tool_qualification_expiration_days")
+	qualification_expiration_never_used = ToolCustomization.get("tool_qualification_expiration_never_used_days")
 	template = get_media_file_contents("tool_qualification_expiration_email.html")
 	if user_office_email and template:
 		if qualification_expiration_days or qualification_expiration_never_used:
 			qualification_expiration_days = quiet_int(qualification_expiration_days, None)
 			qualification_expiration_never_used = quiet_int(qualification_expiration_never_used, None)
 			for qualification in Qualification.objects.filter(user__is_active=True, user__is_staff=False):
 				user = qualification.user
@@ -1347,15 +1342,15 @@
 	return HttpResponse()
 
 
 def send_tool_qualification_expiring_email(qualification: Qualification, last_tool_use: date, expiration_date: date, remaining_days: int = None, request=None):
 	user_office_email = EmailsCustomization.get("user_office_email_address")
 	template = get_media_file_contents("tool_qualification_expiration_email.html")
 	# Add extra cc emails
-	tool_qualification_cc = ToolQualificationCustomization.get("tool_qualification_cc")
+	tool_qualification_cc = ToolCustomization.get("tool_qualification_cc")
 	ccs = [e for e in tool_qualification_cc.split(",") if e]
 	if remaining_days:
 		subject_expiration = f" expires in {remaining_days} days!"
 	else:
 		subject_expiration = " has expired"
 	subject = f"Your {qualification.tool.name} qualification {subject_expiration}"
 	dictionary = {
```

### Comparing `NEMO-4.4.1/NEMO/views/configuration_agenda.py` & `NEMO-4.5.0/NEMO/views/configuration_agenda.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/views/consumables.py` & `NEMO-4.5.0/NEMO/views/consumables.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,30 +4,30 @@
 
 from django.contrib import messages
 from django.http import HttpResponseBadRequest
 from django.shortcuts import get_object_or_404, redirect, render
 from django.utils.text import slugify
 from django.views.decorators.http import require_GET, require_POST, require_http_methods
 
-from NEMO.decorators import staff_member_or_user_office_required, user_office_or_facility_manager_required
+from NEMO.decorators import staff_member_or_user_office_required, user_office_or_manager_required
 from NEMO.exceptions import ProjectChargeException
 from NEMO.forms import ConsumableWithdrawForm, RecurringConsumableChargeForm
 from NEMO.models import Consumable, ConsumableWithdraw, RecurringConsumableCharge, User
+from NEMO.policy import policy_class as policy
 from NEMO.utilities import (
 	BasicDisplayTable,
 	EmailCategory,
 	as_timezone,
 	export_format_datetime,
 	format_datetime,
 	queryset_search_filter, render_email_template,
 	send_mail,
 )
 from NEMO.views.customization import EmailsCustomization, RecurringChargesCustomization, get_media_file_contents
 from NEMO.views.pagination import SortedPaginator
-from NEMO.views.policy import check_billing_to_project
 
 consumables_logger = getLogger(__name__)
 
 
 @staff_member_or_user_office_required
 @require_http_methods(["GET", "POST"])
 def consumables(request):
@@ -43,15 +43,15 @@
 		}
 		return render(request, "consumables/consumables.html", dictionary)
 	elif request.method == "POST":
 		form = ConsumableWithdrawForm(request.POST)
 		if form.is_valid():
 			withdraw = form.save(commit=False)
 			try:
-				check_billing_to_project(withdraw.project, withdraw.customer, withdraw.consumable)
+				policy.check_billing_to_project(withdraw.project, withdraw.customer, withdraw.consumable)
 			except ProjectChargeException as e:
 				return HttpResponseBadRequest(e.msg)
 			add_withdraw_to_session(request, withdraw)
 		else:
 			return HttpResponseBadRequest(form.errors.as_ul())
 		return render(request, "consumables/consumables_order.html")
 
@@ -108,29 +108,29 @@
 			project_id=withdraw["project_id"],
 			request=request,
 		)
 	del request.session["withdrawals"]
 	return redirect("consumables")
 
 
-@user_office_or_facility_manager_required
+@user_office_or_manager_required
 @require_GET
 def recurring_charges(request):
 	page = SortedPaginator(RecurringConsumableCharge.objects.all(), request, order_by="name").get_current_page()
 	dictionary = {"page": page, "extended_permissions": extended_permissions(request)}
 	return render(request, "consumables/recurring_charges.html", dictionary)
 
 
-@user_office_or_facility_manager_required
+@user_office_or_manager_required
 @require_GET
 def search_recurring_charges(request):
 	return queryset_search_filter(RecurringConsumableCharge.objects.all(), ["name", "customer__first_name", "customer__last_name", "customer__username", "project__name"], request, display="search_display")
 
 
-@user_office_or_facility_manager_required
+@user_office_or_manager_required
 @require_GET
 def export_recurring_charges(request):
 	all_one_quantity = set(list(RecurringConsumableCharge.objects.values_list("quantity", flat=True)))
 	table = BasicDisplayTable()
 	table.add_header(("name", "Name"))
 	if len(all_one_quantity) > 1:
 		table.add_header(("quantity", "Quantity"))
@@ -168,15 +168,15 @@
 	response = table.to_csv()
 	feature_name = RecurringChargesCustomization.get("recurring_charges_name")
 	filename = f"{slugify(feature_name.lower()).replace('-', '_')}_{export_format_datetime()}.csv"
 	response["Content-Disposition"] = f'attachment; filename="{filename}"'
 	return response
 
 
-@user_office_or_facility_manager_required
+@user_office_or_manager_required
 @require_http_methods(["GET", "POST"])
 def create_recurring_charge(request, recurring_charge_id: int = None):
 	try:
 		instance = RecurringConsumableCharge.objects.get(pk=recurring_charge_id)
 	except RecurringConsumableCharge.DoesNotExist:
 		instance = None
 	locked = not extended_permissions(request)
@@ -201,26 +201,26 @@
 				obj.save_and_charge_with_user(request.user)
 			else:
 				obj.save_with_user(request.user)
 			return redirect("recurring_charges")
 	return render(request, "consumables/recurring_charge.html", dictionary)
 
 
-@user_office_or_facility_manager_required
+@user_office_or_manager_required
 @require_GET
 def delete_recurring_charge(request, recurring_charge_id: int):
 	if not extended_permissions(request):
 		return redirect("login")
 	recurring_charge = get_object_or_404(RecurringConsumableCharge, pk=recurring_charge_id)
 	if recurring_charge.delete():
 		messages.success(request, f"{recurring_charge.name} was successfully deleted")
 	return redirect("recurring_charges")
 
 
-@user_office_or_facility_manager_required
+@user_office_or_manager_required
 @require_GET
 def clear_recurring_charge(request, recurring_charge_id: int):
 	recurring_charge = get_object_or_404(RecurringConsumableCharge, pk=recurring_charge_id)
 	recurring_charge.clear()
 	return redirect("recurring_charges")
```

### Comparing `NEMO-4.4.1/NEMO/views/customization.py` & `NEMO-4.5.0/NEMO/views/customization.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 from abc import ABC
 from datetime import date, datetime
 from typing import Dict, Iterable
 
+from dateutil.relativedelta import relativedelta
 from django.contrib import messages
 from django.core.exceptions import ValidationError
 from django.core.files.storage import get_storage_class
 from django.core.validators import (
 	validate_comma_separated_integer_list,
 	validate_email,
 	validate_integer,
 )
 from django.http import HttpResponseNotFound
 from django.shortcuts import redirect, render
 from django.template import Context, Template
+from django.utils import timezone
 from django.views.decorators.http import require_GET, require_POST
 
 from NEMO import init_admin_site
 from NEMO.decorators import administrator_required, customization
 from NEMO.exceptions import InvalidCustomizationException
 from NEMO.models import ConsumableCategory, Customization, Project, RecurringConsumableCharge
-from NEMO.utilities import date_input_format, datetime_input_format, quiet_int
+from NEMO.utilities import RecurrenceFrequency, date_input_format, datetime_input_format, quiet_int
 
 
 class CustomizationBase(ABC):
 	_instances = {}
 	# Here we can place variables that we need in NEMO but don't need to be set in UI
 	variables = {"weekend_access_notification_last_sent": ""}
 	files = []
@@ -156,18 +158,20 @@
 		return errors
 
 
 @customization(key="projects_and_accounts", title="Projects & accounts")
 class ProjectsAccountsCustomization(CustomizationBase):
 	variables = {
 		"project_selection_template": "{{ project.name }}",
+		"project_application_identifier_name": "Application identifier",
 		"project_allow_document_upload": "",
 		"account_list_active_only": "",
 		"project_list_active_only": "",
 		"account_list_collapse": "",
+		"project_allow_pi_manage_users": "",
 	}
 
 	def validate(self, name, value):
 		if name == "project_selection_template":
 			try:
 				Template(value).render(Context({"project": Project()}))
 			except Exception as e:
@@ -249,31 +253,72 @@
 		"tool_interlock_failure_message": "Communication with the interlock failed",
 		"door_interlock_failure_message": "Communication with the interlock failed",
 	}
 
 
 @customization(key="requests", title="User requests")
 class UserRequestsCustomization(CustomizationBase):
+	frequencies = [RecurrenceFrequency.DAILY, RecurrenceFrequency.WEEKLY, RecurrenceFrequency.MONTHLY]
 	variables = {
 		"buddy_requests_title": "Buddy requests board",
 		"buddy_board_description": "",
 		"access_requests_title": "Access requests",
 		"access_requests_description": "",
 		"access_requests_minimum_users": "2",
 		"access_requests_display_max": "",
+		"adjustment_requests_enabled": "",
+		"adjustment_requests_tool_usage_enabled": "enabled",
+		"adjustment_requests_area_access_enabled": "enabled",
+		"adjustment_requests_missed_reservation_enabled": "enabled",
+		"adjustment_requests_missed_reservation_times": "",
+		"adjustment_requests_staff_staff_charges_enabled": "enabled",
+		"adjustment_requests_title": "Adjustment requests",
+		"adjustment_requests_description": "",
+		"adjustment_requests_charges_display_number": "10",
+		"adjustment_requests_display_max": "",
+		"adjustment_requests_time_limit_interval": "2",
+		"adjustment_requests_time_limit_frequency": RecurrenceFrequency.WEEKLY.index,
 		"weekend_access_notification_emails": "",
 		"weekend_access_notification_cutoff_hour": "",
 		"weekend_access_notification_cutoff_day": "",
 	}
 
+	@classmethod
+	def get_date_limit(cls) -> datetime:
+		try:
+			interval = cls.get_int("adjustment_requests_time_limit_interval")
+			freq = RecurrenceFrequency(cls.get_int("adjustment_requests_time_limit_frequency"))
+			if interval and freq:
+				delta = (
+					relativedelta(months=interval)
+					if freq == RecurrenceFrequency.MONTHLY
+					else relativedelta(weeks=interval)
+					if freq == RecurrenceFrequency.WEEKLY
+					else relativedelta(days=interval)
+				)
+				return timezone.now() - delta
+		except:
+			pass
+
+	def context(self) -> Dict:
+		context_dict = super().context()
+		context_dict["frequency_choices"] = [(freq.index, freq.display_value) for freq in self.frequencies]
+		return context_dict
+
 	def validate(self, name, value):
 		if name == "weekend_access_notification_emails":
 			recipients = tuple([e for e in value.split(",") if e])
 			for email in recipients:
 				validate_email(email)
+		if value and name == "adjustment_requests_time_limit_frequency":
+			try:
+				if RecurrenceFrequency(int(value)) not in self.frequencies:
+					raise ValidationError(f"frequency must be one of {[freq.display_value for freq in self.frequencies]}")
+			except Exception as e:
+				raise ValidationError(str(e))
 
 
 @customization(key="recurring_charges", title="Recurring charges")
 class RecurringChargesCustomization(CustomizationBase):
 	variables = {
 		"recurring_charges_name": "Recurring charges",
 		"recurring_charges_lock": "",
@@ -301,17 +346,21 @@
 	def save(self, request, element=None):
 		errors = super().save(request, element)
 		if not errors:
 			self.update_title()
 		return errors
 
 
-@customization(key="tool_qualification", title="Tool qualification")
-class ToolQualificationCustomization(CustomizationBase):
+@customization(key="tool", title="Tools")
+class ToolCustomization(CustomizationBase):
 	variables = {
+		"tool_phone_number_required": "enabled",
+		"tool_location_required": "enabled",
+		"tool_control_hide_data_history_users": "",
+		"tool_control_configuration_setting_template": "{{ current_setting }}",
 		"tool_qualification_reminder_days": "",
 		"tool_qualification_expiration_days": "",
 		"tool_qualification_expiration_never_used_days": "",
 		"tool_qualification_cc": "",
 	}
 
 	def validate(self, name, value):
@@ -320,37 +369,52 @@
 		if name == "tool_qualification_reminder_days" and value:
 			# Check that we have an integer or a list of integers
 			validate_comma_separated_integer_list(value)
 		elif name == "tool_qualification_cc":
 			recipients = tuple([e for e in value.split(",") if e])
 			for email in recipients:
 				validate_email(email)
+		if name == "tool_control_configuration_setting_template" and value:
+			try:
+				Template(value).render(Context({"current_setting": "setting"}))
+			except Exception as e:
+				raise ValidationError(str(e))
 
 
 @customization(key="safety", title="Safety")
 class SafetyCustomization(CustomizationBase):
 	variables = {
 		"safety_main_menu": "enabled",
 		"safety_show_safety": "enabled",
 		"safety_show_safety_issues": "enabled",
 		"safety_show_safety_data_sheets": "enabled",
 		"safety_data_sheets_keywords_default": "",
 		"safety_items_expand_categories": "",
 	}
 
 
+@customization(key="remote_work", title="Remote work")
+class RemoteWorkCustomization(CustomizationBase):
+	variables = {
+		"remote_work_validation": "",
+		"remote_work_start_area_access_automatically": "enabled",
+		"remote_work_ask_explicitly": "",
+	}
+
+
 @customization(key="templates", title="File & email templates")
 class TemplatesCustomization(CustomizationBase):
 	files = [
 		("login_banner", ".html"),
 		("authorization_failed", ".html"),
 		("safety_introduction", ".html"),
 		("facility_rules_tutorial", ".html"),
 		("jumbotron_watermark", ".png"),
 		("access_request_notification_email", ".html"),
+		("adjustment_request_notification_email", ".html"),
 		("cancellation_email", ".html"),
 		("counter_threshold_reached_email", ".html"),
 		("feedback_email", ".html"),
 		("generic_email", ".html"),
 		("missed_reservation_email", ".html"),
 		("facility_rules_tutorial_email", ".html"),
 		("new_task_email", ".html"),
```

### Comparing `NEMO-4.4.1/NEMO/views/documents.py` & `NEMO-4.5.0/NEMO/views/documents.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/views/email.py` & `NEMO-4.5.0/NEMO/views/email.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/views/event_details.py` & `NEMO-4.5.0/NEMO/views/event_details.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/views/feedback.py` & `NEMO-4.5.0/NEMO/views/feedback.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/views/get_projects.py` & `NEMO-4.5.0/NEMO/views/get_projects.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/views/history.py` & `NEMO-4.5.0/NEMO/views/history.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/views/jumbotron.py` & `NEMO-4.5.0/NEMO/views/jumbotron.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/views/landing.py` & `NEMO-4.5.0/NEMO/views/landing.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/views/maintenance.py` & `NEMO-4.5.0/NEMO/views/maintenance.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/views/mobile.py` & `NEMO-4.5.0/NEMO/views/mobile.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,22 +7,22 @@
 from django.shortcuts import get_object_or_404, render
 from django.utils import timezone
 from django.utils.dateparse import parse_date, parse_time
 from django.views.decorators.http import require_GET, require_POST
 
 from NEMO.exceptions import ProjectChargeException, RequiredUnansweredQuestionsException
 from NEMO.models import Area, Project, Reservation, ReservationItemType, ScheduledOutage, Tool, User
+from NEMO.policy import policy_class as policy
 from NEMO.utilities import beginning_of_the_day, end_of_the_day, localize
 from NEMO.views.calendar import (
 	extract_configuration,
 	extract_reservation_questions,
 	render_reservation_questions,
 )
 from NEMO.views.customization import CalendarCustomization
-from NEMO.views.policy import check_billing_to_project, check_policy_to_save_reservation
 
 
 @login_required
 @require_GET
 def choose_item(request, next_page):
 	user: User = request.user
 	tools = Tool.objects.filter(visible=True).order_by('_category', 'name')
@@ -105,25 +105,25 @@
 	reservation.reservation_item = item
 	reservation.start = start
 	reservation.end = end
 	if item_type == ReservationItemType.TOOL:
 		reservation.short_notice = item.determine_insufficient_notice(start)
 	else:
 		reservation.short_notice = False
-	policy_problems, overridable = check_policy_to_save_reservation(cancelled_reservation=None, new_reservation=reservation, user_creating_reservation=request.user, explicit_policy_override=False)
+	policy_problems, overridable = policy.check_to_save_reservation(cancelled_reservation=None, new_reservation=reservation, user_creating_reservation=request.user, explicit_policy_override=False)
 
 	# If there was a problem in saving the reservation then return the error...
 	if policy_problems:
 		return render(request, 'mobile/error.html', {'message': policy_problems[0]})
 
 	# All policy checks have passed.
 	try:
 		reservation.project = Project.objects.get(id=request.POST['project_id'])
 		# Check if we are allowed to bill to project
-		check_billing_to_project(reservation.project, request.user, reservation.reservation_item)
+		policy.check_billing_to_project(reservation.project, request.user, reservation.reservation_item)
 	except ProjectChargeException as e:
 		return render(request, 'mobile/error.html', {'message': e.msg})
 	except:
 		if not request.user.is_staff:
 			return render(request, 'mobile/error.html', {'message': 'You must specify a project for your reservation'})
 
 	reservation.additional_information, reservation.self_configuration = extract_configuration(request)
```

### Comparing `NEMO-4.4.1/NEMO/views/news.py` & `NEMO-4.5.0/NEMO/views/news.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 from django.core.paginator import Paginator
 from django.shortcuts import redirect, render
 from django.urls import reverse
 from django.utils import timezone
 from django.views.decorators.http import require_GET, require_POST
 
 from NEMO.decorators import any_staff_required
-from NEMO.models import News
+from NEMO.models import News, Notification
 from NEMO.utilities import format_datetime
 from NEMO.views.notifications import create_news_notification, delete_notification, get_notifications
 
 
 @login_required
 @require_GET
 def view_recent_news(request):
 	dictionary = {
 		"news": News.objects.filter(archived=False).order_by("-pinned", "-last_updated"),
-		"notifications": get_notifications(request.user, News),
+		"notifications": get_notifications(request.user, Notification.Types.NEWS),
 	}
 	return render(request, "news/recent_news.html", dictionary)
 
 
 @login_required
 @require_GET
 def view_archived_news(request, page=1):
@@ -41,15 +41,15 @@
 @any_staff_required
 @require_POST
 def archive_story(request, story_id):
 	try:
 		story = News.objects.get(id=story_id)
 		story.archived = True
 		story.save()
-		delete_notification(News, story.id)
+		delete_notification(Notification.Types.NEWS, story.id)
 	except News.DoesNotExist:
 		pass
 	return redirect(reverse("view_recent_news"))
 
 
 @any_staff_required
 @require_GET
```

### Comparing `NEMO-4.4.1/NEMO/views/pagination.py` & `NEMO-4.5.0/NEMO/views/pagination.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/views/policy.py` & `NEMO-4.5.0/NEMO/policy.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,660 +3,923 @@
 from typing import List, Optional, Union
 
 from django.db.models import Q
 from django.http import HttpResponse, HttpResponseBadRequest
 from django.utils import timezone
 
 from NEMO.exceptions import (
-	InactiveUserError,
-	ItemNotAllowedForProjectException,
-	MaximumCapacityReachedError,
-	NoAccessiblePhysicalAccessUserError,
-	NoActiveProjectsForUserError,
-	NoPhysicalAccessUserError,
-	NotAllowedToChargeProjectException,
-	PhysicalAccessExpiredUserError,
-	ProjectChargeException,
-	ReservationRequiredUserError,
-	ScheduledOutageInProgressError,
-	UnavailableResourcesUserError,
+    InactiveUserError,
+    ItemNotAllowedForProjectException,
+    MaximumCapacityReachedError,
+    NoAccessiblePhysicalAccessUserError,
+    NoActiveProjectsForUserError,
+    NoPhysicalAccessUserError,
+    NotAllowedToChargeProjectException,
+    PhysicalAccessExpiredUserError,
+    ProjectChargeException,
+    ReservationRequiredUserError,
+    ScheduledOutageInProgressError,
+    UnavailableResourcesUserError,
 )
 from NEMO.models import (
-	Area,
-	AreaAccessRecord,
-	ClosureTime,
-	Consumable,
-	PhysicalAccessLevel,
-	Project,
-	Reservation,
-	ReservationItemType,
-	ScheduledOutage,
-	StaffCharge,
-	Tool,
-	User,
+    Area,
+    AreaAccessRecord,
+    ClosureTime,
+    Consumable,
+    PhysicalAccessLevel,
+    Project,
+    Reservation,
+    ReservationItemType,
+    ScheduledOutage,
+    StaffCharge,
+    Tool,
+    User,
 )
 from NEMO.utilities import (
-	EmailCategory,
-	distinct_qs_value_list,
-	format_daterange,
-	format_datetime,
-	render_email_template,
-	send_mail,
+    EmailCategory,
+    distinct_qs_value_list,
+    format_daterange,
+    format_datetime,
+    get_class_from_settings,
+    render_email_template,
+    send_mail,
 )
 from NEMO.views.customization import ApplicationCustomization, EmailsCustomization, get_media_file_contents
 
 
-def check_policy_to_enable_tool(tool: Tool, operator: User, user: User, project: Project, staff_charge: bool):
-	"""
-	Check that the user is allowed to enable the tool. Enable the tool if the policy checks pass.
-	"""
-	facility_name = ApplicationCustomization.get('facility_name')
-
-	# The tool must be visible (or the parent if it's a child tool) to users.
-	visible = tool.parent_tool.visible if tool.is_child_tool() else tool.visible
-	if not visible:
-		return HttpResponseBadRequest("This tool is currently hidden from users.")
-
-	# The tool must be operational.
-	# If the tool is non-operational then it may only be accessed by staff members or service personnel.
-	if not tool.operational and not operator.is_staff and not operator.is_service_personnel:
-		return HttpResponseBadRequest("This tool is currently non-operational.")
-
-	# The tool must not be in use.
-	current_usage_event = tool.get_current_usage_event()
-	if current_usage_event:
-		return HttpResponseBadRequest("The tool is currently being used by " + str(current_usage_event.user) + ".")
-
-	# The user must be qualified to use the tool itself, or the parent tool in case of alternate tool.
-	tool_to_check_qualifications = tool.parent_tool if tool.is_child_tool() else tool
-	if tool_to_check_qualifications not in operator.qualifications.all() and not operator.is_staff:
-		return HttpResponseBadRequest("You are not qualified to use this tool.")
-
-	# Only staff members can operate a tool on behalf of another user.
-	if (user and operator.pk != user.pk) and not operator.is_staff:
-		return HttpResponseBadRequest("You must be a staff member to use a tool on another user's behalf.")
-
-	# All required resources must be available to operate a tool except for staff or service personnel.
-	if tool.required_resource_set.filter(available=False).exists() and not operator.is_staff and not operator.is_service_personnel:
-		return HttpResponseBadRequest("A resource that is required to operate this tool is unavailable.")
-
-	# The tool operator may not activate tools in a particular area unless they are logged in to the area.
-	# Staff are exempt from this rule.
-	if tool.requires_area_access and AreaAccessRecord.objects.filter(area=tool.requires_area_access, customer=operator, staff_charge=None, end=None).count() == 0 and not operator.is_staff:
-		abuse_email_address = EmailsCustomization.get('abuse_email_address')
-		message = get_media_file_contents('unauthorized_tool_access_email.html')
-		if abuse_email_address and message:
-			dictionary = {
-				'operator': operator,
-				'tool': tool,
-				'type': 'access'
-			}
-			rendered_message = render_email_template(message, dictionary)
-			send_mail(subject="Area access requirement", content=rendered_message, from_email=abuse_email_address, to=[abuse_email_address], email_category=EmailCategory.ABUSE)
-		return HttpResponseBadRequest("You must be logged in to the {} to operate this tool.".format(tool.requires_area_access.name))
-
-	# The tool operator may not activate tools in a particular area unless they are still within that area reservation window
-	# Staff and service personnel are exempt from this rule.
-	if not operator.is_staff and not operator.is_service_personnel and tool.requires_area_reservation():
-		if not tool.requires_area_access.get_current_reservation_for_user(operator):
-			abuse_email_address = EmailsCustomization.get('abuse_email_address')
-			message = get_media_file_contents('unauthorized_tool_access_email.html')
-			if abuse_email_address and message:
-				dictionary = {
-					'operator': operator,
-					'tool': tool,
-					'type': 'reservation',
-				}
-				rendered_message = render_email_template(message, dictionary)
-				send_mail(subject="Area reservation requirement", content=rendered_message, from_email=abuse_email_address, to=[abuse_email_address], email_category=EmailCategory.ABUSE)
-			return HttpResponseBadRequest("You must have a current reservation for the {} to operate this tool.".format(tool.requires_area_access.name))
-
-	# Staff may only charge staff time for one user at a time.
-	if staff_charge and operator.charging_staff_time():
-		return HttpResponseBadRequest('You are already charging staff time. You must end the current staff charge before you being another.')
-
-	# Staff may not bill staff time to themselves.
-	if staff_charge and operator == user:
-		return HttpResponseBadRequest('You cannot charge staff time to yourself.')
-
-	# Check if we are allowed to bill to project
-	try:
-		check_billing_to_project(project, user, tool)
-	except ProjectChargeException as e:
-		return HttpResponseBadRequest(e.msg)
-
-	# The tool operator must not have a lock on usage
-	if operator.training_required:
-		return HttpResponseBadRequest(f"You are blocked from using all tools in the {facility_name}. Please complete the {facility_name} rules tutorial in order to use tools.")
-
-	# Users may only use a tool when delayed logoff is not in effect. Staff and service personnel are exempt from this rule.
-	if tool.delayed_logoff_in_progress() and not operator.is_staff and not operator.is_service_personnel:
-		return HttpResponseBadRequest("Delayed tool logoff is in effect. You must wait for the delayed logoff to expire before you can use the tool.")
-
-	# Users may not enable a tool during a scheduled outage. Staff and service personnel are exempt from this rule.
-	if tool.scheduled_outage_in_progress() and not operator.is_staff and not operator.is_service_personnel:
-		return HttpResponseBadRequest("A scheduled outage is in effect. You must wait for the outage to end before you can use the tool.")
-
-	return HttpResponse()
-
-
-def check_policy_to_disable_tool(tool, operator, downtime):
-	""" Check that the user is allowed to disable the tool. """
-	current_usage_event = tool.get_current_usage_event()
-	if current_usage_event.operator != operator and current_usage_event.user != operator and not (operator.is_staff or operator.is_user_office):
-		return HttpResponseBadRequest('You may not disable a tool while another user is using it unless you are a staff member.')
-	if downtime < timedelta():
-		return HttpResponseBadRequest('Downtime cannot be negative.')
-	if downtime > timedelta(minutes=120):
-		return HttpResponseBadRequest('Post-usage tool downtime may not exceed 120 minutes.')
-	if tool.delayed_logoff_in_progress() and downtime > timedelta():
-		return HttpResponseBadRequest('The tool is already in a delayed-logoff state. You may not issue additional delayed logoffs until the existing one expires.')
-	if not tool.allow_delayed_logoff and downtime > timedelta():
-		return HttpResponseBadRequest('Delayed logoff is not allowed for this tool.')
-	return HttpResponse()
-
-
-def check_policy_to_save_reservation(cancelled_reservation: Optional[Reservation], new_reservation: Reservation, user_creating_reservation: User, explicit_policy_override: bool):
-	"""
-		Check the reservation creation policy and return a list of policy problems if any.
-	"""
-	user = new_reservation.user
-
-	facility_name = ApplicationCustomization.get('facility_name')
-
-	# The function will check all policies. Policy problems are placed in the policy_problems list. overridable is True if the policy problems can be overridden by a staff member.
-	policy_problems = []
-	overridable = False
-
-	item_type = new_reservation.reservation_item_type
-
-	# Reservations may not have a start time that is earlier than the end time.
-	if new_reservation.start >= new_reservation.end:
-		policy_problems.append("Reservation start time (" + format_datetime(new_reservation.start) + ") must be before the end time (" + format_datetime(new_reservation.end) + ").")
-
-	check_coincident_item_reservation_policy(cancelled_reservation, new_reservation, user_creating_reservation, policy_problems)
-
-	# Reservations that have been cancelled may not be changed.
-	if new_reservation.cancelled:
-		policy_problems.append("This reservation has already been cancelled by " + str(new_reservation.cancelled_by) + " at " + format_datetime(new_reservation.cancellation_time) + ".")
-
-	# The user must belong to at least one active project to make a reservation.
-	if user.active_project_count() < 1:
-		if user == user_creating_reservation:
-			policy_problems.append("You do not belong to any active projects. Thus, you may not create any reservations.")
-		else:
-			policy_problems.append(str(user) + " does not belong to any active projects and cannot have reservations.")
-
-	# Check if we are allowed to bill to project
-	try:
-		check_billing_to_project(new_reservation.project, user, new_reservation.reservation_item)
-	except ProjectChargeException as e:
-		policy_problems.append(e.msg)
-
-	# If the user is a staff member or there's an explicit policy override then the policy check is finished.
-	if user.is_staff or explicit_policy_override:
-		return policy_problems, overridable
-
-	# If there are no blocking policy conflicts at this point, the rest of the policies can be overridden.
-	if not policy_problems:
-		overridable = True
-
-	# Some tool reservations require a prior area reservation
-	# Staff may break this rule.
-	# An explicit policy override allows this rule to be broken.
-	if item_type == ReservationItemType.TOOL:
-		if new_reservation.tool.requires_area_reservation():
-			area: Area = new_reservation.tool.requires_area_access
-			# Check that a reservation for the area has been made and contains the start time
-			if not Reservation.objects.filter(missed=False, cancelled=False, shortened=False,
-											  user=user, area=area,
-											  start__lte=new_reservation.start,
-											  end__gt=new_reservation.start).exists():
-				if user == user_creating_reservation:
-					policy_problems.append(f"This tool requires a {area} reservation. Please make a reservation in the {area} prior to reserving this tool.")
-				else:
-					policy_problems.append(f"This tool requires a {area} reservation. Please make sure to also create a reservation in the {area} or {str(user)} will not be able to enter the area.")
-
-	# The user must complete training to create reservations.
-	# Staff may break this rule.
-	# An explicit policy override allows this rule to be broken.
-	if user.training_required:
-		if user == user_creating_reservation:
-			policy_problems.append(f"You are blocked from making reservations in the {facility_name}. Please complete the {facility_name} rules tutorial in order to create new reservations.")
-		else:
-			policy_problems.append(f"{str(user)} is blocked from making reservations in the {facility_name}. The user needs to complete the {facility_name} rules tutorial in order to create new reservations.")
-
-	# Users may only change their own reservations.
-	# Staff may break this rule.
-	# An explicit policy override allows this rule to be broken.
-	if cancelled_reservation and user != user_creating_reservation:
-		policy_problems.append("You may not change reservations that you do not own.")
-
-	# The user may not create or move a reservation to have a start time that is earlier than the current time.
-	# Unless it's an extension of an area reservation, in which case the start time is the same.
-	# Staff may break this rule.
-	# An explicit policy override allows this rule to be broken.
-	extension_of_area_reservation = new_reservation.area and cancelled_reservation and cancelled_reservation.start == new_reservation.start
-	if not extension_of_area_reservation and new_reservation.start < timezone.now():
-		policy_problems.append("Reservation start time (" + format_datetime(new_reservation.start) + ") is earlier than the current time (" + format_datetime() + ").")
-
-	# The user may not move or resize a reservation to have an end time that is earlier than the current time.
-	# Staff may break this rule.
-	# An explicit policy override allows this rule to be broken.
-	if new_reservation.end < timezone.now():
-		policy_problems.append("Reservation end time (" + format_datetime(new_reservation.end) + ") is earlier than the current time (" + format_datetime() + ").")
-
-	# The user must be qualified on the tool in question in order to create, move, or resize a reservation.
-	# Staff may break this rule.
-	# An explicit policy override allows this rule to be broken.
-	if new_reservation.tool and new_reservation.tool not in user.qualifications.all():
-		if user == user_creating_reservation:
-			policy_problems.append("You are not qualified to use this tool. Creating, moving, and resizing reservations is forbidden.")
-		else:
-			policy_problems.append(f"{str(user)} is not qualified to use this tool. Creating, moving, and resizing reservations is forbidden.")
-
-	# The user must be authorized on the area in question at the start and end times of the reservation in order to create, move, or resize a reservation.
-	# Staff may break this rule.
-	# An explicit policy override allows this rule to be broken.
-	if item_type == ReservationItemType.AREA:
-		user_access_levels = user.accessible_access_levels_for_area(new_reservation.area)
-		if not any([access_level.accessible_at(new_reservation.start) for access_level in user_access_levels]) or not any([access_level.accessible_at(new_reservation.end) for access_level in user_access_levels]):
-			# it could be inaccessible because of an ongoing closure at the start or end time
-			first_closure_time: ClosureTime = next(iter([access_level.ongoing_closure_time(new_reservation.start) for access_level in user_access_levels]), None)
-			if not first_closure_time:
-				# if there is no closure at start, check at end time
-				first_closure_time = next(iter([access_level.ongoing_closure_time(new_reservation.end) for access_level in user_access_levels]), None)
-			if first_closure_time:
-				details = f" due to the following closure: {first_closure_time.closure.name} ({format_daterange(first_closure_time.start_time, first_closure_time.end_time)})"
-			# or simply due to scheduling
-			else:
-				details = f" (times allowed in this area are: {', '.join([access.get_schedule_display_with_times() for access in user_access_levels])})" if user_access_levels else ''
-			if user == user_creating_reservation:
-				policy_problems.append(f"You are not authorized to access this area at this time{details}. Creating, moving, and resizing reservations is forbidden.")
-			else:
-				policy_problems.append(f"{str(user)} is not authorized to access this area at this time{details}. Creating, moving, and resizing reservations is forbidden.")
-
-	check_tool_reservation_requiring_area(policy_problems, user_creating_reservation, cancelled_reservation, new_reservation)
-
-	# The reservation start time may not exceed the item's reservation horizon.
-	# Staff may break this rule.
-	# An explicit policy override allows this rule to be broken.
-	item = new_reservation.reservation_item
-	if item.reservation_horizon is not None:
-		reservation_horizon = timedelta(days=item.reservation_horizon)
-		if new_reservation.start > timezone.now() + reservation_horizon:
-			policy_problems.append("You may not create reservations further than " + str(reservation_horizon.days) + f" days from now for this {item_type.value}.")
-
-	# Check item policy rules
-	item_policy_problems = []
-	if should_enforce_policy(new_reservation):
-		item_policy_problems = check_policy_rules_for_item(user_creating_reservation, new_reservation, cancelled_reservation)
-
-	# Return the list of all policies that are not met.
-	return policy_problems + item_policy_problems, overridable
-
-
-def check_tool_reservation_requiring_area(policy_problems: List[str], user_creating_reservation: User, cancelled_reservation: Optional[Reservation], new_reservation: Optional[Reservation]):
-	# When modifying an area reservation, check that all tools reservations starting during the cancelled one are still within the new one
-	if cancelled_reservation and cancelled_reservation.reservation_item_type == ReservationItemType.AREA:
-		tools_requiring_cancelled_reservation = Reservation.objects.filter(cancelled=False, missed=False, shortened=False, tool__isnull=False, tool___requires_area_access=cancelled_reservation.area, user=cancelled_reservation.user)
-		tools_requiring_cancelled_reservation = tools_requiring_cancelled_reservation.filter(start__gte=cancelled_reservation.start, start__lt=cancelled_reservation.end)
-		if tools_requiring_cancelled_reservation.exists():
-			if new_reservation:
-				tools_requiring_new_reservation = Reservation.objects.filter(cancelled=False, missed=False, shortened=False, tool__isnull=False, tool___requires_area_access=new_reservation.area, user=new_reservation.user)
-				tools_requiring_new_reservation = tools_requiring_new_reservation.filter(start__gte=new_reservation.start, start__lt=new_reservation.end)
-			else:
-				tools_requiring_new_reservation = Reservation.objects.none()
-			difference: List[Reservation] = [item for item in tools_requiring_cancelled_reservation if item not in tools_requiring_new_reservation]
-			# As long as the new reservation includes the same tool reservations, we are good
-			if difference:
-				user = cancelled_reservation.user
-				area = new_reservation.area if new_reservation else cancelled_reservation.area
-				difference.sort(key=lambda x: x.start)
-				if user == user_creating_reservation:
-					policy_problems.append(f"You have a reservation for the {difference[0].tool} at {format_datetime(difference[0].start)} that requires a {area} reservation. Cancel or reschedule the tool reservation first and try again.")
-				else:
-					policy_problems.append(f"{str(user)} has a reservation for the {difference[0].tool} at {format_datetime(difference[0].start)} that requires a {area} reservation. Cancel or reschedule the tool reservation first and try again.")
-
-
-def check_coincident_item_reservation_policy(cancelled_reservation: Optional[Reservation], new_reservation: Reservation, user_creating_reservation: User, policy_problems: List):
-	user = new_reservation.user
-
-	# For tools the user may not create, move, or resize a reservation to coincide with another user's reservation.
-	# For areas, it cannot coincide with another reservation for the same user, or with a number of other users greater than the area capacity
-	coincident_events = Reservation.objects.filter(cancelled=False, missed=False, shortened=False)
-	# Exclude the reservation we're cancelling in order to create a new one:
-	if cancelled_reservation and cancelled_reservation.id:
-		coincident_events = coincident_events.exclude(id=cancelled_reservation.id)
-	# Exclude events for which the following is true:
-	# The event starts and ends before the time-window, and...
-	# The event starts and ends after the time-window.
-	coincident_events = coincident_events.exclude(start__lt=new_reservation.start, end__lte=new_reservation.start)
-	coincident_events = coincident_events.exclude(start__gte=new_reservation.end, end__gt=new_reservation.end)
-	if new_reservation.reservation_item_type == ReservationItemType.TOOL and coincident_events.filter(**new_reservation.reservation_item_filter).count() > 0:
-		policy_problems.append("Your reservation coincides with another reservation that already exists. Please choose a different time.")
-	if new_reservation.reservation_item_type == ReservationItemType.AREA:
-		if coincident_events.filter(**new_reservation.reservation_item_filter).filter(user=user).count() > 0:
-			if user == user_creating_reservation:
-				policy_problems.append("You already have a reservation that coincides with this one. Please choose a different time.")
-			else:
-				policy_problems.append(f"{str(user)} already has a reservation that coincides with this one. Please choose a different time.")
-		for area in new_reservation.area.get_ancestors(ascending=True, include_self=True):
-			# Check reservations for all other children of the parent areas
-			if not area.count_staff_in_occupancy:
-				coincident_events = coincident_events.filter(user__is_staff=False)
-			if not area.count_service_personnel_in_occupancy:
-				coincident_events = coincident_events.filter(user__is_service_personnel=False)
-			apply_to_user = (not user.is_staff and not user.is_service_personnel) or (user.is_staff and area.count_staff_in_occupancy) or (user.is_service_personnel and area.count_service_personnel_in_occupancy)
-			if apply_to_user and area.maximum_capacity:
-				children_events = coincident_events.filter(area_id__in=[area.id for area in area.get_descendants(include_self=True)])
-				reservations = list(children_events)
-				reservations.append(new_reservation)
-				# Check only distinct users since the same user could make reservations in different rooms
-				maximum_users, time = maximum_users_in_overlapping_reservations(reservations)
-				if maximum_users > area.maximum_capacity:
-					time_display = "at this time" if time is None else "at "+ format_datetime(time, "TIME_FORMAT")
-					policy_problems.append(f"The {area} would be over its maximum capacity {time_display}. Please choose a different time.")
-
-	# The user may not create, move, or resize a reservation to coincide with a scheduled outage.
-	if new_reservation.reservation_item_type == ReservationItemType.TOOL:
-		coincident_events = ScheduledOutage.objects.filter(
-			Q(tool=new_reservation.tool) | Q(resource__fully_dependent_tools__in=[new_reservation.tool]))
-	elif new_reservation.reservation_item_type == ReservationItemType.AREA:
-		coincident_events = new_reservation.area.scheduled_outage_queryset()
-	else:
-		coincident_events = ScheduledOutage.objects.none()
-	# Exclude events for which the following is true:
-	# The event starts and ends before the time-window, and...
-	# The event starts and ends after the time-window.
-	coincident_events = coincident_events.exclude(start__lt=new_reservation.start, end__lte=new_reservation.start)
-	coincident_events = coincident_events.exclude(start__gte=new_reservation.end, end__gt=new_reservation.end)
-	if coincident_events.count() > 0:
-		policy_problems.append("Your reservation coincides with a scheduled outage. Please choose a different time.")
-
-
-def should_enforce_policy(reservation: Reservation):
-	""" Returns whether or not the policy rules should be enforced. """
-	should_enforce = True
-
-	item = reservation.reservation_item
-	start_time = timezone.localtime(reservation.start)
-	end_time = timezone.localtime(reservation.end)
-	if item.policy_off_weekend and start_time.weekday() >= 5 and end_time.weekday() >= 5:
-		should_enforce = False
-	if item.policy_off_between_times and item.policy_off_start_time and item.policy_off_end_time:
-		if item.policy_off_start_time <= item.policy_off_end_time:
-			""" Range is something like 6am-6pm """
-			if item.policy_off_start_time <= start_time.time() <= item.policy_off_end_time and item.policy_off_start_time <= end_time.time() <= item.policy_off_end_time:
-				should_enforce = False
-		else:
-			""" Range is something like 6pm-6am """
-			if (item.policy_off_start_time <= start_time.time() or start_time.time() <= item.policy_off_end_time) and (item.policy_off_start_time <= end_time.time() or end_time.time() <= item.policy_off_end_time):
-				should_enforce = False
-	return should_enforce
-
-
-def check_policy_rules_for_item(user_creating_reservation: User, new_reservation: Reservation, cancelled_reservation: Optional[Reservation]):
-	item_policy_problems = []
-	# Calculate the duration of the reservation:
-	duration = new_reservation.end - new_reservation.start
-
-	# The reservation must be at least as long as the minimum block time for this item.
-	# Staff may break this rule.
-	# An explicit policy override allows this rule to be broken.
-	item = new_reservation.reservation_item
-	item_type = new_reservation.reservation_item_type
-	if item.minimum_usage_block_time:
-		minimum_block_time = timedelta(minutes=item.minimum_usage_block_time)
-		if duration < minimum_block_time:
-			item_policy_problems.append(f"Your reservation has a duration of {str(int(duration.total_seconds() / 60))} minutes. This {item_type.value} requires a minimum reservation duration of {str(int(minimum_block_time.total_seconds() / 60))} minutes.")
-
-	# The reservation may not exceed the maximum block time for this tool.
-	# Staff may break this rule.
-	# An explicit policy override allows this rule to be broken.
-	if item.maximum_usage_block_time:
-		maximum_block_time = timedelta(minutes=item.maximum_usage_block_time)
-		if duration > maximum_block_time:
-			item_policy_problems.append(f"Your reservation has a duration of {str(int(duration.total_seconds() / 60))} minutes. Reservations for this {item_type.value} may not exceed {str(int(maximum_block_time.total_seconds() / 60))} minutes.")
-
-	user = new_reservation.user
-
-	# If there is a limit on number of reservations per user per day then verify that the user has not exceeded it.
-	# Staff may break this rule.
-	# An explicit policy override allows this rule to be broken.
-	if item.maximum_reservations_per_day:
-		start_of_day = new_reservation.start
-		start_of_day = start_of_day.replace(hour=0, minute=0, second=0, microsecond=0)
-		end_of_day = start_of_day + timedelta(days=1)
-		reservations_for_that_day = Reservation.objects.filter(cancelled=False, shortened=False, start__gte=start_of_day, end__lte=end_of_day, user=user)
-		reservations_for_that_day = reservations_for_that_day.filter(**new_reservation.reservation_item_filter)
-		# Exclude any reservation that is being cancelled.
-		if cancelled_reservation and cancelled_reservation.id:
-			reservations_for_that_day = reservations_for_that_day.exclude(id=cancelled_reservation.id)
-		if reservations_for_that_day.count() >= item.maximum_reservations_per_day:
-			if user == user_creating_reservation:
-				item_policy_problems.append(f"You may only have {str(item.maximum_reservations_per_day)} reservations for this {item_type.value} per day. Missed reservations are included when counting the number of reservations per day.")
-			else:
-				item_policy_problems.append(f"{str(user)} may only have {str(item.maximum_reservations_per_day)} reservations for this {item_type.value} per day. Missed reservations are included when counting the number of reservations per day.")
-
-	# A minimum amount of time between reservations for the same user & same tool can be enforced.
-	# Staff may break this rule.
-	# An explicit policy override allows this rule to be broken.
-	if item.minimum_time_between_reservations:
-		buffer_time = timedelta(minutes=item.minimum_time_between_reservations)
-		must_end_before = new_reservation.start - buffer_time
-		too_close = Reservation.objects.filter(cancelled=False, shortened=False, user=user, end__gt=must_end_before, start__lt=new_reservation.start)
-		too_close = too_close.filter(**new_reservation.reservation_item_filter)
-		if cancelled_reservation and cancelled_reservation.id:
-			too_close = too_close.exclude(id=cancelled_reservation.id)
-		if too_close.exists():
-			if user == user_creating_reservation:
-				item_policy_problems.append(f"Separate reservations for this {item_type.value} that belong to you must be at least {str(item.minimum_time_between_reservations)} minutes apart from each other. The proposed reservation ends too close to another reservation.")
-			else:
-				item_policy_problems.append(f"Separate reservations for this {item_type.value} that belong to {str(user)} must be at least {str(item.minimum_time_between_reservations)} minutes apart from each other. The proposed reservation ends too close to another reservation.")
-		must_start_after = new_reservation.end + buffer_time
-		too_close = Reservation.objects.filter(cancelled=False, shortened=False, user=user, start__lt=must_start_after, end__gt=new_reservation.start)
-		too_close = too_close.filter(**new_reservation.reservation_item_filter)
-		if cancelled_reservation and cancelled_reservation.id:
-			too_close = too_close.exclude(id=cancelled_reservation.id)
-		if too_close.exists():
-			if user == user_creating_reservation:
-				item_policy_problems.append(f"Separate reservations for this {item_type.value} that belong to you must be at least {str(item.minimum_time_between_reservations)} minutes apart from each other. The proposed reservation begins too close to another reservation.")
-			else:
-				item_policy_problems.append(f"Separate reservations for this {item_type.value} that belong to {str(user)} must be at least {str(item.minimum_time_between_reservations)} minutes apart from each other. The proposed reservation begins too close to another reservation.")
-
-	# Check that the user is not exceeding the maximum amount of time they may reserve in the future.
-	# Staff may break this rule.
-	# An explicit policy override allows this rule to be broken.
-	if item.maximum_future_reservation_time:
-		reservations_after_now = Reservation.objects.filter(cancelled=False, user=user, start__gte=timezone.now())
-		reservations_after_now = reservations_after_now.filter(**new_reservation.reservation_item_filter)
-		if cancelled_reservation and cancelled_reservation.id:
-			reservations_after_now = reservations_after_now.exclude(id=cancelled_reservation.id)
-		amount_reserved_in_the_future = new_reservation.duration()
-		for r in reservations_after_now:
-			amount_reserved_in_the_future += r.duration()
-		if amount_reserved_in_the_future.total_seconds() / 60 > item.maximum_future_reservation_time:
-			if user == user_creating_reservation:
-				item_policy_problems.append(f"You may only reserve up to {str(item.maximum_future_reservation_time)} minutes of time on this {item_type.value}, starting from the current time onward.")
-			else:
-				item_policy_problems.append(f"{str(user)} may only reserve up to {str(item.maximum_future_reservation_time)} minutes of time on this {item_type.value}, starting from the current time onward.")
-
-	return item_policy_problems
-
-
-def check_policy_to_cancel_reservation(user_cancelling_reservation: User, reservation_to_cancel: Reservation, new_reservation: Optional[Reservation] = None):
-	"""
-	Checks the reservation deletion policy.
-	If all checks pass the function returns an HTTP "OK" response.
-	Otherwise, the function returns an HTTP "Bad Request" with an error message.
-	"""
-
-	move = new_reservation and new_reservation.start != reservation_to_cancel.start
-	resize = new_reservation and new_reservation.start == reservation_to_cancel.start
-	action = 'move' if move else 'resize' if resize else 'cancel'
-
-	# Users may only cancel reservations that they own.
-	# Staff may break this rule.
-	if (reservation_to_cancel.user != user_cancelling_reservation) and not user_cancelling_reservation.is_staff:
-		return HttpResponseBadRequest(f"You may not {action} reservations that you do not own.")
-
-	# Users may not cancel reservations that have already ended.
-	# Staff may break this rule.
-	if reservation_to_cancel.end < timezone.now() and not user_cancelling_reservation.is_staff:
-		return HttpResponseBadRequest(f"You may not {action} reservations that have already ended.")
-
-	# Users may not cancel ongoing area reservations when they are currently logged in that area (unless they are extending it)
-	# Staff may break this rule.
-	if reservation_to_cancel.area and reservation_to_cancel.area.requires_reservation and not resize and reservation_to_cancel.start < timezone.now() < reservation_to_cancel.end and AreaAccessRecord.objects.filter(end=None, staff_charge=None, customer=reservation_to_cancel.user, area=reservation_to_cancel.area) and not user_cancelling_reservation.is_staff:
-		if move:
-			return HttpResponseBadRequest("You may only resize an area reservation while logged in that area.")
-		else:
-			return HttpResponseBadRequest("You may not cancel an area reservation while logged in that area.")
-
-	if reservation_to_cancel.cancelled:
-		return HttpResponseBadRequest("This reservation has already been cancelled by " + str(reservation_to_cancel.cancelled_by) + " on " + format_datetime(reservation_to_cancel.cancellation_time) + ".")
-
-	if reservation_to_cancel.missed:
-		return HttpResponseBadRequest("This reservation was missed and cannot be modified.")
-
-	return HttpResponse()
-
-
-def check_policy_to_create_outage(outage: ScheduledOutage):
-	# Outages may not have a start time that is earlier than the end time.
-	if outage.start >= outage.end:
-		return "Outage start time (" + format_datetime(outage.start) + ") must be before the end time (" + format_datetime(outage.end) + ")."
-
-	# The user may not create, move, or resize an outage to coincide with another user's reservation.
-	coincident_events = Reservation.objects.filter(**outage.outage_item_filter).filter(cancelled=False, missed=False, shortened=False)
-	# Exclude events for which the following is true:
-	# The event starts and ends before the time-window, and...
-	# The event starts and ends after the time-window.
-	coincident_events = coincident_events.exclude(start__lt=outage.start, end__lte=outage.start)
-	coincident_events = coincident_events.exclude(start__gte=outage.end, end__gt=outage.end)
-	if coincident_events.count() > 0:
-		return "Your scheduled outage coincides with a reservation that already exists. Please choose a different time."
-
-	# No policy issues! The outage can be created...
-	return None
-
-
-def check_policy_to_enter_any_area(user: User):
-	"""
-	Checks the area access policy for a user.
-	"""
-	if not user.is_active:
-		raise InactiveUserError(user=user)
-
-	if user.active_project_count() < 1:
-		raise NoActiveProjectsForUserError(user=user)
-
-	if user.access_expiration is not None and user.access_expiration < date.today():
-		raise PhysicalAccessExpiredUserError(user=user)
-
-	user_has_access_to_at_least_one_area = user.accessible_access_levels().exists()
-	if not user_has_access_to_at_least_one_area:
-		raise NoPhysicalAccessUserError(user=user)
-
-
-def check_policy_to_enter_this_area(area: Area, user: User):
-	# If explicitly set on the Physical Access Level, staff & user office may be exempt from being granted explicit access
-	if (user.is_staff or user.is_user_office) and any([access_level.accessible() for access_level in PhysicalAccessLevel.objects.filter(allow_staff_access=True, area=area)]):
-		pass
-	else:
-		# Check if the user normally has access to this area door at the current time (or access to any parent)
-		if not any([access_level.accessible() for access_level in user.accessible_access_levels_for_area(area)]):
-			first_closure_time = next(iter([access_level.ongoing_closure_time() for access_level in user.accessible_access_levels_for_area(area)]), None)
-			raise NoAccessiblePhysicalAccessUserError(user=user, area=area, closure_time=first_closure_time)
-
-	if not user.is_staff and not user.is_service_personnel:
-		for a in area.get_ancestors(ascending=True, include_self=True):
-			unavailable_resources = a.required_resources.filter(available=False)
-			if unavailable_resources:
-				raise UnavailableResourcesUserError(user=user, area=a, resources=unavailable_resources)
-
-		# Non staff users may not enter an area during a scheduled outage.
-		if area.scheduled_outage_in_progress():
-			raise ScheduledOutageInProgressError(user=user, area=area)
-
-		# If we reached maximum capacity, fail (only for non staff users)
-		for a in area.get_ancestors(ascending=True, include_self=True):
-			if a.maximum_capacity and 0 < a.maximum_capacity <= a.occupancy_count():
-				raise MaximumCapacityReachedError(user=user, area=a)
-
-		if area.requires_reservation and not area.get_current_reservation_for_user(user):
-			raise ReservationRequiredUserError(user=user, area=area)
-
-
-def check_billing_to_project(project: Project, user: User, item: Union[Tool, Area, Consumable, StaffCharge] = None):
-	if project:
-		if project not in user.active_projects():
-			raise NotAllowedToChargeProjectException(project=project, user=user)
-
-		if item:
-			# Check if project only allows billing for certain tools
-			allowed_tools = project.only_allow_tools.all()
-			if allowed_tools.exists():
-				if isinstance(item, Tool) and item not in allowed_tools:
-					msg = f"{item.name} is not allowed for project {project.name}"
-					raise ItemNotAllowedForProjectException(project, user, item.name, msg)
-				elif isinstance(item, Area) and item.id not in distinct_qs_value_list(
-						allowed_tools, '_requires_area_access_id'):
-					msg = f"{item.name} is not allowed for project {project.name}"
-					raise ItemNotAllowedForProjectException(project, user, item.name, msg)
-			# Check if consumable withdrawals are allowed
-			if isinstance(item, Consumable):
-				if not project.allow_consumable_withdrawals:
-					msg = f"Consumable withdrawals are not allowed for project {project.name}"
-					raise ItemNotAllowedForProjectException(project, user, "Staff Charges", msg)
-
-
-def maximum_users_in_overlapping_reservations(reservations: List[Reservation]) -> (int, datetime):
-	"""
-	Returns the maximum number of overlapping reservations and the earlier time the maximum is reached
-	This will only count reservations made by different users. i.e. if a user has 3 reservations at the same
-	time for different tools/areas, it will only count as one.
-	"""
-	# First we need to merge reservations by user, since one user could have more than one at the same time. (and we should only count it as one)
-	intervals_by_user = defaultdict(list)
-	for r in reservations:
-		intervals_by_user[r.user.id].append((r.start, r.end))
-
-	merged_intervals = []
-	for user, intervals in intervals_by_user.items():
-		merged_intervals.extend(recursive_merge(sorted(intervals).copy()))
-
-	# Now let's count the maximum overlapping reservations
-	times = []
-	for interval in merged_intervals:
-		start_time, end_time = interval[0], interval[1]
-		times.append((start_time, 'start'))
-		times.append((end_time, 'end'))
-	times = sorted(times)
-
-	count = 0
-	max_count = 0
-	max_time: Optional[datetime] = None
-	for time in times:
-		if time[1] == 'start':
-			count += 1  # increment on arrival/start
-		else:
-			count -= 1  # decrement on departure/end
-		# maintain maximum
-		prev_count = max_count
-		max_count = max(count, max_count)
-		# maintain earlier time max is reached
-		if max_count > prev_count:
-			max_time = time[0]
-	return max_count, max_time
+class NEMOPolicy:
+    def check_to_enable_tool(self, tool: Tool, operator: User, user: User, project: Project, staff_charge: bool):
+        """
+        Check that the user is allowed to enable the tool. Enable the tool if the policy checks pass.
+        """
+        facility_name = ApplicationCustomization.get("facility_name")
+
+        # The tool must be visible (or the parent if it's a child tool) to users.
+        visible = tool.parent_tool.visible if tool.is_child_tool() else tool.visible
+        if not visible:
+            return HttpResponseBadRequest("This tool is currently hidden from users.")
+
+        # The tool must be operational.
+        # If the tool is non-operational then it may only be accessed by staff members or service personnel.
+        if not tool.operational and not operator.is_staff and not operator.is_service_personnel:
+            return HttpResponseBadRequest("This tool is currently non-operational.")
+
+        # The tool must not be in use.
+        current_usage_event = tool.get_current_usage_event()
+        if current_usage_event:
+            return HttpResponseBadRequest("The tool is currently being used by " + str(current_usage_event.user) + ".")
+
+        # The user must be qualified to use the tool itself, or the parent tool in case of alternate tool.
+        tool_to_check_qualifications = tool.parent_tool if tool.is_child_tool() else tool
+        if tool_to_check_qualifications not in operator.qualifications.all() and not operator.is_staff:
+            return HttpResponseBadRequest("You are not qualified to use this tool.")
+
+        # Only staff members can operate a tool on behalf of another user.
+        if (user and operator.pk != user.pk) and not operator.is_staff:
+            return HttpResponseBadRequest("You must be a staff member to use a tool on another user's behalf.")
+
+        # All required resources must be available to operate a tool except for staff or service personnel.
+        unavailable_rss = tool.required_resource_set.filter(available=False).exists()
+        if unavailable_rss and not operator.is_staff and not operator.is_service_personnel:
+            return HttpResponseBadRequest("A resource that is required to operate this tool is unavailable.")
+
+        # The tool operator may not activate tools in a particular area unless they are logged in to the area.
+        # Staff are exempt from this rule.
+        area_for_tool = tool.requires_area_access
+        operator_logged_in = AreaAccessRecord.objects.filter(
+            area=area_for_tool, customer=operator, staff_charge=None, end=None
+        ).exists()
+        if area_for_tool and not operator_logged_in and not operator.is_staff:
+            abuse_email_address = EmailsCustomization.get("abuse_email_address")
+            message = get_media_file_contents("unauthorized_tool_access_email.html")
+            if abuse_email_address and message:
+                dictionary = {"operator": operator, "tool": tool, "type": "access"}
+                rendered_message = render_email_template(message, dictionary)
+                send_mail(
+                    subject="Area access requirement",
+                    content=rendered_message,
+                    from_email=abuse_email_address,
+                    to=[abuse_email_address],
+                    email_category=EmailCategory.ABUSE,
+                )
+            return HttpResponseBadRequest(
+                "You must be logged in to the {} to operate this tool.".format(tool.requires_area_access.name)
+            )
+
+        # The tool operator may not activate tools in a particular area,
+        # unless they are still within that area reservation window.
+        # Staff and service personnel are exempt from this rule.
+        if not operator.is_staff and not operator.is_service_personnel and tool.requires_area_reservation():
+            if not tool.requires_area_access.get_current_reservation_for_user(operator):
+                abuse_email_address = EmailsCustomization.get("abuse_email_address")
+                message = get_media_file_contents("unauthorized_tool_access_email.html")
+                if abuse_email_address and message:
+                    dictionary = {
+                        "operator": operator,
+                        "tool": tool,
+                        "type": "reservation",
+                    }
+                    rendered_message = render_email_template(message, dictionary)
+                    send_mail(
+                        subject="Area reservation requirement",
+                        content=rendered_message,
+                        from_email=abuse_email_address,
+                        to=[abuse_email_address],
+                        email_category=EmailCategory.ABUSE,
+                    )
+                return HttpResponseBadRequest(
+                    "You must have a current reservation for the {} to operate this tool.".format(
+                        tool.requires_area_access.name
+                    )
+                )
+
+        # Staff may only charge staff time for one user at a time.
+        if staff_charge and operator.charging_staff_time():
+            return HttpResponseBadRequest(
+                "You are already charging staff time. You must end the current staff charge before you being another."
+            )
+
+        # Staff may not bill staff time to themselves.
+        if staff_charge and operator == user:
+            return HttpResponseBadRequest("You cannot charge staff time to yourself.")
+
+        # Check if we are allowed to bill to project
+        try:
+            self.check_billing_to_project(project, user, tool)
+        except ProjectChargeException as e:
+            return HttpResponseBadRequest(e.msg)
+
+        # The tool operator must not have a lock on usage
+        if operator.training_required:
+            return HttpResponseBadRequest(
+                f"You are blocked from using all tools in the {facility_name}. Please complete the {facility_name} rules tutorial in order to use tools."
+            )
+
+        # Users may only use a tool when delayed logoff is not in effect.
+        # Staff and service personnel are exempt from this rule.
+        if tool.delayed_logoff_in_progress() and not operator.is_staff and not operator.is_service_personnel:
+            return HttpResponseBadRequest(
+                "Delayed tool logoff is in effect. You must wait for the delayed logoff to expire before you can use the tool."
+            )
+
+        # Users may not enable a tool during a scheduled outage. Staff and service personnel are exempt from this rule.
+        if tool.scheduled_outage_in_progress() and not operator.is_staff and not operator.is_service_personnel:
+            return HttpResponseBadRequest(
+                "A scheduled outage is in effect. You must wait for the outage to end before you can use the tool."
+            )
+
+        return HttpResponse()
+
+    def check_to_disable_tool(self, tool, operator, downtime) -> HttpResponse:
+        """Check that the user is allowed to disable the tool."""
+        current_usage_event = tool.get_current_usage_event()
+        if (
+            current_usage_event.operator != operator
+            and current_usage_event.user != operator
+            and not (operator.is_staff or operator.is_user_office)
+        ):
+            return HttpResponseBadRequest(
+                "You may not disable a tool while another user is using it unless you are a staff member."
+            )
+        if downtime < timedelta():
+            return HttpResponseBadRequest("Downtime cannot be negative.")
+        if downtime > timedelta(minutes=120):
+            return HttpResponseBadRequest("Post-usage tool downtime may not exceed 120 minutes.")
+        if tool.delayed_logoff_in_progress() and downtime > timedelta():
+            return HttpResponseBadRequest(
+                "The tool is already in a delayed-logoff state. You may not issue additional delayed logoffs until the existing one expires."
+            )
+        if not tool.allow_delayed_logoff and downtime > timedelta():
+            return HttpResponseBadRequest("Delayed logoff is not allowed for this tool.")
+        return HttpResponse()
+
+    def check_to_save_reservation(
+        self,
+        cancelled_reservation: Optional[Reservation],
+        new_reservation: Reservation,
+        user_creating_reservation: User,
+        explicit_policy_override: bool,
+    ) -> (List[str], bool):
+        """
+        Check the reservation creation policy and return a list of policy problems if any.
+        """
+        user = new_reservation.user
+
+        facility_name = ApplicationCustomization.get("facility_name")
+
+        # The function will check all policies. Policy problems are placed in the policy_problems list.
+        # Overridable is True if the policy problems can be overridden by a staff member.
+        policy_problems = []
+        overridable = False
+
+        item_type = new_reservation.reservation_item_type
+
+        # Reservations may not have a start time that is earlier than the end time.
+        if new_reservation.start >= new_reservation.end:
+            policy_problems.append(
+                "Reservation start time ("
+                + format_datetime(new_reservation.start)
+                + ") must be before the end time ("
+                + format_datetime(new_reservation.end)
+                + ")."
+            )
+
+        self.check_coincident_item_reservation_policy(
+            cancelled_reservation, new_reservation, user_creating_reservation, policy_problems
+        )
+
+        # Reservations that have been cancelled may not be changed.
+        if new_reservation.cancelled:
+            policy_problems.append(
+                "This reservation has already been cancelled by "
+                + str(new_reservation.cancelled_by)
+                + " at "
+                + format_datetime(new_reservation.cancellation_time)
+                + "."
+            )
+
+        # The user must belong to at least one active project to make a reservation.
+        if user.active_project_count() < 1:
+            if user == user_creating_reservation:
+                policy_problems.append(
+                    "You do not belong to any active projects. Thus, you may not create any reservations."
+                )
+            else:
+                policy_problems.append(
+                    str(user) + " does not belong to any active projects and cannot have reservations."
+                )
+
+        # Check if we are allowed to bill to project
+        try:
+            self.check_billing_to_project(new_reservation.project, user, new_reservation.reservation_item)
+        except ProjectChargeException as e:
+            policy_problems.append(e.msg)
+
+        # If the user is a staff member or there's an explicit policy override then the policy check is finished.
+        if user.is_staff or explicit_policy_override:
+            return policy_problems, overridable
+
+        # If there are no blocking policy conflicts at this point, the rest of the policies can be overridden.
+        if not policy_problems:
+            overridable = True
+
+        # Some tool reservations require a prior area reservation
+        # Staff may break this rule.
+        # An explicit policy override allows this rule to be broken.
+        if item_type == ReservationItemType.TOOL:
+            if new_reservation.tool.requires_area_reservation():
+                area: Area = new_reservation.tool.requires_area_access
+                # Check that a reservation for the area has been made and contains the start time
+                if not Reservation.objects.filter(
+                    missed=False,
+                    cancelled=False,
+                    shortened=False,
+                    user=user,
+                    area=area,
+                    start__lte=new_reservation.start,
+                    end__gt=new_reservation.start,
+                ).exists():
+                    if user == user_creating_reservation:
+                        policy_problems.append(
+                            f"This tool requires a {area} reservation. Please make a reservation in the {area} prior to reserving this tool."
+                        )
+                    else:
+                        policy_problems.append(
+                            f"This tool requires a {area} reservation. Please make sure to also create a reservation in the {area} or {str(user)} will not be able to enter the area."
+                        )
+
+        # The user must complete training to create reservations.
+        # Staff may break this rule.
+        # An explicit policy override allows this rule to be broken.
+        if user.training_required:
+            if user == user_creating_reservation:
+                policy_problems.append(
+                    f"You are blocked from making reservations in the {facility_name}. Please complete the {facility_name} rules tutorial in order to create new reservations."
+                )
+            else:
+                policy_problems.append(
+                    f"{str(user)} is blocked from making reservations in the {facility_name}. The user needs to complete the {facility_name} rules tutorial in order to create new reservations."
+                )
+
+        # Users may only change their own reservations.
+        # Staff may break this rule.
+        # An explicit policy override allows this rule to be broken.
+        if cancelled_reservation and user != user_creating_reservation:
+            policy_problems.append("You may not change reservations that you do not own.")
+
+        # The user may not create or move a reservation to have a start time that is earlier than the current time.
+        # Unless it's an extension of an area reservation, in which case the start time is the same.
+        # Staff may break this rule.
+        # An explicit policy override allows this rule to be broken.
+        extension_of_area_reservation = (
+            new_reservation.area and cancelled_reservation and cancelled_reservation.start == new_reservation.start
+        )
+        if not extension_of_area_reservation and new_reservation.start < timezone.now():
+            policy_problems.append(
+                "Reservation start time ("
+                + format_datetime(new_reservation.start)
+                + ") is earlier than the current time ("
+                + format_datetime()
+                + ")."
+            )
+
+        # The user may not move or resize a reservation to have an end time that is earlier than the current time.
+        # Staff may break this rule.
+        # An explicit policy override allows this rule to be broken.
+        if new_reservation.end < timezone.now():
+            policy_problems.append(
+                "Reservation end time ("
+                + format_datetime(new_reservation.end)
+                + ") is earlier than the current time ("
+                + format_datetime()
+                + ")."
+            )
+
+        # The user must be qualified on the tool in question in order to create, move, or resize a reservation.
+        # Staff may break this rule.
+        # An explicit policy override allows this rule to be broken.
+        if new_reservation.tool and new_reservation.tool not in user.qualifications.all():
+            if user == user_creating_reservation:
+                policy_problems.append(
+                    "You are not qualified to use this tool. Creating, moving, and resizing reservations is forbidden."
+                )
+            else:
+                policy_problems.append(
+                    f"{str(user)} is not qualified to use this tool. Creating, moving, and resizing reservations is forbidden."
+                )
+
+        # The user must be authorized on the area in question at the start and end times of the reservation
+        # in order to create, move, or resize a reservation.
+        # Staff may break this rule.
+        # An explicit policy override allows this rule to be broken.
+        if item_type == ReservationItemType.AREA:
+            user_access_levels = user.accessible_access_levels_for_area(new_reservation.area)
+            if not any(
+                [access_level.accessible_at(new_reservation.start) for access_level in user_access_levels]
+            ) or not any([access_level.accessible_at(new_reservation.end) for access_level in user_access_levels]):
+                # it could be inaccessible because of an ongoing closure at the start or end time
+                first_closure_time: ClosureTime = next(
+                    iter(
+                        [
+                            access_level.ongoing_closure_time(new_reservation.start)
+                            for access_level in user_access_levels
+                        ]
+                    ),
+                    None,
+                )
+                if not first_closure_time:
+                    # if there is no closure at start, check at end time
+                    first_closure_time = next(
+                        iter(
+                            [
+                                access_level.ongoing_closure_time(new_reservation.end)
+                                for access_level in user_access_levels
+                            ]
+                        ),
+                        None,
+                    )
+                if first_closure_time:
+                    details = f" due to the following closure: {first_closure_time.closure.name} ({format_daterange(first_closure_time.start_time, first_closure_time.end_time)})"
+                # or simply due to scheduling
+                else:
+                    details = (
+                        f" (times allowed in this area are: {', '.join([access.get_schedule_display_with_times() for access in user_access_levels])})"
+                        if user_access_levels
+                        else ""
+                    )
+                if user == user_creating_reservation:
+                    policy_problems.append(
+                        f"You are not authorized to access this area at this time{details}. Creating, moving, and resizing reservations is forbidden."
+                    )
+                else:
+                    policy_problems.append(
+                        f"{str(user)} is not authorized to access this area at this time{details}. Creating, moving, and resizing reservations is forbidden."
+                    )
+
+        self.check_tool_reservation_requiring_area(
+            policy_problems, user_creating_reservation, cancelled_reservation, new_reservation
+        )
+
+        # The reservation start time may not exceed the item's reservation horizon.
+        # Staff may break this rule.
+        # An explicit policy override allows this rule to be broken.
+        item = new_reservation.reservation_item
+        if item.reservation_horizon is not None:
+            reservation_horizon = timedelta(days=item.reservation_horizon)
+            if new_reservation.start > timezone.now() + reservation_horizon:
+                policy_problems.append(
+                    "You may not create reservations further than "
+                    + str(reservation_horizon.days)
+                    + f" days from now for this {item_type.value}."
+                )
+
+        # Check item policy rules
+        item_policy_problems = []
+        if self.should_enforce_reservation_policy(new_reservation):
+            item_policy_problems = self.check_reservation_policy_for_item(
+                user_creating_reservation, new_reservation, cancelled_reservation
+            )
+
+        # Return the list of all policies that are not met.
+        return policy_problems + item_policy_problems, overridable
+
+    def check_tool_reservation_requiring_area(
+        self,
+        policy_problems: List[str],
+        user_creating_reservation: User,
+        cancelled_reservation: Optional[Reservation],
+        new_reservation: Optional[Reservation],
+    ):
+        # When modifying an area reservation, check that all tools reservations
+        # starting during the cancelled one are still within the new one
+        if cancelled_reservation and cancelled_reservation.reservation_item_type == ReservationItemType.AREA:
+            tools_requiring_cancelled_reservation = Reservation.objects.filter(
+                cancelled=False,
+                missed=False,
+                shortened=False,
+                tool__isnull=False,
+                tool___requires_area_access=cancelled_reservation.area,
+                user=cancelled_reservation.user,
+            )
+            tools_requiring_cancelled_reservation = tools_requiring_cancelled_reservation.filter(
+                start__gte=cancelled_reservation.start, start__lt=cancelled_reservation.end
+            )
+            if tools_requiring_cancelled_reservation.exists():
+                if new_reservation:
+                    tools_requiring_new_reservation = Reservation.objects.filter(
+                        cancelled=False,
+                        missed=False,
+                        shortened=False,
+                        tool__isnull=False,
+                        tool___requires_area_access=new_reservation.area,
+                        user=new_reservation.user,
+                    )
+                    tools_requiring_new_reservation = tools_requiring_new_reservation.filter(
+                        start__gte=new_reservation.start, start__lt=new_reservation.end
+                    )
+                else:
+                    tools_requiring_new_reservation = Reservation.objects.none()
+                difference: List[Reservation] = [
+                    item
+                    for item in tools_requiring_cancelled_reservation
+                    if item not in tools_requiring_new_reservation
+                ]
+                # As long as the new reservation includes the same tool reservations, we are good
+                if difference:
+                    user = cancelled_reservation.user
+                    area = new_reservation.area if new_reservation else cancelled_reservation.area
+                    difference.sort(key=lambda x: x.start)
+                    if user == user_creating_reservation:
+                        policy_problems.append(
+                            f"You have a reservation for the {difference[0].tool} at {format_datetime(difference[0].start)} that requires a {area} reservation. Cancel or reschedule the tool reservation first and try again."
+                        )
+                    else:
+                        policy_problems.append(
+                            f"{str(user)} has a reservation for the {difference[0].tool} at {format_datetime(difference[0].start)} that requires a {area} reservation. Cancel or reschedule the tool reservation first and try again."
+                        )
+
+    def check_coincident_item_reservation_policy(
+        self,
+        cancelled_reservation: Optional[Reservation],
+        new_reservation: Reservation,
+        user_creating_reservation: User,
+        policy_problems: List,
+    ):
+        user = new_reservation.user
+
+        # For tools the user may not create, move, or resize a reservation to coincide with another user's reservation.
+        # For areas, it cannot coincide with another reservation for the same user, or with a number of other users greater than the area capacity
+        coincident_events = Reservation.objects.filter(cancelled=False, missed=False, shortened=False)
+        # Exclude the reservation we're cancelling in order to create a new one:
+        if cancelled_reservation and cancelled_reservation.id:
+            coincident_events = coincident_events.exclude(id=cancelled_reservation.id)
+        # Exclude events for which the following is true:
+        # The event starts and ends before the time-window, and...
+        # The event starts and ends after the time-window.
+        coincident_events = coincident_events.exclude(start__lt=new_reservation.start, end__lte=new_reservation.start)
+        coincident_events = coincident_events.exclude(start__gte=new_reservation.end, end__gt=new_reservation.end)
+        if (
+            new_reservation.reservation_item_type == ReservationItemType.TOOL
+            and coincident_events.filter(**new_reservation.reservation_item_filter).count() > 0
+        ):
+            policy_problems.append(
+                "Your reservation coincides with another reservation that already exists. Please choose a different time."
+            )
+        if new_reservation.reservation_item_type == ReservationItemType.AREA:
+            if coincident_events.filter(**new_reservation.reservation_item_filter).filter(user=user).count() > 0:
+                if user == user_creating_reservation:
+                    policy_problems.append(
+                        "You already have a reservation that coincides with this one. Please choose a different time."
+                    )
+                else:
+                    policy_problems.append(
+                        f"{str(user)} already has a reservation that coincides with this one. Please choose a different time."
+                    )
+            for area in new_reservation.area.get_ancestors(ascending=True, include_self=True):
+                # Check reservations for all other children of the parent areas
+                if not area.count_staff_in_occupancy:
+                    coincident_events = coincident_events.filter(user__is_staff=False)
+                if not area.count_service_personnel_in_occupancy:
+                    coincident_events = coincident_events.filter(user__is_service_personnel=False)
+                apply_to_user = (
+                    (not user.is_staff and not user.is_service_personnel)
+                    or (user.is_staff and area.count_staff_in_occupancy)
+                    or (user.is_service_personnel and area.count_service_personnel_in_occupancy)
+                )
+                if apply_to_user and area.maximum_capacity:
+                    children_events = coincident_events.filter(
+                        area_id__in=[area.id for area in area.get_descendants(include_self=True)]
+                    )
+                    reservations = list(children_events)
+                    reservations.append(new_reservation)
+                    # Check only distinct users since the same user could make reservations in different rooms
+                    maximum_users, time = self.check_maximum_users_in_overlapping_reservations(reservations)
+                    if maximum_users > area.maximum_capacity:
+                        time_display = "at this time" if time is None else "at " + format_datetime(time, "TIME_FORMAT")
+                        policy_problems.append(
+                            f"The {area} would be over its maximum capacity {time_display}. Please choose a different time."
+                        )
+
+        # The user may not create, move, or resize a reservation to coincide with a scheduled outage.
+        if new_reservation.reservation_item_type == ReservationItemType.TOOL:
+            coincident_events = ScheduledOutage.objects.filter(
+                Q(tool=new_reservation.tool) | Q(resource__fully_dependent_tools__in=[new_reservation.tool])
+            )
+        elif new_reservation.reservation_item_type == ReservationItemType.AREA:
+            coincident_events = new_reservation.area.scheduled_outage_queryset()
+        else:
+            coincident_events = ScheduledOutage.objects.none()
+        # Exclude events for which the following is true:
+        # The event starts and ends before the time-window, and...
+        # The event starts and ends after the time-window.
+        coincident_events = coincident_events.exclude(start__lt=new_reservation.start, end__lte=new_reservation.start)
+        coincident_events = coincident_events.exclude(start__gte=new_reservation.end, end__gt=new_reservation.end)
+        if coincident_events.count() > 0:
+            policy_problems.append(
+                "Your reservation coincides with a scheduled outage. Please choose a different time."
+            )
+
+    def should_enforce_reservation_policy(self, reservation: Reservation) -> bool:
+        """Returns whether the policy rules should be enforced."""
+        should_enforce = True
+
+        item = reservation.reservation_item
+        start_time = timezone.localtime(reservation.start)
+        end_time = timezone.localtime(reservation.end)
+        if item.policy_off_weekend and start_time.weekday() >= 5 and end_time.weekday() >= 5:
+            should_enforce = False
+        if item.policy_off_between_times and item.policy_off_start_time and item.policy_off_end_time:
+            if item.policy_off_start_time <= item.policy_off_end_time:
+                """Range is similar to 6am-6pm"""
+                if (
+                    item.policy_off_start_time <= start_time.time() <= item.policy_off_end_time
+                    and item.policy_off_start_time <= end_time.time() <= item.policy_off_end_time
+                ):
+                    should_enforce = False
+            else:
+                """Range is similar to 6pm-6am"""
+                if (
+                    item.policy_off_start_time <= start_time.time() or start_time.time() <= item.policy_off_end_time
+                ) and (item.policy_off_start_time <= end_time.time() or end_time.time() <= item.policy_off_end_time):
+                    should_enforce = False
+        return should_enforce
+
+    def check_reservation_policy_for_item(
+        self,
+        user_creating_reservation: User,
+        new_reservation: Reservation,
+        cancelled_reservation: Optional[Reservation],
+    ) -> List[str]:
+        item_policy_problems = []
+        # Calculate the duration of the reservation:
+        duration = new_reservation.end - new_reservation.start
+
+        # The reservation must be at least as long as the minimum block time for this item.
+        # Staff may break this rule.
+        # An explicit policy override allows this rule to be broken.
+        item = new_reservation.reservation_item
+        item_type = new_reservation.reservation_item_type
+        if item.minimum_usage_block_time:
+            minimum_block_time = timedelta(minutes=item.minimum_usage_block_time)
+            if duration < minimum_block_time:
+                item_policy_problems.append(
+                    f"Your reservation has a duration of {str(int(duration.total_seconds() / 60))} minutes. This {item_type.value} requires a minimum reservation duration of {str(int(minimum_block_time.total_seconds() / 60))} minutes."
+                )
+
+        # The reservation may not exceed the maximum block time for this tool.
+        # Staff may break this rule.
+        # An explicit policy override allows this rule to be broken.
+        if item.maximum_usage_block_time:
+            maximum_block_time = timedelta(minutes=item.maximum_usage_block_time)
+            if duration > maximum_block_time:
+                item_policy_problems.append(
+                    f"Your reservation has a duration of {str(int(duration.total_seconds() / 60))} minutes. Reservations for this {item_type.value} may not exceed {str(int(maximum_block_time.total_seconds() / 60))} minutes."
+                )
+
+        user = new_reservation.user
+
+        # If there is a limit on number of reservations per user per day then verify that the user has not exceeded it.
+        # Staff may break this rule.
+        # An explicit policy override allows this rule to be broken.
+        if item.maximum_reservations_per_day:
+            start_of_day = new_reservation.start
+            start_of_day = start_of_day.replace(hour=0, minute=0, second=0, microsecond=0)
+            end_of_day = start_of_day + timedelta(days=1)
+            reservations_for_that_day = Reservation.objects.filter(
+                cancelled=False, shortened=False, start__gte=start_of_day, end__lte=end_of_day, user=user
+            )
+            reservations_for_that_day = reservations_for_that_day.filter(**new_reservation.reservation_item_filter)
+            # Exclude any reservation that is being cancelled.
+            if cancelled_reservation and cancelled_reservation.id:
+                reservations_for_that_day = reservations_for_that_day.exclude(id=cancelled_reservation.id)
+            if reservations_for_that_day.count() >= item.maximum_reservations_per_day:
+                if user == user_creating_reservation:
+                    item_policy_problems.append(
+                        f"You may only have {str(item.maximum_reservations_per_day)} reservations for this {item_type.value} per day. Missed reservations are included when counting the number of reservations per day."
+                    )
+                else:
+                    item_policy_problems.append(
+                        f"{str(user)} may only have {str(item.maximum_reservations_per_day)} reservations for this {item_type.value} per day. Missed reservations are included when counting the number of reservations per day."
+                    )
+
+        # A minimum amount of time between reservations for the same user & same tool can be enforced.
+        # Staff may break this rule.
+        # An explicit policy override allows this rule to be broken.
+        if item.minimum_time_between_reservations:
+            buffer_time = timedelta(minutes=item.minimum_time_between_reservations)
+            must_end_before = new_reservation.start - buffer_time
+            too_close = Reservation.objects.filter(
+                cancelled=False, shortened=False, user=user, end__gt=must_end_before, start__lt=new_reservation.start
+            )
+            too_close = too_close.filter(**new_reservation.reservation_item_filter)
+            if cancelled_reservation and cancelled_reservation.id:
+                too_close = too_close.exclude(id=cancelled_reservation.id)
+            if too_close.exists():
+                if user == user_creating_reservation:
+                    item_policy_problems.append(
+                        f"Separate reservations for this {item_type.value} that belong to you must be at least {str(item.minimum_time_between_reservations)} minutes apart from each other. The proposed reservation ends too close to another reservation."
+                    )
+                else:
+                    item_policy_problems.append(
+                        f"Separate reservations for this {item_type.value} that belong to {str(user)} must be at least {str(item.minimum_time_between_reservations)} minutes apart from each other. The proposed reservation ends too close to another reservation."
+                    )
+            must_start_after = new_reservation.end + buffer_time
+            too_close = Reservation.objects.filter(
+                cancelled=False, shortened=False, user=user, start__lt=must_start_after, end__gt=new_reservation.start
+            )
+            too_close = too_close.filter(**new_reservation.reservation_item_filter)
+            if cancelled_reservation and cancelled_reservation.id:
+                too_close = too_close.exclude(id=cancelled_reservation.id)
+            if too_close.exists():
+                if user == user_creating_reservation:
+                    item_policy_problems.append(
+                        f"Separate reservations for this {item_type.value} that belong to you must be at least {str(item.minimum_time_between_reservations)} minutes apart from each other. The proposed reservation begins too close to another reservation."
+                    )
+                else:
+                    item_policy_problems.append(
+                        f"Separate reservations for this {item_type.value} that belong to {str(user)} must be at least {str(item.minimum_time_between_reservations)} minutes apart from each other. The proposed reservation begins too close to another reservation."
+                    )
+
+        # Check that the user is not exceeding the maximum amount of time they may reserve in the future.
+        # Staff may break this rule.
+        # An explicit policy override allows this rule to be broken.
+        if item.maximum_future_reservation_time:
+            reservations_after_now = Reservation.objects.filter(cancelled=False, user=user, start__gte=timezone.now())
+            reservations_after_now = reservations_after_now.filter(**new_reservation.reservation_item_filter)
+            if cancelled_reservation and cancelled_reservation.id:
+                reservations_after_now = reservations_after_now.exclude(id=cancelled_reservation.id)
+            amount_reserved_in_the_future = new_reservation.duration()
+            for r in reservations_after_now:
+                amount_reserved_in_the_future += r.duration()
+            if amount_reserved_in_the_future.total_seconds() / 60 > item.maximum_future_reservation_time:
+                if user == user_creating_reservation:
+                    item_policy_problems.append(
+                        f"You may only reserve up to {str(item.maximum_future_reservation_time)} minutes of time on this {item_type.value}, starting from the current time onward."
+                    )
+                else:
+                    item_policy_problems.append(
+                        f"{str(user)} may only reserve up to {str(item.maximum_future_reservation_time)} minutes of time on this {item_type.value}, starting from the current time onward."
+                    )
+
+        return item_policy_problems
+
+    def check_to_cancel_reservation(
+        self,
+        user_cancelling_reservation: User,
+        reservation_to_cancel: Reservation,
+        new_reservation: Optional[Reservation] = None,
+    ) -> HttpResponse:
+        """
+        Checks the reservation deletion policy.
+        If all checks pass the function returns an HTTP "OK" response.
+        Otherwise, the function returns an HTTP "Bad Request" with an error message.
+        """
+
+        move = new_reservation and new_reservation.start != reservation_to_cancel.start
+        resize = new_reservation and new_reservation.start == reservation_to_cancel.start
+        action = "move" if move else "resize" if resize else "cancel"
+
+        # Users may only cancel reservations that they own.
+        # Staff may break this rule.
+        if (reservation_to_cancel.user != user_cancelling_reservation) and not user_cancelling_reservation.is_staff:
+            return HttpResponseBadRequest(f"You may not {action} reservations that you do not own.")
+
+        # Users may not cancel reservations that have already ended.
+        # Staff may break this rule.
+        if reservation_to_cancel.end < timezone.now() and not user_cancelling_reservation.is_staff:
+            return HttpResponseBadRequest(f"You may not {action} reservations that have already ended.")
+
+        # Users may not cancel ongoing area reservations when they are currently logged
+        # in that area (unless they are extending it)
+        # Staff may break this rule.
+        if (
+            reservation_to_cancel.area
+            and reservation_to_cancel.area.requires_reservation
+            and not resize
+            and reservation_to_cancel.start < timezone.now() < reservation_to_cancel.end
+            and AreaAccessRecord.objects.filter(
+                end=None, staff_charge=None, customer=reservation_to_cancel.user, area=reservation_to_cancel.area
+            )
+            and not user_cancelling_reservation.is_staff
+        ):
+            if move:
+                return HttpResponseBadRequest("You may only resize an area reservation while logged in that area.")
+            else:
+                return HttpResponseBadRequest("You may not cancel an area reservation while logged in that area.")
+
+        if reservation_to_cancel.cancelled:
+            return HttpResponseBadRequest(
+                "This reservation has already been cancelled by "
+                + str(reservation_to_cancel.cancelled_by)
+                + " on "
+                + format_datetime(reservation_to_cancel.cancellation_time)
+                + "."
+            )
+
+        if reservation_to_cancel.missed:
+            return HttpResponseBadRequest("This reservation was missed and cannot be modified.")
+
+        return HttpResponse()
+
+    def check_to_create_outage(self, outage: ScheduledOutage) -> Optional[str]:
+        # Outages may not have a start time that is earlier than the end time.
+        if outage.start >= outage.end:
+            return (
+                "Outage start time ("
+                + format_datetime(outage.start)
+                + ") must be before the end time ("
+                + format_datetime(outage.end)
+                + ")."
+            )
+
+        # The user may not create, move, or resize an outage to coincide with another user's reservation.
+        coincident_events = Reservation.objects.filter(**outage.outage_item_filter).filter(
+            cancelled=False, missed=False, shortened=False
+        )
+        # Exclude events for which the following is true:
+        # The event starts and ends before the time-window, and...
+        # The event starts and ends after the time-window.
+        coincident_events = coincident_events.exclude(start__lt=outage.start, end__lte=outage.start)
+        coincident_events = coincident_events.exclude(start__gte=outage.end, end__gt=outage.end)
+        if coincident_events.count() > 0:
+            return "Your scheduled outage coincides with a reservation that already exists. Please choose a different time."
+
+        # No policy issues! The outage can be created...
+        return None
+
+    def check_to_enter_any_area(self, user: User):
+        """
+        Checks the area access policy for a user.
+        """
+        if not user.is_active:
+            raise InactiveUserError(user=user)
+
+        if user.active_project_count() < 1:
+            raise NoActiveProjectsForUserError(user=user)
+
+        if user.access_expiration is not None and user.access_expiration < date.today():
+            raise PhysicalAccessExpiredUserError(user=user)
+
+        user_has_access_to_at_least_one_area = user.accessible_access_levels().exists()
+        if not user_has_access_to_at_least_one_area:
+            raise NoPhysicalAccessUserError(user=user)
+
+    def check_to_enter_area(self, area: Area, user: User):
+        # If explicitly set on the Physical Access Level, staff & user office
+        # are exempt from being granted explicit access
+        if (user.is_staff or user.is_user_office) and any(
+            [
+                access_level.accessible()
+                for access_level in PhysicalAccessLevel.objects.filter(allow_staff_access=True, area=area)
+            ]
+        ):
+            pass
+        else:
+            # Check if the user normally has access to this area door at the current time (or access to any parent)
+            if not any([access_level.accessible() for access_level in user.accessible_access_levels_for_area(area)]):
+                first_closure_time = next(
+                    iter(
+                        [
+                            access_level.ongoing_closure_time()
+                            for access_level in user.accessible_access_levels_for_area(area)
+                        ]
+                    ),
+                    None,
+                )
+                raise NoAccessiblePhysicalAccessUserError(user=user, area=area, closure_time=first_closure_time)
+
+        if not user.is_staff and not user.is_service_personnel:
+            for a in area.get_ancestors(ascending=True, include_self=True):
+                unavailable_resources = a.required_resources.filter(available=False)
+                if unavailable_resources:
+                    raise UnavailableResourcesUserError(user=user, area=a, resources=unavailable_resources)
+
+            # Non staff users may not enter an area during a scheduled outage.
+            if area.scheduled_outage_in_progress():
+                raise ScheduledOutageInProgressError(user=user, area=area)
+
+            # If we reached maximum capacity, fail (only for non staff users)
+            for a in area.get_ancestors(ascending=True, include_self=True):
+                if a.maximum_capacity and 0 < a.maximum_capacity <= a.occupancy_count():
+                    raise MaximumCapacityReachedError(user=user, area=a)
+
+            if area.requires_reservation and not area.get_current_reservation_for_user(user):
+                raise ReservationRequiredUserError(user=user, area=area)
+
+    def check_billing_to_project(
+        self, project: Project, user: User, item: Union[Tool, Area, Consumable, StaffCharge] = None
+    ):
+        if project:
+            if project not in user.active_projects():
+                raise NotAllowedToChargeProjectException(project=project, user=user)
+
+            if item:
+                # Check if project only allows billing for certain tools
+                allowed_tools = project.only_allow_tools.all()
+                if allowed_tools.exists():
+                    if isinstance(item, Tool) and item not in allowed_tools:
+                        msg = f"{item.name} is not allowed for project {project.name}"
+                        raise ItemNotAllowedForProjectException(project, user, item.name, msg)
+                    elif isinstance(item, Area) and item.id not in distinct_qs_value_list(
+                        allowed_tools, "_requires_area_access_id"
+                    ):
+                        msg = f"{item.name} is not allowed for project {project.name}"
+                        raise ItemNotAllowedForProjectException(project, user, item.name, msg)
+                # Check if consumable withdrawals are allowed
+                if isinstance(item, Consumable):
+                    if not project.allow_consumable_withdrawals:
+                        msg = f"Consumable withdrawals are not allowed for project {project.name}"
+                        raise ItemNotAllowedForProjectException(project, user, "Staff Charges", msg)
+
+    def check_maximum_users_in_overlapping_reservations(self, reservations: List[Reservation]) -> (int, datetime):
+        """
+        Returns the maximum number of overlapping reservations and the earlier time the maximum is reached
+        This will only count reservations made by different users. i.e. if a user has 3 reservations at the same
+        time for different tools/areas, it will only count as one.
+        """
+        # First we need to merge reservations by user, since one user could have more than one at the same time.
+        # (and we should only count it as one)
+        intervals_by_user = defaultdict(list)
+        for r in reservations:
+            intervals_by_user[r.user.id].append((r.start, r.end))
+
+        merged_intervals = []
+        for user, intervals in intervals_by_user.items():
+            merged_intervals.extend(recursive_merge(sorted(intervals).copy()))
+
+        # Now let's count the maximum overlapping reservations
+        times = []
+        for interval in merged_intervals:
+            start_time, end_time = interval[0], interval[1]
+            times.append((start_time, "start"))
+            times.append((end_time, "end"))
+        times = sorted(times)
+
+        count = 0
+        max_count = 0
+        max_time: Optional[datetime] = None
+        for time in times:
+            if time[1] == "start":
+                count += 1  # increment on arrival/start
+            else:
+                count -= 1  # decrement on departure/end
+            # maintain maximum
+            prev_count = max_count
+            max_count = max(count, max_count)
+            # maintain earlier time max is reached
+            if max_count > prev_count:
+                max_time = time[0]
+        return max_count, max_time
 
 
 def recursive_merge(intervals: List[tuple], start_index=0) -> List[tuple]:
-	for i in range(start_index, len(intervals) - 1):
-		if intervals[i][1] > intervals[i + 1][0]:
-			new_start = intervals[i][0]
-			new_end = intervals[i + 1][1]
-			intervals[i] = (new_start, new_end)
-			del intervals[i + 1]
-			return recursive_merge(intervals.copy(), start_index=i)
-	return intervals
+    for i in range(start_index, len(intervals) - 1):
+        if intervals[i][1] > intervals[i + 1][0]:
+            new_start = intervals[i][0]
+            new_end = intervals[i + 1][1]
+            intervals[i] = (new_start, new_end)
+            del intervals[i + 1]
+            return recursive_merge(intervals.copy(), start_index=i)
+    return intervals
+
+
+policy_class: NEMOPolicy = get_class_from_settings("NEMO_POLICY_CLASS", "NEMO.policy.NEMOPolicy")
```

### Comparing `NEMO-4.4.1/NEMO/views/qualifications.py` & `NEMO-4.5.0/NEMO/views/qualifications.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,49 +4,73 @@
 from django.conf import settings
 from django.contrib import messages
 from django.http import HttpResponse, HttpResponseBadRequest
 from django.shortcuts import get_object_or_404, redirect, render
 from django.views.decorators.http import require_GET, require_POST
 
 from NEMO.decorators import staff_member_required
-from NEMO.models import MembershipHistory, Tool, User
+from NEMO.models import MembershipHistory, Tool, ToolQualificationGroup, User
 from NEMO.views.users import get_identity_service
 
 
 @staff_member_required
 @require_GET
 def qualifications(request):
-	""" Present a web page to allow staff to qualify or disqualify users on particular tools. """
+	"""Present a web page to allow staff to qualify or disqualify users on particular tools."""
 	users = User.objects.filter(is_active=True)
 	tools = Tool.objects.filter(visible=True)
-	return render(request, 'qualifications.html', {'users': users, 'tools': tools})
+	tool_groups = ToolQualificationGroup.objects.all()
+	return render(
+		request, "qualifications.html", {"users": users, "tools": list(tools), "tool_groups": list(tool_groups)}
+	)
 
 
 @staff_member_required
 @require_POST
 def modify_qualifications(request):
-	""" Change the tools that a set of users is qualified to use. """
-	action = request.POST.get('action')
-	if action != 'qualify' and action != 'disqualify':
+	"""Change the tools that a set of users is qualified to use."""
+	action = request.POST.get("action")
+	if action != "qualify" and action != "disqualify":
 		return HttpResponseBadRequest("You must specify that you are qualifying or disqualifying users.")
-	users = request.POST.getlist('chosen_user[]') or request.POST.get('chosen_user') or []
+	users = request.POST.getlist("chosen_user[]") or request.POST.get("chosen_user") or []
 	users = User.objects.in_bulk(users)
 	if users == {}:
 		return HttpResponseBadRequest("You must specify at least one user.")
-	tools = request.POST.getlist('chosen_tool[]') or request.POST.get('chosen_tool') or []
+	tools = request.POST.getlist("chosen_tool[]") or request.POST.getlist("chosen_tool") or []
+	tool_groups = (
+		request.POST.getlist("chosen_toolqualificationgroup[]")
+		or request.POST.getlist("chosen_toolqualificationgroup")
+		or []
+	)
+	# Add tools from tool group
+	tools.extend(
+		[
+			tool.id
+			for tool_group in ToolQualificationGroup.objects.filter(id__in=tool_groups)
+			for tool in tool_group.tools.all()
+		]
+	)
 	tools = Tool.objects.in_bulk(tools)
 	if tools == {}:
 		return HttpResponseBadRequest("You must specify at least one tool.")
 
 	for user in users.values():
 		original_qualifications = set(user.qualifications.all())
-		if action == 'qualify':
+		if action == "qualify":
 			user.qualifications.add(*tools)
 			original_physical_access_levels = set(user.physical_access_levels.all())
-			physical_access_level_automatic_enrollment = list(set([t.grant_physical_access_level_upon_qualification for t in tools.values() if t.grant_physical_access_level_upon_qualification]))
+			physical_access_level_automatic_enrollment = list(
+				set(
+					[
+						t.grant_physical_access_level_upon_qualification
+						for t in tools.values()
+						if t.grant_physical_access_level_upon_qualification
+					]
+				)
+			)
 			user.physical_access_levels.add(*physical_access_level_automatic_enrollment)
 			current_physical_access_levels = set(user.physical_access_levels.all())
 			added_physical_access_levels = set(current_physical_access_levels) - set(original_physical_access_levels)
 			for access_level in added_physical_access_levels:
 				entry = MembershipHistory()
 				entry.authorizer = request.user
 				entry.parent_content_object = access_level
@@ -54,21 +78,23 @@
 				entry.action = entry.Action.ADDED
 				entry.save()
 			if get_identity_service().get("available", False):
 				for t in tools:
 					tool = Tool.objects.get(id=t)
 					if tool.grant_badge_reader_access_upon_qualification:
 						parameters = {
-							'username': user.username,
-							'domain': user.domain,
-							'requested_area': tool.grant_badge_reader_access_upon_qualification,
+							"username": user.username,
+							"domain": user.domain,
+							"requested_area": tool.grant_badge_reader_access_upon_qualification,
 						}
-						timeout = settings.IDENTITY_SERVICE.get('timeout', 3)
-						requests.put(urljoin(settings.IDENTITY_SERVICE['url'], '/add/'), data=parameters, timeout=timeout)
-		elif action == 'disqualify':
+						timeout = settings.IDENTITY_SERVICE.get("timeout", 3)
+						requests.put(
+							urljoin(settings.IDENTITY_SERVICE["url"], "/add/"), data=parameters, timeout=timeout
+						)
+		elif action == "disqualify":
 			user.qualifications.remove(*tools)
 		current_qualifications = set(user.qualifications.all())
 		# Record the qualification changes for each tool:
 		added_qualifications = set(current_qualifications) - set(original_qualifications)
 		for tool in added_qualifications:
 			entry = MembershipHistory()
 			entry.authorizer = request.user
@@ -81,25 +107,21 @@
 			entry = MembershipHistory()
 			entry.authorizer = request.user
 			entry.parent_content_object = tool
 			entry.child_content_object = user
 			entry.action = entry.Action.REMOVED
 			entry.save()
 
-	if request.POST.get('redirect') == 'true':
+	if request.POST.get("redirect") == "true":
 		messages.success(request, "Tool qualifications were successfully modified")
 		return redirect("qualifications")
 	else:
 		return HttpResponse()
 
 
 @staff_member_required
 @require_GET
 def get_qualified_users(request):
-	tool = get_object_or_404(Tool, id=request.GET.get('tool_id'))
+	tool = get_object_or_404(Tool, id=request.GET.get("tool_id"))
 	users = User.objects.filter(is_active=True)
-	dictionary = {
-		'tool': tool,
-		'users': users,
-		'expanded': True
-	}
-	return render(request, 'tool_control/qualified_users.html', dictionary)
+	dictionary = {"tool": tool, "users": users, "expanded": True}
+	return render(request, "tool_control/qualified_users.html", dictionary)
```

### Comparing `NEMO-4.4.1/NEMO/views/resources.py` & `NEMO-4.5.0/NEMO/views/resources.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-from datetime import datetime
-
 from django.http import Http404
 from django.shortcuts import get_object_or_404, redirect, render
+from django.utils import timezone
 from django.views.decorators.http import require_GET, require_POST, require_http_methods
 
 from NEMO.decorators import staff_member_required
 from NEMO.forms import ScheduledOutageForm
 from NEMO.models import Resource, ScheduledOutage, ScheduledOutageCategory, Tool, UsageEvent
 
 
@@ -17,15 +16,15 @@
 
 @staff_member_required
 @require_GET
 def resource_details(request, resource_id):
 	resource = get_object_or_404(Resource, id=resource_id)
 	dictionary = {
 		'resource': resource,
-		'outages': ScheduledOutage.objects.filter(resource__id=resource_id, end__gt=datetime.now()),
+		'outages': ScheduledOutage.objects.filter(resource__id=resource_id, end__gt=timezone.now()),
 	}
 	return render(request, 'resources/resource_details.html', dictionary)
 
 
 @staff_member_required
 @require_http_methods(['GET', 'POST'])
 def modify_resource(request, resource_id):
```

### Comparing `NEMO-4.4.1/NEMO/views/safety.py` & `NEMO-4.5.0/NEMO/views/safety.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from django.db.models import Case, When
 from django.shortcuts import get_object_or_404, redirect, render
 from django.urls import reverse
 from django.views.decorators.http import require_GET, require_http_methods
 
 from NEMO.decorators import staff_member_required
 from NEMO.forms import SafetyIssueCreationForm, SafetyIssueUpdateForm
-from NEMO.models import Chemical, ChemicalHazard, SafetyCategory, SafetyIssue, SafetyItem
+from NEMO.models import Chemical, ChemicalHazard, Notification, SafetyCategory, SafetyIssue, SafetyItem
 from NEMO.templatetags.custom_tags_and_filters import navigation_url
 from NEMO.utilities import (
 	BasicDisplayTable,
 	EmailCategory,
 	distinct_qs_value_list,
 	export_format_datetime,
 	get_full_url,
@@ -97,15 +97,15 @@
 @require_http_methods(["GET", "POST"])
 def safety_issues(request):
 	dictionary = safety_dictionary("safety_issues")
 	tickets = SafetyIssue.objects.filter(resolved=False).order_by("-creation_time")
 	if not request.user.is_staff:
 		tickets = tickets.filter(visible=True)
 	dictionary["tickets"] = tickets
-	dictionary["notifications"] = get_notifications(request.user, SafetyIssue)
+	dictionary["notifications"] = get_notifications(request.user, Notification.Types.SAFETY)
 	return render(request, "safety/safety_issues.html", dictionary)
 
 
 @login_required
 @require_http_methods(["GET", "POST"])
 def create_safety_issue(request):
 	dictionary = safety_dictionary("safety_issues")
@@ -154,15 +154,15 @@
 	dictionary = safety_dictionary("safety_issues")
 	if request.method == "POST":
 		ticket = get_object_or_404(SafetyIssue, id=ticket_id)
 		form = SafetyIssueUpdateForm(request.user, data=request.POST, instance=ticket)
 		if form.is_valid():
 			issue = form.save()
 			if issue.resolved:
-				delete_notification(SafetyIssue, issue.id)
+				delete_notification(Notification.Types.SAFETY, issue.id)
 			messages.success(request, "This safety issue was updated successfully")
 			return redirect("safety_issues")
 	dictionary["ticket"] = get_object_or_404(SafetyIssue, id=ticket_id)
 	return render(request, "safety/safety_issues_update.html", dictionary)
 
 
 @login_required
```

### Comparing `NEMO-4.4.1/NEMO/views/sidebar.py` & `NEMO-4.5.0/NEMO/views/sidebar.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/views/status_dashboard.py` & `NEMO-4.5.0/NEMO/views/status_dashboard.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,15 +140,15 @@
 		end_delta = timedelta(weeks=1)
 	end = start + end_delta - timedelta(days=1)
 	# If we are only showing weekdays, we have to subtract 2 days from the end of the week. Only applies to week view
 	if view == "week" and weekdays_only:
 		end = end - timedelta(days=2)
 	# Reset timestamp to be right in the middle of the period
 	timestamp = int((start + timedelta(days=(end - start).days / 2)).timestamp())
-	staffs = StaffAvailability.objects.all()
+	staffs = StaffAvailability.objects.filter(visible=True)
 	staffs.query.add_ordering(F("category__display_order").asc(nulls_last=True))
 	staffs.query.add_ordering(F("staff_member__first_name").asc())
 	days = rrule(DAILY, dtstart=start, until=end)
 	staff_date_format = StatusDashboardCustomization.get("dashboard_staff_status_date_format")
 	if csv_export:
 		return export_staff_status(request, staffs, days, start, end, staff_date_format)
 	return {
@@ -185,15 +185,15 @@
 	timestamp = request.GET.get("timestamp", "")
 	view = request.GET.get("view", "")
 	if request.POST and form.is_valid():
 		form.save()
 		return HttpResponse()
 	dictionary = {
 		"form": form,
-		"staff_members": StaffAvailability.objects.all(),
+		"staff_members": StaffAvailability.objects.filter(visible=True),
 		"page_timestamp": timestamp,
 		"page_view": view,
 	}
 	return render(request, "status_dashboard/staff_absence.html", dictionary)
 
 
 @facility_manager_required
@@ -265,15 +265,15 @@
 	return response
 
 
 def show_staff_status(request):
 	if not settings.ALLOW_CONDITIONAL_URLS:
 		return False
 	dashboard_staff_status_staff_only = StatusDashboardCustomization.get("dashboard_staff_status_staff_only")
-	return StaffAvailability.objects.exists() and (not dashboard_staff_status_staff_only or request.user.is_any_part_of_staff)
+	return StaffAvailability.objects.filter(visible=True).exists() and (not dashboard_staff_status_staff_only or request.user.is_any_part_of_staff)
 
 
 def process_area_access_record_with_parents(user: User):
 	show_not_qualified_areas = StatusDashboardCustomization.get("dashboard_display_not_qualified_areas")
 	records = AreaAccessRecord.objects.filter(end=None, staff_charge=None)
 	if not user.is_any_part_of_staff and show_not_qualified_areas != "enabled":
 		records = records.filter(area__in=user.accessible_areas())
```

### Comparing `NEMO-4.4.1/NEMO/views/tasks.py` & `NEMO-4.5.0/NEMO/views/tasks.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 )
 from NEMO.utilities import (
 	EmailCategory,
 	as_timezone,
 	bootstrap_primary_color,
 	create_email_attachment,
 	format_datetime,
+	get_email_from_settings,
 	get_full_url,
 	render_email_template,
 	resize_image,
 	send_mail,
 )
 from NEMO.views.customization import ApplicationCustomization, EmailsCustomization, get_media_file_contents
 from NEMO.views.safety import send_safety_email_notification
@@ -186,15 +187,15 @@
 {linebreaksbr(task.progress_description)}
 <br/><br/>
 Task resolution description:<br/>
 {linebreaksbr(task.resolution_description)}
 <br/><br/>
 Visit {url} to view the tool control page for the task.<br/>
 """
-		send_mail(subject=f'{task.tool} task {task_status}', content=message, from_email=settings.SERVER_EMAIL, to=recipients, attachments=attachments, email_category=EmailCategory.TASKS)
+		send_mail(subject=f'{task.tool} task {task_status}', content=message, from_email=get_email_from_settings(), to=recipients, attachments=attachments, email_category=EmailCategory.TASKS)
 	except Exception as error:
 		site_title = ApplicationCustomization.get('site_title')
 		error_message = f"{site_title} was unable to send the task updated email. The error message that was received is: " + str(error)
 		tasks_logger.exception(error_message)
 
 
 @staff_member_required
@@ -304,15 +305,15 @@
 				image.save()
 				task_images.append(image)
 	except Exception as e:
 		tasks_logger.exception(e)
 	return task_images
 
 
-def get_task_email_recipients(task: Task) -> List[User]:
+def get_task_email_recipients(task: Task) -> List[str]:
 	# Add all recipients, starting with primary owner
 	recipient_users: List[User] = [task.tool.primary_owner]
 	# Add backup owners
 	recipient_users.extend(task.tool.backup_owners.all())
 	# Add facility managers
 	recipient_users.extend(User.objects.filter(is_active=True, is_facility_manager=True))
 	recipients = [email for user in recipient_users for email in user.get_emails(user.get_preferences().email_send_task_updates)]
```

### Comparing `NEMO-4.4.1/NEMO/views/tool_control.py` & `NEMO-4.5.0/NEMO/views/tool_control.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,33 +30,35 @@
 	TaskCategory,
 	TaskStatus,
 	Tool,
 	ToolUsageCounter,
 	UsageEvent,
 	User,
 )
+from NEMO.policy import policy_class as policy
 from NEMO.utilities import (
 	BasicDisplayTable,
 	EmailCategory,
 	export_format_datetime,
 	extract_optional_beginning_and_end_times,
 	format_datetime,
+	get_email_from_settings,
 	quiet_int,
 	render_email_template,
 	send_mail,
 )
 from NEMO.views.calendar import shorten_reservation
 from NEMO.views.customization import (
 	ApplicationCustomization,
 	CalendarCustomization,
 	EmailsCustomization,
 	InterlockCustomization,
+	RemoteWorkCustomization,
 	get_media_file_contents,
 )
-from NEMO.views.policy import check_policy_to_disable_tool, check_policy_to_enable_tool
 from NEMO.widgets.configuration_editor import ConfigurationEditor
 from NEMO.widgets.dynamic_form import DynamicForm, PostUsageQuestion, render_group_questions
 from NEMO.widgets.item_tree import ItemTree
 
 tool_control_logger = getLogger(__name__)
 
 
@@ -325,47 +327,57 @@
 
 	tool = get_object_or_404(Tool, id=tool_id)
 	operator = request.user
 	user = get_object_or_404(User, id=user_id)
 	project = get_object_or_404(Project, id=project_id)
 	staff_charge = staff_charge == "true"
 	bypass_interlock = request.POST.get("bypass", 'False') == 'True'
-	response = check_policy_to_enable_tool(tool, operator, user, project, staff_charge)
+	response = policy.check_to_enable_tool(tool, operator, user, project, staff_charge)
 	if response.status_code != HTTPStatus.OK:
 		return response
 
 	# All policy checks passed so enable the tool for the user.
 	if tool.interlock and not tool.interlock.unlock():
 		if bypass_interlock and interlock_bypass_allowed(user):
 			pass
 		else:
 			return interlock_error("Enable", user)
 
+	# Figure out if the tool usage is part of remote work
+	# 1: Staff charge means it's always remote work
+	# 2: Always remote if operator is different from the user
+	# 3: Unless customization is set to ask explicitly
+	remote_work = (user != operator and operator.is_staff)
+	if RemoteWorkCustomization.get_bool("remote_work_ask_explicitly"):
+		remote_work = remote_work and bool(request.POST.get("remote_work", False))
 	# Start staff charge before tool usage
 	if staff_charge:
+		# Staff charge means always a remote
+		remote_work = True
 		new_staff_charge = StaffCharge()
 		new_staff_charge.staff_member = request.user
 		new_staff_charge.customer = user
 		new_staff_charge.project = project
 		new_staff_charge.save()
 		# If the tool requires area access, start charging area access time
-		if tool.requires_area_access:
+		if tool.requires_area_access and RemoteWorkCustomization.get_bool("remote_work_start_area_access_automatically"):
 			area_access = AreaAccessRecord()
 			area_access.area = tool.requires_area_access
 			area_access.staff_charge = new_staff_charge
 			area_access.customer = new_staff_charge.customer
 			area_access.project = new_staff_charge.project
 			area_access.save()
 
 	# Create a new usage event to track how long the user uses the tool.
 	new_usage_event = UsageEvent()
 	new_usage_event.operator = operator
 	new_usage_event.user = user
 	new_usage_event.project = project
 	new_usage_event.tool = tool
+	new_usage_event.remote_work = remote_work
 	new_usage_event.save()
 
 	return response
 
 
 @login_required
 @require_POST
@@ -376,15 +388,15 @@
 
 	tool = get_object_or_404(Tool, id=tool_id)
 	if tool.get_current_usage_event() is None:
 		return HttpResponse()
 	user: User = request.user
 	downtime = timedelta(minutes=quiet_int(request.POST.get("downtime")))
 	bypass_interlock = request.POST.get("bypass", 'False') == 'True'
-	response = check_policy_to_disable_tool(tool, user, downtime)
+	response = policy.check_to_disable_tool(tool, user, downtime)
 	if response.status_code != HTTPStatus.OK:
 		return response
 
 	# All policy checks passed so disable the tool for the user.
 	if tool.interlock and not tool.interlock.lock():
 		if bypass_interlock and interlock_bypass_allowed(user):
 			pass
@@ -538,15 +550,15 @@
 	if facility_managers:
 		message = f"""The {counter.name} counter for the {counter.tool.name} was reset to 0 on {formats.localize(counter.last_reset)} by {counter.last_reset_by}.
 	
 Its last value was {counter.last_reset_value}."""
 		send_mail(
 			subject=f"{counter.tool.name} counter reset",
 			content=message,
-			from_email=settings.SERVER_EMAIL,
+			from_email=get_email_from_settings(),
 			to=facility_managers,
 			email_category=EmailCategory.SYSTEM,
 		)
 	return redirect("tool_control")
 
 
 def interlock_bypass_allowed(user: User):
```

### Comparing `NEMO-4.4.1/NEMO/views/training.py` & `NEMO-4.5.0/NEMO/views/training.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,41 @@
 from logging import getLogger
 from re import search
 from urllib.parse import urljoin
 
 import requests
 from django.conf import settings
+from django.db.models import Count
 from django.http import HttpResponseBadRequest
 from django.shortcuts import render
 from django.urls import reverse
 from django.views.decorators.http import require_GET, require_POST
 
 from NEMO.decorators import staff_member_or_tool_superuser_required
 from NEMO.exceptions import ProjectChargeException
-from NEMO.models import MembershipHistory, Project, Tool, TrainingSession, User
-from NEMO.views.policy import check_billing_to_project
+from NEMO.models import MembershipHistory, Project, Tool, ToolQualificationGroup, TrainingSession, User
+from NEMO.policy import policy_class as policy
 from NEMO.views.users import get_identity_service
 
 training_logger = getLogger(__name__)
 
 
 @staff_member_or_tool_superuser_required
 @require_GET
 def training(request):
 	""" Present a web page to allow staff or tool superusers to charge training and qualify users on particular tools. """
 	user: User = request.user
 	users = User.objects.filter(is_active=True).exclude(id=user.id)
 	tools = Tool.objects.filter(visible=True)
+	tool_groups = ToolQualificationGroup.objects.all()
 	if not user.is_staff and user.is_tool_superuser:
 		tools = tools.filter(_superusers__in=[user])
-	return render(request, 'training/training.html', {'users': users, 'tools': tools, 'charge_types': TrainingSession.Type.Choices})
+		# Superusers can only use groups if they are superusers for all those
+		tool_groups = tool_groups.annotate(num_tools=Count("tools")).filter(tools__in=tools).filter(num_tools=len(tools))
+	return render(request, 'training/training.html', {'users': users, 'tools': list(tools), 'tool_groups': list(tool_groups), 'charge_types': TrainingSession.Type.Choices})
 
 
 @staff_member_or_tool_superuser_required
 @require_GET
 def training_entry(request):
 	entry_number = int(request.GET['entry_number'])
 	return render(request, 'training/training_entry.html', {'entry_number': entry_number, 'charge_types': TrainingSession.Type.Choices})
@@ -53,43 +57,49 @@
 				index = int(index)
 				if index not in charges:
 					charges[index] = TrainingSession()
 					charges[index].trainer = trainer
 				if attribute == "chosen_user":
 					charges[index].trainee = User.objects.get(id=to_int_or_negative(value))
 				if attribute == "chosen_tool":
-					charges[index].tool = Tool.objects.get(id=to_int_or_negative(value))
-					if not trainer.is_staff and trainer.is_tool_superuser and charges[index].tool not in trainer.superuser_for_tools.all():
-						raise Exception("The trainer is not authorized to train on this tool")
+					chosen_type = request.POST.get(f"chosen_type{separator}{index}", "tool")
+					identifier = to_int_or_negative(value)
+					setattr(charges[index], "qualify_tools", [Tool.objects.get(id=identifier)] if chosen_type == "tool" else ToolQualificationGroup.objects.get(id=identifier).tools.all())
+					# Even with a group of tools, we only charge training on the first one
+					charges[index].tool = next(iter(charges[index].qualify_tools))
+					if not trainer.is_staff and trainer.is_tool_superuser:
+						if not set(charges[index].qualify_tools).issubset(trainer.superuser_for_tools.all()):
+							return HttpResponseBadRequest("The trainer is not authorized to train on this tool")
 				if attribute == "chosen_project":
 					charges[index].project = Project.objects.get(id=to_int_or_negative(value))
 				if attribute == "duration":
 					charges[index].duration = int(value)
 				if attribute == "charge_type":
 					charges[index].type = int(value)
 				if attribute == "qualify":
 					charges[index].qualified = (value == "on")
 		for c in charges.values():
 			c.full_clean()
-			check_billing_to_project(c.project, c.trainee, c.tool)
+			policy.check_billing_to_project(c.project, c.trainee, c.tool)
 	except ProjectChargeException as e:
 		return HttpResponseBadRequest(e.msg)
 	except User.DoesNotExist:
 		return HttpResponseBadRequest("Please select a trainee from the list")
 	except Tool.DoesNotExist:
 		return HttpResponseBadRequest("Please select a tool from the list")
 	except Project.DoesNotExist:
 		return HttpResponseBadRequest("Please select a project from the list")
 	except Exception as e:
 		training_logger.exception(e)
 		return HttpResponseBadRequest('An error occurred while processing the training charges. None of the charges were committed to the database. Please review the form for errors and omissions then submit the form again.')
 	else:
 		for c in charges.values():
 			if c.qualified:
-				qualify(c.trainer, c.trainee, c.tool)
+				for tool in c.qualify_tools:
+					qualify(c.trainer, c.trainee, tool)
 			c.save()
 		dictionary = {
 			'title': 'Success!',
 			'content': 'Training charges were successfully saved.',
 			'redirect': reverse('landing'),
 		}
 		return render(request, 'display_success_and_redirect.html', dictionary)
```

### Comparing `NEMO-4.4.1/NEMO/views/tutorials.py` & `NEMO-4.5.0/NEMO/views/tutorials.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO/views/usage.py` & `NEMO-4.5.0/NEMO/views/usage.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 	billable_items_area_access_records,
 	billable_items_consumable_withdrawals,
 	billable_items_missed_reservations,
 	billable_items_staff_charges,
 	billable_items_training_sessions,
 	billable_items_usage_events,
 )
+from NEMO.views.customization import UserRequestsCustomization
 
 logger = getLogger(__name__)
 
 
 # Class for Applications that can be used for autocomplete
 class Application(object):
 	def __init__(self, name):
@@ -87,15 +88,15 @@
 	identifier = request.GET.get("id")
 	dictionary = {
 		'month_list': month_list(),
 		'start_date': start_date,
 		'end_date': end_date,
 		'kind': kind,
 		'identifier': identifier,
-		'tab_url': get_url_for_other_tab(request),
+		'tab_url': get_url_for_other_tab(request) if  get_billing_service().get('available', False) else '',
 		'billing_service': get_billing_service().get('available', False),
 	}
 	return dictionary, start_date, end_date, kind, identifier
 
 
 @login_required
 @require_GET
@@ -128,14 +129,15 @@
 		dictionary = {
 			'area_access': area_access,
 			'consumables': consumables,
 			'missed_reservations': missed_reservations,
 			'staff_charges': staff_charges,
 			'training_sessions': training_sessions,
 			'usage_events': usage_events,
+			'adjustment_time_limit': UserRequestsCustomization.get_date_limit(),
 			'can_export': True,
 		}
 		if user_managed_projects:
 			dictionary['pi_projects'] = user_managed_projects
 		dictionary['no_charges'] = not (dictionary['area_access'] or dictionary['consumables'] or dictionary['missed_reservations'] or dictionary['staff_charges'] or dictionary['training_sessions'] or dictionary['usage_events'])
 		return render(request, 'usage/usage.html', {**base_dictionary, **dictionary})
 
@@ -205,14 +207,15 @@
 		'search_items': set(Account.objects.all()) | set(Project.objects.all()) | set(get_project_applications()) | set(User.objects.filter(is_active=True)),
 		'area_access': area_access,
 		'consumables': consumables,
 		'missed_reservations': missed_reservations,
 		'staff_charges': staff_charges,
 		'training_sessions': training_sessions,
 		'usage_events': usage_events,
+		'adjustment_time_limit': UserRequestsCustomization.get_date_limit(),
 		'project_autocomplete': True,
 		'selection': selection,
 		'can_export': True,
 	}
 	dictionary['no_charges'] = not (dictionary['area_access'] or dictionary['consumables'] or dictionary['missed_reservations'] or dictionary['staff_charges'] or dictionary['training_sessions'] or dictionary['usage_events'])
 	return render(request, 'usage/usage.html', {**base_dictionary, **dictionary})
```

### Comparing `NEMO-4.4.1/NEMO/views/user_requests.py` & `NEMO-4.5.0/NEMO/views/user_requests.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,18 +8,20 @@
 
 @login_required
 @require_GET
 def user_requests(request, tab: str = None):
 	active_tab = (
 		tab or "access"
 		if PhysicalAccessLevel.objects.filter(allow_user_request=True).exists()
-		   and User.objects.filter(is_active=True, is_facility_manager=True).exists()
+		and User.objects.filter(is_active=True, is_facility_manager=True).exists()
 		else "buddy"
 	)
 	buddy_requests_title = UserRequestsCustomization.get("buddy_requests_title")
 	access_requests_title = UserRequestsCustomization.get("access_requests_title")
+	adjustment_requests_title = UserRequestsCustomization.get("adjustment_requests_title")
 	dictionary = {
 		"tab": active_tab,
 		"buddy_requests_title": buddy_requests_title,
 		"access_requests_title": access_requests_title,
+		"adjustment_requests_title": adjustment_requests_title,
 	}
 	return render(request, "requests/user_requests.html", dictionary)
```

### Comparing `NEMO-4.4.1/NEMO/views/users.py` & `NEMO-4.5.0/NEMO/views/users.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from django.contrib import messages
 from django.contrib.auth.decorators import login_required
 from django.http import HttpResponseBadRequest
 from django.shortcuts import get_object_or_404, redirect, render
 from django.utils import timezone
 from django.views.decorators.http import require_GET, require_POST, require_http_methods
 
-from NEMO.decorators import any_staff_required, user_office_or_facility_manager_required
+from NEMO.decorators import any_staff_required, user_office_or_manager_required
 from NEMO.forms import UserForm, UserPreferencesForm
 from NEMO.models import (
 	ActivityHistory,
 	Area,
 	AreaAccessRecord,
 	PhysicalAccessLevel,
 	Project,
@@ -220,15 +220,15 @@
 		message = f"{user} has been added successfully to {site_title}" if user_id == 'new' else f"{user} has been updated successfully"
 		messages.success(request, message)
 		return redirect(request.GET.get("next") or "users")
 	else:
 		return HttpResponseBadRequest('Invalid method')
 
 
-@user_office_or_facility_manager_required
+@user_office_or_manager_required
 @require_http_methods(['GET', 'POST'])
 def deactivate(request, user_id):
 	dictionary = {
 		'user_to_deactivate': get_object_or_404(User, id=user_id),
 		'reservations': Reservation.objects.filter(user=user_id, cancelled=False, missed=False, end__gt=timezone.now()),
 		'staff_charges': StaffCharge.objects.filter(customer=user_id, end=None),
 		'tool_usage': UsageEvent.objects.filter(user=user_id, end=None).prefetch_related('tool'),
@@ -307,60 +307,74 @@
 		activity_entry.save()
 
 		message = f"{user_to_deactivate} has been successfully deactivated"
 		messages.success(request, message)
 		return redirect('users')
 
 
-@user_office_or_facility_manager_required
+@user_office_or_manager_required
 @require_POST
 def reset_password(request, user_id):
 	try:
 		identity_service = get_identity_service()
-		user = get_object_or_404(User, id=user_id)
-		timeout = identity_service.get('timeout', 3)
-		result = requests.post(urljoin(identity_service['url'], '/reset_password/'), {'username': user.username, 'domain': user.domain}, timeout=timeout)
-		if result.status_code == HTTPStatus.OK:
-			dictionary = {
-				'title': 'Password reset',
-				'heading': 'The account password was set to the default',
-			}
+		if identity_service.get("available", False):
+			user = get_object_or_404(User, id=user_id)
+			timeout = identity_service.get('timeout', 3)
+			result = requests.post(urljoin(identity_service['url'], '/reset_password/'), {'username': user.username, 'domain': user.domain}, timeout=timeout)
+			if result.status_code == HTTPStatus.OK:
+				dictionary = {
+					'title': 'Password reset',
+					'heading': 'The account password was set to the default',
+				}
+			else:
+				dictionary = {
+					'title': 'Oops',
+					'heading': 'There was a problem resetting the password',
+					'content': 'The identity service returned HTTP error code {}. {}'.format(result.status_code, result.text),
+				}
 		else:
 			dictionary = {
-				'title': 'Oops',
+				'title': 'Identity service not available',
 				'heading': 'There was a problem resetting the password',
-				'content': 'The identity service returned HTTP error code {}. {}'.format(result.status_code, result.text),
+				'content': 'The identity service is not set or not available'
 			}
 	except Exception as e:
 		dictionary = {
 			'title': 'Oops',
 			'heading': 'There was a problem communicating with the identity service',
 			'content': 'Exception caught: {}. {}'.format(type(e).__name__, str(e)),
 		}
 	return render(request, 'acknowledgement.html', dictionary)
 
 
-@user_office_or_facility_manager_required
+@user_office_or_manager_required
 @require_POST
 def unlock_account(request, user_id):
 	try:
 		identity_service = get_identity_service()
-		user = get_object_or_404(User, id=user_id)
-		timeout = identity_service.get('timeout', 3)
-		result = requests.post(urljoin(identity_service['url'], '/unlock_account/'), {'username': user.username, 'domain': user.domain}, timeout=timeout)
-		if result.status_code == HTTPStatus.OK:
-			dictionary = {
-				'title': 'Account unlocked',
-				'heading': 'The account is now unlocked',
-			}
+		if identity_service.get("available", False):
+			user = get_object_or_404(User, id=user_id)
+			timeout = identity_service.get('timeout', 3)
+			result = requests.post(urljoin(identity_service['url'], '/unlock_account/'), {'username': user.username, 'domain': user.domain}, timeout=timeout)
+			if result.status_code == HTTPStatus.OK:
+				dictionary = {
+					'title': 'Account unlocked',
+					'heading': 'The account is now unlocked',
+				}
+			else:
+				dictionary = {
+					'title': 'Oops',
+					'heading': 'There was a problem unlocking the account',
+					'content': 'The identity service returned HTTP error code {}. {}'.format(result.status_code, result.text),
+				}
 		else:
 			dictionary = {
-				'title': 'Oops',
+				'title': 'Identity service not available',
 				'heading': 'There was a problem unlocking the account',
-				'content': 'The identity service returned HTTP error code {}. {}'.format(result.status_code, result.text),
+				'content': 'The identity service is not set or not available'
 			}
 	except Exception as e:
 		dictionary = {
 			'title': 'Oops',
 			'heading': 'There was a problem communicating with the identity service',
 			'content': 'Exception caught: {}. {}'.format(type(e).__name__, str(e)),
 		}
```

### Comparing `NEMO-4.4.1/NEMO/widgets/configuration_editor.py` & `NEMO-4.5.0/NEMO/widgets/configuration_editor.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from django.forms import Widget
+from django.template import Context, Template
 from django.urls import reverse
 from django.utils.html import escape
 from django.utils.safestring import mark_safe
 
 
 class ConfigurationEditor(Widget):
 	def __init__(self, attrs=None):
@@ -30,15 +31,15 @@
 			for index, option in enumerate(config.available_settings_as_list()):
 				result += "<option value=" + str(index)
 				if option == current_setting:
 					result += " selected"
 				result += ">" + escape(option) + "</option>"
 			result += "</select>"
 		else:
-			result += escape(current_setting)
+			result += self.display_setting(current_setting)
 		result += "</label></p>"
 		return result
 
 	def __render_for_multiple(self, config, render_as_form=None):
 		result = "<p>" + escape(config.name) + ":<ul>"
 		for setting_index, current_setting in enumerate(config.current_settings_as_list()):
 			result += "<li>"
@@ -48,10 +49,20 @@
 				for option_index, option in enumerate(config.available_settings_as_list()):
 					result += "<option value=" + str(option_index)
 					if option == current_setting:
 						result += " selected"
 					result += ">" + escape(option) + "</option>"
 				result += "</select></label>"
 			else:
-				result += config.configurable_item_name + " #" + str(setting_index + 1) + ": " + escape(current_setting)
+				result += config.configurable_item_name + " #" + str(setting_index + 1) + ": " + self.display_setting(current_setting)
 		result += "</ul></p>"
 		return result
+
+	def display_setting(self, current_setting):
+		from NEMO.views.customization import ToolCustomization
+		template = ToolCustomization.get("tool_control_configuration_setting_template")
+		contents = "{{ current_setting }}"
+		try:
+			contents = Template(template).render(Context({"current_setting": escape(current_setting)}))
+		except:
+			pass
+		return contents
```

### Comparing `NEMO-4.4.1/NEMO/widgets/dynamic_form.py` & `NEMO-4.5.0/NEMO/widgets/dynamic_form.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,15 +40,16 @@
 		self.min = self._init_property("min")
 		self.max = self._init_property("max")
 		self.precision = self._init_property("precision")
 		self.step = self._init_property("step")
 		self.rows = self._init_property("rows")
 		self.consumable = self._init_property("consumable")
 		self.required = self._init_property("required", True)
-		self.default_choice = self._init_property("default_choice")
+		# For backwards compatibility keep default choice
+		self.default_value = self._init_property("default_value") or self._init_property("default_choice")
 		self.choices = self._init_property("choices")
 		self.group_add_button_name = self._init_property("group_add_button_name") or "Add"
 		self.index = index
 		if index and not isinstance(self, PostUsageGroupQuestion):
 			self.name = f"{self.name}_{index}"
 		# form_name is used in forms and extraction to avoid potential conflicts with other data
 		self.form_name = f"df_{self.name}"
@@ -114,21 +115,60 @@
 
 	def render_element(self, virtual_inputs: bool, group_question_url: str, group_item_id: int) -> str:
 		title = self.title_html or self.title
 		result = f'<div class="form-group"><div style="white-space: pre-wrap">{title}{self.required_span if self.required else ""}</div>'
 		for choice in self.choices:
 			result += '<div class="radio">'
 			required = "required" if self.required else ""
-			is_default_choice = "checked" if self.default_choice and self.default_choice == choice else ""
+			is_default_choice = "checked" if self.default_value and self.default_value == choice else ""
 			result += f'<label><input type="radio" name="{self.form_name}" value="{choice}" {required} {is_default_choice}>{choice}</label>'
 			result += "</div>"
 		result += "</div>"
 		return result
 
 
+class PostUsageCheckboxQuestion(PostUsageQuestion):
+	question_type = "Question of type checkbox"
+
+	def validate(self):
+		super().validate()
+		self.validate_property_exists("choices")
+
+	def render_element(self, virtual_inputs: bool, group_question_url: str, group_item_id: int) -> str:
+		title = self.title_html or self.title
+		result = f'<div class="form-group"><div style="white-space: pre-wrap">{title}{self.required_span if self.required else ""}</div>'
+		result += f'<input aria-label="hidden field used for required answer" id="required_{ self.form_name }" type="checkbox" value="" style="display: none" { "required" if self.required else "" }/>'
+		for choice in self.choices:
+			result += '<div class="checkbox">'
+			required = f"""onclick="checkbox_required('{self.form_name}')" """ if self.required else ""
+			is_default_choice = "checked" if self.default_value and self.default_value == choice else ""
+			result += f'<label><input type="checkbox" name="{self.form_name}" value="{choice}" {required} {is_default_choice}>{choice}</label>'
+			result += "</div>"
+		result += "</div>"
+		return result
+
+	def render_script(self, virtual_inputs: bool, group_question_url: str, group_item_id: int) -> str:
+		result = "<script>"
+		result += "function checkbox_required(form_name) {"
+		result += "if ($('input[name=' + form_name + ']:checkbox:checked').length > 0) {"
+		result += "$('#required_' + form_name).prop('checked', true).change();"
+		result += "} else {"
+		result += "$('#required_'+ form_name).prop('checked', false).change();"
+		result += "} }"
+		result += "</script>"
+		return result
+
+	def extract(self, request, index=None) -> Dict:
+		answered_question = copy(self.properties)
+		user_input = request.POST.getlist(f"{self.form_name}_{index}" if index else self.form_name)
+		if user_input:
+			answered_question["user_input"] = user_input
+		return answered_question
+
+
 class PostUsageDropdownQuestion(PostUsageQuestion):
 	question_type = "Question of type dropdown"
 
 	def validate(self):
 		super().validate()
 		self.validate_property_exists("max-width")
 		self.validate_property_exists("choices")
@@ -141,15 +181,15 @@
 		result += (
 			f'<select name="{self.form_name}" {required} style="margin-top: 5px;{max_width}" class="form-control">'
 		)
 		blank_disabled = 'disabled="disabled"' if required else ""
 		placeholder = self.placeholder if self.placeholder else "Select an option"
 		result += f'<option {blank_disabled} selected="selected" value="">{placeholder}</option>'
 		for choice in self.choices:
-			is_default_choice = "selected" if self.default_choice and self.default_choice == choice else ""
+			is_default_choice = "selected" if self.default_value and self.default_value == choice else ""
 			result += f'<option value="{choice}" {is_default_choice}>{choice}</option>'
 		result += "</select>"
 		if self.help:
 			result += f'<div style="font-size:smaller;color:#999;{max_width}">{self.help}</div>'
 		result += "</div>"
 		return result
 
@@ -170,27 +210,28 @@
 		if input_group_required:
 			result += f'<div class="input-group" style="{max_width}">'
 		if self.prefix:
 			result += f'<span class="input-group-addon">{self.prefix}</span>'
 		required = "required" if self.required else ""
 		pattern = f'pattern="{self.pattern}"' if self.pattern else ""
 		placeholder = f'placeholder="{self.placeholder}"' if self.placeholder else ""
-		result += self.render_input(required, pattern, placeholder)
+		default_value = f'value="{self.default_value}"' if self.default_value else ""
+		result += self.render_input(required, pattern, placeholder, default_value)
 		if self.suffix:
 			result += f'<span class="input-group-addon">{self.suffix}</span>'
 		if input_group_required:
 			result += "</div>"
 		if self.help:
 			result += f'<div style="font-size:smaller;color:#999;{max_width}">{self.help}</div>'
 		result += "</div>"
 		return result
 
-	def render_input(self, required: str, pattern: str, placeholder: str) -> str:
+	def render_input(self, required: str, pattern: str, placeholder: str, default_value: str) -> str:
 		maxlength = f'maxlength="{self.maxlength}"' if self.maxlength else ""
-		return f'<input type="text" class="form-control" id="{self.form_name}" name="{self.form_name}" {maxlength} {placeholder} {pattern} {required} style="max-width:{self.max_width}px" spellcheck="false" autocapitalize="off" autocomplete="off" autocorrect="off">'
+		return f'<input type="text" class="form-control" id="{self.form_name}" name="{self.form_name}" {maxlength} {placeholder} {pattern} {default_value} {required} style="max-width:{self.max_width}px" spellcheck="false" autocapitalize="off" autocomplete="off" autocorrect="off">'
 
 	def render_script(self, virtual_inputs: bool, group_question_url: str, item_id: int) -> str:
 		if virtual_inputs:
 			return f"<script>$('#{self.form_name}').keyboard();</script>"
 		return super().render_script(virtual_inputs, group_question_url, item_id)
 
 	def render_as_text(self) -> str:
@@ -202,27 +243,27 @@
 			result += f" {self.suffix}"
 		return result
 
 
 class PostUsageTextAreaFieldQuestion(PostUsageTextFieldQuestion):
 	question_type = "Question of type textarea"
 
-	def render_input(self, required: str, pattern: str, placeholder: str) -> str:
+	def render_input(self, required: str, pattern: str, placeholder: str, default_value: str) -> str:
 		rows = f'rows="{str(self.rows)}"' if self.rows else ""
-		return f'<textarea class="form-control" id="{self.form_name}" name="{self.form_name}" {rows} {placeholder} {required} style="max-width:{self.max_width}px;height:inherit" spellcheck="false" autocapitalize="off" autocomplete="off" autocorrect="off"></textarea>'
+		return f'<textarea class="form-control" id="{self.form_name}" name="{self.form_name}" {rows} {placeholder} {required} style="max-width:{self.max_width}px;height:inherit" spellcheck="false" autocapitalize="off" autocomplete="off" autocorrect="off">{self.default_value or ""}</textarea>'
 
 
 class PostUsageNumberFieldQuestion(PostUsageTextFieldQuestion):
 	question_type = "Question of type number"
 
-	def render_input(self, required: str, pattern: str, placeholder: str) -> str:
+	def render_input(self, required: str, pattern: str, placeholder: str, default_value: str) -> str:
 		minimum = f'min="{self.min}"' if self.min else ""
 		maximum = f'max="{self.max}"' if self.max else ""
 		step = f'step="{self.step}"' if self.step else ""
-		return f'<input type="number" class="form-control" id="{self.form_name}" name="{self.form_name}" {placeholder} {pattern} {minimum} {maximum} {step} {required} style="max-width:{self.max_width}px" spellcheck="false" autocapitalize="off" autocomplete="off" autocorrect="off">'
+		return f'<input type="number" class="form-control" id="{self.form_name}" name="{self.form_name}" {placeholder} {pattern} {minimum} {maximum} {default_value} {step} {required} style="max-width:{self.max_width}px" spellcheck="false" autocapitalize="off" autocomplete="off" autocorrect="off">'
 
 	def render_script(self, virtual_inputs: bool, group_question_url: str, item_id: int) -> str:
 		if virtual_inputs:
 			return f"<script>$('#{self.form_name}').numpad({{'readonly': false, 'hidePlusMinusButton': true, 'hideDecimalButton': true}});</script>"
 		return super().render_script(virtual_inputs, group_question_url, item_id)
 
 	def render_as_text(self) -> str:
@@ -238,18 +279,18 @@
 			result += ")"
 		return result
 
 
 class PostUsageFloatFieldQuestion(PostUsageTextFieldQuestion):
 	question_type = "Question of type float"
 
-	def render_input(self, required: str, pattern: str, placeholder: str) -> str:
+	def render_input(self, required: str, pattern: str, placeholder: str, default_value: str) -> str:
 		precision = self.precision if self.precision else 2
 		pattern = f'pattern="^\s*(?=.*[0-9])\d*(?:\.\d{"{1," + str(precision) + "}"})?\s*$"'
-		return f'<input type="text" class="form-control" id="{self.form_name}" name="{self.form_name}" {placeholder} {pattern} {required} style="max-width:{self.max_width}px" spellcheck="false" autocapitalize="off" autocomplete="off" autocorrect="off">'
+		return f'<input type="text" class="form-control" id="{self.form_name}" name="{self.form_name}" {placeholder} {pattern} {default_value} {required} style="max-width:{self.max_width}px" spellcheck="false" autocapitalize="off" autocomplete="off" autocorrect="off">'
 
 	def render_script(self, virtual_inputs: bool, group_question_url: str, item_id: int) -> str:
 		if virtual_inputs:
 			return f"<script>$('#{self.form_name}').numpad({{'readonly': false, 'hidePlusMinusButton': true, 'hideDecimalButton': false}});</script>"
 		return super().render_script(virtual_inputs, group_question_url, item_id)
 
 
@@ -548,10 +589,11 @@
 
 question_types : Dict[str, Type[PostUsageQuestion]] = {
 	"number": PostUsageNumberFieldQuestion,
 	"float": PostUsageFloatFieldQuestion,
 	"textbox": PostUsageTextFieldQuestion,
 	"textarea": PostUsageTextAreaFieldQuestion,
 	"radio": PostUsageRadioQuestion,
+	"checkbox": PostUsageCheckboxQuestion,
 	"dropdown": PostUsageDropdownQuestion,
 	"group": PostUsageGroupQuestion,
 }
```

### Comparing `NEMO-4.4.1/NEMO/widgets/item_tree.py` & `NEMO-4.5.0/NEMO/widgets/item_tree.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.4.1/NEMO.egg-info/PKG-INFO` & `NEMO-4.5.0/NEMO.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: NEMO
-Version: 4.4.1
+Version: 4.5.0
 Summary: NEMO is a laboratory logistics web application. Use it to schedule reservations, control tool access, track maintenance issues, and more.
 Home-page: https://github.com/usnistgov/NEMO
 Author: Center for Nanoscale Science and Technology
 Author-email: CNSTapplications@nist.gov
 License: Public domain
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: Public Domain
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.8
+Requires-Python: >=3.8, <4
 License-File: LICENSE.md
 
 Find out more about NEMO on the GitHub project page https://github.com/usnistgov/NEMO
```

### Comparing `NEMO-4.4.1/NEMO.egg-info/SOURCES.txt` & `NEMO-4.5.0/NEMO.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -8,20 +8,22 @@
 NEMO/admin.py
 NEMO/context_processors.py
 NEMO/decorators.py
 NEMO/exceptions.py
 NEMO/fields.py
 NEMO/forms.py
 NEMO/interlocks.py
-NEMO/manage.py
 NEMO/middleware.py
 NEMO/migrations_utils.py
+NEMO/mixins.py
 NEMO/model_tree.py
 NEMO/models.py
+NEMO/parsers.py
 NEMO/permissions.py
+NEMO/policy.py
 NEMO/provisioning.py
 NEMO/rates.py
 NEMO/rest_filter_backend.py
 NEMO/serializers.py
 NEMO/urls.py
 NEMO/utilities.py
 NEMO/wsgi.py
@@ -124,14 +126,15 @@
 NEMO/migrations/0038_version_4_0_0.py
 NEMO/migrations/0039_version_4_1_0.py
 NEMO/migrations/0040_version_4_2_0.py
 NEMO/migrations/0041_version_4_2_1.py
 NEMO/migrations/0042_version_4_3_0.py
 NEMO/migrations/0043_version_4_3_2.py
 NEMO/migrations/0044_version_4_4_0.py
+NEMO/migrations/0045_version_4_5_0.py
 NEMO/migrations/__init__.py
 NEMO/static/badge_reader.js
 NEMO/static/favicon.ico
 NEMO/static/jquery.js
 NEMO/static/jquery.min.js
 NEMO/static/jumbotron_watermark.bmp
 NEMO/static/mobile.js
@@ -194,15 +197,14 @@
 NEMO/templates/history.html
 NEMO/templates/impersonate.html
 NEMO/templates/landing.html
 NEMO/templates/login.html
 NEMO/templates/no_project.html
 NEMO/templates/qualifications.html
 NEMO/templates/refresh_sidebar_icons.html
-NEMO/templates/remote_work.html
 NEMO/templates/abuse/abuse.html
 NEMO/templates/abuse/user_drill_down.html
 NEMO/templates/accounts_and_projects/account_and_projects.html
 NEMO/templates/accounts_and_projects/accounts_and_projects.html
 NEMO/templates/accounts_and_projects/create_account.html
 NEMO/templates/accounts_and_projects/create_project.html
 NEMO/templates/accounts_and_projects/documents_for_project.html
@@ -214,16 +216,15 @@
 NEMO/templates/area_access/login_areas.html
 NEMO/templates/area_access/new_area_access_record.html
 NEMO/templates/area_access/new_area_access_record_details.html
 NEMO/templates/area_access/self_login.html
 NEMO/templates/base/footer.html
 NEMO/templates/base/impersonate_header.html
 NEMO/templates/base/navbar.html
-NEMO/templates/base/navbar_admin.html
-NEMO/templates/base/navbar_main.html
+NEMO/templates/base/navbar_base.html
 NEMO/templates/base/popup.html
 NEMO/templates/calendar/calendar.html
 NEMO/templates/calendar/configuration.html
 NEMO/templates/calendar/configuration_helper.html
 NEMO/templates/calendar/policy_dialog.html
 NEMO/templates/calendar/project_choice.html
 NEMO/templates/calendar/proxy_reservation.html
@@ -243,18 +244,19 @@
 NEMO/templates/customizations/customizations_calendar.html
 NEMO/templates/customizations/customizations_dashboard.html
 NEMO/templates/customizations/customizations_emails.html
 NEMO/templates/customizations/customizations_interlock.html
 NEMO/templates/customizations/customizations_projects_and_accounts.html
 NEMO/templates/customizations/customizations_rates.html
 NEMO/templates/customizations/customizations_recurring_charges.html
+NEMO/templates/customizations/customizations_remote_work.html
 NEMO/templates/customizations/customizations_requests.html
 NEMO/templates/customizations/customizations_safety.html
 NEMO/templates/customizations/customizations_templates.html
-NEMO/templates/customizations/customizations_tool_qualification.html
+NEMO/templates/customizations/customizations_tool.html
 NEMO/templates/customizations/customizations_upload.html
 NEMO/templates/customizations/customizations_user.html
 NEMO/templates/email/compose_email.html
 NEMO/templates/email/email_broadcast.html
 NEMO/templates/email/email_form.html
 NEMO/templates/event_details/area_access_details.html
 NEMO/templates/event_details/outage_details.html
@@ -281,24 +283,31 @@
 NEMO/templates/occupancy/occupancy.html
 NEMO/templates/occupancy/occupancy_content.html
 NEMO/templates/occupancy/occupancy_count.html
 NEMO/templates/pagination/pagination_base.html
 NEMO/templates/pagination/pagination_column.html
 NEMO/templates/pagination/pagination_pages.html
 NEMO/templates/pagination/pagination_selector.html
+NEMO/templates/remote_work/remote_work.html
+NEMO/templates/remote_work/remote_work_base.html
 NEMO/templates/requests/user_requests.html
 NEMO/templates/requests/access_requests/access_request.html
 NEMO/templates/requests/access_requests/access_requests.html
 NEMO/templates/requests/access_requests/access_requests_table.html
+NEMO/templates/requests/adjustment_requests/adjustment_request.html
+NEMO/templates/requests/adjustment_requests/adjustment_requests.html
+NEMO/templates/requests/adjustment_requests/adjustment_requests_table.html
 NEMO/templates/requests/buddy_requests/buddy_request.html
 NEMO/templates/requests/buddy_requests/buddy_requests.html
 NEMO/templates/resources/modify_resource.html
 NEMO/templates/resources/resource_details.html
 NEMO/templates/resources/resources.html
 NEMO/templates/resources/scheduled_outage.html
+NEMO/templates/rest_framework/api.html
+NEMO/templates/rest_framework/custom_error.html
 NEMO/templates/safety/safety.html
 NEMO/templates/safety/safety_base.html
 NEMO/templates/safety/safety_data_sheets.html
 NEMO/templates/safety/safety_issues.html
 NEMO/templates/safety/safety_issues_create.html
 NEMO/templates/safety/safety_issues_resolved.html
 NEMO/templates/safety/safety_issues_update.html
@@ -327,30 +336,33 @@
 NEMO/templates/tool_control/tool_control.html
 NEMO/templates/tool_control/tool_status.html
 NEMO/templates/tool_control/usage_data.html
 NEMO/templates/tool_control/use_tool_for_other.html
 NEMO/templates/training/get_projects.html
 NEMO/templates/training/training.html
 NEMO/templates/training/training_entry.html
+NEMO/templates/usage/adjustment_request_button.html
 NEMO/templates/usage/billing.html
 NEMO/templates/usage/usage.html
 NEMO/templates/usage/usage_base.html
 NEMO/templates/users/create_or_modify_user.html
 NEMO/templates/users/preferences.html
 NEMO/templates/users/safe_deactivation.html
 NEMO/templates/users/users.html
 NEMO/templatetags/__init__.py
 NEMO/templatetags/custom_tags_and_filters.py
 NEMO/views/__init__.py
 NEMO/views/abuse.py
 NEMO/views/access_requests.py
 NEMO/views/accounts_and_projects.py
+NEMO/views/adjustment_requests.py
 NEMO/views/alerts.py
 NEMO/views/api.py
 NEMO/views/api_billing.py
+NEMO/views/api_file_import.py
 NEMO/views/area_access.py
 NEMO/views/authentication.py
 NEMO/views/buddy_requests.py
 NEMO/views/calendar.py
 NEMO/views/configuration_agenda.py
 NEMO/views/constants.py
 NEMO/views/consumables.py
@@ -365,21 +377,19 @@
 NEMO/views/jumbotron.py
 NEMO/views/landing.py
 NEMO/views/maintenance.py
 NEMO/views/mobile.py
 NEMO/views/news.py
 NEMO/views/notifications.py
 NEMO/views/pagination.py
-NEMO/views/policy.py
 NEMO/views/qualifications.py
 NEMO/views/remote_work.py
 NEMO/views/resources.py
 NEMO/views/safety.py
 NEMO/views/sidebar.py
-NEMO/views/staff_charges.py
 NEMO/views/status_dashboard.py
 NEMO/views/tasks.py
 NEMO/views/tool_control.py
 NEMO/views/training.py
 NEMO/views/tutorials.py
 NEMO/views/usage.py
 NEMO/views/user_requests.py
```

### Comparing `NEMO-4.4.1/PKG-INFO` & `NEMO-4.5.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: NEMO
-Version: 4.4.1
+Version: 4.5.0
 Summary: NEMO is a laboratory logistics web application. Use it to schedule reservations, control tool access, track maintenance issues, and more.
 Home-page: https://github.com/usnistgov/NEMO
 Author: Center for Nanoscale Science and Technology
 Author-email: CNSTapplications@nist.gov
 License: Public domain
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: Public Domain
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.8
+Requires-Python: >=3.8, <4
 License-File: LICENSE.md
 
 Find out more about NEMO on the GitHub project page https://github.com/usnistgov/NEMO
```

### Comparing `NEMO-4.4.1/README.md` & `NEMO-4.5.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/NEMO?label=python)](https://www.python.org/downloads/release/python-380/)
+[![Docker Image Version (latest semver)](https://img.shields.io/docker/v/nanofab/nemo?label=NEMO%20docker%20version)](https://hub.docker.com/r/nanofab/nemo)
+[![GitHub release (latest by date)](https://img.shields.io/github/v/release/usnistgov/nemo?label=NEMO%20github%20version)](https://github.com/usnistgov/NEMO/releases)
+[![PyPI](https://img.shields.io/pypi/v/nemo?label=NEMO%20pypi%20version)](https://pypi.org/project/NEMO/)
+
 The NEMO web application is laboratory logistics software that strives to be intuitive and easy to use, making life easier in the lab. NEMO manages tool reservations, control access to tools, and streamline logistics and communication. The code is open source and free so that other labs can benefit.
 
 # Online demo
 An online version of the splash pad is available at [https://nemo.nist.gov/demo](https://nemo.nist.gov/demo).
 
 ### User roles
 You will be automatically logged in as superadmin "captain".<br>
```

### Comparing `NEMO-4.4.1/resources/splash_pad_settings.py` & `NEMO-4.5.0/resources/splash_pad_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 				'django.contrib.messages.context_processors.messages',
 			],
 		},
 	},
 ]
 
 REST_FRAMEWORK = {
-	'DEFAULT_PERMISSION_CLASSES': ('NEMO.permissions.BillingAPI',),
+	'DEFAULT_PERMISSION_CLASSES': ('NEMO.permissions.DjangoModelPermissions',),
 	'DEFAULT_FILTER_BACKENDS': ('django_filters.rest_framework.DjangoFilterBackend',),
 	'DEFAULT_PAGINATION_CLASS': 'rest_framework.pagination.PageNumberPagination',
 	'PAGE_SIZE': 1000,
 }
 
 SERVER_EMAIL = 'NEMO Server Administrator <nemo.admin@example.org>'
```

### Comparing `NEMO-4.4.1/setup.py` & `NEMO-4.5.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_namespace_packages, setup
 
 setup(
 	name='NEMO',
-	version='4.4.1',
-	python_requires='>=3.8',
+	version='4.5.0',
+	python_requires='>=3.8, <4',
 	packages=find_namespace_packages(exclude=['NEMO.tests', 'NEMO.tests.*']),
 	include_package_data=True,
 	url='https://github.com/usnistgov/NEMO',
 	license='Public domain',
 	author='Center for Nanoscale Science and Technology',
 	author_email='CNSTapplications@nist.gov',
 	description='NEMO is a laboratory logistics web application. Use it to schedule reservations, control tool access, track maintenance issues, and more.',
@@ -20,26 +20,26 @@
 		'Intended Audience :: System Administrators',
 		'License :: Public Domain',
 		'Natural Language :: English',
 		'Operating System :: OS Independent',
 		'Programming Language :: Python :: 3.8',
 	],
 	install_requires=[
-		'cryptography==39.0.0',
-		'Django==3.2.16',
+		'cryptography==40.0.1',
+		'Django==3.2.18',
 		'django-auditlog==2.2.2',
-		'django-filter==22.1',
+		'django-filter==23.1',
 		'django-mptt==0.14.0',
 		'djangorestframework==3.14.0',
-		'drf-excel==2.2.0',
-		'drf-flex-fields==1.0.0',
+		'drf-excel==2.3.0',
+		'drf-flex-fields==1.0.2',
 		'ldap3==2.9.1',
-		'Pillow==9.4.0',
-		'pymodbus==3.1.1',
+		'Pillow==9.5.0',
+		'pymodbus==3.2.2',
 		'python-dateutil==2.8.2',
-		'pytz==2022.7.1',
+		'pytz==2023.3',
 		'requests==2.28.2',
 	],
 	entry_points={
 		'console_scripts': ['nemo=NEMO.provisioning:entry_point'],
 	},
 )
```

