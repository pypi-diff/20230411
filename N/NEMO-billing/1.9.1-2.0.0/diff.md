# Comparing `tmp/NEMO_billing-1.9.1-py3-none-any.whl.zip` & `tmp/NEMO_billing-2.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,74 +1,128 @@
-Zip file size: 79939 bytes, number of entries: 72
--rw-r--r--  2.0 unx      428 b- defN 21-Sep-13 16:58 NEMO_billing/__init__.py
--rw-r--r--  2.0 unx    10761 b- defN 21-Sep-13 16:58 NEMO_billing/admin.py
--rw-r--r--  2.0 unx      203 b- defN 21-Sep-13 16:58 NEMO_billing/app_settings.py
--rw-r--r--  2.0 unx     2752 b- defN 21-Sep-13 16:58 NEMO_billing/models.py
--rw-r--r--  2.0 unx      890 b- defN 21-Sep-13 16:58 NEMO_billing/urls.py
--rw-r--r--  2.0 unx     7323 b- defN 21-Sep-13 16:58 NEMO_billing/views.py
--rw-r--r--  2.0 unx      449 b- defN 21-Sep-13 16:58 NEMO_billing/invoices/__init__.py
--rw-r--r--  2.0 unx     6410 b- defN 21-Sep-13 16:58 NEMO_billing/invoices/admin.py
--rw-r--r--  2.0 unx      333 b- defN 21-Sep-13 16:58 NEMO_billing/invoices/app_settings.py
--rw-r--r--  2.0 unx     1939 b- defN 21-Sep-13 16:58 NEMO_billing/invoices/exceptions.py
--rw-r--r--  2.0 unx    19596 b- defN 21-Sep-13 16:58 NEMO_billing/invoices/invoice_data_processor.py
--rw-r--r--  2.0 unx    20957 b- defN 21-Sep-13 16:58 NEMO_billing/invoices/invoice_generator.py
--rw-r--r--  2.0 unx    21491 b- defN 21-Sep-13 16:58 NEMO_billing/invoices/models.py
--rw-r--r--  2.0 unx    12468 b- defN 21-Sep-13 16:58 NEMO_billing/invoices/pdf_utilities.py
--rw-r--r--  2.0 unx       60 b- defN 21-Sep-13 16:58 NEMO_billing/invoices/tests.py
--rw-r--r--  2.0 unx     1802 b- defN 21-Sep-13 16:58 NEMO_billing/invoices/urls.py
--rw-r--r--  2.0 unx     3319 b- defN 21-Sep-13 16:58 NEMO_billing/invoices/utilities.py
--rw-r--r--  2.0 unx        0 b- defN 21-Sep-13 16:58 NEMO_billing/invoices/management/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 21-Sep-13 16:58 NEMO_billing/invoices/management/commands/__init__.py
--rw-r--r--  2.0 unx      298 b- defN 21-Sep-13 16:58 NEMO_billing/invoices/management/commands/deactivate_expired_projects.py
--rw-r--r--  2.0 unx      319 b- defN 21-Sep-13 16:58 NEMO_billing/invoices/management/commands/send_invoice_payment_reminder.py
--rw-r--r--  2.0 unx     9795 b- defN 21-Sep-13 16:58 NEMO_billing/invoices/migrations/0001_initial.py
--rw-r--r--  2.0 unx     2781 b- defN 21-Sep-13 16:58 NEMO_billing/invoices/migrations/0002_version_1_2_0.py
--rw-r--r--  2.0 unx     1063 b- defN 21-Sep-13 16:58 NEMO_billing/invoices/migrations/0003_version_1_4_0.py
--rw-r--r--  2.0 unx      467 b- defN 21-Sep-13 16:58 NEMO_billing/invoices/migrations/0004_version_1_6_0.py
--rw-r--r--  2.0 unx      485 b- defN 21-Sep-13 16:58 NEMO_billing/invoices/migrations/0005_version_1_6_1.py
--rw-r--r--  2.0 unx      518 b- defN 21-Sep-13 16:58 NEMO_billing/invoices/migrations/0006_version_1_7_1.py
--rw-r--r--  2.0 unx      458 b- defN 21-Sep-13 16:58 NEMO_billing/invoices/migrations/0007_version_1_8_0.py
--rw-r--r--  2.0 unx        0 b- defN 21-Sep-13 16:58 NEMO_billing/invoices/migrations/__init__.py
--rw-rw-rw-  2.0 unx      868 b- defN 21-Sep-13 16:58 NEMO_billing/invoices/static/invoices/invoices.css
--rw-rw-rw-  2.0 unx      212 b- defN 21-Sep-13 16:58 NEMO_billing/invoices/templates/invoices/base.html
--rw-rw-rw-  2.0 unx    11521 b- defN 21-Sep-13 16:58 NEMO_billing/invoices/templates/invoices/invoice.html
--rw-rw-rw-  2.0 unx     3249 b- defN 21-Sep-13 16:58 NEMO_billing/invoices/templates/invoices/invoice_details.html
--rw-rw-rw-  2.0 unx     7295 b- defN 21-Sep-13 16:58 NEMO_billing/invoices/templates/invoices/invoices.html
--rw-rw-rw-  2.0 unx     1320 b- defN 21-Sep-13 16:58 NEMO_billing/invoices/templates/invoices/email/email_send_invoice_message.html
--rw-rw-rw-  2.0 unx     1334 b- defN 21-Sep-13 16:58 NEMO_billing/invoices/templates/invoices/email/email_send_invoice_reminder_message.html
--rw-rw-rw-  2.0 unx      155 b- defN 21-Sep-13 16:58 NEMO_billing/invoices/templates/invoices/email/email_send_invoice_reminder_subject.txt
--rw-rw-rw-  2.0 unx      155 b- defN 21-Sep-13 16:58 NEMO_billing/invoices/templates/invoices/email/email_send_invoice_subject.txt
--rw-rw-rw-  2.0 unx     9616 b- defN 21-Sep-13 16:58 NEMO_billing/invoices/templates/invoices/project/edit_project.html
--rw-rw-rw-  2.0 unx     3069 b- defN 21-Sep-13 16:58 NEMO_billing/invoices/templates/invoices/project/view_project_additional_info.html
--rw-r--r--  2.0 unx        0 b- defN 21-Sep-13 16:58 NEMO_billing/invoices/views/__init__.py
--rw-r--r--  2.0 unx    10485 b- defN 21-Sep-13 16:58 NEMO_billing/invoices/views/invoices.py
--rw-r--r--  2.0 unx     4983 b- defN 21-Sep-13 16:58 NEMO_billing/invoices/views/project.py
--rw-r--r--  2.0 unx     3156 b- defN 21-Sep-13 16:58 NEMO_billing/migrations/0001_initial.py
--rw-r--r--  2.0 unx      573 b- defN 21-Sep-13 16:58 NEMO_billing/migrations/0002_version_1_2_0.py
--rw-r--r--  2.0 unx        0 b- defN 21-Sep-13 16:58 NEMO_billing/migrations/__init__.py
--rw-r--r--  2.0 unx      434 b- defN 21-Sep-13 16:58 NEMO_billing/rates/__init__.py
--rw-r--r--  2.0 unx     2038 b- defN 21-Sep-13 16:58 NEMO_billing/rates/admin.py
--rw-r--r--  2.0 unx       61 b- defN 21-Sep-13 16:58 NEMO_billing/rates/app_settings.py
--rw-r--r--  2.0 unx     1913 b- defN 21-Sep-13 16:58 NEMO_billing/rates/model_diff.py
--rw-r--r--  2.0 unx    13381 b- defN 21-Sep-13 16:58 NEMO_billing/rates/models.py
--rw-r--r--  2.0 unx     1833 b- defN 21-Sep-13 16:58 NEMO_billing/rates/rates_class.py
--rw-r--r--  2.0 unx       60 b- defN 21-Sep-13 16:58 NEMO_billing/rates/tests.py
--rw-r--r--  2.0 unx      395 b- defN 21-Sep-13 16:58 NEMO_billing/rates/urls.py
--rw-r--r--  2.0 unx     8121 b- defN 21-Sep-13 16:58 NEMO_billing/rates/views.py
--rw-r--r--  2.0 unx     5101 b- defN 21-Sep-13 16:58 NEMO_billing/rates/migrations/0001_initial.py
--rw-r--r--  2.0 unx        0 b- defN 21-Sep-13 16:58 NEMO_billing/rates/migrations/__init__.py
--rw-rw-rw-  2.0 unx       81 b- defN 21-Sep-13 16:58 NEMO_billing/rates/static/rates/rates.css
--rw-rw-rw-  2.0 unx      160 b- defN 21-Sep-13 16:58 NEMO_billing/rates/templates/rates/base.html
--rw-rw-rw-  2.0 unx     4550 b- defN 21-Sep-13 16:58 NEMO_billing/rates/templates/rates/rate.html
--rw-rw-rw-  2.0 unx     4153 b- defN 21-Sep-13 16:58 NEMO_billing/rates/templates/rates/rate_form_details.html
--rw-rw-rw-  2.0 unx     2479 b- defN 21-Sep-13 16:58 NEMO_billing/rates/templates/rates/rates.html
--rw-rw-rw-  2.0 unx     4959 b- defN 21-Sep-13 16:58 NEMO_billing/templates/base/navbar.html
--rw-rw-rw-  2.0 unx     8242 b- defN 21-Sep-13 16:58 NEMO_billing/templates/billing/custom_charge.html
--rw-rw-rw-  2.0 unx     1731 b- defN 21-Sep-13 16:58 NEMO_billing/templates/billing/custom_charges.html
--rw-rw-rw-  2.0 unx     1185 b- defN 21-Sep-13 16:58 NEMO_billing/templates/staff_charges/choose_project.html
--rw-rw-rw-  2.0 unx     1973 b- defN 21-Sep-13 16:58 NEMO_billing/templates/staff_charges/new_custom_staff_charge.html
--rw-rw-rw-  2.0 unx     1081 b- defN 21-Sep-13 16:58 NEMO_billing-1.9.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     4030 b- defN 21-Sep-13 16:58 NEMO_billing-1.9.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 21-Sep-13 16:58 NEMO_billing-1.9.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       13 b- defN 21-Sep-13 16:58 NEMO_billing-1.9.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     7193 b- defN 21-Sep-13 16:58 NEMO_billing-1.9.1.dist-info/RECORD
-72 files, 260615 bytes uncompressed, 68077 bytes compressed:  73.9%
+Zip file size: 156208 bytes, number of entries: 126
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 21:04 NEMO_billing/__init__.py
+-rw-r--r--  2.0 unx    11303 b- defN 23-Apr-11 21:04 NEMO_billing/admin.py
+-rw-r--r--  2.0 unx     1368 b- defN 23-Apr-11 21:04 NEMO_billing/api.py
+-rw-r--r--  2.0 unx      203 b- defN 23-Apr-11 21:04 NEMO_billing/app_settings.py
+-rw-r--r--  2.0 unx      426 b- defN 23-Apr-11 21:04 NEMO_billing/apps.py
+-rw-r--r--  2.0 unx      199 b- defN 23-Apr-11 21:04 NEMO_billing/decorators.py
+-rw-r--r--  2.0 unx      122 b- defN 23-Apr-11 21:04 NEMO_billing/exceptions.py
+-rw-r--r--  2.0 unx     4612 b- defN 23-Apr-11 21:04 NEMO_billing/models.py
+-rw-r--r--  2.0 unx     1126 b- defN 23-Apr-11 21:04 NEMO_billing/urls.py
+-rw-r--r--  2.0 unx      417 b- defN 23-Apr-11 21:04 NEMO_billing/utilities.py
+-rw-r--r--  2.0 unx     7757 b- defN 23-Apr-11 21:04 NEMO_billing/views.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 21:04 NEMO_billing/cap_discount/__init__.py
+-rw-r--r--  2.0 unx     5307 b- defN 23-Apr-11 21:04 NEMO_billing/cap_discount/admin.py
+-rw-r--r--  2.0 unx      102 b- defN 23-Apr-11 21:04 NEMO_billing/cap_discount/app_settings.py
+-rw-r--r--  2.0 unx      436 b- defN 23-Apr-11 21:04 NEMO_billing/cap_discount/apps.py
+-rw-r--r--  2.0 unx     2991 b- defN 23-Apr-11 21:04 NEMO_billing/cap_discount/customization.py
+-rw-r--r--  2.0 unx      446 b- defN 23-Apr-11 21:04 NEMO_billing/cap_discount/exceptions.py
+-rw-r--r--  2.0 unx    16857 b- defN 23-Apr-11 21:04 NEMO_billing/cap_discount/models.py
+-rw-r--r--  2.0 unx    20261 b- defN 23-Apr-11 21:04 NEMO_billing/cap_discount/processors.py
+-rw-r--r--  2.0 unx      461 b- defN 23-Apr-11 21:04 NEMO_billing/cap_discount/urls.py
+-rw-r--r--  2.0 unx     1280 b- defN 23-Apr-11 21:04 NEMO_billing/cap_discount/views.py
+-rw-r--r--  2.0 unx     7594 b- defN 23-Apr-11 21:04 NEMO_billing/cap_discount/migrations/0001_initial.py
+-rw-r--r--  2.0 unx     1665 b- defN 23-Apr-11 21:04 NEMO_billing/cap_discount/migrations/0002_version_2_0_0.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 21:04 NEMO_billing/cap_discount/migrations/__init__.py
+-rw-rw-rw-  2.0 unx     1664 b- defN 23-Apr-11 21:04 NEMO_billing/cap_discount/templates/cap_discount/usage_cap_discounts.html
+-rw-rw-rw-  2.0 unx     4068 b- defN 23-Apr-11 21:04 NEMO_billing/cap_discount/templates/customizations/customizations_cap_discount.html
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 21:04 NEMO_billing/invoices/__init__.py
+-rw-r--r--  2.0 unx    10232 b- defN 23-Apr-11 21:04 NEMO_billing/invoices/admin.py
+-rw-r--r--  2.0 unx     5485 b- defN 23-Apr-11 21:04 NEMO_billing/invoices/api.py
+-rw-r--r--  2.0 unx      176 b- defN 23-Apr-11 21:04 NEMO_billing/invoices/app_settings.py
+-rw-r--r--  2.0 unx      437 b- defN 23-Apr-11 21:04 NEMO_billing/invoices/apps.py
+-rw-r--r--  2.0 unx     4397 b- defN 23-Apr-11 21:04 NEMO_billing/invoices/customization.py
+-rw-r--r--  2.0 unx     2642 b- defN 23-Apr-11 21:04 NEMO_billing/invoices/exceptions.py
+-rw-r--r--  2.0 unx    22806 b- defN 23-Apr-11 21:04 NEMO_billing/invoices/models.py
+-rw-r--r--  2.0 unx    12477 b- defN 23-Apr-11 21:04 NEMO_billing/invoices/pdf_utilities.py
+-rw-r--r--  2.0 unx    27120 b- defN 23-Apr-11 21:04 NEMO_billing/invoices/processors.py
+-rw-r--r--  2.0 unx    25415 b- defN 23-Apr-11 21:04 NEMO_billing/invoices/renderers.py
+-rw-r--r--  2.0 unx     2859 b- defN 23-Apr-11 21:04 NEMO_billing/invoices/urls.py
+-rw-r--r--  2.0 unx     4235 b- defN 23-Apr-11 21:04 NEMO_billing/invoices/utilities.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 21:04 NEMO_billing/invoices/management/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 21:04 NEMO_billing/invoices/management/commands/__init__.py
+-rw-r--r--  2.0 unx      298 b- defN 23-Apr-11 21:04 NEMO_billing/invoices/management/commands/deactivate_expired_projects.py
+-rw-r--r--  2.0 unx      318 b- defN 23-Apr-11 21:04 NEMO_billing/invoices/management/commands/send_invoice_payment_reminder.py
+-rw-r--r--  2.0 unx     9795 b- defN 23-Apr-11 21:04 NEMO_billing/invoices/migrations/0001_initial.py
+-rw-r--r--  2.0 unx     2781 b- defN 23-Apr-11 21:04 NEMO_billing/invoices/migrations/0002_version_1_2_0.py
+-rw-r--r--  2.0 unx     1063 b- defN 23-Apr-11 21:04 NEMO_billing/invoices/migrations/0003_version_1_4_0.py
+-rw-r--r--  2.0 unx      467 b- defN 23-Apr-11 21:04 NEMO_billing/invoices/migrations/0004_version_1_6_0.py
+-rw-r--r--  2.0 unx      485 b- defN 23-Apr-11 21:04 NEMO_billing/invoices/migrations/0005_version_1_6_1.py
+-rw-r--r--  2.0 unx      518 b- defN 23-Apr-11 21:04 NEMO_billing/invoices/migrations/0006_version_1_7_1.py
+-rw-r--r--  2.0 unx      458 b- defN 23-Apr-11 21:04 NEMO_billing/invoices/migrations/0007_version_1_8_0.py
+-rw-r--r--  2.0 unx      437 b- defN 23-Apr-11 21:04 NEMO_billing/invoices/migrations/0008_version_1_10_0.py
+-rw-r--r--  2.0 unx     1183 b- defN 23-Apr-11 21:04 NEMO_billing/invoices/migrations/0009_version_1_23_0.py
+-rw-r--r--  2.0 unx      439 b- defN 23-Apr-11 21:04 NEMO_billing/invoices/migrations/0010_version_2_0_0.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 21:04 NEMO_billing/invoices/migrations/__init__.py
+-rw-rw-rw-  2.0 unx     1030 b- defN 23-Apr-11 21:04 NEMO_billing/invoices/static/invoices/invoices.css
+-rw-rw-rw-  2.0 unx     4924 b- defN 23-Apr-11 21:04 NEMO_billing/invoices/templates/customizations/customizations_billing.html
+-rw-rw-rw-  2.0 unx     8157 b- defN 23-Apr-11 21:04 NEMO_billing/invoices/templates/customizations/customizations_invoices.html
+-rw-rw-rw-  2.0 unx      212 b- defN 23-Apr-11 21:04 NEMO_billing/invoices/templates/invoices/base.html
+-rw-rw-rw-  2.0 unx    12867 b- defN 23-Apr-11 21:04 NEMO_billing/invoices/templates/invoices/invoice.html
+-rw-rw-rw-  2.0 unx     3375 b- defN 23-Apr-11 21:04 NEMO_billing/invoices/templates/invoices/invoice_details.html
+-rw-rw-rw-  2.0 unx    12238 b- defN 23-Apr-11 21:04 NEMO_billing/invoices/templates/invoices/invoices.html
+-rw-rw-rw-  2.0 unx     9831 b- defN 23-Apr-11 21:04 NEMO_billing/invoices/templates/invoices/usage.html
+-rw-rw-rw-  2.0 unx     1274 b- defN 23-Apr-11 21:04 NEMO_billing/invoices/templates/invoices/email/billing_project_expiration_reminder_email_message.html
+-rw-rw-rw-  2.0 unx      173 b- defN 23-Apr-11 21:04 NEMO_billing/invoices/templates/invoices/email/billing_project_expiration_reminder_email_subject.txt
+-rw-rw-rw-  2.0 unx     1330 b- defN 23-Apr-11 21:04 NEMO_billing/invoices/templates/invoices/email/email_send_invoice_message.html
+-rw-rw-rw-  2.0 unx     1344 b- defN 23-Apr-11 21:04 NEMO_billing/invoices/templates/invoices/email/email_send_invoice_reminder_message.html
+-rw-rw-rw-  2.0 unx      155 b- defN 23-Apr-11 21:04 NEMO_billing/invoices/templates/invoices/email/email_send_invoice_reminder_subject.txt
+-rw-rw-rw-  2.0 unx      155 b- defN 23-Apr-11 21:04 NEMO_billing/invoices/templates/invoices/email/email_send_invoice_subject.txt
+-rw-rw-rw-  2.0 unx    11496 b- defN 23-Apr-11 21:04 NEMO_billing/invoices/templates/invoices/project/edit_project.html
+-rw-rw-rw-  2.0 unx     3069 b- defN 23-Apr-11 21:04 NEMO_billing/invoices/templates/invoices/project/view_project_additional_info.html
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 21:04 NEMO_billing/invoices/views/__init__.py
+-rw-r--r--  2.0 unx    18824 b- defN 23-Apr-11 21:04 NEMO_billing/invoices/views/invoices.py
+-rw-r--r--  2.0 unx     6749 b- defN 23-Apr-11 21:04 NEMO_billing/invoices/views/project.py
+-rw-r--r--  2.0 unx     9105 b- defN 23-Apr-11 21:04 NEMO_billing/invoices/views/usage.py
+-rw-r--r--  2.0 unx     3156 b- defN 23-Apr-11 21:04 NEMO_billing/migrations/0001_initial.py
+-rw-r--r--  2.0 unx      573 b- defN 23-Apr-11 21:04 NEMO_billing/migrations/0002_version_1_2_0.py
+-rw-r--r--  2.0 unx      466 b- defN 23-Apr-11 21:04 NEMO_billing/migrations/0003_version_2_0_0.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 21:04 NEMO_billing/migrations/__init__.py
+-rw-r--r--  2.0 unx        1 b- defN 23-Apr-11 21:04 NEMO_billing/rates/__init__.py
+-rw-r--r--  2.0 unx     8665 b- defN 23-Apr-11 21:04 NEMO_billing/rates/admin.py
+-rw-r--r--  2.0 unx     1935 b- defN 23-Apr-11 21:04 NEMO_billing/rates/api.py
+-rw-r--r--  2.0 unx      100 b- defN 23-Apr-11 21:04 NEMO_billing/rates/app_settings.py
+-rw-r--r--  2.0 unx      707 b- defN 23-Apr-11 21:04 NEMO_billing/rates/apps.py
+-rw-r--r--  2.0 unx      489 b- defN 23-Apr-11 21:04 NEMO_billing/rates/customization.py
+-rw-r--r--  2.0 unx     1913 b- defN 23-Apr-11 21:04 NEMO_billing/rates/model_diff.py
+-rw-r--r--  2.0 unx    22269 b- defN 23-Apr-11 21:04 NEMO_billing/rates/models.py
+-rw-r--r--  2.0 unx     4042 b- defN 23-Apr-11 21:04 NEMO_billing/rates/rates_class.py
+-rw-r--r--  2.0 unx      777 b- defN 23-Apr-11 21:04 NEMO_billing/rates/urls.py
+-rw-r--r--  2.0 unx    12329 b- defN 23-Apr-11 21:04 NEMO_billing/rates/views.py
+-rw-r--r--  2.0 unx     5101 b- defN 23-Apr-11 21:04 NEMO_billing/rates/migrations/0001_initial.py
+-rw-r--r--  2.0 unx      602 b- defN 23-Apr-11 21:04 NEMO_billing/rates/migrations/0002_version_1_15_0.py
+-rw-r--r--  2.0 unx     1999 b- defN 23-Apr-11 21:04 NEMO_billing/rates/migrations/0003_version_1_17_0.py
+-rw-r--r--  2.0 unx      421 b- defN 23-Apr-11 21:04 NEMO_billing/rates/migrations/0004_version_2_0_0.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 21:04 NEMO_billing/rates/migrations/__init__.py
+-rw-rw-rw-  2.0 unx       81 b- defN 23-Apr-11 21:04 NEMO_billing/rates/static/rates/rates.css
+-rw-rw-rw-  2.0 unx     1242 b- defN 23-Apr-11 21:04 NEMO_billing/rates/templates/customizations/customizations_billing_rates.html
+-rw-rw-rw-  2.0 unx      160 b- defN 23-Apr-11 21:04 NEMO_billing/rates/templates/rates/base.html
+-rw-rw-rw-  2.0 unx     6047 b- defN 23-Apr-11 21:04 NEMO_billing/rates/templates/rates/rate.html
+-rw-rw-rw-  2.0 unx     4968 b- defN 23-Apr-11 21:04 NEMO_billing/rates/templates/rates/rate_form_details.html
+-rw-rw-rw-  2.0 unx     4602 b- defN 23-Apr-11 21:04 NEMO_billing/rates/templates/rates/rates.html
+-rw-rw-rw-  2.0 unx      192 b- defN 23-Apr-11 21:04 NEMO_billing/templates/base/navbar.html
+-rw-rw-rw-  2.0 unx      461 b- defN 23-Apr-11 21:04 NEMO_billing/templates/base/navbar_billing.html
+-rw-rw-rw-  2.0 unx     8882 b- defN 23-Apr-11 21:04 NEMO_billing/templates/billing/custom_charge.html
+-rw-rw-rw-  2.0 unx     1856 b- defN 23-Apr-11 21:04 NEMO_billing/templates/billing/custom_charges.html
+-rw-rw-rw-  2.0 unx     1259 b- defN 23-Apr-11 21:04 NEMO_billing/templates/staff_charges/choose_project.html
+-rw-rw-rw-  2.0 unx     1979 b- defN 23-Apr-11 21:04 NEMO_billing/templates/staff_charges/new_custom_staff_charge.html
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 21:04 NEMO_billing/templatetags/__init__.py
+-rw-r--r--  2.0 unx     1013 b- defN 23-Apr-11 21:04 NEMO_billing/templatetags/billing_tags.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 21:04 NEMO_billing/tests/__init__.py
+-rw-r--r--  2.0 unx     3047 b- defN 23-Apr-11 21:04 NEMO_billing/tests/test_settings.py
+-rw-r--r--  2.0 unx     1472 b- defN 23-Apr-11 21:04 NEMO_billing/tests/test_urls.py
+-rw-r--r--  2.0 unx     1094 b- defN 23-Apr-11 21:04 NEMO_billing/tests/test_utilities.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 21:04 NEMO_billing/tests/cap/__init__.py
+-rw-r--r--  2.0 unx    19023 b- defN 23-Apr-11 21:04 NEMO_billing/tests/cap/test_cap_discount.py
+-rw-r--r--  2.0 unx    29198 b- defN 23-Apr-11 21:04 NEMO_billing/tests/cap/test_cap_invoicing.py
+-rw-r--r--  2.0 unx     4252 b- defN 23-Apr-11 21:04 NEMO_billing/tests/cap/test_cap_utilities.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 21:04 NEMO_billing/tests/rates/__init__.py
+-rw-r--r--  2.0 unx    26426 b- defN 23-Apr-11 21:04 NEMO_billing/tests/rates/test_rate_amount.py
+-rw-r--r--  2.0 unx    20895 b- defN 23-Apr-11 21:04 NEMO_billing/tests/rates/test_rate_time.py
+-rw-r--r--  2.0 unx     6164 b- defN 23-Apr-11 21:04 NEMO_billing/tests/rates/test_rate_uniqueness.py
+-rw-r--r--  2.0 unx    27008 b- defN 23-Apr-11 21:04 NEMO_billing/tests/rates/test_split_billables.py
+-rw-rw-rw-  2.0 unx     1074 b- defN 23-Apr-11 21:05 NEMO_billing-2.0.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5031 b- defN 23-Apr-11 21:05 NEMO_billing-2.0.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-11 21:05 NEMO_billing-2.0.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 23-Apr-11 21:05 NEMO_billing-2.0.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    12665 b- defN 23-Apr-11 21:05 NEMO_billing-2.0.0.dist-info/RECORD
+126 files, 589237 bytes uncompressed, 135404 bytes compressed:  77.0%
```

## zipnote {}

```diff
@@ -1,50 +1,116 @@
 Filename: NEMO_billing/__init__.py
 Comment: 
 
 Filename: NEMO_billing/admin.py
 Comment: 
 
+Filename: NEMO_billing/api.py
+Comment: 
+
 Filename: NEMO_billing/app_settings.py
 Comment: 
 
+Filename: NEMO_billing/apps.py
+Comment: 
+
+Filename: NEMO_billing/decorators.py
+Comment: 
+
+Filename: NEMO_billing/exceptions.py
+Comment: 
+
 Filename: NEMO_billing/models.py
 Comment: 
 
 Filename: NEMO_billing/urls.py
 Comment: 
 
+Filename: NEMO_billing/utilities.py
+Comment: 
+
 Filename: NEMO_billing/views.py
 Comment: 
 
+Filename: NEMO_billing/cap_discount/__init__.py
+Comment: 
+
+Filename: NEMO_billing/cap_discount/admin.py
+Comment: 
+
+Filename: NEMO_billing/cap_discount/app_settings.py
+Comment: 
+
+Filename: NEMO_billing/cap_discount/apps.py
+Comment: 
+
+Filename: NEMO_billing/cap_discount/customization.py
+Comment: 
+
+Filename: NEMO_billing/cap_discount/exceptions.py
+Comment: 
+
+Filename: NEMO_billing/cap_discount/models.py
+Comment: 
+
+Filename: NEMO_billing/cap_discount/processors.py
+Comment: 
+
+Filename: NEMO_billing/cap_discount/urls.py
+Comment: 
+
+Filename: NEMO_billing/cap_discount/views.py
+Comment: 
+
+Filename: NEMO_billing/cap_discount/migrations/0001_initial.py
+Comment: 
+
+Filename: NEMO_billing/cap_discount/migrations/0002_version_2_0_0.py
+Comment: 
+
+Filename: NEMO_billing/cap_discount/migrations/__init__.py
+Comment: 
+
+Filename: NEMO_billing/cap_discount/templates/cap_discount/usage_cap_discounts.html
+Comment: 
+
+Filename: NEMO_billing/cap_discount/templates/customizations/customizations_cap_discount.html
+Comment: 
+
 Filename: NEMO_billing/invoices/__init__.py
 Comment: 
 
 Filename: NEMO_billing/invoices/admin.py
 Comment: 
 
+Filename: NEMO_billing/invoices/api.py
+Comment: 
+
 Filename: NEMO_billing/invoices/app_settings.py
 Comment: 
 
-Filename: NEMO_billing/invoices/exceptions.py
+Filename: NEMO_billing/invoices/apps.py
 Comment: 
 
-Filename: NEMO_billing/invoices/invoice_data_processor.py
+Filename: NEMO_billing/invoices/customization.py
 Comment: 
 
-Filename: NEMO_billing/invoices/invoice_generator.py
+Filename: NEMO_billing/invoices/exceptions.py
 Comment: 
 
 Filename: NEMO_billing/invoices/models.py
 Comment: 
 
 Filename: NEMO_billing/invoices/pdf_utilities.py
 Comment: 
 
-Filename: NEMO_billing/invoices/tests.py
+Filename: NEMO_billing/invoices/processors.py
+Comment: 
+
+Filename: NEMO_billing/invoices/renderers.py
 Comment: 
 
 Filename: NEMO_billing/invoices/urls.py
 Comment: 
 
 Filename: NEMO_billing/invoices/utilities.py
 Comment: 
@@ -78,32 +144,56 @@
 
 Filename: NEMO_billing/invoices/migrations/0006_version_1_7_1.py
 Comment: 
 
 Filename: NEMO_billing/invoices/migrations/0007_version_1_8_0.py
 Comment: 
 
+Filename: NEMO_billing/invoices/migrations/0008_version_1_10_0.py
+Comment: 
+
+Filename: NEMO_billing/invoices/migrations/0009_version_1_23_0.py
+Comment: 
+
+Filename: NEMO_billing/invoices/migrations/0010_version_2_0_0.py
+Comment: 
+
 Filename: NEMO_billing/invoices/migrations/__init__.py
 Comment: 
 
 Filename: NEMO_billing/invoices/static/invoices/invoices.css
 Comment: 
 
+Filename: NEMO_billing/invoices/templates/customizations/customizations_billing.html
+Comment: 
+
+Filename: NEMO_billing/invoices/templates/customizations/customizations_invoices.html
+Comment: 
+
 Filename: NEMO_billing/invoices/templates/invoices/base.html
 Comment: 
 
 Filename: NEMO_billing/invoices/templates/invoices/invoice.html
 Comment: 
 
 Filename: NEMO_billing/invoices/templates/invoices/invoice_details.html
 Comment: 
 
 Filename: NEMO_billing/invoices/templates/invoices/invoices.html
 Comment: 
 
+Filename: NEMO_billing/invoices/templates/invoices/usage.html
+Comment: 
+
+Filename: NEMO_billing/invoices/templates/invoices/email/billing_project_expiration_reminder_email_message.html
+Comment: 
+
+Filename: NEMO_billing/invoices/templates/invoices/email/billing_project_expiration_reminder_email_subject.txt
+Comment: 
+
 Filename: NEMO_billing/invoices/templates/invoices/email/email_send_invoice_message.html
 Comment: 
 
 Filename: NEMO_billing/invoices/templates/invoices/email/email_send_invoice_reminder_message.html
 Comment: 
 
 Filename: NEMO_billing/invoices/templates/invoices/email/email_send_invoice_reminder_subject.txt
@@ -123,59 +213,83 @@
 
 Filename: NEMO_billing/invoices/views/invoices.py
 Comment: 
 
 Filename: NEMO_billing/invoices/views/project.py
 Comment: 
 
+Filename: NEMO_billing/invoices/views/usage.py
+Comment: 
+
 Filename: NEMO_billing/migrations/0001_initial.py
 Comment: 
 
 Filename: NEMO_billing/migrations/0002_version_1_2_0.py
 Comment: 
 
+Filename: NEMO_billing/migrations/0003_version_2_0_0.py
+Comment: 
+
 Filename: NEMO_billing/migrations/__init__.py
 Comment: 
 
 Filename: NEMO_billing/rates/__init__.py
 Comment: 
 
 Filename: NEMO_billing/rates/admin.py
 Comment: 
 
+Filename: NEMO_billing/rates/api.py
+Comment: 
+
 Filename: NEMO_billing/rates/app_settings.py
 Comment: 
 
+Filename: NEMO_billing/rates/apps.py
+Comment: 
+
+Filename: NEMO_billing/rates/customization.py
+Comment: 
+
 Filename: NEMO_billing/rates/model_diff.py
 Comment: 
 
 Filename: NEMO_billing/rates/models.py
 Comment: 
 
 Filename: NEMO_billing/rates/rates_class.py
 Comment: 
 
-Filename: NEMO_billing/rates/tests.py
-Comment: 
-
 Filename: NEMO_billing/rates/urls.py
 Comment: 
 
 Filename: NEMO_billing/rates/views.py
 Comment: 
 
 Filename: NEMO_billing/rates/migrations/0001_initial.py
 Comment: 
 
+Filename: NEMO_billing/rates/migrations/0002_version_1_15_0.py
+Comment: 
+
+Filename: NEMO_billing/rates/migrations/0003_version_1_17_0.py
+Comment: 
+
+Filename: NEMO_billing/rates/migrations/0004_version_2_0_0.py
+Comment: 
+
 Filename: NEMO_billing/rates/migrations/__init__.py
 Comment: 
 
 Filename: NEMO_billing/rates/static/rates/rates.css
 Comment: 
 
+Filename: NEMO_billing/rates/templates/customizations/customizations_billing_rates.html
+Comment: 
+
 Filename: NEMO_billing/rates/templates/rates/base.html
 Comment: 
 
 Filename: NEMO_billing/rates/templates/rates/rate.html
 Comment: 
 
 Filename: NEMO_billing/rates/templates/rates/rate_form_details.html
@@ -183,35 +297,83 @@
 
 Filename: NEMO_billing/rates/templates/rates/rates.html
 Comment: 
 
 Filename: NEMO_billing/templates/base/navbar.html
 Comment: 
 
+Filename: NEMO_billing/templates/base/navbar_billing.html
+Comment: 
+
 Filename: NEMO_billing/templates/billing/custom_charge.html
 Comment: 
 
 Filename: NEMO_billing/templates/billing/custom_charges.html
 Comment: 
 
 Filename: NEMO_billing/templates/staff_charges/choose_project.html
 Comment: 
 
 Filename: NEMO_billing/templates/staff_charges/new_custom_staff_charge.html
 Comment: 
 
-Filename: NEMO_billing-1.9.1.dist-info/LICENSE
+Filename: NEMO_billing/templatetags/__init__.py
+Comment: 
+
+Filename: NEMO_billing/templatetags/billing_tags.py
+Comment: 
+
+Filename: NEMO_billing/tests/__init__.py
+Comment: 
+
+Filename: NEMO_billing/tests/test_settings.py
+Comment: 
+
+Filename: NEMO_billing/tests/test_urls.py
+Comment: 
+
+Filename: NEMO_billing/tests/test_utilities.py
+Comment: 
+
+Filename: NEMO_billing/tests/cap/__init__.py
+Comment: 
+
+Filename: NEMO_billing/tests/cap/test_cap_discount.py
+Comment: 
+
+Filename: NEMO_billing/tests/cap/test_cap_invoicing.py
+Comment: 
+
+Filename: NEMO_billing/tests/cap/test_cap_utilities.py
+Comment: 
+
+Filename: NEMO_billing/tests/rates/__init__.py
+Comment: 
+
+Filename: NEMO_billing/tests/rates/test_rate_amount.py
+Comment: 
+
+Filename: NEMO_billing/tests/rates/test_rate_time.py
+Comment: 
+
+Filename: NEMO_billing/tests/rates/test_rate_uniqueness.py
+Comment: 
+
+Filename: NEMO_billing/tests/rates/test_split_billables.py
+Comment: 
+
+Filename: NEMO_billing-2.0.0.dist-info/LICENSE
 Comment: 
 
-Filename: NEMO_billing-1.9.1.dist-info/METADATA
+Filename: NEMO_billing-2.0.0.dist-info/METADATA
 Comment: 
 
-Filename: NEMO_billing-1.9.1.dist-info/WHEEL
+Filename: NEMO_billing-2.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: NEMO_billing-1.9.1.dist-info/top_level.txt
+Filename: NEMO_billing-2.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: NEMO_billing-1.9.1.dist-info/RECORD
+Filename: NEMO_billing-2.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## NEMO_billing/__init__.py

```diff
@@ -1,27 +0,0 @@
-00000000: 6672 6f6d 2064 6a61 6e67 6f2e 6170 7073  from django.apps
-00000010: 2069 6d70 6f72 7420 4170 7043 6f6e 6669   import AppConfi
-00000020: 670a 0a66 726f 6d20 2e20 696d 706f 7274  g..from . import
-00000030: 2061 7070 5f73 6574 7469 6e67 7320 6173   app_settings as
-00000040: 2064 6566 6175 6c74 730a 6672 6f6d 2064   defaults.from d
-00000050: 6a61 6e67 6f2e 636f 6e66 2069 6d70 6f72  jango.conf impor
-00000060: 7420 7365 7474 696e 6773 0a0a 2320 5365  t settings..# Se
-00000070: 7420 736f 6d65 2061 7070 2064 6566 6175  t some app defau
-00000080: 6c74 2073 6574 7469 6e67 730a 666f 7220  lt settings.for 
-00000090: 6e61 6d65 2069 6e20 6469 7228 6465 6661  name in dir(defa
-000000a0: 756c 7473 293a 0a20 2020 2069 6620 6e61  ults):.    if na
-000000b0: 6d65 2e69 7375 7070 6572 2829 2061 6e64  me.isupper() and
-000000c0: 206e 6f74 2068 6173 6174 7472 2873 6574   not hasattr(set
-000000d0: 7469 6e67 732c 206e 616d 6529 3a0a 2020  tings, name):.  
-000000e0: 2020 2020 2020 7365 7461 7474 7228 7365        setattr(se
-000000f0: 7474 696e 6773 2c20 6e61 6d65 2c20 6765  ttings, name, ge
-00000100: 7461 7474 7228 6465 6661 756c 7473 2c20  tattr(defaults, 
-00000110: 6e61 6d65 2929 0a0a 0a63 6c61 7373 204e  name))...class N
-00000120: 454d 4f42 696c 6c69 6e67 436f 6e66 6967  EMOBillingConfig
-00000130: 2841 7070 436f 6e66 6967 293a 0a20 2020  (AppConfig):.   
-00000140: 206e 616d 6520 3d20 224e 454d 4f5f 6269   name = "NEMO_bi
-00000150: 6c6c 696e 6722 0a20 2020 2076 6572 626f  lling".    verbo
-00000160: 7365 5f6e 616d 6520 3d20 2242 696c 6c69  se_name = "Billi
-00000170: 6e67 220a 0a0a 6465 6661 756c 745f 6170  ng"...default_ap
-00000180: 705f 636f 6e66 6967 203d 2022 4e45 4d4f  p_config = "NEMO
-00000190: 5f62 696c 6c69 6e67 2e4e 454d 4f42 696c  _billing.NEMOBil
-000001a0: 6c69 6e67 436f 6e66 6967 220a            lingConfig".
```

## NEMO_billing/admin.py

```diff
@@ -1,21 +1,23 @@
 from copy import deepcopy
 from typing import Optional
 
-from NEMO.admin import ToolAdminForm, ToolAdmin, AreaAdminForm, AreaAdmin, ConsumableAdmin, StaffChargeAdmin
-from NEMO.models import Tool, Consumable, Area, StaffCharge
+from NEMO.admin import AreaAdmin, AreaAdminForm, ConsumableAdmin, StaffChargeAdmin, ToolAdmin, ToolAdminForm
+from NEMO.models import Area, Consumable, StaffCharge, Tool
 from django import forms
 from django.conf import settings
 from django.contrib import admin
 from django.contrib.admin import register
 from django.contrib.admin.widgets import FilteredSelectMultiple
 from django.core.exceptions import ValidationError
 from django.db.models import Q
 
 from NEMO_billing.models import CoreFacility, CoreRelationship, CustomCharge
+from NEMO_billing.templatetags.billing_tags import cap_discount_installed
+from NEMO_billing.utilities import hide_form_field
 
 
 def changed_or_added(change, original_set, current_set):
     # If the model object is being changed then we can get the list of previous members.
     if change:
         original_members = set(original_set)
     else:  # The model object is being created (instead of changed) so we can assume there are no members (initially).
@@ -24,15 +26,15 @@
     added_members = []
     removed_members = []
 
     # Log membership changes if they occurred.
     symmetric_difference = original_members ^ current_members
     if symmetric_difference:
         if change:  # the members have changed, so find out what was added and removed...
-            # We can can see the previous members of the object model by looking it up
+            # We can see the previous members of the object model by looking it up
             # in the database because the member list hasn't been committed yet.
             added_members = set(current_members) - set(original_members)
             removed_members = set(original_members) - set(current_members)
 
         else:  # a model object is being created (instead of changed) so we can assume all the members are new...
             added_members = current_set
     return added_members, removed_members
@@ -82,15 +84,18 @@
     )
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         # We are filtering out already set tools, areas and consumables
         no_facility_filter = Q(core_rel__isnull=True)
         tool_filter = Q(core_rel__in=self.instance.corerelationship_set.filter(tool__isnull=False))
-        self.fields["core_facility_tools"].queryset = Tool.objects.filter(tool_filter | no_facility_filter)
+        # Exclude children tools since their core facility is their parent's
+        self.fields["core_facility_tools"].queryset = Tool.objects.filter(tool_filter | no_facility_filter).exclude(
+            parent_tool__isnull=False
+        )
         area_filter = Q(core_rel__in=self.instance.corerelationship_set.filter(area__isnull=False))
         self.fields["core_facility_areas"].queryset = Area.objects.filter(area_filter | no_facility_filter)
         consumable_filter = Q(core_rel__in=self.instance.corerelationship_set.filter(consumable__isnull=False))
         self.fields["core_facility_consumables"].queryset = Consumable.objects.filter(
             consumable_filter | no_facility_filter
         )
         if self.instance.pk:
@@ -123,30 +128,37 @@
                 form.cleaned_data["core_facility_consumables"], original_items, obj, "consumable", change
             )
 
 
 class NewToolAdminForm(ToolAdminForm):
     core_facility = forms.ModelChoiceField(
         queryset=CoreFacility.objects.all(),
-        required=settings.TOOL_CORE_FACILITY_REQUIRED,
+        required=False,
         help_text="The core facility this tool belongs to. Used for billing purposes.",
     )
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         if self.instance.pk:
             self.fields["core_facility"].initial = self.instance.core_facility
 
+    def clean_core_facility(self):
+        parent_tool = self.cleaned_data.get("parent_tool")
+        core_facility = self.cleaned_data.get("core_facility")
+        if not parent_tool and not core_facility and settings.TOOL_CORE_FACILITY_REQUIRED:
+            raise ValidationError("This field is required.")
+        return core_facility
+
 
 class NewToolAdmin(ToolAdmin):
     form = NewToolAdminForm
 
     def save_model(self, request, obj: Tool, form, change):
         super().save_model(request, obj, form, change)
-        save_or_delete_core_facility(obj, form.cleaned_data["core_facility"], "tool")
+        save_or_delete_core_facility(obj, form.cleaned_data.get("core_facility"), "tool")
 
     def get_fieldsets(self, request, obj: Area = None):
         # Add core_facility field
         fieldsets = deepcopy(super().get_fieldsets(request, obj))
         fieldsets[0][1]["fields"] = fieldsets[0][1]["fields"] + ("core_facility",)
         return fieldsets
 
@@ -227,19 +239,18 @@
 
     core_facility = forms.ModelChoiceField(
         queryset=CoreFacility.objects.all(),
         required=settings.CUSTOM_CHARGE_CORE_FACILITY_REQUIRED,
         help_text="The core facility this tool belongs to. Used for billing purposes.",
     )
 
-    def clean_amount(self):
-        amount = self.cleaned_data["amount"]
-        if amount == 0:
-            raise ValidationError("Please enter a positive or negative amount")
-        return amount
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        if not cap_discount_installed():
+            hide_form_field(self, "cap_eligible")
 
 
 @register(CustomCharge)
 class CustomChargeAdmin(admin.ModelAdmin):
     list_display = ("name", "date", "amount", "customer", "project", "amount", "creator", "core_facility")
     search_fields = ("name", "customer__first_name", "customer__last_name", "customer__username", "project__name")
     list_filter = ("date", "project", "core_facility")
```

## NEMO_billing/models.py

```diff
@@ -1,39 +1,45 @@
-from NEMO.models import Tool, Consumable, Area, User, Project, StaffCharge
+from NEMO.models import Area, BaseModel, Consumable, Project, StaffCharge, Tool, User
+from django.core.exceptions import ValidationError
 from django.db import models
 
+from NEMO_billing.invoices.models import BillableItemType
+from NEMO_billing.templatetags.billing_tags import cap_discount_installed
 
-class CoreFacility(models.Model):
+
+class CoreFacility(BaseModel):
     name = models.CharField(max_length=200, unique=True, help_text="The name of this core facility.")
 
     def __str__(self):
         return self.name
 
     class Meta:
         ordering = ["name"]
         verbose_name_plural = "Core facilities"
 
 
-class CoreRelationship(models.Model):
+class CoreRelationship(BaseModel):
     core_facility = models.ForeignKey(CoreFacility, on_delete=models.CASCADE)
     tool = models.OneToOneField(Tool, related_name="core_rel", blank=True, null=True, on_delete=models.CASCADE)
     area = models.OneToOneField(Area, related_name="core_rel", blank=True, null=True, on_delete=models.CASCADE)
-    staff_charge = models.OneToOneField(StaffCharge, related_name="core_rel", blank=True, null=True, on_delete=models.CASCADE)
+    staff_charge = models.OneToOneField(
+        StaffCharge, related_name="core_rel", blank=True, null=True, on_delete=models.CASCADE
+    )
     consumable = models.OneToOneField(
         Consumable, related_name="core_rel", blank=True, null=True, on_delete=models.CASCADE
     )
 
     def get_item(self):
-        return self.area if self.area else self.tool if self.tool else self.consumable
+        return self.area or self.tool or self.consumable or self.staff_charge
 
     def __str__(self):
         return f"{self.get_item()} - {self.core_facility}"
 
 
-class CustomCharge(models.Model):
+class CustomCharge(BaseModel):
     name = models.CharField(max_length=255, help_text="The name of this custom charge.")
     additional_details = models.CharField(
         max_length=255, null=True, blank=True, help_text="Additional details for this charge."
     )
     customer = models.ForeignKey(
         User, related_name="custom_charge_customer", on_delete=models.CASCADE, help_text="The customer to charge."
     )
@@ -41,23 +47,55 @@
         User,
         related_name="custom_charge_creator",
         on_delete=models.CASCADE,
         help_text="The person who created this charge.",
     )
     project = models.ForeignKey(Project, on_delete=models.CASCADE, help_text="The project to bill for this charge.")
     date = models.DateTimeField(help_text="The date of the custom charge.")
-    amount = models.DecimalField(decimal_places=2, max_digits=8, help_text="The amount of the charge. Use a negative amount for adjustments.")
+    amount = models.DecimalField(
+        decimal_places=2, max_digits=8, help_text="The amount of the charge. Use a negative amount for adjustments."
+    )
     core_facility = models.ForeignKey(CoreFacility, null=True, blank=True, on_delete=models.SET_NULL)
+    cap_eligible = models.BooleanField(default=False, help_text="Check this box to make this charge count towards CAP")
+
+    def clean(self):
+        errors = {}
+        if self.amount == 0:
+            errors["amount"] = "Please enter a positive or negative amount"
+        if cap_discount_installed():
+            # If this custom charge is cap eligible, check that there is actually a matching CAP configuration
+            if self.cap_eligible:
+                if self.customer_id and self.project_id:
+                    from NEMO_billing.cap_discount.models import CAPDiscountConfiguration
+
+                    rate_category = self.project.projectbillingdetails.category
+                    cap_filter = CAPDiscountConfiguration.objects.filter(
+                        rate_category=rate_category,
+                        charge_types__contains=BillableItemType.CUSTOM_CHARGE.value,
+                    )
+                    if self.core_facility:
+                        cap_filter = cap_filter.filter(core_facility=self.core_facility)
+                    else:
+                        cap_filter = cap_filter.filter(core_facility__isnull=True)
+                    if not cap_filter.exists():
+                        errors[
+                            "cap_eligible"
+                        ] = f"No CAP configuration accepting Custom charges exists for this rate category ({rate_category})"
+        if errors:
+            raise ValidationError(errors)
 
     def __str__(self):
         return self.name
 
 
 # Create and add a shortcut function to get core_facility from Tool, Consumable, Area or Staff Charge
 def get_core_facility(self):
+    # Add an exception for tool children, whose core facility is the parent's core facility
+    if isinstance(self, Tool) and self.is_child_tool():
+        return self.parent_tool.core_facility
     if hasattr(self, "core_rel"):
         return self.core_rel.core_facility
 
 
 setattr(Tool, "core_facility", property(get_core_facility))
 setattr(Consumable, "core_facility", property(get_core_facility))
 setattr(Area, "core_facility", property(get_core_facility))
```

## NEMO_billing/urls.py

```diff
@@ -1,15 +1,20 @@
+from NEMO.urls import router
 from django.urls import path
 
-from NEMO_billing import views
+from NEMO_billing import api, views
+
+# Rest API URLs
+router.register(r"custom_charges", api.CustomChargeViewSet)
 
 urlpatterns = [
     path("custom_charges/", views.custom_charges, name="custom_charges"),
     path("custom_charge/", views.create_or_modify_custom_charge, name="create_custom_charge"),
     path("custom_charge/<int:custom_charge_id>", views.create_or_modify_custom_charge, name="edit_custom_charge"),
+    path("get_projects_for_custom_charges/", views.get_projects_for_custom_charges, name="get_projects_for_custom_charges"),
 
     # Overriding NEMO create staff charge URLs to add core facility selection
     path("staff_charges/", views.custom_staff_charges, name="staff_charges"),
     path("begin_staff_charge/", views.custom_begin_staff_charge, name="begin_staff_charge"),
 
     # Overriding NEMO enable tool URL to set the core facility on staff charge based on the tool's core facility
     path("enable_tool/<int:tool_id>/user/<int:user_id>/project/<int:project_id>/staff_charge/<str:staff_charge>/", views.custom_enable_tool, name="enable_tool"),
```

## NEMO_billing/views.py

```diff
@@ -1,40 +1,48 @@
 from http import HTTPStatus
 
+from NEMO.decorators import (
+    accounting_or_user_office_or_manager_required,
+    any_staff_required,
+    staff_member_required,
+    synchronized,
+)
 from NEMO.exceptions import ProjectChargeException
-from NEMO.models import User, StaffCharge, Project, Tool, AreaAccessRecord, UsageEvent
-from NEMO.tasks import synchronized
+from NEMO.models import AreaAccessRecord, Project, StaffCharge, Tool, UsageEvent, User
+from NEMO.views.get_projects import get_projects
 from NEMO.views.pagination import SortedPaginator
-from NEMO.views.policy import check_billing_to_project, check_policy_to_enable_tool
-from NEMO.views.staff_charges import staff_charges
+from NEMO.policy import policy_class as policy
+try:
+    from NEMO.views.staff_charges import staff_charges
+except ModuleNotFoundError:
+    from NEMO.views.remote_work import staff_charges
 from NEMO.views.tool_control import interlock_bypass_allowed, interlock_error
 from django.conf import settings
 from django.contrib import messages
-from django.contrib.admin.views.decorators import staff_member_required
 from django.contrib.auth.decorators import login_required
 from django.http import HttpResponseBadRequest
-from django.shortcuts import render, redirect, get_object_or_404
+from django.shortcuts import get_object_or_404, redirect, render
 from django.urls import reverse
-from django.views.decorators.http import require_http_methods, require_GET, require_POST
+from django.views.decorators.http import require_GET, require_POST, require_http_methods
 
 from NEMO_billing.admin import CustomChargeAdminForm, save_or_delete_core_facility
-from NEMO_billing.models import CustomCharge, CoreFacility
+from NEMO_billing.models import CoreFacility, CustomCharge
 
 
-@staff_member_required(login_url=None)
+@accounting_or_user_office_or_manager_required
 @require_http_methods(["GET", "POST"])
 def custom_charges(request):
     page = SortedPaginator(CustomCharge.objects.all(), request, order_by="-date").get_current_page()
     core_facilities_exist = CoreFacility.objects.exists()
     return render(
         request, "billing/custom_charges.html", {"page": page, "core_facilities_exist": core_facilities_exist}
     )
 
 
-@staff_member_required(login_url=None)
+@accounting_or_user_office_or_manager_required
 @require_http_methods(["GET", "POST"])
 def create_or_modify_custom_charge(request, custom_charge_id=None):
     custom_charge = None
     try:
         custom_charge = CustomCharge.objects.get(id=custom_charge_id)
     except CustomCharge.DoesNotExist:
         pass
@@ -57,15 +65,15 @@
             dictionary["projects"] = custom_charge.customer.active_projects()
         if hasattr(form, "cleaned_data") and "customer" in form.cleaned_data:
             dictionary["projects"] = form.cleaned_data["customer"].active_projects()
         return render(request, "billing/custom_charge.html", dictionary)
 
 
 # Overriding begin staff charge
-@staff_member_required(login_url=None)
+@staff_member_required
 @require_GET
 def custom_staff_charges(request):
     staff_member: User = request.user
     staff_charge: StaffCharge = staff_member.get_staff_charge()
     dictionary = dict()
     error = None
     customer = None
@@ -74,26 +82,29 @@
     except:
         pass
     if staff_charge:
         return staff_charges(request)
     if customer:
         if customer.active_project_count() > 0:
             dictionary["customer"] = customer
-            dictionary["core_facility_id"] = request.GET["core_facility"]
-            return render(request, "staff_charges/choose_project.html", dictionary)
+            dictionary["core_facility_id"] = request.GET.get("core_facility")
+            if not settings.STAFF_CHARGE_CORE_FACILITY_REQUIRED or dictionary["core_facility_id"]:
+                return render(request, "staff_charges/choose_project.html", dictionary)
+            else:
+                error = "you must select a core facility"
         else:
             error = str(customer) + " does not have any active projects. You cannot bill staff time to this user."
     dictionary["users"] = User.objects.filter(is_active=True).exclude(id=request.user.id)
     dictionary["core_facilities"] = CoreFacility.objects.all()
     dictionary["core_facility_required"] = settings.STAFF_CHARGE_CORE_FACILITY_REQUIRED
     dictionary["error"] = error
     return render(request, "staff_charges/new_custom_staff_charge.html", dictionary)
 
 
-@staff_member_required(login_url=None)
+@staff_member_required
 @require_POST
 def custom_begin_staff_charge(request):
     if request.user.charging_staff_time():
         return HttpResponseBadRequest("You cannot create a new staff charge when one is already in progress.")
     charge = StaffCharge()
     charge.customer = User.objects.get(id=request.POST["customer"])
     charge.project = Project.objects.get(id=request.POST["project"])
@@ -102,15 +113,15 @@
         core_facility = CoreFacility.objects.get(id=request.POST["core_facility"])
     except:
         pass
     if settings.STAFF_CHARGE_CORE_FACILITY_REQUIRED and not core_facility:
         return HttpResponseBadRequest("You cannot create a new staff charge without a core facility.")
     # Check if we are allowed to bill to project
     try:
-        check_billing_to_project(charge.project, charge.customer, charge)
+        policy.check_billing_to_project(charge.project, charge.customer, charge)
     except ProjectChargeException as e:
         return HttpResponseBadRequest(e.msg)
     charge.staff_member = request.user
     charge.save()
     if core_facility:
         save_or_delete_core_facility(charge, core_facility, "staff_charge")
     return redirect(reverse("staff_charges"))
@@ -128,15 +139,15 @@
 
     tool = get_object_or_404(Tool, id=tool_id)
     operator = request.user
     user = get_object_or_404(User, id=user_id)
     project = get_object_or_404(Project, id=project_id)
     staff_charge = staff_charge == "true"
     bypass_interlock = request.POST.get("bypass", "False") == "True"
-    response = check_policy_to_enable_tool(tool, operator, user, project, staff_charge)
+    response = policy.check_to_enable_tool(tool, operator, user, project, staff_charge)
     if response.status_code != HTTPStatus.OK:
         return response
 
     # All policy checks passed so enable the tool for the user.
     if tool.interlock and not tool.interlock.unlock():
         if bypass_interlock and interlock_bypass_allowed(user):
             pass
@@ -166,7 +177,13 @@
     new_usage_event.operator = operator
     new_usage_event.user = user
     new_usage_event.project = project
     new_usage_event.tool = tool
     new_usage_event.save()
 
     return response
+
+
+@any_staff_required
+@require_GET
+def get_projects_for_custom_charges(request):
+    return get_projects(request)
```

## NEMO_billing/invoices/__init__.py

```diff
@@ -1,29 +0,0 @@
-00000000: 6672 6f6d 2064 6a61 6e67 6f2e 6170 7073  from django.apps
-00000010: 2069 6d70 6f72 7420 4170 7043 6f6e 6669   import AppConfi
-00000020: 670a 0a66 726f 6d20 2e20 696d 706f 7274  g..from . import
-00000030: 2061 7070 5f73 6574 7469 6e67 7320 6173   app_settings as
-00000040: 2064 6566 6175 6c74 730a 6672 6f6d 2064   defaults.from d
-00000050: 6a61 6e67 6f2e 636f 6e66 2069 6d70 6f72  jango.conf impor
-00000060: 7420 7365 7474 696e 6773 0a0a 2320 5365  t settings..# Se
-00000070: 7420 736f 6d65 2061 7070 2064 6566 6175  t some app defau
-00000080: 6c74 2073 6574 7469 6e67 730a 666f 7220  lt settings.for 
-00000090: 6e61 6d65 2069 6e20 6469 7228 6465 6661  name in dir(defa
-000000a0: 756c 7473 293a 0a20 2020 2069 6620 6e61  ults):.    if na
-000000b0: 6d65 2e69 7375 7070 6572 2829 2061 6e64  me.isupper() and
-000000c0: 206e 6f74 2068 6173 6174 7472 2873 6574   not hasattr(set
-000000d0: 7469 6e67 732c 206e 616d 6529 3a0a 2020  tings, name):.  
-000000e0: 2020 2020 2020 7365 7461 7474 7228 7365        setattr(se
-000000f0: 7474 696e 6773 2c20 6e61 6d65 2c20 6765  ttings, name, ge
-00000100: 7461 7474 7228 6465 6661 756c 7473 2c20  tattr(defaults, 
-00000110: 6e61 6d65 2929 0a0a 0a63 6c61 7373 204e  name))...class N
-00000120: 454d 4f49 6e76 6f69 6365 7343 6f6e 6669  EMOInvoicesConfi
-00000130: 6728 4170 7043 6f6e 6669 6729 3a0a 2020  g(AppConfig):.  
-00000140: 2020 6e61 6d65 203d 2022 4e45 4d4f 5f62    name = "NEMO_b
-00000150: 696c 6c69 6e67 2e69 6e76 6f69 6365 7322  illing.invoices"
-00000160: 0a20 2020 2076 6572 626f 7365 5f6e 616d  .    verbose_nam
-00000170: 6520 3d20 2249 6e76 6f69 6365 7322 0a0a  e = "Invoices"..
-00000180: 0a64 6566 6175 6c74 5f61 7070 5f63 6f6e  .default_app_con
-00000190: 6669 6720 3d20 224e 454d 4f5f 6269 6c6c  fig = "NEMO_bill
-000001a0: 696e 672e 696e 766f 6963 6573 2e4e 454d  ing.invoices.NEM
-000001b0: 4f49 6e76 6f69 6365 7343 6f6e 6669 6722  OInvoicesConfig"
-000001c0: 0a                                       .
```

## NEMO_billing/invoices/admin.py

```diff
@@ -1,21 +1,67 @@
 from NEMO.admin import ProjectAdmin
 from NEMO.models import Project
+from NEMO.utilities import format_datetime
+from django.apps import apps
 from django.contrib import admin
-from django.contrib.admin import register, SimpleListFilter
+from django.contrib.admin import SimpleListFilter, register
+from django.contrib.contenttypes.models import ContentType
+from django.db.models.functions import Length
+from django.urls import NoReverseMatch, reverse
+from django.utils.html import format_html
 
 from NEMO_billing.invoices.models import (
     Invoice,
     InvoiceConfiguration,
-    ProjectBillingDetails,
+    InvoiceDetailItem,
     InvoicePayment,
     InvoiceSummaryItem,
-    InvoiceDetailItem,
+    ProjectBillingDetails,
 )
-from NEMO_billing.invoices.views.invoices import zip_response, review_invoice, void_invoice, send_invoice
+from NEMO_billing.invoices.processors import invoice_data_processor_class as data_processor
+from NEMO_billing.invoices.views.invoices import (
+    delete_invoice,
+    review_invoice,
+    send_invoice,
+    void_invoice,
+    zip_response,
+)
+
+
+def clone_project(project: Project):
+    """
+    Create a clone of selected projects and save them.
+
+    :param project:
+    :return: Newly cloned project
+    """
+    project_details = getattr(project, "projectbillingdetails", None)
+    # Only copy active users and PIs
+    project_users = project.user_set.filter(is_active=True)
+    project_pis = project.manager_set.filter(is_active=True)
+    only_allow_tools = project.only_allow_tools.all()
+    new_project = project
+    new_project.pk = None
+    new_project.name = f"Copy of {project.name}"
+    new_project.save()
+    # Set relations
+    new_project.user_set.set(project_users)
+    new_project.manager_set.set(project_pis)
+    new_project.only_allow_tools.set(only_allow_tools)
+    if project_details:
+        project_details.pk = None
+        project_details.project = new_project
+        project_details.save()
+    return project
+
+
+@admin.action(description="Clone selected projects")
+def clone_projects(modeladmin, request, queryset):
+    for project in queryset.all():
+        clone_project(project)
 
 
 def clone_configuration(configuration: InvoiceConfiguration):
     """
     Create a clone of selected configurations and save them.
 
     :param configuration:
@@ -24,51 +70,46 @@
     configuration.pk = None
     configuration.name = f"Copy of {configuration.name}"
     configuration.save()
 
     return configuration
 
 
+@admin.action(description="Clone selected Configurations")
 def clone_configurations(modeladmin, request, queryset):
     for configuration in queryset.all():
         clone_configuration(configuration)
 
 
-clone_configurations.short_description = "Clone selected Configurations"
-
-
+@admin.action(description="Email selected invoices to customers")
 def email_invoices(modeladmin, request, queryset):
     for invoice in queryset.all():
         send_invoice(request, invoice.id)
 
 
-email_invoices.short_description = "Email selected invoices to customers"
-
-
+@admin.action(description="Mark selected invoices as reviewed")
 def review_invoices(modeladmin, request, queryset):
     for invoice in queryset.all():
         review_invoice(request, invoice.id)
 
 
-review_invoices.short_description = "Mark selected invoices as reviewed"
-
-
+@admin.action(description="Mark selected invoices as void")
 def void_invoices(modeladmin, request, queryset):
     for invoice in queryset.all():
         void_invoice(request, invoice.id)
 
 
-void_invoices.short_description = "Mark selected invoices as void"
-
-
+@admin.action(description="Download selected invoices")
 def zip_invoices(modeladmin, request, queryset):
     return zip_response(request, queryset.all())
 
 
-zip_invoices.short_description = "Download selected invoices"
+@admin.action(description="Export invoice data in CSV")
+def zip_invoices_csv(modeladmin, request, queryset):
+    return zip_response(request, queryset.all(), "csv")
 
 
 class InvoiceSummaryItemInline(admin.TabularInline):
     model = InvoiceSummaryItem
     can_delete = False
 
     def has_change_permission(self, request, obj=None):
@@ -77,21 +118,45 @@
     def has_add_permission(self, request, obj=None):
         return False
 
 
 class InvoiceDetailItemInline(admin.TabularInline):
     model = InvoiceDetailItem
     can_delete = False
+    exclude = ("content_type", "object_id")
+    readonly_fields = ("get_item",)
+    fields = ("get_item", "core_facility", "item_type", "name", "quantity", "start", "end", "user", "rate", "amount")
 
     def has_change_permission(self, request, obj=None):
         return False
 
     def has_add_permission(self, request, obj=None):
         return False
 
+    @admin.display(description="Item")
+    def get_item(self, obj: InvoiceDetailItem):
+        if not obj.content_type or not obj.object_id:
+            return "-"
+        app_label, model = obj.content_type.app_label, obj.content_type.model
+        viewname = f"admin:{app_label}_{model}_change"
+        try:
+            args = [obj.object_id]
+            link = reverse(viewname, args=args)
+        except NoReverseMatch:
+            return "-"
+        else:
+            return format_html('<a href="{}">{} - #{}</a>', link, self.get_model_name(obj.content_type), obj.object_id)
+
+    def get_model_name(self, content_type: ContentType):
+        try:
+            model = apps.get_model(content_type.app_label, content_type.model)
+            return model._meta.verbose_name.capitalize()
+        except (LookupError, AttributeError):
+            return ""
+
 
 class InvoiceStatusFilter(SimpleListFilter):
     title = "status"
     parameter_name = "status"
 
     def lookups(self, request, model_admin):
         return [
@@ -119,40 +184,61 @@
 
 
 @register(Invoice)
 class InvoiceAdmin(admin.ModelAdmin):
     inlines = (InvoiceSummaryItemInline, InvoiceDetailItemInline)
     list_display = (
         "invoice_number",
+        "get_invoice_date",
         "get_total_amount_currency",
         "get_tax_display",
         "project_details",
         "configuration",
         "created_date",
         "due_date",
         "last_sent_date",
         "reviewed_date",
         "voided_date",
         "file",
     )
-    list_filter = (InvoiceStatusFilter, "due_date", "configuration__currency")
-    ordering = ("-invoice_number",)
+    list_filter = (
+        InvoiceStatusFilter,
+        "start",
+        "due_date",
+        "configuration__currency",
+        "project_details__project__name",
+    )
+    ordering = (Length("invoice_number").desc(), "-invoice_number")
     readonly_fields = ("created_by", "created_date")
-    actions = (email_invoices, review_invoices, void_invoices, zip_invoices)
+    date_hierarchy = "start"
+    search_fields = ["invoice_number", "project_details__project__name"]
+    actions = (email_invoices, review_invoices, void_invoices, zip_invoices, zip_invoices_csv)
+
+    @admin.display(description="Date", ordering="start")
+    def get_invoice_date(self, obj: Invoice):
+        return format_datetime(obj.start, "F Y")
 
+    @admin.display(description="Amount", ordering="total_amount")
     def get_total_amount_currency(self, obj: Invoice):
         return obj.total_amount_display()
 
-    get_total_amount_currency.admin_order_field = "total_amount"
-    get_total_amount_currency.short_description = "Amount"
-
+    @admin.display(description="Tax")
     def get_tax_display(self, obj: Invoice):
         return obj.tax_display()
 
-    get_tax_display.short_description = "Tax"
+    def delete_queryset(self, request, queryset):
+        for invoice in queryset:
+            if Invoice.objects.filter(id=invoice.id).exists():
+                delete_invoice(request, invoice.id)
+
+    def delete_model(self, request, obj: Invoice):
+        delete_invoice(request, obj.id)
+
+    def get_deleted_objects(self, objs, request):
+        return data_processor.get_deleted_objects(objs, request, self.admin_site)
 
 
 @register(InvoiceConfiguration)
 class InvoiceConfigurationAdmin(admin.ModelAdmin):
     list_display = ("id", "name", "merchant_name", "currency")
     ordering = ("name",)
     actions = (clone_configurations,)
@@ -178,30 +264,44 @@
         ),
     )
 
 
 @register(InvoicePayment)
 class InvoicePaymentAdmin(admin.ModelAdmin):
     readonly_fields = ("created_by", "created_date", "updated_by", "updated_date")
-    list_display = ("invoice", "payment_received", "payment_processed", "updated_by", "updated_date")
-    list_filter = ("invoice", "invoice__project_details__project__name")
+    list_display = (
+        "invoice",
+        "payment_received",
+        "payment_processed",
+        "get_amount_display",
+        "updated_by",
+        "updated_date",
+    )
+    list_filter = ("payment_received", "payment_processed", "invoice__project_details__project__name", "invoice")
+    date_hierarchy = "payment_received"
+
+    @admin.display(description="Amount", ordering="amount")
+    def get_amount_display(self, obj: InvoicePayment):
+        return obj.amount_display()
 
     def save_model(self, request, obj, form, change):
         if not change:
             obj.created_by = request.user
         obj.updated_by = request.user
         obj.save()
 
 
 class ProjectBillingDetailsInline(admin.StackedInline):
     model = ProjectBillingDetails
     can_delete = False
+    min_num = 1
     verbose_name_plural = "details"
 
 
 class NewProjectAdmin(ProjectAdmin):
-    inlines = (ProjectBillingDetailsInline,)
+    actions = list(ProjectAdmin.actions) + [clone_projects]
+    inlines = list(ProjectAdmin.inlines) + [ProjectBillingDetailsInline]
 
 
 # Re-register ProjectAdmin
 admin.site.unregister(Project)
 admin.site.register(Project, NewProjectAdmin)
```

## NEMO_billing/invoices/app_settings.py

```diff
@@ -1,10 +1,5 @@
-from datetime import datetime
-
 INVOICE_DATE_FORMAT = "%B %d, %Y"
 INVOICE_DATETIME_FORMAT = "%m/%d/%Y %H:%M:%S"
 INVOICE_EMAIL_SUBJECT_PREFIX = "[NEMO Billing] "
 
 INVOICE_ALL_ITEMS_MUST_BE_IN_FACILITY = False
-
-# Display all months since this date in generate invoice page
-INVOICE_MONTH_LIST_SINCE = datetime(year=2021, month=1, day=1)
```

## NEMO_billing/invoices/exceptions.py

```diff
@@ -1,51 +1,67 @@
-from NEMO.exceptions import NEMOException
-from NEMO.models import Tool, Area, Consumable, Project
-from NEMO_billing.invoices.models import Invoice, InvoiceDetailItem
+from NEMO.models import Area, Consumable, Project, Tool
 
+from NEMO_billing.exceptions import BillingException
+from NEMO_billing.invoices.models import Invoice, InvoiceDetailItem
 from NEMO_billing.rates.models import RateCategory, RateType
 
 
-class NoRateSetException(NEMOException):
+class NoRateSetException(BillingException):
     def __init__(
         self,
-        rate_type_id: int,
+        rate_type: RateType,
         category: RateCategory = None,
         tool: Tool = None,
         area: Area = None,
         consumable: Consumable = None,
     ):
-        self.rate_type = RateType.objects.get(id=rate_type_id)
+        self.rate_type = rate_type
         self.category = category
         self.tool = tool
         self.area = area
         self.consumable = consumable
         for_category = f" for category: {category}" if category else ""
         for_item = (
             f" for: {tool if tool else area if area else consumable if consumable else ''}"
             if tool or area or consumable
             else ""
         )
         msg = f"No {self.rate_type.get_type_display()} rate is set{for_item}{for_category}"
         super().__init__(msg)
 
 
-class NoProjectDetailsSetException(NEMOException):
+class NoProjectCategorySetException(BillingException):
+    def __init__(self, rate_type: RateType, project: Project):
+        self.rate_type = rate_type
+        self.project = project
+        msg = f"{self.rate_type.get_type_display()} is category specific but no category is set on project {project}"
+        super().__init__(msg)
+
+
+class NoProjectDetailsSetException(BillingException):
     def __init__(self, project: Project):
         self.project = project
-        msg = f"There are no project details set for project {project.name}"
+        msg = f"There are no project details set for project {project}"
         super().__init__(msg)
 
 
-class InvoiceAlreadyExistException(NEMOException):
+class InvoiceAlreadyExistException(BillingException):
     def __init__(self, invoice: Invoice):
         self.invoice = invoice
         msg = f"An invoice ({invoice.invoice_number}) already exist for this project for this date range. Void it to be able to generate it again"
         super().__init__(msg)
 
 
-class InvoiceItemsNotInFacilityException(NEMOException):
+class InvoiceItemsNotInFacilityException(BillingException):
     def __init__(self, item: InvoiceDetailItem):
         self.item = item
         item_type_display = item.get_item_type_display().replace("_", " ")
         msg = f"Error generating invoice. A {item_type_display}: {item.name} for user {item.user} is not part of any core facilities"
         super().__init__(msg)
+
+
+class InvoiceGenerationException(BillingException):
+    def __init__(self, invoice: Invoice, renderer, e: Exception):
+        self.invoice = invoice
+        self.renderer = renderer
+        msg = f"Error rendering invoice {invoice.invoice_number} with {renderer.__class__.__name__} for project {invoice.project_details.project_name}: {str(e)}."
+        super().__init__(msg)
```

## NEMO_billing/invoices/models.py

```diff
@@ -1,64 +1,105 @@
 import os
 from datetime import timedelta
 from decimal import Decimal
-from typing import List, Dict
+from enum import Enum, unique
+from logging import getLogger
+from typing import Dict, List
 
 from NEMO import fields
-from NEMO.models import Project, User, Customization, TaskImages
+from NEMO.models import BaseModel, Customization, Project, User
 from NEMO.utilities import create_email_attachment
+from django.contrib.contenttypes.fields import GenericForeignKey
+from django.contrib.contenttypes.models import ContentType
 from django.core.exceptions import ValidationError
+from django.core.files.base import ContentFile
 from django.db import models
-from django.db.models import Sum, Case, When, DecimalField
+from django.db.models import Case, Sum, When
 from django.db.models.functions import Coalesce
 from django.urls import reverse
 from django.utils import timezone
 from django.utils.text import slugify
 
 from NEMO_billing.invoices.utilities import (
+    category_name_for_item_type,
+    display_amount,
+    export_invoice_filename,
     get_invoice_document_filename,
     get_merchant_logo_filename,
-    display_amount,
     render_and_send_email,
 )
-from NEMO_billing.models import CoreFacility
-from NEMO_billing.rates.models import Rate, RateCategory
+from NEMO_billing.rates.models import RateCategory
+
+
+@unique
+class BillableItemType(Enum):
+    TOOL_USAGE = 1
+    AREA_ACCESS = 2
+    CONSUMABLE = 3
+    MISSED_RESERVATION = 4
+    STAFF_CHARGE = 5
+    TRAINING = 6
+    CUSTOM_CHARGE = 7
+
+    @classmethod
+    def choices(cls):
+        return (
+            (cls.TOOL_USAGE.value, "tool_usage"),
+            (cls.AREA_ACCESS.value, "area_access"),
+            (cls.CONSUMABLE.value, "consumable"),
+            (cls.MISSED_RESERVATION.value, "missed_reservation"),
+            (cls.STAFF_CHARGE.value, "staff_charge"),
+            (cls.TRAINING.value, "training_session"),
+            (cls.CUSTOM_CHARGE.value, "custom_charge"),
+        )
 
+    def is_time_type(self):
+        return self in [
+            BillableItemType.TOOL_USAGE,
+            BillableItemType.AREA_ACCESS,
+            BillableItemType.TRAINING,
+            BillableItemType.STAFF_CHARGE,
+            BillableItemType.MISSED_RESERVATION,
+        ]
+
+    def display_name(self):
+        choices_as_dict = dict(self.choices())
+        return choices_as_dict.get(self.value)
 
-class ProjectBillingDetails(models.Model):
+    def category_name_for_item_type(self):
+        return category_name_for_item_type(self)
+
+
+class ProjectBillingDetails(BaseModel):
     project = models.OneToOneField(Project, on_delete=models.CASCADE)
     category = models.ForeignKey(RateCategory, null=True, blank=True, on_delete=models.SET_NULL)
     project_name = models.CharField(
         null=True,
         blank=True,
         max_length=200,
         help_text="The project name that will appear on the invoices. Leave blank to use NEMO project name",
     )
     contact_name = models.CharField(
         null=True, blank=True, max_length=255, help_text="The contact name to use in the invoice email"
     )
-    contact_phone = models.CharField(
-        null=True, blank=True, max_length=40, help_text="The contact's phone number"
-    )
+    contact_phone = models.CharField(null=True, blank=True, max_length=40, help_text="The contact's phone number")
     contact_email = fields.MultiEmailField(
         null=True,
         blank=True,
         help_text="Email to send the invoice to. A comma-separated list can be used. Leave blank to use project managers/PIs emails",
     )
     expires_on = models.DateField(
         null=True, blank=True, help_text="Date after which this project will be automatically deactivated."
     )
     addressee = models.TextField(null=True, blank=True, help_text="The addressee details to be included in the invoice")
     comments = models.TextField(null=True, blank=True)
     no_charge = models.BooleanField(
         default=False, help_text="Check this box if invoices should not be created for this project."
     )
-    no_tax = models.BooleanField(
-        default=False, help_text="Check this box if this project is tax exempt."
-    )
+    no_tax = models.BooleanField(default=False, help_text="Check this box if this project is tax exempt.")
 
     @property
     def name(self):
         return self.project_name if self.project_name else self.project.name
 
     def clean(self):
         if not self.category and RateCategory.objects.exists():
@@ -74,15 +115,15 @@
     def __str__(self):
         return self.name
 
     class Meta:
         verbose_name_plural = "Project details"
 
 
-class InvoiceConfiguration(models.Model):
+class InvoiceConfiguration(BaseModel):
     name = models.CharField(max_length=200, unique=True, help_text="The name of this invoice configuration")
     invoice_due_in = models.PositiveIntegerField(
         help_text="The default number of days invoices are due after", default=30
     )
     reminder_frequency = models.PositiveIntegerField(
         null=True,
         blank=True,
@@ -109,14 +150,15 @@
         null=True, blank=True, decimal_places=3, max_digits=5, help_text="Tax in percent. For 20.5% enter 20.5"
     )
     tax_name = models.CharField(max_length=50, null=True, blank=True, default="VAT")
 
     detailed_invoice = models.BooleanField(
         default=True, help_text="Check this box if customers should receive a detailed invoice."
     )
+    hide_zero_charge = models.BooleanField(default=True, help_text="Hide charges with an amount equal to 0.")
 
     separate_tool_usage_charges = models.BooleanField(
         default=False, help_text="Check this box to display tool usage charges as a separate invoice category"
     )
     separate_area_access_charges = models.BooleanField(
         default=False, help_text="Check this box to display area access charges as a separate invoice category"
     )
@@ -141,16 +183,25 @@
 
     def tax_amount(self):
         return self.tax / Decimal(100)
 
     def __str__(self):
         return self.name
 
+    @classmethod
+    def first_or_default(cls):
+        try:
+            if cls.objects.exists():
+                return cls.objects.first()
+        except Exception as e:
+            getLogger(__name__).warning(e)
+        return cls(currency="", currency_symbol="")
+
 
-class Invoice(models.Model):
+class Invoice(BaseModel):
     invoice_number = models.CharField(
         null=False, blank=True, max_length=100, unique=True, help_text="Leave blank to be assigned automatically"
     )
     start = models.DateTimeField()
     end = models.DateTimeField()
 
     configuration = models.ForeignKey(InvoiceConfiguration, on_delete=models.PROTECT)
@@ -171,47 +222,69 @@
 
     created_by = models.ForeignKey(User, on_delete=models.PROTECT)
     created_date = models.DateTimeField(auto_now_add=True)
 
     total_amount = models.DecimalField(decimal_places=2, max_digits=14)
 
     file = models.FileField(null=True, blank=True, max_length=255, upload_to=get_invoice_document_filename)
-    temp_file = None
 
     def generate_invoice_number(self, update: bool = False):
-        number_format = get_invoice_customization("invoice_number_format", "{:04d}")
+        from NEMO_billing.invoices.customization import InvoiceCustomization
+
+        number_format = InvoiceCustomization.get("invoice_number_format")
         current_number = 0
         try:
-            current_number = int(get_invoice_customization("invoice_number_current", "0"))
+            current_number = int(InvoiceCustomization.get("invoice_number_current"))
         except ValueError:
             pass
         current_number += 1
         if update:
             Customization.objects.update_or_create(
                 name="invoice_number_current", defaults={"value": str(current_number)}
             )
         return number_format.format(current_number)
 
     def save(self, *args, **kwargs):
         if not self.invoice_number:
             self.invoice_number = self.generate_invoice_number(True)
         super().save(*args, **kwargs)
 
+    def save_all(self, detail_items, summary_items):
+        # Save invoice, detail items and summary items
+        self.save()
+        for detail_item in detail_items:
+            detail_item.invoice = self
+            detail_item.save(force_insert=True)
+        for summary_item in summary_items:
+            summary_item.invoice = self
+            summary_item.save(force_insert=True)
+        # We want to generate/render the invoice now and save the file so that it is set once and for all
+        # (rather than generating it on the fly which would potentially use newer project info and config)
+        # if an error rendering happens, the file will need to be regenerated
+        self.render_and_save_file()
+
     def get_absolute_url(self):
         return reverse("invoice", kwargs={"invoice_id": self.id})
 
-    def filename(self):
-        return os.path.basename(self.file.name)
-
-    def filename_for_zip(self):
-        ext = os.path.splitext(self.filename())[1]
-        month = self.created_date.strftime("%B")
-        year = self.created_date.strftime("%Y")
-        name = slugify(self.project_details.name)
-        return f"{name}/{name}-{month}-{year}-{slugify(self.invoice_number)}." + ext
+    def filename(self, extension=None):
+        extension = f".{extension}" if extension else os.path.splitext(self.file.path)[1]
+        return f"{slugify(self.invoice_number)}_{slugify(self.project_details.name)}{extension}"
+
+    def filename_for_zip(self, extension=None):
+        extension = f".{extension}" if extension else os.path.splitext(self.file.path)[1]
+        return export_invoice_filename(self) + extension
+
+    def render_and_save_file(self):
+        from NEMO_billing.invoices.renderers import invoice_renderer_class
+
+        content = invoice_renderer_class.render_invoice(self)
+        content.seek(0)
+        self.file = ContentFile(content.read(), "invoice." + invoice_renderer_class.get_file_extension())
+        content.close()
+        self.save(update_fields=["file"])
 
     def _email_invoice(self, template_name) -> bool:
         attachment = create_email_attachment(self.file, self.filename())
         sent = render_and_send_email(
             template_name,
             {"invoice": self},
             to=self.project_details.email_to(),
@@ -239,16 +312,19 @@
                 # Invoice hasn't been paid in full, reminder should be sent
                 self.last_reminder_sent_date = timezone.now()
                 if self._email_invoice("invoices/email/email_send_invoice_reminder"):
                     self.save()
                     return True
         return False
 
-    def sorted_core_facilities(self):
-        core_facilities = list(self.invoicedetailitem_set.values_list("core_facility", flat=True).distinct())
+    def sorted_core_facilities(self, detail_items=None) -> List[str]:
+        if detail_items:
+            core_facilities = list({item.core_facility for item in detail_items})
+        else:
+            core_facilities = list(self.invoicedetailitem_set.values_list("core_facility", flat=True).distinct())
         core_facilities.sort(key=lambda x: x if x else "", reverse=True)
         return core_facilities
 
     def summary_dict(self) -> Dict[str, List]:
         summary_details = {}
         for core_facility in self.sorted_core_facilities():
             summary_details.setdefault(core_facility, self.invoicesummaryitem_set.filter(core_facility=core_facility))
@@ -269,65 +345,79 @@
             core_facility_items.setdefault("trainings", self.training_details(core_facility=core_facility))
             core_facility_items.setdefault(
                 "missed_reservations", self.missed_reservation_details(core_facility=core_facility)
             )
             core_facility_items.setdefault("custom_charges", self.custom_charges_details(core_facility=core_facility))
         return details
 
-    def tool_usage_details(self, core_facility: CoreFacility):
-        return self.invoicedetailitem_set.filter(
-            core_facility=core_facility, item_type=InvoiceDetailItem.InvoiceDetailItemType.TOOL_USAGE
-        ).order_by("start")
-
-    def area_access_details(self, core_facility: CoreFacility):
-        return self.invoicedetailitem_set.filter(
-            core_facility=core_facility, item_type=InvoiceDetailItem.InvoiceDetailItemType.AREA_ACCESS
-        ).order_by("start")
-
-    def staff_charge_details(self, core_facility: CoreFacility):
-        return self.invoicedetailitem_set.filter(
-            core_facility=core_facility, item_type=InvoiceDetailItem.InvoiceDetailItemType.STAFF_CHARGE
+    def invoice_details(self):
+        details = self.invoicedetailitem_set.all()
+        if self.configuration.hide_zero_charge:
+            details = details.exclude(amount=0)
+        return details
+
+    def tool_usage_details(self, core_facility: str):
+        return (
+            self.invoice_details()
+            .filter(core_facility=core_facility, item_type=BillableItemType.TOOL_USAGE.value)
+            .order_by("start")
+        )
+
+    def area_access_details(self, core_facility: str):
+        return (
+            self.invoice_details()
+            .filter(core_facility=core_facility, item_type=BillableItemType.AREA_ACCESS.value)
+            .order_by("start")
         )
 
-    def consumable_withdrawal_details(self, core_facility: CoreFacility):
-        return self.invoicedetailitem_set.filter(
-            core_facility=core_facility, item_type=InvoiceDetailItem.InvoiceDetailItemType.CONSUMABLE
-        ).order_by("start")
-
-    def training_details(self, core_facility: CoreFacility):
-        return self.invoicedetailitem_set.filter(
-            core_facility=core_facility, item_type=InvoiceDetailItem.InvoiceDetailItemType.TRAINING
-        ).order_by("start")
-
-    def missed_reservation_details(self, core_facility: CoreFacility):
-        return self.invoicedetailitem_set.filter(
-            core_facility=core_facility, item_type=InvoiceDetailItem.InvoiceDetailItemType.MISSED_RESERVATION
-        ).order_by("start")
-
-    def custom_charges_details(self, core_facility: CoreFacility):
-        return self.invoicedetailitem_set.filter(
-            core_facility=core_facility, item_type=InvoiceDetailItem.InvoiceDetailItemType.CUSTOM_CHARGE
-        ).order_by("start")
+    def staff_charge_details(self, core_facility: str):
+        return self.invoice_details().filter(core_facility=core_facility, item_type=BillableItemType.STAFF_CHARGE.value)
+
+    def consumable_withdrawal_details(self, core_facility: str):
+        return (
+            self.invoice_details()
+            .filter(core_facility=core_facility, item_type=BillableItemType.CONSUMABLE.value)
+            .order_by("start")
+        )
+
+    def training_details(self, core_facility: str):
+        return (
+            self.invoice_details()
+            .filter(core_facility=core_facility, item_type=BillableItemType.TRAINING.value)
+            .order_by("start")
+        )
+
+    def missed_reservation_details(self, core_facility: str):
+        return (
+            self.invoice_details()
+            .filter(core_facility=core_facility, item_type=BillableItemType.MISSED_RESERVATION.value)
+            .order_by("start")
+        )
+
+    def custom_charges_details(self, core_facility: str):
+        return (
+            self.invoice_details()
+            .filter(core_facility=core_facility, item_type=BillableItemType.CUSTOM_CHARGE.value)
+            .order_by("start")
+        )
 
     def total_amount_display(self) -> str:
         return display_amount(self.total_amount, self.configuration)
 
     def total_payments_received(self) -> Decimal:
         return self.invoicepayment_set.aggregate(
             total_received=Coalesce(
-                Sum(Case(When(payment_received__isnull=False, then="amount"), output_field=DecimalField(), default=0)),
-                0,
+                Sum(Case(When(payment_received__isnull=False, then="amount"), default=Decimal(0))), Decimal(0)
             )
         )["total_received"]
 
     def total_payments_processed(self) -> Decimal:
         return self.invoicepayment_set.aggregate(
             total_processed=Coalesce(
-                Sum(Case(When(payment_processed__isnull=False, then="amount"), output_field=DecimalField(), default=0)),
-                0,
+                Sum(Case(When(payment_processed__isnull=False, then="amount"), default=Decimal(0))), Decimal(0)
             )
         )["total_processed"]
 
     def total_outstanding_amount(self) -> Decimal:
         return self.total_amount - self.total_payments_received()
 
     def total_outstanding_display(self) -> str:
@@ -340,104 +430,63 @@
     def tax_display(self) -> str:
         return display_amount(
             self.invoicesummaryitem_set.aggregate(
                 total_tax=Coalesce(
                     Sum(
                         Case(
                             When(summary_item_type=InvoiceSummaryItem.InvoiceSummaryItemType.TAX, then="amount"),
-                            output_field=DecimalField(),
-                            default=0,
+                            default=Decimal(0),
                         )
                     ),
-                    0,
+                    Decimal(0),
                 )
             )["total_tax"],
             self.configuration,
         )
 
-    def facilities_subtotals(self) -> Dict:
-        result = {}
-        # We are creating subtotals for all facilities, and None which correspond to general charges
-        facility_names = [facility.name for facility in CoreFacility.objects.all()] + [None]
-        for facility_name in facility_names:
-            result[facility_name] = display_amount(Decimal(0), self.configuration)
-            try:
-                facility_subtotal = self.invoicesummaryitem_set.get(
-                    core_facility=facility_name, summary_item_type=InvoiceSummaryItem.InvoiceSummaryItemType.SUBTOTAL
-                )
-                result[facility_name] = facility_subtotal.amount_display()
-            except InvoiceSummaryItem.DoesNotExist:
-                pass
-        return result
-
     def __str__(self):
         created_date = f" ({self.created_date.date()})" if self.created_date else ""
         return f"{self.invoice_number}: {self.project_details.name}{created_date}"
 
     class Meta:
         ordering = ["-created_date", "-invoice_number"]
 
 
-class InvoiceDetailItem(models.Model):
-    class InvoiceDetailItemType(object):
-        TOOL_USAGE = 1
-        AREA_ACCESS = 2
-        CONSUMABLE = 3
-        MISSED_RESERVATION = 4
-        STAFF_CHARGE = 5
-        TRAINING = 6
-        CUSTOM_CHARGE = 7
-        choices = (
-            (TOOL_USAGE, "tool_usage"),
-            (AREA_ACCESS, "area_access"),
-            (CONSUMABLE, "consumable"),
-            (MISSED_RESERVATION, "missed_reservation"),
-            (STAFF_CHARGE, "staff_charge"),
-            (TRAINING, "training_session"),
-            (CUSTOM_CHARGE, "custom_charge"),
-        )
-
-        @classmethod
-        def is_time_type(cls, item_type):
-            return item_type in [
-                InvoiceDetailItem.InvoiceDetailItemType.TOOL_USAGE,
-                InvoiceDetailItem.InvoiceDetailItemType.AREA_ACCESS,
-                InvoiceDetailItem.InvoiceDetailItemType.TRAINING,
-                InvoiceDetailItem.InvoiceDetailItemType.STAFF_CHARGE,
-            ]
-
-        @classmethod
-        def category_name_for_item_type(cls, item_type):
-            from NEMO_billing.invoices.invoice_generator import invoice_generator_class
-
-            return invoice_generator_class.get_invoice_data_processor().category_name_for_item_type(item_type)
-
+class InvoiceDetailItem(BaseModel):
+    content_type = models.ForeignKey(ContentType, null=True, blank=True, on_delete=models.CASCADE)
+    object_id = models.PositiveIntegerField(null=True, blank=True)
+    content_object = GenericForeignKey("content_type", "object_id")
     invoice = models.ForeignKey(Invoice, on_delete=models.CASCADE)
     core_facility = models.CharField(null=True, blank=True, max_length=255)
-    item_type = models.IntegerField(choices=InvoiceDetailItemType.choices)
+    item_type = models.IntegerField(choices=BillableItemType.choices())
     name = models.CharField(max_length=255)
     quantity = models.DecimalField(decimal_places=2, max_digits=8)
     start = models.DateTimeField()
     end = models.DateTimeField()
     user = models.CharField(max_length=200)
     rate = models.CharField(null=True, blank=True, max_length=100)
     amount = models.DecimalField(decimal_places=2, max_digits=14)
+    discount = models.DecimalField(null=True, blank=True, decimal_places=2, max_digits=14)
 
     def quantity_display(self):
-        quantity = f"{self.quantity:.2f}"
-        if self.InvoiceDetailItemType.is_time_type(self.item_type):
-            return f"{quantity} min"
+        if self.item_type and BillableItemType(self.item_type).is_time_type():
+            return f"{round(self.quantity)} min"
         else:
-            return quantity
+            return f"{self.quantity:.2f}"
 
     def amount_display(self):
         return display_amount(self.amount, self.invoice.configuration)
 
+    class Meta:
+        indexes = [
+            models.Index(fields=["content_type", "object_id"]),
+        ]
+
 
-class InvoiceSummaryItem(models.Model):
+class InvoiceSummaryItem(BaseModel):
     class InvoiceSummaryItemType(object):
         ITEM = 1  # Any billable summary item
         SUBTOTAL = 2  # Facility subtotal (sum of billable summary item minus discounts)
         DISCOUNT_SUBTOTAL = 3  # Facility amount for discount (only used to calculate future accumulation discounts)
         DISCOUNT = 4  # Facility discount
         TAX = 5  # Tax
         OTHER = 6  # Other
@@ -448,45 +497,39 @@
             (DISCOUNT, "discount"),
             (TAX, "tax"),
             (OTHER, "other"),
         )
 
     invoice = models.ForeignKey(Invoice, on_delete=models.CASCADE)
     summary_item_type = models.IntegerField(choices=InvoiceSummaryItemType.choices)
-    item_type = models.IntegerField(null=True, blank=True, choices=InvoiceDetailItem.InvoiceDetailItemType.choices)
+    item_type = models.IntegerField(null=True, blank=True, choices=BillableItemType.choices())
     core_facility = models.CharField(null=True, blank=True, max_length=255)
     name = models.CharField(max_length=255)
     details = models.CharField(null=True, blank=True, max_length=100)
     amount = models.DecimalField(null=True, blank=True, decimal_places=2, max_digits=14)
 
     def amount_display(self):
         return display_amount(self.amount, self.invoice.configuration)
 
     def category_name_for_item_type(self):
-        return InvoiceDetailItem.InvoiceDetailItemType.category_name_for_item_type(self.item_type)
+        return category_name_for_item_type(self.item_type)
 
 
-class InvoicePayment(models.Model):
+class InvoicePayment(BaseModel):
     invoice = models.ForeignKey(Invoice, on_delete=models.CASCADE)
     payment_received = models.DateField(help_text="Date when payment was received")
     payment_processed = models.DateField(null=True, blank=True, help_text="Date when payment was processed")
     amount = models.DecimalField(decimal_places=2, max_digits=14, help_text="Amount received")
+    note = models.CharField(null=True, blank=True, max_length=255, help_text="Payment note")
     created_date = models.DateTimeField(auto_now_add=True)
     created_by = models.ForeignKey(User, related_name="payment_created_by_set", on_delete=models.PROTECT)
     updated_date = models.DateTimeField(auto_now=True)
     updated_by = models.ForeignKey(User, related_name="payment_updated_by_set", on_delete=models.PROTECT)
 
     def amount_display(self):
         return display_amount(self.amount, self.invoice.configuration)
 
     def __str__(self):
         return f"Payment for invoice {self.invoice.invoice_number}"
 
     class Meta:
         ordering = ["-payment_received"]
-
-
-def get_invoice_customization(name, default_value=None):
-    try:
-        return Customization.objects.get(name=name).value
-    except Customization.DoesNotExist:
-        return default_value
```

## NEMO_billing/invoices/pdf_utilities.py

```diff
@@ -1,19 +1,19 @@
-from typing import Tuple, List, Any, Union, Optional
+from typing import Any, List, Optional, Tuple, Union
 
 from django.db.models.fields.files import FieldFile
 from django.utils.text import normalize_newlines
-from reportlab.lib import utils, colors
-from reportlab.lib.enums import TA_CENTER, TA_RIGHT, TA_LEFT
+from reportlab.lib import colors, utils
+from reportlab.lib.enums import TA_CENTER, TA_LEFT, TA_RIGHT
 from reportlab.lib.fonts import tt2ps
 from reportlab.lib.pagesizes import A4, letter
-from reportlab.lib.styles import getSampleStyleSheet, ParagraphStyle, StyleSheet1
+from reportlab.lib.styles import ParagraphStyle, StyleSheet1, getSampleStyleSheet
 from reportlab.lib.units import mm
 from reportlab.pdfgen import canvas
-from reportlab.platypus import SimpleDocTemplate, Paragraph, Image, Spacer, PageBreak, Table, TableStyle, KeepInFrame
+from reportlab.platypus import Image, KeepInFrame, PageBreak, Paragraph, SimpleDocTemplate, Spacer, Table, TableStyle
 
 FONT_RIGHT = "Right"
 FONT_CENTERED = "Centered"
 HEADING_FONT = "Heading"
 HEADING_FONT_RIGHT = f"{HEADING_FONT}{FONT_RIGHT}"
 HEADING_FONT_CENTERED = f"{HEADING_FONT}{FONT_CENTERED}"
 SMALL_FONT = "Small"
@@ -144,15 +144,15 @@
         add_table_style(table_data, grid, border)
         self.elements.append(table_data)
 
     def _get_resized_paragraph_to_fit_height(
         self, text, content_width, content_height, size=12, style_name=SMALL_FONT
     ) -> Tuple[Paragraph, int, int]:
         font_size = size
-        while True:
+        while font_size > 0:
             paragraph = Paragraph(keep_linebreaks(text), self.styles[f"{style_name}Base{font_size}"])
             w, h = paragraph.wrap(content_width, content_height)
             if h <= content_height and w <= content_width:
                 break
             else:
                 font_size -= 1
         return paragraph, w, h
```

## NEMO_billing/invoices/urls.py

```diff
@@ -1,27 +1,44 @@
-from django.urls import path
+from NEMO.urls import router
+from django.urls import path, re_path
 
-from NEMO_billing.invoices.views import invoices, project
+from NEMO_billing.invoices import api
+from NEMO_billing.invoices.views import invoices, project, usage
+
+# Rest API URLs
+router.register(r"invoice_payments", api.InvoicePaymentViewSet)
+router.register(r"billing_data", api.BillingDataViewSet, basename="billingdata")
 
 urlpatterns = [
     path("invoices/", invoices.invoices, name="invoices"),
+    path("invoices/filter/<int:year>/", invoices.invoices, name="invoices_year"),
+    path("invoices/filter/<int:year>/<int:month>/", invoices.invoices, name="invoices_month"),
+    path("invoices/search/", invoices.search_invoices, name="search_invoices"),
     path("invoices/<int:invoice_id>/", invoices.view_invoice, name="view_invoice"),
     path("invoices/<int:invoice_id>/review/", invoices.review_invoice, name="review_invoice"),
     path("invoices/<int:invoice_id>/send/", invoices.send_invoice, name="send_invoice"),
     path("invoices/<int:invoice_id>/void/", invoices.void_invoice, name="void_invoice"),
+    path("invoices/<int:invoice_id>/delete/", invoices.delete_invoice, name="delete_invoice"),
+    path("invoices/<int:invoice_id>/csv/", invoices.csv_invoice, name="csv_invoice"),
+    path("invoices/<int:invoice_id>/re_render/", invoices.re_render_invoice, name="re_render_invoice"),
     path("invoices/zip/", invoices.zip_invoices, name="zip_invoices"),
+    re_path(r"invoices/zip/(?P<file_type>csv)/$", invoices.zip_invoices, name="zip_invoices"),
     path("invoices/generate_monthly_invoices/", invoices.generate_monthly_invoices, name="generate_monthly_invoices"),
     path("invoice_payment/<int:invoice_id>/received", invoices.invoice_payment_received, name="invoice_payment_received"),
     path("invoice_payment/<int:payment_id>/processed", invoices.invoice_payment_processed, name="invoice_payment_processed"),
 
     # Overriding NEMO's create project URLs
     path("create_project/", project.edit_project, name='invoices_create_project'),
     path("projects/<int:project_id>/edit/", project.edit_project, name='invoices_edit_project'),
 
     # Overriding NEMO's account and project URLs to add billing details
     path("project/<int:identifier>/", project.custom_project_view, kwargs={'kind': 'project'}, name='custom_project_view'),
     path("account/<int:identifier>/", project.custom_project_view, kwargs={'kind': 'account'}, name='custom_account_view'),
 
+    # Overriding NEMO's usage URLs to add rate and cost
+    path("project_usage/", usage.project_usage, name='project_usage'),
+    path("usage/", usage.usage, name='usage'),
+
     # Billing related periodic events
     path("invoices/send_invoice_payment_reminder/", invoices.send_invoice_payment_reminder, name="send_invoice_payment_reminder"),
     path("projects/deactivate_expired_projects/", project.deactivate_expired_projects, name='deactivate_expired_projects'),
 ]
```

## NEMO_billing/invoices/utilities.py

```diff
@@ -1,24 +1,39 @@
 import ntpath
 import os
 from datetime import datetime
 from decimal import Decimal
-from typing import Optional
+from typing import Iterable, List, Optional
 
 from NEMO.utilities import send_mail
 from NEMO.views.customization import get_media_file_contents
 from django.conf import settings
-from django.http import HttpResponse
-from django.shortcuts import render
-from django.template import Template, Context
+from django.template import Context, Template
 from django.template.loader import render_to_string
 from django.utils.encoding import force_str
 from django.utils.formats import number_format
 from django.utils.text import slugify
 
+from NEMO_billing.invoices.customization import InvoiceCustomization
+
+
+def export_invoice_filename(invoice):
+    invoice_filename_template = InvoiceCustomization.get("invoice_zip_export_template")
+    default_template = InvoiceCustomization.variables["invoice_zip_export_template"]
+    dictionary = {
+        "invoice": invoice,
+        "project_name": slugify(invoice.project_details.name),
+        "account_name": slugify(invoice.project_details.project.account.name),
+    }
+    try:
+        filename = Template(invoice_filename_template).render(Context(dictionary))
+    except:
+        filename = Template(default_template).render(Context(dictionary))
+    return filename
+
 
 def get_invoice_document_filename(invoice, filename):
     account_name = slugify(invoice.project_details.project.account.name)
     project_name = slugify(invoice.project_details.name)
     now = datetime.now()
     # generated_date = now.strftime("%Y-%m-%d_%H-%M-%S")
     year = now.strftime("%Y")
@@ -32,25 +47,26 @@
     return f"merchant_logos/{name}{ext}"
 
 
 def display_amount(amount: Optional[Decimal], configuration=None) -> str:
     # We need to specifically check for None since amount = 0 will evaluate to False
     if amount is None:
         return ""
+    rounded_amount = round(amount, 2)
     currency = (
         f"{configuration.currency_symbol}"
         if configuration and configuration.currency_symbol
         else f"{configuration.currency} "
-        if configuration
+        if configuration and configuration.currency
         else ""
     )
     if amount < 0:
-        return f"({currency}{number_format(abs(amount), decimal_pos=2)})"
+        return f"({currency}{number_format(abs(rounded_amount), decimal_pos=2)})"
     else:
-        return f"{currency}{number_format(amount, decimal_pos=2)}"
+        return f"{currency}{number_format(rounded_amount, decimal_pos=2)}"
 
 
 def render_and_send_email(template_prefix, context, from_email, to=None, bcc=None, cc=None, attachments=None) -> int:
     subject = render_template_from_media("{0}_subject.txt".format(template_prefix), context)
     # remove superfluous line breaks
     subject = " ".join(subject.splitlines()).strip()
     subject = format_email_subject(subject)
@@ -63,22 +79,31 @@
 
 def format_email_subject(subject):
     prefix = getattr(settings, "INVOICE_EMAIL_SUBJECT_PREFIX", "")
     return prefix + force_str(subject)
 
 
 def render_template_from_media(template_name, context):
-    """ Try to find the template in media folder. if it doesn't exists, look in project templates """
+    """Try to find the template in media folder. if it doesn't exist, look in project templates"""
     file_name = ntpath.basename(template_name)
     email_contents = get_media_file_contents(file_name)
     if email_contents:
         return Template(email_contents).render(Context(context))
     else:
-        # otherwise look in templates
+        # otherwise, look in templates
         return render_to_string(template_name, context)
 
 
-def render_combine_responses(request, original_response: HttpResponse, template_name, context):
-    """ Combines contents of an original http response with a new one """
-    additional_content = render(request, template_name, context)
-    original_response.content += additional_content.content
-    return original_response
+def category_name_for_item_type(billable_item_type) -> str:
+    from NEMO_billing.invoices.processors import invoice_data_processor_class
+
+    return invoice_data_processor_class.category_name_for_item_type(billable_item_type)
+
+
+def name_for_billable_item(billable_item) -> str:
+    from NEMO_billing.invoices.processors import invoice_data_processor_class
+
+    return invoice_data_processor_class.name_for_item(billable_item)
+
+
+def flatten(iterable: Iterable[Iterable]) -> List:
+    return [item for sublist in iterable for item in sublist]
```

## NEMO_billing/invoices/management/commands/send_invoice_payment_reminder.py

```diff
@@ -1,10 +1,10 @@
 from django.core.management import BaseCommand
 
 from NEMO_billing.invoices.views.invoices import do_send_invoice_payment_reminder
 
 
 class Command(BaseCommand):
-    help = "Run every day to send payment reminders for unpaid invoices. "
+    help = "Run every day to send payment reminders for unpaid invoices."
 
     def handle(self, *args, **options):
         do_send_invoice_payment_reminder()
```

## NEMO_billing/invoices/static/invoices/invoices.css

```diff
@@ -30,7 +30,20 @@
     margin-bottom: 7px;
 }
 
 table.invoice-details-table thead th, table.invoice-summary-table thead th
 {
     background-color: #dbdbdb;
 }
+
+.table-display
+{
+    display: table;
+    width: 100%;
+}
+
+.table-cell-display
+{
+    display: table-cell;
+    vertical-align: middle;
+    float: none !important;
+}
```

## NEMO_billing/invoices/templates/invoices/invoice.html

```diff
@@ -1,32 +1,34 @@
 {% extends 'invoices/base.html' %}
 {% load custom_tags_and_filters %}
 {% block title %}Invoice{% endblock %}
 {% block invoiceextrahead %}
 	{% load static %}
-	<script type="text/javascript" src="{% static "datetimepicker/bootstrap-datepicker.js" %}"></script>
-	<link rel="stylesheet" type="text/css" href="{% static "datetimepicker/bootstrap-datepicker3.css" %}"/>
+	<script type="text/javascript" src="{% static "datetimepicker/bootstrap-datetimepicker.js" %}"></script>
+	<link rel="stylesheet" type="text/css" href="{% static "datetimepicker/bootstrap-datetimepicker.css" %}"/>
 {% endblock %}
 {% block content %}
-	<h1>{% if invoice.voided_date %}<s>{% endif %}
-		Invoice {{ invoice.invoice_number }} for {{ invoice.project_details.name }} {% if invoice.project_details.category %}({{ invoice.project_details.category }}){% endif %}
-		{% if invoice.voided_date %}</s> (Void){% endif %}
-	</h1>
-	<h3><i>From {{ invoice.start|date:'F jS, Y' }} to {{ invoice.end|date:'F jS, Y' }}</i></h3>
+	<div class="col-lg-offset-1 col-lg-10 col-sm-12">
+		<h1>{% if invoice.voided_date %}<s>{% endif %}
+			Invoice {{ invoice.invoice_number }} for {{ invoice.project_details.name }} {% if invoice.project_details.category %}({{ invoice.project_details.category }}){% endif %}
+			{% if invoice.voided_date %}</s> (Void){% endif %}
+		</h1>
+		<h3><i>From {{ invoice.start|date:'F jS, Y' }} to {{ invoice.end|date:'F jS, Y' }}</i></h3>
+	</div>
 
 	<div class="row" style="margin-left: 0;margin-right: 0">
-		<div class="panel panel-default col-lg-10 col-md-10 col-sm-12" style="margin-top: 30px">
+		<div class="panel panel-default col-lg-offset-1 col-lg-10 col-sm-12" style="margin-top: 30px">
 			<div class="form-horizontal">
 				<div class="form-group" style="margin-top: 15px">
 					<div class="control-label col-sm-2"><strong>Created:</strong></div>
 					<div class="col-sm-4">
 						<p class="form-control-static">{{ invoice.created_date|date:'F jS, Y @ g:i A' }} ({{ invoice.created_by.username }})</p>
 					</div>
 					{% if invoice.project_details.project.application_identifier %}
-						<div class="control-label col-sm-2"><strong>Reference/PO:</strong></div>
+						<div class="control-label col-sm-2"><strong>{{ "projects_and_accounts"|customization:"project_application_identifier_name" }}</strong></div>
 						<div class="col-sm-4">
 							<p class="form-control-static">{{ invoice.project_details.project.application_identifier|default_if_none:'' }}</p>
 						</div>
 					{% endif %}
 				</div>
 				<div class="form-group">
 					<div class="control-label col-sm-2"><strong>Total</strong></div>
@@ -34,72 +36,87 @@
 						<p class="form-control-static">{{ invoice.total_amount_display }}</p>
 					</div>
 					<div class="control-label col-sm-2"><strong>Outstanding</strong></div>
 					<div class="col-sm-4">
 						<p class="form-control-static">{{ invoice.total_payments_display }}</p>
 					</div>
 				</div>
-				<div class="form-group">
-					<div class="control-label col-sm-2"><strong>Reviewed</strong></div>
-					<div class="col-sm-4">
-						{% if invoice.reviewed_date %}
-							<p class="form-control-static">{{ invoice.reviewed_date|date:'F jS, Y @ g:i A' }} ({{ invoice.reviewed_by.username }})</p>
-						{% else %}
-							<form action="{% url 'review_invoice' invoice.id %}" method="post">
-								{% csrf_token %}
-								<input type="submit" class="btn btn-sm btn-info" value="Mark as reviewed" onclick="show_spinner();">
-							</form>
-						{% endif %}
-					</div>
-					<div class="control-label col-sm-2"><strong>Void</strong></div>
-					<div class="col-sm-4">
-						{% if invoice.voided_date %}
-							<p class="form-control-static">{{ invoice.voided_date|date:'F jS, Y @ g:i A' }} ({{ invoice.voided_by.username }})</p>
-						{% else %}
-							<form action="{% url 'void_invoice' invoice.id %}" method="post">
-								{% csrf_token %}
-								<input type="submit" class="btn btn-sm btn-danger" value="Void invoice" onclick="show_spinner();">
-							</form>
-						{% endif %}
+				{% if user.is_accouting_officer or user.is_facility_manager or user.is_superuser %}
+					<div class="form-group">
+						<div class="control-label col-sm-2"><strong>Reviewed</strong></div>
+						<div class="col-sm-4">
+							{% if invoice.reviewed_date %}
+								<p class="form-control-static">{{ invoice.reviewed_date|date:'F jS, Y @ g:i A' }} ({{ invoice.reviewed_by.username }})</p>
+							{% else %}
+								<form action="{% url 'review_invoice' invoice.id %}" method="post">
+									{% csrf_token %}
+									{% button type="info" submit=True size="small" value="Mark as reviewed" onclick="show_spinner();" icon="glyphicon-ok-circle" %}
+								</form>
+							{% endif %}
+						</div>
+						<div class="control-label col-sm-2"><strong>Void</strong></div>
+						<div class="col-sm-4">
+							{% if invoice.voided_date %}
+								<p class="form-control-static">{{ invoice.voided_date|date:'F jS, Y @ g:i A' }} ({{ invoice.voided_by.username }})</p>
+							{% else %}
+								<form action="{% url 'void_invoice' invoice.id %}" method="post">
+									{% csrf_token %}
+									{% button type="delete" submit=True size="small" value="Void invoice" onclick="show_spinner();" icon="glyphicon-ban-circle" %}
+								</form>
+							{% endif %}
+						</div>
 					</div>
-				</div>
+				{% endif %}
 				<div class="form-group">
-					<div class="control-label col-sm-2"><strong>Last sent</strong></div>
-					<div class="col-sm-4">
-						{% if invoice.last_sent_date %}
-							<div class="form-control-static" style="display: inline-block;vertical-align: sub;">{{ invoice.last_sent_date|date:'F jS, Y @ g:i A' }}</div>
-						{% elif not invoice.reviewed_date %}
-							<p class="form-control-static">Invoice hasn't been reviewed</p>
-						{% endif %}
-						{% if invoice.reviewed_date %}
-							<form action="{% url 'send_invoice' invoice.id %}" method="post" style="display: inline-block">
-								{% csrf_token %}
-								<input type="submit" class="btn btn-sm btn-success" value="{% if invoice.last_sent_date %}Re-send{% else %}Send invoice{% endif %}" onclick="show_spinner();">
-							</form>
-						{% endif %}
-					</div>
+					{% if user.is_accouting_officer or user.is_facility_manager or user.is_superuser %}
+						<div class="control-label col-sm-2"><strong>Last sent</strong></div>
+						<div class="col-sm-4">
+							{% if invoice.last_sent_date %}
+								<div class="form-control-static" style="display: inline-block;vertical-align: sub;">{{ invoice.last_sent_date|date:'F jS, Y @ g:i A' }}</div>
+							{% elif not invoice.reviewed_date %}
+								<p class="form-control-static">Invoice hasn't been reviewed</p>
+							{% endif %}
+							{% if invoice.reviewed_date %}
+								<form action="{% url 'send_invoice' invoice.id %}" method="post" style="display: inline-block">
+									{% csrf_token %}
+									{% button type="save" size="small" value=invoice.last_sent_date|yesno:"Re-send,Send invoice" onclick="show_spinner();" icon="glyphicon-send" %}
+								</form>
+							{% endif %}
+						</div>
+					{% endif %}
 					<div class="control-label col-sm-2"><strong>File</strong></div>
 					<div class="col-sm-4">
-						<p class="form-control-static"><a href="{{ invoice.file.url }}" target="_blank">{{ invoice.filename }}</a></p>
+						{% if invoice.file %}
+							<p class="form-control-static"><a href="{{ invoice.file.url }}" target="_blank">{{ invoice.filename }}</a></p>
+						{% else %}
+							{% url 're_render_invoice' invoice.id as re_render_url %}
+							{% button type="warn" size="small" value="Re-render invoice file" onclick="show_spinner();" url=re_render_url icon="glyphicon-refresh" %}
+						{% endif %}
 					</div>
 				</div>
 			</div>
 		</div>
 	</div>
 
-	<div style="margin-top:30px">
-		<ul class="nav nav-pills" id="tabs">
-			<li class="active"><a href="#summary">Summary</a></li>
-			<li><a href="#details">Details</a></li>
-			<li><a href="#payments">Payments</a></li>
-		</ul>
+	<div class="row" style="margin-top:30px">
+		<div class="col-xs-7 col-lg-offset-1">
+			<ul class="nav nav-pills" id="tabs">
+				<li class="active"><a href="#summary">Summary</a></li>
+				<li><a href="#details">Details</a></li>
+				<li><a href="#payments">Payments</a></li>
+			</ul>
+		</div>
+		<div class="col-lg-3 col-xs-5 text-right">
+			{% url 'csv_invoice' invoice.id as export_csv_url %}
+			{% button type="export" value="Export data in CSV" url=export_csv_url %}
+		</div>
 	</div>
 
 	<div class="tab-content" style="margin-top: 15px">
-		<div id="summary" class="tab-pane active col-lg-10 col-md-10 col-sm-12" style="padding: 0">
+		<div id="summary" class="tab-pane active col-lg-offset-1 col-lg-10 col-sm-12" style="padding: 0">
 			<table class="invoice-summary-table table table-hover">
 				<thead>
 					<tr>
 						<th>Item</th>
 						<th>Details</th>
 						<th class="button-column-minimum">Amount</th>
 					</tr>
@@ -136,37 +153,37 @@
 				</tr>
 				</tbody>
 			</table>
 		</div>
 		<div id="details" class="tab-pane">
 			{% for core_facility, items in invoice.details_dict.items %}
 				<div class="h2 text-center panel panel-default" style="margin-top: 30px;padding: 15px">{{ core_facility|default_if_none:"General charges" }}</div>
-				{% include 'invoices/invoice_details.html' with items=items|get_item:'tool_usage' key='tool_usage' title='Tool usage' %}
-				{% include 'invoices/invoice_details.html' with items=items|get_item:'area_access' key='area_access' title='Area access' %}
-				{% include 'invoices/invoice_details.html' with items=items|get_item:'staff_charges' key='staff_charges' title='Staff charges' %}
-				{% include 'invoices/invoice_details.html' with items=items|get_item:'consumable_withdrawals' key='consumable_withdrawals' title='Supplies' %}
-				{% include 'invoices/invoice_details.html' with items=items|get_item:'trainings' key='trainings' title='Trainings' %}
-				{% include 'invoices/invoice_details.html' with items=items|get_item:'missed_reservations' key='missed_reservations' title='Missed Reservations' %}
-				{% include 'invoices/invoice_details.html' with items=items|get_item:'custom_charges' key='custom_charges' title='Other charges' %}
+				{% include 'invoices/invoice_details.html' with items=items|get_item:'tool_usage' key='tool_usage' title=tool_title %}
+				{% include 'invoices/invoice_details.html' with items=items|get_item:'area_access' key='area_access' title=area_title %}
+				{% include 'invoices/invoice_details.html' with items=items|get_item:'staff_charges' key='staff_charges' title=staff_charge_title %}
+				{% include 'invoices/invoice_details.html' with items=items|get_item:'consumable_withdrawals' key='consumable_withdrawals' title=consumable_title %}
+				{% include 'invoices/invoice_details.html' with items=items|get_item:'trainings' key='trainings' title=training_title %}
+				{% include 'invoices/invoice_details.html' with items=items|get_item:'missed_reservations' key='missed_reservations' title=missed_reservation_title %}
+				{% include 'invoices/invoice_details.html' with items=items|get_item:'custom_charges' key='custom_charges' title=custom_charge_title %}
 			{% endfor %}
 		</div>
 		<div id="payments" class="tab-pane">
 			<ul class="invoice-payment-list">
 				{% for payment in invoice.invoicepayment_set.all %}
 					<li>
 						<div class="form-inline" style="display:inline-block;">
 							<div class="form-control-static">
-								{{ payment.amount_display }} received on {{ payment.payment_received|date:'F jS, Y' }}
+								{{ payment.amount_display }} {% if payment.note %}({{ payment.note }}){% endif %} received on {{ payment.payment_received|date:'F jS, Y' }}
 							</div>
 						</div>
 						{% if payment.payment_processed %}
 							<div class="form-inline" style="display:inline-block;"><div class="form-control-static">- processed on {{ payment.payment_processed|date:'F jS, Y' }}</div></div>
 						{% else %}
-							<button class="btn btn-sm btn-info" onclick="$(this).hide();$('#form_payment_processed_{{ payment.id }}').css('display','inline');$('#payment_processed_date_{{ payment.id }}').datepicker({ format: 'mm/dd/yyyy', autoclose: true });">Mark as processed</button>
-							<form id="form_payment_processed_{{ payment.id }}" style="display: none" action="{% url 'invoice_payment_processed' payment.id %}" method="post" class="form-inline">
+							<button class="btn btn-sm btn-info" onclick="$(this).hide();$('#form_payment_processed_{{ payment.id }}').css('display','inline');$('#payment_processed_date_{{ payment.id }}').datetimepicker({ format: '{{ date_input_js_format }}', useCurrent: false });">Mark as processed</button>
+							<form id="form_payment_processed_{{ payment.id }}" style="display: none;position: relative" action="{% url 'invoice_payment_processed' payment.id %}" method="post" class="form-inline">
 								{% csrf_token %}
 								<div class="form-group">
 									<label style="vertical-align: text-bottom" class="form-control-static" for="payment_processed_date_{{ payment.id }}">- processed on:</label>
 								</div>
 								<div class="form-group extra-side-padding">
 									<input id="payment_processed_date_{{ payment.id }}" name="payment_processed_date" autocomplete="off" class="form-control input-sm" type="text" required>
 								</div>
@@ -192,34 +209,40 @@
 						{% csrf_token %}
 						<div class="form-group">
 							<label for="payment_received_date" class="control-label col-sm-3">Received on:</label>
 							<div class="col-sm-4">
 								<input id="payment_received_date" name="payment_received_date" autocomplete="off" class="form-control input-sm" type="text" required>
 							</div>
 						</div>
-						<div class="form-group" style="margin-bottom: 0">
+						<div class="form-group">
 							<label for="payment_received_amount" class="control-label col-sm-3">Amount:</label>
 							<div class="col-sm-4">
 								<input id="payment_received_amount" name="payment_received_amount" autocomplete="off" class="form-control input-sm" type="number" step=".01" min="1" required>
 							</div>
+						</div>
+						<div class="form-group" style="margin-bottom: 0">
+							<label for="payment_note" class="control-label col-sm-3">Note:</label>
+							<div class="col-sm-4">
+								<input id="payment_note" name="payment_note" autocomplete="off" class="form-control input-sm">
+							</div>
 							<div class="col-sm-5">
 								<input class="btn btn-sm btn-success pull-right" type="submit" value="Confirm">
 							</div>
 						</div>
 					</form>
 				</div>
 			</div>
 		</div>
 	</div>
 	<script>
 		function show_add_payment_modal()
 		{
 		    $("#new-payment-dialog .modal-content").html($('#form_add_payment_content').html());
 			$("#new-payment-dialog").modal('show');
-			$("#payment_received_date").datepicker({ format: 'mm/dd/yyyy', zIndexOffset:2048, autoclose: true });
+			$("#payment_received_date").datetimepicker({ format: '{{ date_input_js_format }}', useCurrent: false });
 		}
 		window.addEventListener('load', function ()
 		{
 			$("#tabs").find("a").click(switch_tab);
 		});
 	</script>
 {% endblock %}
```

### html2text {}

```diff
@@ -1,56 +1,72 @@
 {% extends 'invoices/base.html' %} {% load custom_tags_and_filters %} {% block
 title %}Invoice{% endblock %} {% block invoiceextrahead %} {% load static %}
-ootstrap-datepicker.js" %}">
-ootstrap-datepicker3.css" %}"/> {% endblock %} {% block content %}
+ootstrap-datetimepicker.js" %}">
+ootstrap-datetimepicker.css" %}"/> {% endblock %} {% block content %}
 ****** {% if invoice.voided_date %}{% endif %} Invoice {
 { invoice.invoice_number }} for {{ invoice.project_details.name }} {% if
 invoice.project_details.category %}({{ invoice.project_details.category }}){%
 endif %} {% if invoice.voided_date %} (Void){% endif %} ******
 **** From {{ invoice.start|date:'F jS, Y' }} to {{ invoice.end|date:'F jS, Y'
 }} ****
 Created:
 {{ invoice.created_date|date:'F jS, Y @ g:i A' }} ({
 { invoice.created_by.username }})
 {% if invoice.project_details.project.application_identifier %}
-Reference/PO:
+{{ "projects_and_accounts"|customization:"project_application_identifier_name"
+}}
 {{ invoice.project_details.project.application_identifier|default_if_none:'' }}
 {% endif %}
 Total
 {{ invoice.total_amount_display }}
 Outstanding
 {{ invoice.total_payments_display }}
+{% if user.is_accouting_officer or user.is_facility_manager or
+user.is_superuser %}
 Reviewed
 {% if invoice.reviewed_date %}
 {{ invoice.reviewed_date|date:'F jS, Y @ g:i A' }} ({
 { invoice.reviewed_by.username }})
 {% else %}
-{% csrf_token %} [Mark as reviewed]
+{% csrf_token %} {% button type="info" submit=True size="small" value="Mark as
+reviewed" onclick="show_spinner();" icon="glyphicon-ok-circle" %}
 {% endif %}
 Void
 {% if invoice.voided_date %}
 {{ invoice.voided_date|date:'F jS, Y @ g:i A' }} ({{ invoice.voided_by.username
 }})
 {% else %}
-{% csrf_token %} [Void invoice]
+{% csrf_token %} {% button type="delete" submit=True size="small" value="Void
+invoice" onclick="show_spinner();" icon="glyphicon-ban-circle" %}
+{% endif %}
 {% endif %}
+{% if user.is_accouting_officer or user.is_facility_manager or
+user.is_superuser %}
 Last sent
 {% if invoice.last_sent_date %}
 {{ invoice.last_sent_date|date:'F jS, Y @ g:i A' }}
 {% elif not invoice.reviewed_date %}
 Invoice hasn't been reviewed
 {% endif %} {% if invoice.reviewed_date %}
-{% csrf_token %} [{% if invoice.last_sent_date %}Re-send{% else %}Send invoice
-{% endif %}]
+{% csrf_token %} {% button type="save" size="small"
+value=invoice.last_sent_date|yesno:"Re-send,Send invoice" onclick="show_spinner
+();" icon="glyphicon-send" %}
+{% endif %}
 {% endif %}
 File
+{% if invoice.file %}
 {{_invoice.filename_}}
+{% else %} {% url 're_render_invoice' invoice.id as re_render_url %} {% button
+type="warn" size="small" value="Re-render invoice file" onclick="show_spinner
+();" url=re_render_url icon="glyphicon-refresh" %} {% endif %}
     * Summary
     * Details
     * Payments
+{% url 'csv_invoice' invoice.id as export_csv_url %} {% button type="export"
+value="Export data in CSV" url=export_csv_url %}
 Item                                     Details                               Amount
 {{ facility|default_if_none:'General
 Charges' }}
 {% if
 summary_item.category_name_for_item_type
 %}{                                      {                                     {
 {                                        {                                     {
@@ -62,29 +78,29 @@
 {{ summary_item.name|default_if_none:''  {                                     {
 }}                                       summary_item.details|default_if_none: summary_item.amount_display|default_if_none:
                                          '' }}                                 '' }}
 Grand Total                                                                    {{ invoice.total_amount_display }}
 {% for core_facility, items in invoice.details_dict.items %}
 {{ core_facility|default_if_none:"General charges" }}
 {% include 'invoices/invoice_details.html' with items=items|get_item:
-'tool_usage' key='tool_usage' title='Tool usage' %} {% include 'invoices/
+'tool_usage' key='tool_usage' title=tool_title %} {% include 'invoices/
 invoice_details.html' with items=items|get_item:'area_access' key='area_access'
-title='Area access' %} {% include 'invoices/invoice_details.html' with
-items=items|get_item:'staff_charges' key='staff_charges' title='Staff charges'
+title=area_title %} {% include 'invoices/invoice_details.html' with
+items=items|get_item:'staff_charges' key='staff_charges'
+title=staff_charge_title %} {% include 'invoices/invoice_details.html' with
+items=items|get_item:'consumable_withdrawals' key='consumable_withdrawals'
+title=consumable_title %} {% include 'invoices/invoice_details.html' with
+items=items|get_item:'trainings' key='trainings' title=training_title %} {%
+include 'invoices/invoice_details.html' with items=items|get_item:
+'missed_reservations' key='missed_reservations' title=missed_reservation_title
 %} {% include 'invoices/invoice_details.html' with items=items|get_item:
-'consumable_withdrawals' key='consumable_withdrawals' title='Supplies' %} {%
-include 'invoices/invoice_details.html' with items=items|get_item:'trainings'
-key='trainings' title='Trainings' %} {% include 'invoices/invoice_details.html'
-with items=items|get_item:'missed_reservations' key='missed_reservations'
-title='Missed Reservations' %} {% include 'invoices/invoice_details.html' with
-items=items|get_item:'custom_charges' key='custom_charges' title='Other
-charges' %} {% endfor %}
+'custom_charges' key='custom_charges' title=custom_charge_title %} {% endfor %}
     * {% for payment in invoice.invoicepayment_set.all %}
-    * {{ payment.amount_display }} received on {
-      { payment.payment_received|date:'F jS, Y' }}
+    * {{ payment.amount_display }} {% if payment.note %}({{ payment.note }}){%
+      endif %} received on {{ payment.payment_received|date:'F jS, Y' }}
       {% if payment.payment_processed %}
       - processed on {{ payment.payment_processed|date:'F jS, Y' }}
       {% else %} Mark as processed
       {% csrf_token %}
       - processed on:
       [payment_processed_date]
       [Confirm]
@@ -93,9 +109,11 @@
 Record new payment
 **** Payment received form ****
 {% csrf_token %}
 Received on:
 [payment_received_date]
 Amount:
 [Unknown INPUT type]
+Note:
+[payment_note        ]
 [Confirm]
  {% endblock %}
```

## NEMO_billing/invoices/templates/invoices/invoice_details.html

```diff
@@ -4,28 +4,32 @@
 		<table class="invoice-details-table table table-hover">
 			<thead>
 				<tr>
 					<th>User</th>
 					<th>{% if key == 'tool_usage' or key == 'trainings' %}Tool{% elif key == 'area_access' %}Area{% elif key == 'missed_reservations' %}Reservation{% elif key == 'staff_charge' %}Item{% endif %}</th>
 					<th>Rate</th>
 					{% if key != 'missed_reservation' %}<th>Quantity</th>{% endif %}
-					<th>Start</th>
-					<th>End</th>
+					{% if key == 'trainings' %}
+						<th>Date</th>
+					{% else %}
+						<th>Start</th>
+						<th>End</th>
+					{% endif %}
 					<th class="button-column-minimum">Amount</th>
 				</tr>
 			</thead>
 			<tbody>
 				{% for detail_item in items %}
 					<tr class="detail-item-{{ detail_item.get_item_type_display }}">
 						<td class="detail-item-user">{{ detail_item.user|default_if_none:'' }}</td>
 						<td class="detail-item-name">{{ detail_item.name|default_if_none:'' }}</td>
 						<td class="detail-item-rate">{{ detail_item.rate|default_if_none:'' }}</td>
 						{% if key != 'missed_reservation' %}<td class="detail-item-quantity">{{ detail_item.quantity_display|default_if_none:'' }}</td>{% endif %}
 						<td class="detail-item-start">{{ detail_item.start|default_if_none:'' }}</td>
-						<td class="detail-item-end">{{ detail_item.end|default_if_none:'' }}</td>
+						{% if key != 'trainings' %}<td class="detail-item-end">{{ detail_item.end|default_if_none:'' }}</td>{% endif %}
 						<td class="detail-item-amount">{{ detail_item.amount_display|default_if_none:'' }}</td>
 					</tr>
 				{% endfor %}
 			</tbody>
 		</table>
 	{% elif key == 'consumable_withdrawals' %}
 		<table class="invoice-details-table table table-hover">
```

### html2text {}

```diff
@@ -1,14 +1,14 @@
 {% if items %}
 *** {{ title }} ***
 {% if key == 'tool_usage' or key == 'area_access' or key == 'staff_charges' or
 key == 'trainings' or key == 'missed_reservations' %}
                                   {% if key == 'tool_usage' or key
                                   == 'trainings' %}Tool{% elif key
-User                              == 'area_access' %}Area{% elif    Rate                              Quantity                                      Start                              End                              Amount
+User                              == 'area_access' %}Area{% elif    Rate                              Quantity                                      Date                               Start                            End                                         Amount
                                   key == 'missed_reservations'
                                   %}Reservation{% elif key ==
                                   'staff_charge' %}Item{% endif %}
 {                                 {                                 {                                 {                                             {                                  {                                {
 {                                 {                                 {                                 {                                             {                                  {                                {
 detail_item.user|default_if_none: detail_item.name|default_if_none: detail_item.rate|default_if_none: detail_item.quantity_display|default_if_none: detail_item.start|default_if_none: detail_item.end|default_if_none: detail_item.amount_display|default_if_none:
 '' }}                             '' }}                             '' }}                             '' }}                                         '' }}                              '' }}                            '' }}
```

## NEMO_billing/invoices/templates/invoices/invoices.html

```diff
@@ -1,9 +1,10 @@
 {% extends 'pagination/pagination_base.html' %}
 {% load custom_tags_and_filters %}
+{% load billing_tags %}
 {% block title %}Invoices{% endblock %}
 {% block before_pagination %}
 	<h1>
 		Invoices
 	</h1>
 	{% if not configuration_list and user.is_superuser %}
 		<h3 style="margin-bottom: 30px">There are no invoice configurations set</h3>
@@ -12,132 +13,174 @@
 		</h3>
 	{% else %}
 		<div class="row" style="margin-bottom: 40px">
 			<div class="col-sm-4">
 				<input id="search" type="text" placeholder="Search for an invoice" class="form-control" autofocus>
 			</div>
 		</div>
-		<form id="generate-invoice-form" action="{% url 'generate_monthly_invoices' %}" class="row form-inline text-right" method="post" style="; margin-right: 0">
-			{% csrf_token %}
-			<div class="form-group extra-side-padding">
-				<label for="month" class="control-label">Month</label>
-			</div>
-			<div class="form-group">
-				<select name="month" id="month" class="form-control" required>
-					<option selected disabled value=""></option>
-					{% for month in month_list %}
-						<option>{{ month|date:"F, Y" }}</option>
-					{% endfor %}
-				</select>
-			</div>
-			<div class="form-group extra-side-padding">
-				<label for="project_id" class="control-label">Project</label>
-			</div>
-			<div class="form-group">
-				<select name="project_id" id="project_id" class="form-control" style="max-width: 250px" required>
-					<option selected disabled value=""></option>
-					<option value="All">All</option>
-					{% regroup projects by account as projects_by_account %}
-					{% for account in projects_by_account %}
-						<optgroup label="{{ account.grouper.name }}">
-						{% for project in account.list %}
-							<option value="{{ project.id }}">{{ project.name }}</option>
-						{% endfor %}
-						</optgroup>
-					{% endfor %}
-				</select>
-			</div>
-			{% if configuration_list|length_is:1 %}
-				<input type="hidden" name="configuration_id" value="{{ configuration_list.0.id }}">
-			{% else %}
-				<div class="form-group extra-side-padding">
-					<label for="configuration_id" class="control-label">Configuration</label>
+		{% if user.accounting_officer or user.is_facility_manager or user.is_superuser %}
+			<form id="generate-invoice-form" action="{% url 'generate_monthly_invoices' %}" class="form-horizontal" method="post">
+				{% csrf_token %}
+				<div class="col-xs-12 col-sm-6 {% if configuration_list|length_is:1 %}col-md-4{% else %}col-md-3{% endif %}" style="margin-bottom: 15px; padding: 0;">
+					<label for="month" class="col-xs-2 col-sm-3 control-label">Month</label>
+					<div class="col-xs-10 col-sm-9" style="padding-right:0;">
+						<select name="month" id="month" class="form-control" required>
+							<option selected disabled value=""></option>
+							{% for month in month_list %}
+								<option>{{ month|date:"F, Y" }}</option>
+							{% endfor %}
+						</select>
+					</div>
 				</div>
-				<div class="form-group">
-					<select class="form-control" name="configuration_id" id="configuration_id" required>
-						<option disabled selected value="">Select a configuration</option>
-						{% for configuration in configuration_list %}
-							<option value="{{ configuration.id }}">{{ configuration.name }}</option>
-						{% endfor %}
-					</select>
+				<div class="col-xs-12 col-sm-6 {% if configuration_list|length_is:1 %}col-md-5{% else %}col-md-5{% endif %}" style="margin-bottom: 15px; padding: 0">
+					{% cap_discount_installed as cap_discount_installed %}
+					<label for="project_id" class="col-xs-2 col-sm-3 control-label">{% if cap_discount_installed %}Account{% else %}Project{% endif %}</label>
+					<div class="col-xs-10 col-sm-9" style="padding-right:0;">
+						<select name="project_id" id="project_id" class="form-control" required>
+							<option selected disabled value=""></option>
+							<option value="All">All</option>
+							{% regroup projects by account as projects_by_account %}
+							{% for account in projects_by_account %}
+								<option value="account:{{ account.grouper.id }}">{{ account.grouper.name }}</option>
+								{% if not cap_discount_installed %}
+									{# Don't allow single project invoice generation if we have account caps #}
+									{% for project in account.list %}
+										<option value="{{ project.id }}">&nbsp;&nbsp;&nbsp;&nbsp;{{ project.name }}</option>
+									{% endfor %}
+								{% endif %}
+							{% endfor %}
+						</select>
+					</div>
 				</div>
-			{% endif %}
-			<div class="form-group extra-side-padding" style="padding-right: 0">
-				<input type="submit" class="btn btn-success" onclick="show_spinner(this.form);" value="Generate invoice(s)">
-			</div>
-		</form>
+				{% if configuration_list|length_is:1 %}
+					<input type="hidden" name="configuration_id" value="{{ configuration_list.0.id }}">
+				{% else %}
+					<div class="col-xs-12 col-sm-6 col-md-4" style="margin-bottom: 15px; padding: 0">
+						<label for="configuration_id" class="col-xs-2 col-sm-3 control-label">Config</label>
+						<div class="col-xs-10 col-sm-9" style="padding-right:0;">
+							<select class="form-control" name="configuration_id" id="configuration_id" required>
+								<option disabled selected value="">Select a configuration</option>
+								{% for configuration in configuration_list %}
+									<option value="{{ configuration.id }}">{{ configuration.name }}</option>
+								{% endfor %}
+							</select>
+						</div>
+					</div>
+				{% endif %}
+				<div class="col-xs-12 col-sm-6 {% if configuration_list|length_is:1 %}col-md-3 col-sm-offset-6 col-md-offset-0{% else %}col-md-4 col-md-offset-8{% endif %} text-right" style="margin-bottom: 15px; padding-right:0;">
+					{% button type="save" onclick="show_spinner(this.form);" value="Generate invoice(s)" icon="glyphicon-list-alt" %}
+				</div>
+			</form>
+		{% endif %}
 		<div id="download_invoices" class="row" style="display: none; margin-top: 15px; margin-right: 0">
 			<div class="form-group">
-				<button class="btn btn-info pull-right" onclick="$('#zip-invoices').submit();$('#zip-invoices :checkbox').prop('checked', false);update_download_button_state();">Download selected invoices</button>
+				{% url 'zip_invoices' 'csv' as zip_csv_url %}
+				{% url 'zip_invoices' as zip_url %}
+				{% button type="export" style="margin-left: 10px; float: right;" value="Export selected invoices (CSV)" onclick="$('#zip-invoices').attr('action', '"|concat:zip_csv_url|concat:"');$('#zip-invoices').submit();$('#zip-invoices :checkbox').prop('checked', false);update_download_button_state();" %}
+				{% button type="export" style="float: right;" value="Export selected invoices" onclick="$('#zip-invoices').attr('action', '"|concat:zip_url|concat:"');$('#zip-invoices').submit();$('#zip-invoices :checkbox').prop('checked', false);update_download_button_state();" %}
 			</div>
 		</div>
 	{% endif %}
 {% endblock %}
+{% block pagination_header %}
+	<div class="row" style="width: 100%; margin: 20px 0;">
+		{% regroup filter_month_list by year as filter_by_year %}
+		{% if filter_month_list %}
+			<div class="col-sm-12" style="padding-left: 0">
+				{% for year in filter_by_year %}
+					<button style="margin-right: 2px" class="year-button btn btn-sm btn-default {% if filter_year and filter_year == year.grouper %}focus{% endif %}" type="button" onclick="$('.year-button').removeClass('focus');$('.filter_year').hide();$('#filter_year_{{ year.grouper }}').show();">{{ year.grouper }}</button>
+				{% endfor %}
+				{% if filter_month %}<a class="btn btn-sm btn-default" type="button" href="{% url 'invoices' %}"><i class="glyphicon glyphicon-remove"></i> Clear</a>{% endif %}
+			</div>
+			<div class="col-xs-7 col-sm-8 col-lg-10" style="padding-left: 0">
+				{% for year in filter_by_year %}
+					<div id="filter_year_{{ year.grouper }}" class="filter_year" style="margin-top:10px; {% if not filter_year or filter_year != year.grouper %}display: none;{% endif %}">
+						{% for month in year.list %}
+							<a style="margin-right: 10px" href="{% url 'invoices_month' month.year month.month %}">{{ month|date:"F" }}</a>
+						{% endfor %}
+					</div>
+				{% endfor %}
+			</div>
+		{% endif %}
+		<div class="col-xs-5 col-sm-4 col-lg-2 text-right" style="padding-right: 0">
+			{% include "pagination/pagination_selector.html" %}
+		</div>
+	</div>
+{% endblock %}
 {% block pagination_content %}
 	<form id="zip-invoices" action="{% url 'zip_invoices' %}" method="post">
 		{% csrf_token %}
 		<table class="table table-bordered table-condensed table-striped table-hover thead-light">
 			<thead>
 				<tr>
 					<th class="button-column-minimum"><input type="checkbox" onchange="$('#zip-invoices :checkbox').prop('checked', $(this).prop('checked'));update_download_button_state();"></th>
-					<th class="button-column-minimum">{% include 'pagination/pagination_column.html' with order_by='invoice_number' name='Number' align='yes' %}</th>
-					<th>{% include 'pagination/pagination_column.html' with order_by='created_date' name='Created' %}</th>
+					<th class="button-column-minimum">{% include 'pagination/pagination_column.html' with order_by='invoice_number' name='#' %}</th>
+					{% if "created_date" not in hide_columns %}<th>{% include 'pagination/pagination_column.html' with order_by='created_date' name='Created' %}</th>{% endif %}
+					{% if "month" not in hide_columns %}<th>{% include 'pagination/pagination_column.html' with order_by='start' name='Month' %}</th>{% endif %}
 					<th>{% include 'pagination/pagination_column.html' with order_by='project_details__project__name' name='Project' %}</th>
-					<th>{% include 'pagination/pagination_column.html' with order_by='last_sent_date' name='Last sent' %}</th>
-					<th>{% include 'pagination/pagination_column.html' with order_by='due_date' name='Due date' %}</th>
-					<th>{% include 'pagination/pagination_column.html' with order_by='reviewed_date' name='Reviewed' %}</th>
+					<th>{% include 'pagination/pagination_column.html' with order_by='project_details__project__account__name' name='Account' %}</th>
+					{% if "sent_date" not in hide_columns %}<th>{% include 'pagination/pagination_column.html' with order_by='last_sent_date' name='Sent' %}</th>{% endif %}
+					{% if "due_date" not in hide_columns %}<th>{% include 'pagination/pagination_column.html' with order_by='due_date' name='Due' %}</th>{% endif %}
+					{% if "review_date" not in hide_columns %}<th>{% include 'pagination/pagination_column.html' with order_by='reviewed_date' name='Reviewed' %}</th>{% endif %}
 					<th>{% include 'pagination/pagination_column.html' with order_by='total_amount' name='Total' %}</th>
 					{% for core_facility in core_facilities %}
-						<th>{{ core_facility.name }}</th>
+						<th>{% include 'pagination/pagination_column.html' with order_by='facility_total_'|concat:core_facility.id name=core_facility.name %}</th>
 					{% endfor %}
-					{% if display_general_facility %}<th>General</th>{% endif %}
-					<th>{% include 'pagination/pagination_column.html' with order_by='total_tax' name='Tax' %}</th>
-					<th>{% include 'pagination/pagination_column.html' with order_by='outstanding' name='Outstanding' %}</th>
-					<th class="button-column-minimum"></th>
+					{% if display_general_facility %}<th>{% include 'pagination/pagination_column.html' with order_by='facility_total_general' name="General" %}</th>{% endif %}
+					{% if "tax" not in hide_columns %}<th>{% include 'pagination/pagination_column.html' with order_by='total_tax' name='Tax' %}</th>{% endif %}
+					{% if "outstanding" not in hide_columns %}<th>{% include 'pagination/pagination_column.html' with order_by='outstanding' name='Outstanding' %}</th>{% endif %}
+					{% if "actions" not in hide_columns %}<th class="button-column-minimum"></th>{% endif %}
 				</tr>
 			</thead>
 			<tbody>
 				{% for invoice in page %}
-					<tr>
-						<td class="text-center"><input type="checkbox" id="select_{{ invoice.id }}" name="selected_invoice_id[]" value="{{ invoice.id }}" onchange="update_download_button_state();"/></td>
-						<td><label for="select_{{ invoice.id }}">{{ invoice.invoice_number }}</label></td>
-						<td>{{ invoice.created_date|date:"SHORT_DATETIME_FORMAT" }}</td>
-						<td>{{ invoice.project_details.project.name }}</td>
-						<td>{{ invoice.last_sent_date|date|default_if_none:"" }}</td>
-						<td>{{ invoice.due_date|date|default_if_none:"" }}</td>
-						<td>{{ invoice.reviewed_date|date|default_if_none:"" }}</td>
-						<td class="text-right">{{ invoice.total_amount_display }}</td>
-						{% for core_facility in core_facilities %}
-							<td class="text-right">
-							{% if invoice and invoice.facilities_subtotals %}
-								{{ invoice.facilities_subtotals|get_item:core_facility.name }}
+					{% url 'view_invoice' invoice.id as view_invoice_url %}
+					{% with td_attribute="onclick=\"window.location.href = '"|concat:view_invoice_url|concat:"'\" style=\"cursor:pointer\"" %}
+						<tr>
+							<td class="text-center"><input type="checkbox" id="select_{{ invoice.id }}" name="selected_invoice_id[]" aria-label="{{ invoice.invoice_number }}" value="{{ invoice.id }}" onchange="update_download_button_state();"/></td>
+							<td style="white-space: nowrap"><label for="select_{{ invoice.id }}">{{ invoice.invoice_number }}</label></td>
+							{% if "created_date" not in hide_columns %}<td {{ td_attribute|safe }}>{{ invoice.created_date|date:"SHORT_DATETIME_FORMAT" }}</td>{% endif %}
+							{% if "month" not in hide_columns %}<td {{ td_attribute|safe }}>{{ invoice.start|date:"F Y" }}</td>{% endif %}
+							<td {{ td_attribute|safe }}>{{ invoice.project_details.project.name }}</td>
+							<td {{ td_attribute|safe }}>{{ invoice.project_details.project.account.name }}</td>
+							{% if "sent_date" not in hide_columns %}<td {{ td_attribute|safe }}>{{ invoice.last_sent_date|date|default_if_none:"" }}</td>{% endif %}
+							{% if "due_date" not in hide_columns %}<td {{ td_attribute|safe }}>{{ invoice.due_date|date|default_if_none:"" }}</td>{% endif %}
+							{% if "review_date" not in hide_columns %}<td {{ td_attribute|safe }}>{{ invoice.reviewed_date|date|default_if_none:"" }}</td>{% endif %}
+							<td {{ td_attribute|safe }} class="text-right">{{ invoice.total_amount_display }}</td>
+							{% for core_facility in core_facilities %}
+								<td {{ td_attribute|safe }} class="text-right">
+								{% with facility_subtotal=invoice.facility_subtotals|to_dict:"core_facility"|get_item:core_facility.name %}
+									{{ facility_subtotal.amount|default:0|display_amount:invoice.configuration }}
+								{% endwith %}
+								</td>
+							{% endfor %}
+							{% if display_general_facility %}
+								<td {{ td_attribute|safe }} class="text-right">
+									{% with general_subtotal=invoice.facility_subtotals|to_dict:"core_facility"|get_item:None %}
+										{{ general_subtotal.amount|default:0|display_amount:invoice.configuration }}
+									{% endwith %}
+								</td>
 							{% endif %}
-							</td>
-						{% endfor %}
-						{% if display_general_facility %}
-							<td class="text-right">
-								{% if invoice and invoice.facilities_subtotals %}
-									{{ invoice.facilities_subtotals|get_item:None }}
-								{% endif %}
-							</td>
-						{% endif %}
-						<td class="text-right">{{ invoice.tax_display }}</td>
-						<td class="text-right">{{ invoice.total_outstanding_display }}</td>
-						<td>
-							<button type="button" class="btn btn-xs btn-primary" title="View invoice" onclick="window.location = '{% url 'view_invoice' invoice.id %}'"><i class="glyphicon glyphicon-search"></i></button>
-						</td>
-					</tr>
+							{% if "tax" not in hide_columns %}<td {{ td_attribute|safe }} class="text-right">{{ invoice.total_tax|display_amount:invoice.configuration }}</td>{% endif %}
+							{% if "outstanding" not in hide_columns %}<td {{ td_attribute|safe }} class="text-right">{{ invoice.outstanding|display_amount:invoice.configuration }}</td>{% endif %}
+							{% if "actions" not in hide_columns %}
+								<td>
+									{% button size="xsmall" type="view" value="View" title="View invoice" url=view_invoice_url %}
+								</td>
+							{% endif %}
+						</tr>
+					{% endwith %}
 				{% endfor %}
 			</tbody>
 		</table>
 	</form>
 {% endblock %}
 {% block table_empty_content %}
 	<div style="margin-top: 35px">
-		<i>No invoices have been generated yet.</i>
+		<i>No invoices could be found.</i>
 	</div>
 {% endblock %}
 {% block after_pagination %}
 	<script>
 		function update_download_button_state()
 		{
 			if ($("#zip-invoices input:checkbox:checked").length > 0)
@@ -151,12 +194,12 @@
 		}
 		function get_invoice(jquery_event, search_selection, dataset_name)
 		{
 			window.location.href = "{% url 'view_invoice' 999 %}".replace('999', search_selection.id);
 		}
 		function on_load()
 		{
-			$("#search").autocomplete('invoices', get_invoice, {{ invoices_search|json_search_base }}).focus();
+            $("#search").autocomplete('invoices', get_invoice, '{% url 'search_invoices' %}', true).focus();
 		}
 		window.addEventListener('load', on_load, true);
 	</script>
 {% endblock %}
```

### html2text {}

```diff
@@ -1,45 +1,73 @@
 {% extends 'pagination/pagination_base.html' %} {% load custom_tags_and_filters
-%} {% block title %}Invoices{% endblock %} {% block before_pagination %}
+%} {% load billing_tags %} {% block title %}Invoices{% endblock %} {% block
+before_pagination %}
 ****** Invoices ******
 {% if not configuration_list and user.is_superuser %}
 **** There are no invoice configurations set ****
 **** You can change that in the Invoice_Configuration_section_of_'Detailed
 Administration'. ****
 {% else %}
 [                    ]
+{% if user.accounting_officer or user.is_facility_manager or user.is_superuser
+%}
 {% csrf_token %}
 Month
 {% for month in month_list %}
 {{ month|date:"F, Y" }}
 {% endfor %}
-Project
+{% cap_discount_installed as cap_discount_installed %} {% if
+cap_discount_installed %}Account{% else %}Project{% endif %}
 All
 {% regroup projects by account as projects_by_account %} {% for account in
-projects_by_account %}  {% for project in account.list %}
-{{ project.name }}
-{% endfor %}  {% endfor %}
+projects_by_account %}
+{{ account.grouper.name }}
+{% if not cap_discount_installed %} {# Don't allow single project invoice
+generation if we have account caps #} {% for project in account.list %}
+    {{ project.name }}
+{% endfor %} {% endif %} {% endfor %}
 {% if configuration_list|length_is:1 %}  {% else %}
-Configuration
+Config
 {% for configuration in configuration_list %}
 {{ configuration.name }}
 {% endfor %}
 {% endif %}
-[Generate invoice(s)]
-Download selected invoices
-{% endif %} {% endblock %} {% block pagination_content %}
+{% button type="save" onclick="show_spinner(this.form);" value="Generate
+invoice(s)" icon="glyphicon-list-alt" %}
+{% endif %}
+{% url 'zip_invoices' 'csv' as zip_csv_url %} {% url 'zip_invoices' as zip_url
+%} {% button type="export" style="margin-left: 10px; float: right;"
+value="Export selected invoices (CSV)" onclick="$('#zip-invoices').attr
+('action', '"|concat:zip_csv_url|concat:"');$('#zip-invoices').submit();$
+('#zip-invoices :checkbox').prop('checked', false);update_download_button_state
+();" %} {% button type="export" style="float: right;" value="Export selected
+invoices" onclick="$('#zip-invoices').attr('action', '"|concat:zip_url|concat:
+"');$('#zip-invoices').submit();$('#zip-invoices :checkbox').prop('checked',
+false);update_download_button_state();" %}
+{% endif %} {% endblock %} {% block pagination_header %}
+{% regroup filter_month_list by year as filter_by_year %} {% if
+filter_month_list %}
+{% for year in filter_by_year %} {{ year.grouper }} {% endfor %} {% if
+filter_month %}
+ Clear
+{% endif %}
+{% for year in filter_by_year %}
+{% for month in year.list %} {{_month|date:"F"_}} {% endfor %}
+{% endfor %}
+{% endif %}
+{% include "pagination/pagination_selector.html" %}
+{% endblock %} {% block pagination_content %}
 {% csrf_token %}
-  {% include 'pagination/   {% include 'pagination/                                                                                                                                                                                                                                                                                         {% include 'pagination/
-  pagination_column.html'   pagination_column.html'    {% include 'pagination/                   {% include 'pagination/                      {% include 'pagination/                {% include 'pagination/                     {% include 'pagination/                                                                                    pagination_column.html' {% include 'pagination/
-�with                      with                       pagination_column.html' with              pagination_column.html' with                 pagination_column.html' with           pagination_column.html' with                pagination_column.html' with {{ core_facility.name }}               General                                with                    pagination_column.html' with
-  order_by='invoice_number' order_by='created_date'    order_by='project_details__project__name' order_by='last_sent_date' name='Last sent'   order_by='due_date' name='Due date' %} order_by='reviewed_date' name='Reviewed' %} order_by='total_amount'                                                                                    order_by='total_tax'    order_by='outstanding'
-  name='Number' align='yes' name='Created' %}          name='Project' %}                         %}                                                                                                                              name='Total' %}                                                                                            name='Tax' %}           name='Outstanding' %}
-  %}
-                            {                                                                    {                                            {                                      {                                           {                            {% if invoice and                      {% if invoice and                                              {
-  {{ invoice.invoice_number {                          {{ invoice.project_details.project.name   {                                            {                                      {                                           {                            invoice.facilities_subtotals %} {      invoice.facilities_subtotals %} {      {{ invoice.tax_display  {
-�}}                        invoice.created_date|date: }}                                        invoice.last_sent_date|date|default_if_none: invoice.due_date|date|default_if_none: invoice.reviewed_date|date|default_if_none: invoice.total_amount_display {                                      {                                      }}                      invoice.total_outstanding_display
-                            "SHORT_DATETIME_FORMAT" }}                                           "" }}                                        "" }}                                  "" }}                                       }}                           invoice.facilities_subtotals|get_item: invoice.facilities_subtotals|get_item:                         }}
-                                                                                                                                                                                                                                                              core_facility.name }} {% endif %}      None }} {% endif %}
+  {% include 'pagination/   {% include 'pagination/ {% include 'pagination/ {% include 'pagination/                   {% include 'pagination/pagination_column.html'     {% include 'pagination/   {% include 'pagination/ {% include 'pagination/  {% include 'pagination/ {% include 'pagination/            {% include 'pagination/           {% include 'pagination/ {% include 'pagination/
+  pagination_column.html'   pagination_column.html' pagination_column.html' pagination_column.html' with              with                                               pagination_column.html'   pagination_column.html' pagination_column.html'  pagination_column.html' pagination_column.html' with       pagination_column.html' with      pagination_column.html' pagination_column.html'
+�with                      with                    with order_by='start'   order_by='project_details__project__name' order_by='project_details__project__account__name' with                      with                    with                     with                    order_by='facility_total_'|concat: order_by='facility_total_general' with                    with
+  order_by='invoice_number' order_by='created_date' name='Month' %}         name='Project' %}                         name='Account' %}                                  order_by='last_sent_date' order_by='due_date'     order_by='reviewed_date' order_by='total_amount' core_facility.id                   name="General" %}                 order_by='total_tax'    order_by='outstanding'
+  name='#' %}               name='Created' %}                                                                                                                            name='Sent' %}            name='Due' %}           name='Reviewed' %}       name='Total' %}         name=core_facility.name %}                                           name='Tax' %}           name='Outstanding' %}
+                            {% button size="xsmall"
+  {{ invoice.invoice_number type="view"
+�}}                        value="View"
+                            title="View invoice"
+                            url=view_invoice_url %}
 {% endblock %} {% block table_empty_content %}
-No invoices have been generated yet.
+No invoices could be found.
 {% endblock %} {% block after_pagination %}
  {% endblock %}
```

## NEMO_billing/invoices/templates/invoices/email/email_send_invoice_message.html

```diff
@@ -1,8 +1,8 @@
-<html>
+<html lang="en">
 <head>
 	<meta charset="utf-8">
 	<meta name="viewport" content="width=device-width, initial-scale=1">
 </head>
 <body style="font-family: 'Avenir Next', 'Helvetica Neue', 'Helvetica', 'Arial', 'sans-serif'">
 <!--[if mso]><table width="600" align="center"><tr><td><![endif]-->
 <table align="center" style="width:100%; max-width:600px">
```

## NEMO_billing/invoices/templates/invoices/email/email_send_invoice_reminder_message.html

```diff
@@ -1,8 +1,8 @@
-<html>
+<html lang="en">
 <head>
 	<meta charset="utf-8">
 	<meta name="viewport" content="width=device-width, initial-scale=1">
 </head>
 <body style="font-family: 'Avenir Next', 'Helvetica Neue', 'Helvetica', 'Arial', 'sans-serif'">
 <!--[if mso]><table width="600" align="center"><tr><td><![endif]-->
 <table align="center" style="width:100%; max-width:600px">
```

## NEMO_billing/invoices/templates/invoices/project/edit_project.html

```diff
@@ -5,21 +5,23 @@
 	{% load static %}
 	<script type="text/javascript" src="{% static "datetimepicker/bootstrap-datetimepicker.js" %}"></script>
 	<link rel="stylesheet" type="text/css" href="{% static "datetimepicker/bootstrap-datetimepicker.css" %}"/>
 {% endblock %}
 {% block content %}
 	{% with edit=form.instance.pk %}
 		<h1 class="form-group">{% if edit %}Edit{% else %}New{% endif %} project</h1>
-		{% if form.non_field_errors %}
-			<div class="alert alert-danger">
-				Oops! Something went wrong. The project was not created because:<br>
-				{{ form.non_field_errors }}
+		{% if form.errors %}
+			<div class="col-sm-12">
+				<div class="col-sm-6 alert alert-danger">
+					Oops! Something went wrong. Please correct the errors highlighted below.<br>
+					{{ form.non_field_errors }}
+				</div>
 			</div>
 		{% endif %}
-		<form method="post" action="{% if edit %}{% url 'invoices_edit_project' form.instance.id %}{% else %}{% url 'invoices_create_project' %}{% endif %}" class="form-horizontal">
+		<form id="project_form" method="post" action="{% if edit %}{% url 'invoices_edit_project' form.instance.id %}{% else %}{% url 'invoices_create_project' %}{% endif %}" class="form-horizontal" enctype="multipart/form-data">
 			{% csrf_token %}
 			<div class="form-group">
 				<label for="name" class="control-label col-sm-2"><b>Name</b></label>
 				<div class="col-sm-4">
 					<input type="text" name="name" id="name" maxlength="100" class="form-control" value="{{ form.name.value|default_if_none:'' }}" autofocus required>
 				</div>
 				<div class="col-sm-6 form-control-static danger-highlight">
@@ -33,22 +35,37 @@
 					<input type="button" id="selected_account" class="btn btn-default" onclick="clear_account_selection()" value="{% if edit %}{{ form.instance.account }}{% else %}{{ form.cleaned_data.account|default_if_none:"" }}{% endif %}" style="{% if not form.account.value %}display:none{% endif %}">
 				</div>
 				<div class="col-sm-6 form-control-static danger-highlight">
 					{{ form.account.errors|striptags }}
 				</div>
 			</div>
 			<div class="form-group">
-				<label for="application_identifier" class="control-label col-sm-2"><b>Reference/PO</b></label>
+				<label for="application_identifier" class="control-label col-sm-2"><b>{{ "projects_and_accounts"|customization:"project_application_identifier_name" }}</b></label>
 				<div class="col-sm-4">
 					<input type="text" name="application_identifier" id="application_identifier" maxlength="100" class="form-control" value="{{ form.application_identifier.value|default_if_none:'' }}" required>
 				</div>
 				<div class="col-sm-6 form-control-static danger-highlight">
 					{{ form.application_identifier.errors|striptags }}
 				</div>
 			</div>
+			{% if form.fields.discipline.choices.queryset %}
+				<div class="form-group">
+					<label for="discipline" class="control-label col-sm-2">Discipline</label>
+					<div class="col-sm-4">
+						<select name="discipline" id="discipline" class="form-control">
+							{% for discipline_id, discipline_name in form.fields.discipline.choices %}
+								<option value="{{ discipline_id }}" {% if discipline_id == form.discipline.value|to_int %}selected{% endif %}>{{ discipline_name|default_if_none:'' }}</option>
+							{% endfor %}
+						</select>
+					</div>
+					<div class="col-sm-6 form-control-static danger-highlight">
+						{{ form.discipline.errors|striptags }}
+					</div>
+				</div>
+			{% endif %}
 			{% if rate_categories %}
 				<div class="form-group">
 					<label for="category" class="control-label col-sm-2"><b>Rate Category</b></label>
 					<div class="col-sm-4">
 						<select name="category" id="category" class="form-control" required>
 							<option disabled selected value="">&nbsp;</option>
 							{% for rate_category in rate_categories %}
@@ -119,24 +136,24 @@
 				<div class="col-sm-6 form-control-static danger-highlight">
 					{{ form_details.comments.errors|striptags }}
 				</div>
 			</div>
 			<div class="form-group">
 				<label for="start_date" class="control-label col-sm-2">Start date</label>
 				<div class="col-sm-4">
-					<input type="text" id="start_date" name="start_date" class="form-control" placeholder="Choose a date" value="{{ form.start_date.value|date:"m/d/Y" }}">
+					<input type="text" id="start_date" name="start_date" class="form-control" placeholder="Choose a date" value="{{ form.start_date.value|input_date_format }}">
 				</div>
 				<div class="col-sm-6 form-control-static danger-highlight">
 					{{ form.start_date.errors|striptags }}
 				</div>
 			</div>
 			<div class="form-group">
 				<label for="expires_on" class="control-label col-sm-2">Expires on</label>
 				<div class="col-sm-2">
-					<input id="expires_on" name="expires_on" type="text" autocomplete="off" class="form-control" value="{{ form_details.expires_on.value|default_if_none:'' }}">
+					<input id="expires_on" name="expires_on" type="text" autocomplete="off" class="form-control" value="{{ form_details.expires_on.value|input_date_format }}">
 				</div>
 				<div class="col-sm-8 form-control-static danger-highlight">
 					{{ form_details.expires_on.errors|striptags }}
 				</div>
 			</div>
 			<div class="form-group">
 				<div class="col-sm-offset-2 col-sm-10">
@@ -152,26 +169,41 @@
 					<div class="checkbox">
 						<label>
 							<input type="checkbox" name="no_tax" {% if form_details.no_tax.value %}checked{% endif %}> Tax exempt
 						</label>
 					</div>
 				</div>
 			</div>
+			{% if form.instance.project_documents.all or allow_document_upload %}
+				<div class="form-group">
+					<span class="control-label col-sm-2">Documents</span>
+					<div class="col-sm-10">
+						{% for d in form.instance.project_documents.all %}
+							<div id="document_{{ d.id }}"><a href="javascript:mark_document_for_removal('{{ d.id }}')" class="grey hover-black" title="Remove {{ d.filename }}"><span class="glyphicon glyphicon-remove-circle"></span></a> <a href="{{ d.document.url }}" target="_blank" style="margin-right: 5px">{{ d.filename }}</a></div>
+						{% endfor %}
+					{% if allow_document_upload %}
+						<div style="padding-top: 10px">
+							<input id="fileupload" type="file" name="project_documents" multiple>
+						</div>
+					{% endif %}
+					</div>
+				</div>
+			{% endif %}
 			<div class="form-group">
 				<div class="col-sm-offset-2 col-sm-10">
 					<div class="checkbox">
 						<label>
 							<input type="checkbox" name="active" {% if form.active.value %}checked{% endif %}> Active
 						</label>
 					</div>
 				</div>
 			</div>
 			<div class="form-group">
 				<div class="col-sm-offset-2 col-sm-10">
-					<input type="submit" class="btn btn-success" value="{% if edit %}Save changes{% else %}Create new project{% endif %}">
+					{% button type="save" value=edit|yesno:"Save changes,Create new project" %}
 				</div>
 			</div>
 		</form>
 		<script>
 			function select_pi(jquery_event, search_selection, dataset_name)
 			{
 				$('#pi_search').typeahead('val', search_selection.id).hide();
@@ -188,17 +220,22 @@
 				$("#selected_account").val(search_selection.name).show();
 			}
 			function clear_account_selection()
 			{
 				$("#selected_account").hide();
 				$('#account_search').typeahead('val', '').show().focus();
 			}
+            function mark_document_for_removal(document_id)
+			{
+				$("#document_"+document_id).remove();
+				$("#project_form").append('<input type="hidden" name="remove_documents" value="'+document_id+'" />');
+			}
 			window.addEventListener('load', function ()
 			{
-				$("#expires_on").datetimepicker({format: 'MM/DD/YYYY'});
-				$("#start_date").datetimepicker({format: 'MM/DD/YYYY'});
+				$("#expires_on").datetimepicker({format: '{{ date_input_js_format }}'});
+				$("#start_date").datetimepicker({format: '{{ date_input_js_format }}'});
 			    $('#pi_search').autocomplete('pi', select_pi, {{ user_list|json_search_base }});
 				$('#account_search').autocomplete('account', select_account, {{ account_list|json_search_base }});
 			});
 		</script>
 	{% endwith %}
 {% endblock %}
```

### html2text {}

```diff
@@ -1,31 +1,39 @@
 {% extends 'base.html' %} {% load custom_tags_and_filters %} {% block title %}
 {% if form.instance.pk %}Edit{% else %}New{% endif %} project{% endblock %} {%
 block extrahead %} {% load static %}
 ootstrap-datetimepicker.js" %}">
 ootstrap-datetimepicker.css" %}"/> {% endblock %} {% block content %} {% with
 edit=form.instance.pk %}
 ****** {% if edit %}Edit{% else %}New{% endif %} project ******
-{% if form.non_field_errors %}
-Oops! Something went wrong. The project was not created because:
+{% if form.errors %}
+Oops! Something went wrong. Please correct the errors highlighted below.
 {{ form.non_field_errors }}
 {% endif %}
 {% csrf_token %}
 Name
 [{{ form.name.value|default_if_none:'' }}]
 {{ form.name.errors|striptags }}
 Account
  }}" {% if form.account.value %}style="display:none"{% else %} required{% endif
 %}>
  }}{% endif %}" style="{% if not form.account.value %}display:none{% endif %}">
 {{ form.account.errors|striptags }}
-Reference/PO
+{{ "projects_and_accounts"|customization:"project_application_identifier_name"
+}}
 [{{ form.application_identifier.value|default_if_none:'' }}]
 {{ form.application_identifier.errors|striptags }}
-{% if rate_categories %}
+{% if form.fields.discipline.choices.queryset %}
+Discipline
+{% for discipline_id, discipline_name in form.fields.discipline.choices %}
+% if discipline_id == form.discipline.value|to_int %}selected{% endif %}>{
+{ discipline_name|default_if_none:'' }}
+{% endfor %}
+{{ form.discipline.errors|striptags }}
+{% endif %} {% if rate_categories %}
 Rate Category
 {% for rate_category in rate_categories %}
 % if rate_category.id == form_details.category.value|to_int %}selected{% endif
 %}>{{ rate_category.name|default_if_none:'' }}
 {% endfor %}
 {{ form_details.category.errors|striptags }}
 {% endif %}
@@ -49,21 +57,29 @@
 {{ form_details.addressee.value|default_if_none:'' }}
 Addressee details will be displayed on the invoice
 {{ form_details.addressee.errors|striptags }}
 Comments
 {{ form_details.comments.value|default_if_none:'' }}
 {{ form_details.comments.errors|striptags }}
 Start date
-/Y" }}">
+[{{ form.start_date.value|input_date_format }}]
 {{ form.start_date.errors|striptags }}
 Expires on
-[{{ form_details.expires_on.value|default_if_none:'' }}]
+[{{ form_details.expires_on.value|input_date_format }}]
 {{ form_details.expires_on.errors|striptags }}
 
 % if form_details.no_charge.value %}checked{% endif %}> No charge (invoices
 will not be generated for this project)
 
 % if form_details.no_tax.value %}checked{% endif %}> Tax exempt
+{% if form.instance.project_documents.all or allow_document_upload %}
+Documents
+{% for d in form.instance.project_documents.all %}
+ {{_d.filename_}}
+{% endfor %} {% if allow_document_upload %}
+[File]
+{% endif %}
+{% endif %}
 
 % if form.active.value %}checked{% endif %}> Active
-[{% if edit %}Save changes{% else %}Create new project{% endif %}]
+{% button type="save" value=edit|yesno:"Save changes,Create new project" %}
  {% endwith %} {% endblock %}
```

## NEMO_billing/invoices/templates/invoices/project/view_project_additional_info.html

```diff
@@ -1,11 +1,13 @@
+{% load custom_tags_and_filters %}
 {% for project in projects %}
 	{% with billing_detail=project.projectbillingdetails %}
 		<div id="project_edit_button_{{ project.id }}" style="position: relative; display: inline; margin-left: 10px">
-			<button style="position: absolute" class="btn btn-xs btn-info" title="Edit" onclick="window.location = '{% url 'invoices_edit_project' project.id %}'"><i class="glyphicon glyphicon-pencil"></i></button>
+			{% url 'invoices_edit_project' project.id as edit_project_url %}
+			{% button type="edit" size="xsmall" style="position: absolute" value="Edit" url=edit_project_url %}
 		</div>
 		<div id="project_{{ project.id }}">
 			{% if billing_detail.project_name and billing_detail.project_name != billing_detail.project.name %}
 			<div>
 				<label class="control-label">Billing name:</label>
 				<span class="grey">{{ billing_detail.project_name }}</span>
 			</div>
```

## NEMO_billing/invoices/views/invoices.py

```diff
@@ -1,141 +1,271 @@
 import io
 import zipfile
 from datetime import datetime
 from decimal import Decimal
+from logging import getLogger
 from typing import List
 
-from NEMO.models import Project
-from NEMO.tasks import synchronized
-from NEMO.utilities import month_list
+from NEMO.decorators import accounting_or_user_office_or_manager_required, synchronized
+from NEMO.models import Account, Project
+from NEMO.utilities import date_input_format, month_list, queryset_search_filter
 from NEMO.views.pagination import SortedPaginator
 from django.conf import settings
 from django.contrib import messages
-from django.contrib.admin.views.decorators import staff_member_required
 from django.contrib.auth.decorators import login_required, permission_required
-from django.db.models import F, Sum, Case, When, DecimalField
-from django.db.models.functions import Coalesce
+from django.db.models import Case, F, Func, OuterRef, Prefetch, Subquery, Sum, When
+from django.db.models.functions import Coalesce, Length
 from django.http import HttpResponse
-from django.shortcuts import render, get_object_or_404, redirect
+from django.shortcuts import get_object_or_404, redirect, render
 from django.urls import reverse
 from django.utils import timezone
 from django.utils.formats import date_format
 from django.utils.safestring import mark_safe
 from django.views.decorators.http import require_GET, require_POST
 
+from NEMO_billing.decorators import accounting_or_manager_required
+from NEMO_billing.invoices.customization import InvoiceCustomization
 from NEMO_billing.invoices.exceptions import (
-    NoRateSetException,
-    NoProjectDetailsSetException,
     InvoiceAlreadyExistException,
+    InvoiceGenerationException,
     InvoiceItemsNotInFacilityException,
+    NoProjectCategorySetException,
+    NoProjectDetailsSetException,
+    NoRateSetException,
 )
-from NEMO_billing.invoices.invoice_generator import generate_monthly_invoice
-from NEMO_billing.invoices.models import Invoice, InvoiceConfiguration, InvoicePayment, InvoiceSummaryItem
+from NEMO_billing.invoices.models import (
+    BillableItemType,
+    Invoice,
+    InvoiceConfiguration,
+    InvoicePayment,
+    InvoiceSummaryItem,
+)
+from NEMO_billing.invoices.processors import invoice_data_processor_class as processor
+from NEMO_billing.invoices.renderers import CSVInvoiceRenderer
+from NEMO_billing.invoices.utilities import category_name_for_item_type
 from NEMO_billing.models import CoreFacility
+from NEMO_billing.rates.models import RateType
+
+invoices_logger = getLogger(__name__)
 
 
-@staff_member_required(login_url=None)
+@accounting_or_user_office_or_manager_required
 @require_GET
-def invoices(request):
+def invoices(request, year: int = None, month: int = None):
+    invoice_list = Invoice.objects.filter(voided_date=None)
+    if year:
+        invoice_list = invoice_list.filter(start__year=year)
+        if month:
+            invoice_list = invoice_list.filter(start__month=month)
+    # Add outstanding balance (sortable column)
+    outstanding_sub = (
+        InvoicePayment.objects.filter(invoice=OuterRef("pk"))
+        .annotate(total_payments=Coalesce(Func("amount", function="Sum"), Decimal(0)))
+        .values("total_payments")
+    )
+    invoice_list = invoice_list.annotate(outstanding=F("total_amount") - Subquery(outstanding_sub))
+
+    # Add total tax (sortable column). TODO: might need to change to subquery to avoid issue with duplicates in list of related fields
+    invoice_list = invoice_list.annotate(
+        total_tax=Sum(
+            Case(
+                When(
+                    invoicesummaryitem__summary_item_type=InvoiceSummaryItem.InvoiceSummaryItemType.TAX,
+                    then=F("invoicesummaryitem__amount"),
+                ),
+                default=Decimal(0),
+            )
+        )
+    )
+
+    core_facilities = CoreFacility.objects.all()
+
+    for facility in core_facilities:
+        sub = InvoiceSummaryItem.objects.filter(
+            invoice=OuterRef("pk"),
+            core_facility=facility.name,
+            summary_item_type=InvoiceSummaryItem.InvoiceSummaryItemType.SUBTOTAL,
+        ).values("amount")
+        invoice_list = invoice_list.annotate(**{f"facility_total_{facility.id}": Subquery(sub)})
+    # Add general (None) subtotal too
+    sub = InvoiceSummaryItem.objects.filter(
+        invoice=OuterRef("pk"), core_facility=None, summary_item_type=InvoiceSummaryItem.InvoiceSummaryItemType.SUBTOTAL
+    ).values("amount")
+    invoice_list = invoice_list.annotate(**{f"facility_total_general": Subquery(sub)})
 
-    # Add outstanding balance and total tax that will be sortable columns
+    # Prefetch facility subtotals, projects and configurations
     invoice_list = (
-        Invoice.objects.filter(voided_date=None)
-        .annotate(outstanding=F("total_amount") - Coalesce(Sum("invoicepayment__amount"), 0))
-        .annotate(
-            total_tax=Sum(
-                Case(
-                    When(
-                        invoicesummaryitem__summary_item_type=InvoiceSummaryItem.InvoiceSummaryItemType.TAX,
-                        then=F("invoicesummaryitem__amount"),
-                    ),
-                    output_field=DecimalField(),
-                    default=0,
-                )
+        invoice_list.prefetch_related(
+            Prefetch(
+                "invoicesummaryitem_set",
+                queryset=InvoiceSummaryItem.objects.filter(
+                    summary_item_type=InvoiceSummaryItem.InvoiceSummaryItemType.SUBTOTAL
+                ),
+                to_attr="facility_subtotals",
             )
         )
+        .prefetch_related("project_details__project")
+        .prefetch_related("configuration")
     )
 
-    page = SortedPaginator(invoice_list, request, order_by="-created_date").get_current_page()
+    # Fixed sort by number in case they are longer
+    paginator = SortedPaginator(invoice_list, request, order_by="-created_date")
+    order = request.GET.get("o")
+    if order == "-invoice_number":
+        paginator.object_list = paginator.object_list.order_by(Length("invoice_number").desc(), "-invoice_number")
+    elif order == "invoice_number":
+        paginator.object_list = paginator.object_list.order_by(Length("invoice_number").asc(), "invoice_number")
 
-    core_facilities = CoreFacility.objects.all()
+    page = paginator.get_current_page()
+
+    month_list_since = InvoiceCustomization.get_date("invoice_month_list_since", False) or datetime(
+        year=2021, month=1, day=1
+    )
 
     return render(
         request,
         "invoices/invoices.html",
         {
             "page": page,
-            "month_list": month_list(since=settings.INVOICE_MONTH_LIST_SINCE),
-            "projects": Project.objects.filter(active=True).order_by("account__name"),
+            "month_list": month_list(since=month_list_since),
+            "projects": Project.objects.prefetch_related("account").order_by("account__name"),
             "configuration_list": InvoiceConfiguration.objects.all(),
-            "invoices_search": Invoice.objects.all(),
+            "filter_month_list": Invoice.objects.filter(voided_date=None).dates("start", "month", order="DESC"),
+            "filter_year": year or datetime.now().year,
+            "filter_month": month,
+            "hide_columns": InvoiceCustomization.hide_column_names(),
             "core_facilities": core_facilities,
             "display_general_facility": not core_facilities.exists()
             or not settings.INVOICE_ALL_ITEMS_MUST_BE_IN_FACILITY,
         },
     )
 
 
-@staff_member_required(login_url=None)
+@accounting_or_manager_required
 @require_POST
 @synchronized()
 def generate_monthly_invoices(request):
+    extra_tags = "data-speed=30000"
+    warning_extra_tags = "data-speed=40000"
+    error_extra_tags = "data-speed=30000 trigger=manual"
+    generated_invoices = []
+    has_errors = True
     try:
-        project_id = request.POST["project_id"]
+        project_id: str = request.POST["project_id"]
         configuration_id = request.POST["configuration_id"]
         configuration = get_object_or_404(InvoiceConfiguration, id=configuration_id)
+        month = request.POST["month"]
         if project_id == "All":
-            for project in Project.objects.filter(active=True):
-                generate_monthly_invoice(request.POST["month"], project, configuration, request.user)
+            for account in Account.objects.all():
+                invoice_list = processor.generate_invoice_for_account(month, account, configuration, request.user)
+                generated_invoices.extend(invoice_list)
+        elif project_id.startswith("account:"):
+            account: Account = get_object_or_404(Account, id=project_id.replace("account:", ""))
+            invoice_list = processor.generate_invoice_for_account(month, account, configuration, request.user)
+            generated_invoices.extend(invoice_list)
         else:
             project = get_object_or_404(Project, id=project_id)
-            invoice = generate_monthly_invoice(request.POST["month"], project, configuration, request.user, True)
+            invoice = processor.generate_invoice_for_project(month, project, configuration, request.user, True)
             if not invoice:
-                messages.warning(request, f"No billable items were found for project: {project}")
+                messages.warning(request, f"No billable items were found for project: {project}", warning_extra_tags)
+        has_errors = False
     except NoProjectDetailsSetException as e:
         link = reverse("project", args=[e.project.id])
         message = "Invoice generation failed: " + e.msg + f" - click <a href='{link}'>here</a> to add some."
-        messages.error(request, mark_safe(message))
+        messages.error(request, mark_safe(message), error_extra_tags)
     except NoRateSetException as e:
-        link = reverse("rates")
+        link = create_rate_link(e.rate_type, e.tool, e.area, e.consumable)
         message = "Invoice generation failed: " + e.msg + f" - click <a href='{link}'>here</a> to create one."
-        messages.error(request, mark_safe(message))
+        messages.error(request, mark_safe(message), error_extra_tags)
     except InvoiceAlreadyExistException as e:
         link = reverse("view_invoice", args=[e.invoice.id])
         message = "Invoice generation failed: " + e.msg + f" - click <a href='{link}'>here</a> to view it."
-        messages.error(request, mark_safe(message))
+        messages.error(request, mark_safe(message), error_extra_tags)
+    except NoProjectCategorySetException as e:
+        link = reverse("project", args=[e.project.id])
+        message = "Invoice generation failed: " + e.msg + f" - click <a href='{link}'>here</a> to set it."
+        messages.error(request, mark_safe(message), error_extra_tags)
     except InvoiceItemsNotInFacilityException as e:
-        messages.error(request, e.msg)
+        messages.error(request, e.msg, error_extra_tags)
+    except InvoiceGenerationException as e:
+        link = reverse("re_render_invoice", args=e.invoice.id)
+        message = e.msg + f" - click <a href='{link}'>here</a> to try generating it again."
+        messages.error(request, mark_safe(message), error_extra_tags)
+    except Exception as e:
+        invoices_logger.exception(e)
+        messages.error(request, str(e), error_extra_tags)
+    if generated_invoices:
+        messages.success(request, f"{len(generated_invoices)} invoice(s) were generated successfully.", extra_tags)
+    else:
+        messages.warning(
+            request,
+            f"No invoices were generated. {'Either the invoices already exist or there was no usage for that month' if not has_errors else ' Please correct the issues and try again.'}",
+            warning_extra_tags,
+        )
     return redirect("invoices")
 
 
-@staff_member_required(login_url=None)
+@accounting_or_user_office_or_manager_required
+@require_GET
+def search_invoices(request):
+    return queryset_search_filter(
+        Invoice.objects.all(),
+        ["invoice_number", "project_details__project__name", "project_details__project__account__name"],
+        request,
+    )
+
+
+@accounting_or_user_office_or_manager_required
 @require_GET
 def view_invoice(request, invoice_id):
     invoice = get_object_or_404(Invoice, id=invoice_id)
-    return render(
-        request, "invoices/invoice.html", {"invoice": invoice, "core_facilities": CoreFacility.objects.exists()}
-    )
+    dictionary = {
+        "invoice": invoice,
+        "core_facilities": CoreFacility.objects.exists(),
+        "tool_title": category_name_for_item_type(BillableItemType.TOOL_USAGE),
+        "area_title": category_name_for_item_type(BillableItemType.AREA_ACCESS),
+        "staff_charge_title": category_name_for_item_type(BillableItemType.STAFF_CHARGE),
+        "consumable_title": category_name_for_item_type(BillableItemType.CONSUMABLE),
+        "training_title": category_name_for_item_type(BillableItemType.TRAINING),
+        "missed_reservation_title": category_name_for_item_type(BillableItemType.MISSED_RESERVATION),
+        "custom_charge_title": category_name_for_item_type(BillableItemType.CUSTOM_CHARGE),
+    }
+    return render(request, "invoices/invoice.html", dictionary)
+
 
+def create_rate_link(rate_type, tool, area, consumable):
+    try:
+        if rate_type and rate_type.type == RateType.Type.CONSUMABLE:
+            return reverse("create_rate", args=[RateType.Type.CONSUMABLE, consumable.id])
+        elif rate_type and rate_type.get_rate_group_type() == RateType.Type.TOOL:
+            return reverse("create_rate", args=[RateType.Type.TOOL, tool.id])
+        elif rate_type and rate_type.get_rate_group_type() == RateType.Type.AREA:
+            return reverse("create_rate", args=[RateType.Type.AREA, area.id])
+        elif rate_type:
+            reverse("create_rate", args=rate_type.type)
+    except:
+        pass
+    return reverse("create_rate")
 
-@staff_member_required(login_url=None)
+
+@accounting_or_manager_required
 @require_POST
 def review_invoice(request, invoice_id):
     invoice = get_object_or_404(Invoice, id=invoice_id)
     if not invoice.reviewed_date:
         invoice.reviewed_date = timezone.now()
         invoice.reviewed_by = request.user
         invoice.save()
         messages.success(request, f"Invoice {invoice.invoice_number} was successfully marked as reviewed.")
     else:
         messages.error(request, f"Invoice {invoice.invoice_number} has already been reviewed.")
     return redirect("view_invoice", invoice_id=invoice_id)
 
 
-@staff_member_required(login_url=None)
+@accounting_or_manager_required
 @require_POST
 def send_invoice(request, invoice_id):
     invoice = get_object_or_404(Invoice, id=invoice_id)
     if invoice.reviewed_date:
         if not invoice.project_details.email_to():
             link = reverse("project", args=[invoice.project_details.project.id])
             messages.error(
@@ -151,62 +281,101 @@
             else:
                 messages.error(request, f"Invoice {invoice.invoice_number} could not be sent.")
     else:
         messages.error(request, f"Invoice {invoice.invoice_number} needs to be reviewed before sending.")
     return redirect("view_invoice", invoice_id=invoice_id)
 
 
-@staff_member_required(login_url=None)
+@accounting_or_manager_required
 @require_POST
 def void_invoice(request, invoice_id):
     invoice = get_object_or_404(Invoice, id=invoice_id)
-    if not invoice.voided_date:
-        invoice.voided_date = timezone.now()
-        invoice.voided_by = request.user
-        invoice.save()
-        messages.success(request, f"Invoice {invoice.invoice_number} was successfully marked as void.")
-    else:
-        messages.error(request, f"Invoice {invoice.invoice_number} is already void.")
+    processor.void_invoice(invoice, request)
     return redirect("view_invoice", invoice_id=invoice_id)
 
 
-@staff_member_required(login_url=None)
+@accounting_or_manager_required
 @require_POST
-def zip_invoices(request):
+def delete_invoice(request, invoice_id):
+    invoice = get_object_or_404(Invoice, id=invoice_id)
+    processor.delete_invoice(invoice, request)
+    return redirect("invoices")
+
+
+@accounting_or_user_office_or_manager_required
+@require_POST
+def zip_invoices(request, file_type="file"):
     invoice_ids: List[str] = request.POST.getlist("selected_invoice_id[]")
     if not invoice_ids:
         return redirect("invoices")
     else:
-        return zip_response(request, Invoice.objects.filter(id__in=invoice_ids))
+        return zip_response(request, Invoice.objects.filter(id__in=invoice_ids), file_type)
+
+
+@accounting_or_user_office_or_manager_required
+@require_GET
+def re_render_invoice(request, invoice_id):
+    invoice = get_object_or_404(Invoice, pk=invoice_id)
+    try:
+        if invoice.file:
+            messages.warning(request, "This invoice already has a rendered invoice on file")
+        else:
+            invoice.render_and_save_file()
+            messages.success(request, "Invoice generated successfully")
+    except InvoiceGenerationException as e:
+        extra_tags = "data-speed=30000"
+        link = reverse("re_render_invoice", args=e.invoice.id)
+        message = e.msg + f" - click <a href='{link}'>here</a> to try generating it again."
+        messages.error(request, mark_safe(message), extra_tags)
+    return redirect(request.META.get("HTTP_REFERER", "invoices"))
+
+
+@accounting_or_user_office_or_manager_required
+@require_GET
+def csv_invoice(request, invoice_id):
+    invoice = get_object_or_404(Invoice, pk=invoice_id)
+    try:
+        invoice_renderer = CSVInvoiceRenderer()
+        content = invoice_renderer.render_invoice(invoice)
+        content.seek(0)
+        response = HttpResponse(content.read(), content_type="text/csv")
+        response[
+            "Content-Disposition"
+        ] = f'attachment; filename="{invoice.filename(invoice_renderer.get_file_extension())}"'
+        return response
+    except InvoiceGenerationException as e:
+        messages.error(request, e.msg)
+        return HttpResponse()
 
 
-@staff_member_required(login_url=None)
+@accounting_or_manager_required
 @require_POST
 def invoice_payment_received(request, invoice_id):
     invoice = get_object_or_404(Invoice, id=invoice_id)
     payment = InvoicePayment()
     payment.invoice = invoice
     payment.created_by = request.user
     payment.updated_by = request.user
-    payment.payment_received = datetime.strptime(request.POST["payment_received_date"], "%m/%d/%Y")
+    payment.payment_received = datetime.strptime(request.POST["payment_received_date"], date_input_format)
     payment.amount = Decimal(request.POST["payment_received_amount"])
+    payment.note = request.POST.get("payment_note")
     payment.save()
     messages.success(
         request,
         f"The payment of {payment.amount_display()} for invoice {invoice.invoice_number} was marked as received on {date_format(payment.payment_received)}.",
     )
     return redirect("view_invoice", invoice_id=invoice_id)
 
 
-@staff_member_required(login_url=None)
+@accounting_or_manager_required
 @require_POST
 def invoice_payment_processed(request, payment_id):
     payment = get_object_or_404(InvoicePayment, id=payment_id)
     payment.updated_by = request.user
-    payment.payment_processed = datetime.strptime(request.POST["payment_processed_date"], "%m/%d/%Y")
+    payment.payment_processed = datetime.strptime(request.POST["payment_processed_date"], date_input_format)
     payment.save()
     messages.success(
         request,
         f"The payment of {payment.amount_display()} for invoice {payment.invoice.invoice_number} was marked as processed on {date_format(payment.payment_processed)}.",
     )
     return redirect("view_invoice", invoice_id=payment.invoice_id)
 
@@ -234,19 +403,26 @@
                 )
                 # Send reminder if none has been sent yet, or if it's been too long
                 if too_long_since_last:
                     unpaid_invoice.send_reminder()
     return HttpResponse()
 
 
-def zip_response(request, invoice_list: List[Invoice]):
+def zip_response(request, invoice_list: List[Invoice], file_type="file"):
     generated_date = datetime.now().strftime("%Y-%m-%d_%H-%M-%S")
     parent_folder_name = f"invoices_{generated_date}"
     zip_io = io.BytesIO()
     with zipfile.ZipFile(zip_io, mode="w", compression=zipfile.ZIP_DEFLATED) as backup_zip:
+        csv_invoice_renderer = CSVInvoiceRenderer()
         for invoice in invoice_list:
-            if invoice.file:
+            if file_type.lower() == "csv":
+                ext = csv_invoice_renderer.get_file_extension()
+                content = csv_invoice_renderer.render_invoice(invoice)
+                content.seek(0)
+                backup_zip.writestr(f"{parent_folder_name}/" + invoice.filename_for_zip(ext), content.read())
+                content.close()
+            elif invoice.file:
                 backup_zip.write(invoice.file.path, f"{parent_folder_name}/" + invoice.filename_for_zip())
     response = HttpResponse(zip_io.getvalue(), content_type="application/x-zip-compressed")
     response["Content-Disposition"] = "attachment; filename=%s" % parent_folder_name + ".zip"
     response["Content-Length"] = zip_io.tell()
     return response
```

## NEMO_billing/invoices/views/project.py

```diff
@@ -1,42 +1,34 @@
-from datetime import datetime
+from datetime import date, datetime, timedelta
 
+from NEMO.decorators import accounting_or_user_office_or_manager_required
 from NEMO.forms import ProjectForm
-from NEMO.models import Project, Account, User, MembershipHistory, ActivityHistory
+from NEMO.models import Account, ActivityHistory, MembershipHistory, Project, ProjectDocuments, User
+from NEMO.utilities import render_combine_responses
 from NEMO.views.accounts_and_projects import select_accounts_and_projects
-from django.contrib.admin.views.decorators import staff_member_required
+from NEMO.views.customization import ProjectsAccountsCustomization
 from django.contrib.auth.decorators import login_required, permission_required
 from django.forms import models
 from django.http import HttpResponse
-from django.shortcuts import render, redirect
-from django.views.decorators.http import require_http_methods, require_GET
+from django.shortcuts import redirect, render
+from django.views.decorators.http import require_GET, require_http_methods
 
+from NEMO_billing.invoices.customization import BillingCustomization
 from NEMO_billing.invoices.models import ProjectBillingDetails
-from NEMO_billing.invoices.utilities import render_combine_responses
+from NEMO_billing.invoices.utilities import render_and_send_email
 from NEMO_billing.rates.models import RateCategory
 
 
 class ProjectDetailsForm(models.ModelForm):
     class Meta:
         model = ProjectBillingDetails
-        fields = [
-            "category",
-            "project_name",
-            "contact_name",
-            "contact_phone",
-            "contact_email",
-            "addressee",
-            "comments",
-            "no_charge",
-            "no_tax",
-            "expires_on",
-        ]
+        exclude = ["project"]
 
 
-@staff_member_required(login_url=None)
+@accounting_or_user_office_or_manager_required
 @require_http_methods(["GET", "POST"])
 def edit_project(request, project_id=None):
     try:
         project = Project.objects.get(id=project_id)
     except (Project.DoesNotExist, ValueError):
         project = None
     try:
@@ -45,21 +37,24 @@
         project_details = ProjectBillingDetails(project=project)
     form = ProjectForm(request.POST or None, instance=project)
     details_form = ProjectDetailsForm(request.POST or None, instance=project_details)
     dictionary = {
         "account_list": Account.objects.all(),
         "user_list": User.objects.filter(is_active=True),
         "rate_categories": RateCategory.objects.all(),
+        "allow_document_upload": ProjectsAccountsCustomization.get_bool("project_allow_document_upload"),
         "form": form,
         "form_details": details_form,
     }
     if request.method == "GET":
         return render(request, "invoices/project/edit_project.html", dictionary)
     elif request.method == "POST":
         if not form.is_valid() or not details_form.is_valid():
+            if request.FILES.getlist("project_documents") or request.POST.get("remove_documents"):
+                form.add_error(field=None, error="Project document changes were lost, please resubmit them.")
             return render(request, "invoices/project/edit_project.html", dictionary)
         else:
             project = form.save()
             details_form.instance.project = project
             details_form.save()
             active_changed = form.initial.get("active", None) != project.active
             account_changed = form.initial.get("account", None) != project.account.id
@@ -79,40 +74,66 @@
                 account_history.save()
             if not project_id or active_changed:
                 project_history = ActivityHistory()
                 project_history.authorizer = request.user
                 project_history.action = project.active
                 project_history.content_object = project
                 project_history.save()
+
+            # Handle file uploads
+            for f in request.FILES.getlist("project_documents"):
+                ProjectDocuments.objects.create(document=f, project=project)
+            ProjectDocuments.objects.filter(id__in=request.POST.getlist("remove_documents")).delete()
+
             return redirect("project", project.id)
 
 
-@staff_member_required(login_url=None)
+@accounting_or_user_office_or_manager_required
 @require_http_methods(["GET", "POST"])
 def custom_project_view(request, kind=None, identifier=None):
     original_response = select_accounts_and_projects(request, kind=kind, identifier=identifier)
     projects = []
     if kind == "project":
         projects = Project.objects.filter(id=identifier)
     elif kind == "account":
         projects = Project.objects.filter(account_id=identifier)
-    rate_categories = RateCategory.objects.exists()
     return render_combine_responses(
         request,
         original_response,
         "invoices/project/view_project_additional_info.html",
-        {"projects": projects, "rate_categories": rate_categories},
+        {"projects": projects, "rate_categories": RateCategory.objects.exists()},
     )
 
 
 @login_required
 @require_GET
 @permission_required("NEMO.trigger_timed_services", raise_exception=True)
 def deactivate_expired_projects(request):
     return do_deactivate_expired_projects()
 
 
 def do_deactivate_expired_projects():
     for project in Project.objects.filter(active=True, projectbillingdetails__expires_on__lt=datetime.now()):
         project.active = False
         project.save()
+    send_project_expiration_reminders()
     return HttpResponse()
+
+
+def send_project_expiration_reminders():
+    accounting_email = BillingCustomization.get("billing_accounting_email_address")
+    expiration_reminder_days = BillingCustomization.get("billing_project_expiration_reminder_days")
+    if accounting_email and expiration_reminder_days:
+        project_expiration_reminder_cc = BillingCustomization.get("billing_project_expiration_reminder_cc")
+        ccs = [e for e in project_expiration_reminder_cc.split(",") if e]
+        for remaining_days in [int(days) for days in expiration_reminder_days.split(",")]:
+            expiration_date = date.today() + timedelta(days=remaining_days)
+            for project in Project.objects.filter(active=True, projectbillingdetails__expires_on=expiration_date):
+                send_to = project.projectbillingdetails.email_to()
+                if send_to:
+                    render_and_send_email(
+                        "invoices/email/billing_project_expiration_reminder_email",
+                        {"project": project, "remaining_days": remaining_days},
+                        to=send_to,
+                        from_email=accounting_email,
+                        cc=ccs,
+                    )
```

## NEMO_billing/rates/__init__.py

```diff
@@ -1,28 +1 @@
-00000000: 6672 6f6d 2064 6a61 6e67 6f2e 6170 7073  from django.apps
-00000010: 2069 6d70 6f72 7420 4170 7043 6f6e 6669   import AppConfi
-00000020: 670a 0a66 726f 6d20 2e20 696d 706f 7274  g..from . import
-00000030: 2061 7070 5f73 6574 7469 6e67 7320 6173   app_settings as
-00000040: 2064 6566 6175 6c74 730a 6672 6f6d 2064   defaults.from d
-00000050: 6a61 6e67 6f2e 636f 6e66 2069 6d70 6f72  jango.conf impor
-00000060: 7420 7365 7474 696e 6773 0a0a 2320 5365  t settings..# Se
-00000070: 7420 736f 6d65 2061 7070 2064 6566 6175  t some app defau
-00000080: 6c74 2073 6574 7469 6e67 730a 666f 7220  lt settings.for 
-00000090: 6e61 6d65 2069 6e20 6469 7228 6465 6661  name in dir(defa
-000000a0: 756c 7473 293a 0a20 2020 2069 6620 6e61  ults):.    if na
-000000b0: 6d65 2e69 7375 7070 6572 2829 2061 6e64  me.isupper() and
-000000c0: 206e 6f74 2068 6173 6174 7472 2873 6574   not hasattr(set
-000000d0: 7469 6e67 732c 206e 616d 6529 3a0a 2020  tings, name):.  
-000000e0: 2020 2020 2020 7365 7461 7474 7228 7365        setattr(se
-000000f0: 7474 696e 6773 2c20 6e61 6d65 2c20 6765  ttings, name, ge
-00000100: 7461 7474 7228 6465 6661 756c 7473 2c20  tattr(defaults, 
-00000110: 6e61 6d65 2929 0a0a 0a63 6c61 7373 204e  name))...class N
-00000120: 454d 4f52 6174 6573 436f 6e66 6967 2841  EMORatesConfig(A
-00000130: 7070 436f 6e66 6967 293a 0a20 2020 206e  ppConfig):.    n
-00000140: 616d 6520 3d20 224e 454d 4f5f 6269 6c6c  ame = "NEMO_bill
-00000150: 696e 672e 7261 7465 7322 0a20 2020 2076  ing.rates".    v
-00000160: 6572 626f 7365 5f6e 616d 6520 3d20 2252  erbose_name = "R
-00000170: 6174 6573 220a 0a0a 6465 6661 756c 745f  ates"...default_
-00000180: 6170 705f 636f 6e66 6967 203d 2022 4e45  app_config = "NE
-00000190: 4d4f 5f62 696c 6c69 6e67 2e72 6174 6573  MO_billing.rates
-000001a0: 2e4e 454d 4f52 6174 6573 436f 6e66 6967  .NEMORatesConfig
-000001b0: 220a                                     ".
+00000000: 0a                                       .
```

## NEMO_billing/rates/admin.py

```diff
@@ -1,30 +1,189 @@
+from datetime import datetime
+from typing import List
+
 from django import forms
-from django.contrib import admin
+from django.contrib import admin, messages
 from django.contrib.admin import register
-
-from NEMO_billing.rates.models import RateType, Rate, RateLog, RateCategory
+from django.db.models import Q
+from django.forms import BaseInlineFormSet
+from django.urls import reverse
+from django.utils.safestring import mark_safe
+
+from NEMO_billing.rates.models import DailySchedule, Rate, RateCategory, RateLog, RateTime, RateType
+
+
+class AtLeastOneRequiredInlineFormSet(BaseInlineFormSet):
+    def clean(self):
+        """Check that at least one item has been entered."""
+        super().clean()
+        if any(self.errors):
+            return
+        if not any(cleaned_data and not cleaned_data.get("DELETE", False) for cleaned_data in self.cleaned_data):
+            raise forms.ValidationError("A minimum of one item is required.")
+
+
+def delete_rates_with_message(request, rates: List[Rate], message=None):
+    if rates:
+        for rate in rates:
+            delete_message = f"{rate} was deleted"
+            if message:
+                delete_message += f" ({message})"
+            messages.warning(request, delete_message)
+            rate.delete_with_user(request.user)
+
+
+@register(RateCategory)
+class RateCategoryAdmin(admin.ModelAdmin):
+    list_display = ("name",)
+
+    def save_model(self, request, obj, form, change):
+        super().save_model(request, obj, form, change)
+        # On add of first category, delete all category specific rates without a category
+        delete_rates_with_message(
+            request,
+            Rate.non_deleted().filter(type__category_specific=True, category__isnull=True),
+            "rate is category specific but had no category",
+        )
 
 
 @register(RateType)
 class RateTypeAdmin(admin.ModelAdmin):
     list_display = ("type", "category_specific", "item_specific")
-    readonly_fields = ("type",)
+
+    def get_readonly_fields(self, request, obj=None):
+        if obj:
+            return self.readonly_fields + ("type",)
+        return self.readonly_fields
+
+    def save_model(self, request, obj, form, change):
+        old_rate_type = None
+        if obj.pk:
+            old_rate_type = RateType.objects.get(pk=obj.pk)
+        super().save_model(request, obj, form, change)
+        if old_rate_type:
+            categories_exists = RateCategory.objects.exists()
+            rate_qs = Rate.non_deleted()
+            # Not category specific becomes category specific: delete old matching rates with no category (unless no Categories exist)
+            if categories_exists and not old_rate_type.category_specific and obj.category_specific:
+                delete_rates_with_message(
+                    request,
+                    rate_qs.filter(type=obj, category__isnull=True),
+                    "had no category and rate type is now category specific",
+                )
+            # Not item specific becomes item specific: delete old matching rates with no item
+            if not old_rate_type.item_specific and obj.item_specific:
+                delete_rates_with_message(
+                    request,
+                    rate_qs.filter(type=obj, tool__isnull=True, area__isnull=True, consumable__isnull=True),
+                    "had no item and rate type is now item specific",
+                )
+            # Category specific becomes not category specific: delete old matching rates with categories
+            if old_rate_type.category_specific and not obj.category_specific:
+                delete_rates_with_message(
+                    request,
+                    rate_qs.filter(type=obj, category__isnull=False),
+                    "had a category and rate type is now non-category specific",
+                )
+            # Item specific becomes not item specific: delete old matching rates with items
+            if old_rate_type.item_specific and not obj.item_specific:
+                delete_rates_with_message(
+                    request,
+                    rate_qs.filter(type=obj).filter(
+                        Q(tool__isnull=False) | Q(area__isnull=False) | Q(consumable__isnull=False)
+                    ),
+                    "had an item and rate type is now non-item specific",
+                )
 
 
 class RateAdminForm(forms.ModelForm):
+    def __init__(self, *args, **kwargs):
+        self.form_number = kwargs.pop("form_number", None)
+        super().__init__(*args, **kwargs)
+
+    def display_title(self):
+        return f"{self.instance.type}{self.instance.display_category_time()}"
+
+    def has_rate_amount(self):
+        self.full_clean()
+        amount_field = self.cleaned_data.get("amount")
+        return amount_field == 0 or amount_field
+
     class Meta:
         model = Rate
         fields = "__all__"
 
 
+class DailyScheduleAdminFormset(AtLeastOneRequiredInlineFormSet):
+    def clean(self):
+        # check that there is no overlap between each of the schedules in this formset
+        super().clean()
+        if any(self.errors):
+            return
+        if len(self.forms) > 1:
+            previous_schedules = []
+            control_datetime = datetime.today()
+            for form in self.forms:
+                if self.can_delete and self._should_delete_form(form) or not form.cleaned_data:
+                    continue
+                schedule = DailySchedule(
+                    start_time=form.cleaned_data.get("start_time"),
+                    end_time=form.cleaned_data.get("end_time"),
+                    weekday=form.cleaned_data.get("weekday"),
+                )
+                for previous_schedule in previous_schedules:
+                    if previous_schedule.overlaps(control_datetime, schedule):
+                        raise forms.ValidationError(f"{previous_schedule} overlaps with {schedule}")
+                previous_schedules.append(schedule)
+
+
+class DailyScheduleAdminInline(admin.TabularInline):
+    model = DailySchedule
+    formset = DailyScheduleAdminFormset
+    min_num = 1
+    extra = 0
+
+
+class RateTimeAdminForm(forms.ModelForm):
+    class Meta:
+        model = RateTime
+        fields = "__all__"
+
+
+@register(RateTime)
+class RateTimeAdmin(admin.ModelAdmin):
+    form = RateTimeAdminForm
+    inlines = (DailyScheduleAdminInline,)
+    list_display = ("name", "get_schedules_display")
+
+    @admin.display(description="Schedule")
+    def get_schedules_display(self, rate_time: RateTime) -> str:
+        return mark_safe("<br>".join([str(schedule) for schedule in DailySchedule.objects.filter(rate_time=rate_time)]))
+
+
 @register(Rate)
 class RateAdmin(admin.ModelAdmin):
     form = RateAdminForm
-    list_display = ("get_item", "type", "category", "amount", "flat", "minimum_charge")
+    list_display = ("get_item", "type", "category", "time", "amount", "flat", "minimum_charge")
+    list_filter = ("type", "category", "time", "flat", "tool", "area", "consumable", "deleted")
+
+    def get_queryset(self, request):
+        # All of this to only show non-deleted rates
+        try:
+            # We have to match only the rate list URL since this queryset function is used to also edit etc.
+            rates_url = reverse("admin:rates_rate_changelist")
+            if request.path.endswith(rates_url):
+                deleted_in_request = (
+                    request and request.GET and any([param for param in request.GET if "deleted" in param.lower()])
+                )
+                if not deleted_in_request:
+                    return super().get_queryset(request).filter(deleted=False)
+        except:
+            pass
+        return super().get_queryset(request)
 
     def formfield_for_foreignkey(self, db_field, request, **kwargs):
         if db_field.name == "type":
             return super().formfield_for_foreignkey(db_field, request, **kwargs)
         return super().formfield_for_foreignkey(db_field, request, **kwargs)
 
     def save_model(self, request, obj: Rate, form, change):
@@ -40,27 +199,22 @@
 
 @register(RateLog)
 class RateLogAdmin(admin.ModelAdmin):
     list_display = ("id", "action", "user", "date", "get_content_object_display")
     list_filter = ["action"]
     date_hierarchy = "date"
 
+    @admin.display(description="Item", ordering="content_type")
     def get_content_object_display(self, rate_log: RateLog):
         content_object = rate_log.content_object
         if not content_object:
             content_object = "Staff Charge"
         return content_object
 
-    get_content_object_display.admin_order_field = "content_type"  # Allows column order sorting
-    get_content_object_display.short_description = "Item"  # Renames column head
-
     def has_delete_permission(self, request, obj=None):
         return False
 
     def has_add_permission(self, request):
         return False
 
     def has_change_permission(self, request, obj=None):
         return False
-
-
-admin.site.register(RateCategory)
```

## NEMO_billing/rates/app_settings.py

```diff
@@ -1 +1,2 @@
 RATES_CLASS = "NEMO_billing.rates.rates_class.DatabaseRates"
+DEFAULT_MISSED_RESERVATION_FLAT = True
```

## NEMO_billing/rates/models.py

```diff
@@ -1,42 +1,52 @@
+from datetime import datetime, time, timedelta
 from decimal import Decimal
 from logging import getLogger
+from typing import Any, List, Optional, Tuple
 
-from NEMO.models import Tool, Area, Consumable, User
+from NEMO.models import Area, BaseModel, Consumable, Tool, User
+from NEMO.utilities import as_timezone, format_datetime
 from django.contrib.contenttypes.fields import GenericForeignKey
 from django.contrib.contenttypes.models import ContentType
-from django.core.exceptions import ValidationError, NON_FIELD_ERRORS
+from django.core.exceptions import NON_FIELD_ERRORS, ValidationError
 from django.db import models
 from django.db.models import QuerySet
+from django.urls import reverse
+from django.utils.safestring import mark_safe
 from mptt.fields import TreeForeignKey
 
 from NEMO_billing.rates.model_diff import ModelDiff
 
 model_logger = getLogger(__name__)
 
 
+DAYS = ["Monday", "Tuesday", "Wednesday", "Thursday", "Friday", "Saturday", "Sunday"]
+MIDNIGHT = time(0, 0, 0, 0)
+
+
 class ActionLog(object):
     ADD = 0
     DELETE = 1
     UPDATE = 2
     Choices = ((ADD, "Add"), (DELETE, "Delete"), (UPDATE, "Update"))
 
 
-class RateCategory(models.Model):
-    name = models.CharField(max_length=200, help_text="The name of this rate category")
+class RateCategory(BaseModel):
+    name = models.CharField(max_length=200, help_text="The name of this rate category", unique=True)
 
     def __str__(self):
         return self.name
 
     class Meta:
         verbose_name = "Rate category"
         verbose_name_plural = "Rate categories"
+        ordering = ["name"]
 
 
-class RateType(models.Model):
+class RateType(BaseModel):
     class Type(object):
         TOOL = "Tool"
         TOOL_USAGE = "TOOL_USAGE"
         TOOL_TRAINING_INDIVIDUAL = "TOOL_TRAINING_INDIVIDUAL"
         TOOL_TRAINING_GROUP = "TOOL_TRAINING_GROUP"
         TOOL_MISSED_RESERVATION = "TOOL_MISSED_RESERVATION"
         AREA = "Area"
@@ -90,34 +100,162 @@
         if self.is_tool_rate() and self.item_specific:
             return RateType.Type.TOOL
         elif self.is_area_rate() and self.item_specific:
             return RateType.Type.AREA
         else:
             return self.type
 
-    def get_type_form_name(self, category: RateCategory = None):
-        # name to use in forms to identify
-        name = str(self.type).lower()
-        if self.category_specific and category:
-            name = name + "_" + category.name.lower()
-        return name
+    def can_have_rate_time(self):
+        return self.type not in [
+            RateType.Type.CONSUMABLE,
+            RateType.Type.TOOL_TRAINING_GROUP,
+            RateType.Type.TOOL_TRAINING_INDIVIDUAL,
+        ]
+
+    def clean(self):
+        if (
+            self.type
+            and not self.item_specific
+            and self.type in [self.Type.TOOL_USAGE, self.Type.AREA_USAGE, self.Type.CONSUMABLE]
+        ):
+            raise ValidationError({"item_specific": "This rate has to be item specific"})
+
+    def validate_unique(self, exclude=None):
+        super().validate_unique(exclude)
+        if not exclude or exclude and "type" not in exclude and self.type:
+            if self.pk is None and RateType.objects.filter(type=self.type).exists():
+                raise ValidationError({"type": f"There is already a {self.get_type_display()} rate type"})
 
     def __str__(self):
         return self.get_type_display()
 
 
-class Rate(models.Model):
+class RateTime(BaseModel):
+    name = models.CharField(max_length=255, unique=True)
+
+    def earliest_match(self, start_time: datetime, end_time: datetime) -> Optional[Tuple[datetime, datetime]]:
+        # This function returns the earliest start (and end time) this time applies to in the daterange if any.
+        # For example if this RateTime is MON-FRI 4-5PM, given a start (MON 3PM) and end (MON 8PM),
+        # It will send back the earliest start & end date times (MON 4PM to MON 5PM) when this applies
+        start_time_tz = as_timezone(start_time)
+        end_time_tz = as_timezone(end_time)
+        possible_dates: List[Tuple[datetime, datetime]] = []
+        # Loop over 2 weeks, to make sure we go over all days
+        for i in [0, 1]:
+            datetime_control = start_time_tz + timedelta(weeks=i)
+            for time_and_day in self.dailyschedule_set.all():
+                start_datetime, end_datetime = time_and_day.datetime_range(datetime_control)
+                # If there is overlap, add start to list
+                if (start_time_tz < end_datetime) and (end_time_tz > start_datetime):
+                    possible_dates.append((max(start_time_tz, start_datetime), min(end_time_tz, end_datetime)))
+        return min(possible_dates) if possible_dates else (None, None)
+
+    def overlaps(self, rate_time) -> bool:
+        # Function returning whether this rate time overlaps with another
+        # They overlap if any of their schedules overlap
+        control_datetime = datetime.today()
+        for daily_schedule in self.dailyschedule_set.all():
+            for other_daily_schedule in rate_time.dailyschedule_set.all():
+                if daily_schedule.overlaps(control_datetime, other_daily_schedule):
+                    return True
+        return False
+
+    def __str__(self):
+        return self.name
+
+
+class DailySchedule(BaseModel):
+    rate_time = models.ForeignKey(RateTime, on_delete=models.CASCADE)
+    weekday = models.IntegerField(verbose_name="start day", choices=[(DAYS.index(day_name), day_name) for day_name in DAYS])
+    start_time = models.TimeField(blank=True, null=True, help_text="The start time")
+    end_time = models.TimeField(blank=True, null=True, help_text="The end time")
+
+    def datetime_range(self, control_datetime) -> (datetime, datetime):
+        # Given a control datetime, a weekday, start and end time, returns a full datetime range
+        beginning_of_the_week = control_datetime - timedelta(days=control_datetime.weekday())
+        start_day = beginning_of_the_week + timedelta(days=self.weekday)
+        start_datetime = datetime.combine(start_day, self.start_time or MIDNIGHT, control_datetime.tzinfo)
+        end_datetime = start_datetime + timedelta(seconds=self.duration().total_seconds())
+        return start_datetime, end_datetime
+
+    def overlaps(self, control_datetime: datetime, daily_schedule) -> bool:
+        first_start, first_end = self.datetime_range(control_datetime)
+        second_start, second_end = daily_schedule.datetime_range(control_datetime)
+        return first_start < second_end and first_end > second_start
+
+    def is_time_range_split(self):
+        # Returns whether the time range is across 2 days, like 6pm - 6am
+        # We have to treat midnight separately since 6pm - 12am is not split even though 6pm is technically after 12am
+        return self.start_time and self.end_time and self.start_time >= self.end_time != MIDNIGHT
+
+    def duration(self) -> timedelta:
+        today = datetime.today()
+        start_datetime = datetime.combine(today, self.start_time or MIDNIGHT)
+        end_datetime = datetime.combine(today, self.end_time or MIDNIGHT)
+        end_edge_cases = not self.end_time or self.end_time == MIDNIGHT or self.end_time == self.start_time
+        if self.is_time_range_split() or end_edge_cases:
+            end_datetime = end_datetime + timedelta(days=1)
+        return end_datetime - start_datetime
+
+    def clean(self):
+        errors = {}
+        if self.weekday == 6 and self.is_time_range_split():
+            errors["end_time"] = ValidationError(
+                "Sunday schedule has to end at Midnight at the latest (add a Monday schedule if needed)"
+            )
+        # Check for rates already using this time
+        if self.rate_time and self.rate_time.pk:
+            control_datetime = datetime.today()
+            for rate in self.rate_time.rate_set.all():
+                rate_filter = rate.rate_queryset_uniqueness()
+                if rate_filter.exists():
+                    # Check for overlapping times on previous rates
+                    for other_rate_with_time in rate_filter:
+                        for other_daily_schedule in other_rate_with_time.time.dailyschedule_set.all():
+                            if self.overlaps(control_datetime, other_daily_schedule):
+                                link = reverse("admin:rates_ratetime_change", args=[other_rate_with_time.time.id])
+                                errors[NON_FIELD_ERRORS] = ValidationError(
+                                    mark_safe(
+                                        f'This time would now overlap with {other_rate_with_time}<br>Click <a href="{link}">here</a> to change the other rate time'
+                                    )
+                                )
+        if errors:
+            raise ValidationError(errors)
+
+    def __str__(self):
+        end_time = (
+            format_datetime(self.end_time)
+            if self.end_time and not self.end_time == MIDNIGHT and not self.is_time_range_split()
+            else f"{next_as_loop(DAYS, self.get_weekday_display())}, {format_datetime(self.end_time or MIDNIGHT)}"
+        )
+        return f"{self.get_weekday_display()}, {format_datetime(self.start_time or MIDNIGHT)} to {end_time}"
+
+    class Meta:
+        ordering = ("weekday", "start_time")
+
+
+class Rate(BaseModel):
     type = models.ForeignKey(RateType, on_delete=models.CASCADE)
+    time = models.ForeignKey(RateTime, null=True, blank=True, on_delete=models.CASCADE)
     category = models.ForeignKey(RateCategory, null=True, blank=True, on_delete=models.CASCADE)
     tool = models.ForeignKey(Tool, null=True, blank=True, on_delete=models.CASCADE)
     area = TreeForeignKey(Area, null=True, blank=True, on_delete=models.CASCADE)
     consumable = models.ForeignKey(Consumable, null=True, blank=True, on_delete=models.CASCADE)
-    amount = models.DecimalField(decimal_places=2, max_digits=8, help_text="The rate per hour if this isn't a flat rate")
+    amount = models.DecimalField(
+        decimal_places=2, max_digits=8, help_text="The rate per hour if this isn't a flat rate"
+    )
     flat = models.BooleanField(default=False, help_text="Check this box to make this a flat rate (independent of time)")
-    minimum_charge = models.DecimalField(decimal_places=2, max_digits=8, null=True, blank=True, help_text="The minimum charge for this rate")
+    minimum_charge = models.DecimalField(
+        decimal_places=2, max_digits=8, null=True, blank=True, help_text="The minimum charge for this rate"
+    )
+    deleted = models.BooleanField(default=False, help_text="Indicates that this rate was deleted")
+
+    @classmethod
+    def non_deleted(cls):
+        return cls.objects.filter(deleted=False)
 
     def get_item(self):
         if self.type.is_tool_rate():
             return self.tool
         elif self.type.is_area_rate():
             return self.area
         elif self.type.is_consumable_rate():
@@ -162,131 +300,153 @@
                 errors[NON_FIELD_ERRORS] = ValidationError(
                     "You cannot select a tool, area or consumable for a non item specific rate type"
                 )
             if RateCategory.objects.exists() and self.type.category_specific and not self.category:
                 errors["category"] = ValidationError("This rate type is category specific. Please select a category")
             if not self.type.category_specific and self.category:
                 errors["category"] = ValidationError("The rate type you selected is not category specific")
+            # We cannot have different rate times for Consumable or Training rates
+            if self.time:
+                if not self.type.can_have_rate_time():
+                    errors["time"] = ValidationError("This rate type doesn't allow different rate times")
+                elif self.flat:
+                    errors["time"] = ValidationError("A flat rate cannot have different schedule/times")
         if errors:
             raise ValidationError(errors)
 
-    def validate_unique(self, exclude=None):
-        super().validate_unique(exclude)
-        if exclude and "type" not in exclude and self.type:
-            # Essentially a type that is category_specific but no categories exist is the same as non category specific
-            category_specific = self.type.category_specific and RateCategory.objects.exists()
-            if not category_specific and not self.type.item_specific:
-                rate_already_exists = Rate.objects.filter(type=self.type).exclude(pk=self.pk).exists()
-                if rate_already_exists:
-                    raise ValidationError("A rate of this type already exists")
-            elif not category_specific and self.type.item_specific:
-                rate_already_exists = (
-                    self.rate_item_filter(Rate.objects.filter(type=self.type)).exclude(pk=self.pk).exists()
-                )
-                if rate_already_exists:
-                    raise ValidationError(f"A rate of this type already exists for {self.get_item()}")
-            elif category_specific and self.type.item_specific:
-                rate_already_exists = (
-                    self.rate_item_filter(Rate.objects.filter(type=self.type, category=self.category))
-                    .exclude(pk=self.pk)
-                    .exists()
-                )
-                if rate_already_exists:
-                    raise ValidationError(
-                        f"A rate of this type already exists for {self.get_item()} and category {self.category}"
-                    )
-            elif category_specific and not self.type.item_specific:
-                rate_already_exists = (
-                    Rate.objects.filter(type=self.type, category=self.category).exclude(pk=self.pk).exists()
-                )
-                if rate_already_exists:
-                    raise ValidationError(f"A rate of this type already exists for category {self.category}")
+    def rate_queryset_uniqueness(self) -> QuerySet:
+        # This function returns a queryset used to check for other rates of the same type and category/item if applicable
+        # Essentially a type that is category_specific but no categories exist is the same as non category specific
+        category_specific = self.type.category_specific and RateCategory.objects.exists()
+        rate_filter = Rate.non_deleted().filter(time__isnull=not self.time).exclude(pk=self.pk)
+        if not category_specific and not self.type.item_specific:
+            rate_filter = rate_filter.filter(type=self.type)
+        elif not category_specific and self.type.item_specific:
+            rate_filter = self.rate_item_filter(rate_filter.filter(type=self.type))
+        elif category_specific and self.type.item_specific:
+            rate_filter = self.rate_item_filter(rate_filter.filter(type=self.type, category=self.category))
+        elif category_specific and not self.type.item_specific:
+            rate_filter = rate_filter.filter(type=self.type, category=self.category)
+        return rate_filter
 
     def rate_item_filter(self, queryset: QuerySet) -> QuerySet:
         if self.type:
             if self.type.is_tool_rate():
                 return queryset.filter(tool=self.tool)
             elif self.type.is_area_rate():
                 return queryset.filter(area=self.area)
             elif self.type.is_consumable_rate():
                 return queryset.filter(consumable=self.consumable)
         return queryset
 
+    def validate_unique(self, exclude=None):
+        super().validate_unique(exclude)
+        if not exclude or exclude and "type" not in exclude and self.type:
+            error_message = f"A rate of this type already exists or overlaps this one"
+            rate_filter = self.rate_queryset_uniqueness()
+            if rate_filter.exists():
+                # If we have a time, check for overlapping times on previous rates
+                if self.time:
+                    for other_rate_with_time in rate_filter:
+                        if self.time.overlaps(other_rate_with_time.time):
+                            raise ValidationError(mark_safe(f"{error_message}: {str(other_rate_with_time)}"))
+                else:
+                    already_existing_rate = rate_filter.first()
+                    raise ValidationError(mark_safe(f"{error_message}: {str(already_existing_rate)}"))
+
     # Use this method instead of regular save to allow rates audit log
     def save_with_user(self, user: User, force_insert=False, force_update=False, using=None, update_fields=None):
         try:
             rate_pre_save_log(self, user)
         except Exception as e:
             model_logger.exception(e)
         super().save(force_insert, force_update, using, update_fields)
 
-    def delete_with_user(self, user: User, using=None, keep_parents=False):
+    def delete_with_user(self, user: User):
         try:
             rate_pre_delete_log(self, user)
         except Exception as e:
             model_logger.exception(e)
-        return super().delete(using, keep_parents)
+        self.deleted = True
+        self.save(update_fields=["deleted"])
 
     def is_hourly_rate(self):
         return self.type.type in [
             RateType.Type.TOOL_USAGE,
             RateType.Type.AREA_USAGE,
             RateType.Type.STAFF_CHARGE,
             RateType.Type.TOOL_TRAINING_GROUP,
             RateType.Type.TOOL_TRAINING_INDIVIDUAL,
+            RateType.Type.AREA_MISSED_RESERVATION,
+            RateType.Type.TOOL_MISSED_RESERVATION,
         ]
 
     def display_rate(self) -> str:
         amount = f"{self.amount:.2f}"
         if self.is_hourly_rate():
             if self.flat:
-                # Display flat explicitly when we have a hourly rate set as flat
+                # Display flat explicitly when we have an hourly rate set as flat
                 amount = f"flat {amount}"
             else:
                 # Display hourly when we have an hourly rate not set as flat
                 amount = f"{amount}/hr"
         minimum = f" ({self.minimum_charge:.2f} minimum)" if self.minimum_charge else ""
         return f"{amount}{minimum}"
 
     def calculate_amount(self, quantity: Decimal) -> Decimal:
         effective_quantity = quantity
         if self.is_hourly_rate():
             if self.flat:
                 # If hourly rate is set as flat, disregard quantity
                 effective_quantity = 1
             else:
-                # Otherwise divide by 60 since quantity is in minutes
+                # Otherwise, divide by 60 since quantity is in minutes
                 effective_quantity = quantity / Decimal(60)
         amount = effective_quantity * self.amount
         if self.minimum_charge:
             amount = max(amount, self.minimum_charge)
         return amount
 
+    def display_category_time(self):
+        category = self.category.name if self.category else None
+        rate_time = self.time.name if self.time else None
+        cat_time = (
+            [category, rate_time]
+            if category and rate_time
+            else [category]
+            if category
+            else [rate_time]
+            if rate_time
+            else []
+        )
+        return f" ({'/'.join(cat_time)})" if cat_time else ""
+
     def __str__(self):
         item_name = f"{self.get_item()} " if self.get_item() else ""
-        category = self.category if self.category else ""
-        return f"{item_name}{self.type} {category}"
+        category = f" ({self.category})" if self.category else ""
+        rate_time = f", {self.time}" if self.time else ""
+        return f"{item_name}{self.type}{category}{rate_time}"
 
 
-class RateLog(models.Model):
+class RateLog(BaseModel):
     content_type = models.ForeignKey(ContentType, null=True, on_delete=models.SET_NULL)
     object_id = models.PositiveIntegerField(null=True)
     content_object = GenericForeignKey("content_type", "object_id")
     action = models.IntegerField(choices=ActionLog.Choices)
     date = models.DateTimeField(auto_now_add=True)
     user = models.ForeignKey(User, on_delete=models.CASCADE)
     details = models.TextField(null=True, blank=True)
 
 
 def get_rate_content_object(rate: Rate):
     item = rate.get_item()
     return item if isinstance(item, models.Model) else None
 
 
-def rate_pre_save_log(rate: Rate, user: User, **kwargs):
+def rate_pre_save_log(rate: Rate, user: User):
     try:
         original: Rate = Rate.objects.get(pk=rate.pk)
     except Rate.DoesNotExist:
         RateLog.objects.create(
             action=ActionLog.ADD,
             user=user,
             content_object=get_rate_content_object(rate),
@@ -299,14 +459,25 @@
                 action=ActionLog.UPDATE,
                 user=user,
                 content_object=get_rate_content_object(original),
                 details=model_diff.model_diff_display,
             )
 
 
-def rate_pre_delete_log(rate: Rate, user: User, **kwargs):
+def rate_pre_delete_log(rate: Rate, user: User):
     RateLog.objects.create(
         action=ActionLog.DELETE,
         user=user,
         content_object=get_rate_content_object(rate),
         details=ModelDiff(rate).model_diff_display,
     )
+
+
+def next_as_loop(elements: List, match: Any, backwards=False) -> Any:
+    # this function returns the next element after the match, looping back to the beginning if the match is the last one
+    # or if reverse is True, the previous element before the match, looping back to the end if match is first element
+    # For example, next_as_loop([1,2,3,4,5], 5) will return 1 and next_as_loop([1,2,3,4,5], 1, backwards) will return 5
+    index_match = elements.index(match)
+    if not backwards:
+        return elements[0] if index_match == len(elements) - 1 else elements[index_match + 1]
+    else:
+        return elements[len(elements) - 1] if index_match == 0 else elements[index_match - 1]
```

## NEMO_billing/rates/rates_class.py

```diff
@@ -1,50 +1,73 @@
 from itertools import groupby
-from typing import List, Dict
+from typing import Dict, Iterable, List
 
 from NEMO.models import Consumable, Tool
 from NEMO.rates import Rates
+from NEMO.utilities import distinct_qs_value_list
 from django.conf import settings
 from django.utils.formats import number_format
 
-from NEMO_billing.rates.models import Rate
+from NEMO_billing.invoices.models import InvoiceConfiguration
+from NEMO_billing.invoices.processors import get_rate_with_currency
+from NEMO_billing.rates.models import Rate, RateCategory
 
 
 class DatabaseRates(Rates):
+
+    expand_rates_table = False
+
     def __init__(self):
         self.currency = getattr(settings, "RATE_CURRENCY", "$")
+        self.configuration = InvoiceConfiguration.first_or_default()
 
-    def load_rates(self):
-        pass
+    def load_rates(self, force_reload=False):
+        super().load_rates(force_reload=force_reload)
 
     def get_consumable_rates(self, consumables: List[Consumable]) -> Dict[str, str]:
         return {
             rate.consumable.name: self.consumable_rate_display(rate)
-            for rate in Rate.objects.filter(consumable__in=consumables)
+            for rate in Rate.non_deleted().filter(consumable__in=consumables)
         }
 
     def get_consumable_rate(self, consumable: Consumable) -> str:
-        consumable_rate = Rate.objects.get(consumable=consumable)
+        consumable_rate = Rate.non_deleted().get(consumable=consumable)
         if consumable_rate.exists():
             return self.consumable_rate_display(consumable_rate)
 
     def get_tool_rate(self, tool: Tool) -> str:
-        tool_rates = Rate.objects.filter(tool=tool).order_by("type", "category")
-        list_by_type = groupby(tool_rates, key=lambda x: x.type)
-        return "<br>".join(
-            [
-                f"{rate_type.get_type_display()}: {self.tool_rate_display_by_category(tool_rates)}"
-                for rate_type, tool_rates in list_by_type
-            ]
-        )
+        all_tool_rates = Rate.non_deleted().filter(tool=tool).order_by("type", "category")
+        if not all_tool_rates:
+            return ""
+        list_by_type = groupby(all_tool_rates, key=lambda x: x.type)
+        rate_categories = distinct_qs_value_list(all_tool_rates, "category")
+        rate_categories = sorted([RateCategory.objects.get(id=cat_id).name for cat_id in rate_categories if cat_id])
+        html_rate = f'<div class="media"><a onclick="toggle_details(this)" class="pointer collapsed" data-toggle="collapse" data-target="#rates_details"><span class="glyphicon glyphicon-list-alt pull-left notification-icon primary-highlight"></span><span class="glyphicon pull-left chevron glyphicon-chevron-{"down" if self.get_expand_rates_table() else "right"}"></span></a>'
+        html_rate += f'<div class="media-body"><span class="media-heading">Rates</span><div id="rates_details" class="collapse {"in" if self.get_expand_rates_table() else ""}"><table class="table table-bordered table-hover thead-light" style="width: auto !important; margin-bottom: 0">'
+        if rate_categories:
+            html_rate += '<tr><th class="text-center"></th><th class="text-center">'
+            html_rate += '</th><th class="text-center">'.join(rate_categories)
+            html_rate += "</tr>"
+        for rate_type, tool_rates in list_by_type:
+            html_rate += (
+                f'<tr><th class="text-center" style="vertical-align: middle">{rate_type.get_type_display()}</th>'
+            )
+            if not rate_type.category_specific or not RateCategory.objects.exists():
+                html_rate += f'<td class="text-center" style="vertical-align: middle" colspan="{len(rate_categories)}">{self.tool_rate_display_with_details(tool_rates)}</td>'
+            else:
+                for rate_category in rate_categories:
+                    tool_rate_category = all_tool_rates.filter(type=rate_type, category__name=rate_category)
+                    html_rate += f'<td class="text-center" style="vertical-align: middle">{self.tool_rate_display_with_details(tool_rate_category)}</td>'
+        html_rate += "</tr></table></div></div></div>"
+        return html_rate
 
-    def tool_rate_display_by_category(self, rates: List[Rate]):
-        return ", ".join(
+    def tool_rate_display_with_details(self, rates: Iterable[Rate]):
+        return "<br>".join(
             [
-                f"<b>{self.display_amount(rate.amount)}</b>{' (' + rate.category.name + ')' if rate.category else ''}"
+                f"{get_rate_with_currency(self.configuration, rate.display_rate())}{' (' + rate.time.name + ')' if rate.time else ''}"
                 for rate in rates
             ]
         )
 
     def consumable_rate_display(self, rate: Rate) -> str:
         return f"<b>{self.display_amount(rate.amount)}</b>"
```

## NEMO_billing/rates/urls.py

```diff
@@ -1,10 +1,18 @@
+from NEMO.urls import router
 from django.urls import path
 
-from NEMO_billing.rates import views
+from NEMO_billing.rates import api, views
+
+# Rest API URLs
+router.register(r"rates", api.RateViewSet)
+router.register(r"rate_types", api.RateTypeViewSet)
 
 urlpatterns = [
     path("rates/", views.rates, name="rates"),
+    path("rates/<str:rate_type_choice>/", views.rates, name="rates"),
     path("rate/", views.create_or_modify_rate, name="create_rate"),
     path("rate/<str:rate_type_choice>/", views.create_or_modify_rate, name="create_rate"),
-    path("rate/<str:rate_type_choice>/<int:rate_id>/", views.create_or_modify_rate, name="edit_rate"),
+    path("rate/<str:rate_type_choice>/<int:item_id>/", views.create_or_modify_rate, name="create_rate"),
+    path("rate_form/", views.new_time_rate_form, name="new_time_rate_form"),
+    path("rate_time/<int:rate_id>/", views.delete_rate_time, name="delete_rate_time"),
 ]
```

## NEMO_billing/rates/views.py

```diff
@@ -1,150 +1,189 @@
-from typing import List, Dict, Tuple
+from typing import List, Tuple
 
-from NEMO.models import Tool, Area, Consumable
+from NEMO.models import Area, Consumable, Tool
+from NEMO.utilities import distinct_qs_value_list
 from NEMO.views.pagination import SortedPaginator
+from django.conf import settings
 from django.contrib import messages
-from django.contrib.admin.views.decorators import staff_member_required
-from django.db.models import Model
-from django.shortcuts import render, redirect
+from django.db.models import Q
+from django.http import HttpResponse, HttpResponseBadRequest
+from django.shortcuts import get_object_or_404, redirect, render
 from django.utils.html import escape
 from django.utils.safestring import mark_safe
-from django.views.decorators.http import require_http_methods, require_GET
+from django.views.decorators.http import require_GET, require_http_methods
 
+from NEMO_billing.decorators import accounting_or_manager_required
 from NEMO_billing.rates.admin import RateAdminForm
-from NEMO_billing.rates.models import RateCategory, Rate, RateType
+from NEMO_billing.rates.customization import BillingRatesCustomization
+from NEMO_billing.rates.models import Rate, RateCategory, RateTime, RateType
 
 
-@staff_member_required(login_url=None)
+@accounting_or_manager_required
 @require_GET
-def rates(request):
-    page = SortedPaginator(Rate.objects.all(), request, order_by="type").get_current_page()
+def rates(request, rate_type_choice: str = None):
+    rate_type = rate_type_choice or RateType.Type.TOOL
+    rate_types = get_rate_types(rate_type)
+    rate_order_by = [rate_type.lower(), "type", "category", "time"]
+    if rate_type_choice and rate_type_choice.lower() == "other":
+        rate_types = RateType.objects.filter(item_specific=False)
+        rate_order_by = []
+    rate_qs = Rate.non_deleted()
+    page_qs = rate_qs.filter(type__in=rate_types).order_by(*rate_order_by)
+    page = SortedPaginator(page_qs, request, order_by="type" if not rate_order_by else None).get_current_page()
+    # remove when fixed in NEMO (allowing no order_type)
+    if rate_order_by:
+        page.paginator.order_by = ""
 
     # Creating rates list for search autocomplete
-    type_filter = set()
-    search_rates = "["
-    for item in Rate.objects.all():
-        identifier = (
-            item.get_item().id if item.type.item_specific else item.id if not item.type.category_specific else ""
+    rate_search = "["
+    for tool_id in distinct_qs_value_list(rate_qs.filter(tool__isnull=False), "tool"):
+        tool = Tool.objects.get(pk=tool_id)
+        rate_search += '{{"name":"{0}", "id":{1}, "type_value": "{2}"}},'.format(
+            escape(tool.name), tool_id, RateType.Type.TOOL
         )
-        type_name = f"{item.type.get_rate_group_type()}_{identifier}"
-        if type_name not in type_filter:
-            type_filter.add(type_name)
-            item_name = str(item.get_item() or str(item.type))
-            search_rates += '{{"name":"{0}", "id":{1}, "type": "{2}", "type_value": "{3}"}},'.format(
-                escape(item_name), item.id, item.type.get_rate_group_type().upper(), item.type.get_rate_group_type()
-            )
-    search_rates = search_rates.rstrip(",") + "]"
-    search_rates = mark_safe(search_rates)
+    for area_id in distinct_qs_value_list(rate_qs.filter(area__isnull=False), "area"):
+        area = Area.objects.get(pk=area_id)
+        rate_search += '{{"name":"{0}", "id":{1}, "type_value": "{2}"}},'.format(
+            escape(area.name), area_id, RateType.Type.AREA
+        )
+    for consumable_id in distinct_qs_value_list(rate_qs.filter(consumable__isnull=False), "consumable"):
+        consumable = Consumable.objects.get(pk=consumable_id)
+        rate_search += '{{"name":"{0}", "id":{1}, "type_value": "{2}"}},'.format(
+            escape(consumable.name), consumable_id, RateType.Type.CONSUMABLE
+        )
+    for rate_type_item in RateType.objects.all():
+        if not rate_type_item.item_specific:
+            if rate_qs.filter(type=rate_type_item).exists():
+                rate_search += '{{"name":"{0}", "id":"{1}", "type_value": "{2}"}},'.format(
+                    escape(str(rate_type_item)), "", rate_type_item.get_rate_group_type()
+                )
+    rate_search = rate_search.rstrip(",") + "]"
+    rate_search = mark_safe(rate_search)
 
-    return render(
-        request,
-        "rates/rates.html",
-        {"page": page, "rate_categories_exist": RateCategory.objects.exists(), "search_rates": search_rates},
-    )
+    dictionary = {
+        "rate_type": rate_type,
+        "page": page,
+        "show_type": page_qs.values("type").distinct().count() > 1 or rate_type.lower() == "other",
+        "show_category": page_qs.filter(category__isnull=False).exists(),
+        "show_time": page_qs.filter(time__isnull=False).exists(),
+        "search_rates": rate_search,
+    }
+
+    return render(request, "rates/rates.html", dictionary)
 
 
-@staff_member_required(login_url=None)
+@accounting_or_manager_required
 @require_http_methods(["GET", "POST"])
-def create_or_modify_rate(request, rate_type_choice=None, rate_id=None):
-    rate = None
-    try:
-        rate = Rate.objects.get(id=rate_id)
-    except Rate.DoesNotExist:
-        pass
+def create_or_modify_rate(request, rate_type_choice=None, item_id=None):
+    tool = get_object_or_404(Tool, pk=item_id) if item_id and rate_type_choice == RateType.Type.TOOL else None
+    area = get_object_or_404(Area, pk=item_id) if item_id and rate_type_choice == RateType.Type.AREA else None
+    consumable = (
+        get_object_or_404(Consumable, pk=item_id) if item_id and rate_type_choice == RateType.Type.CONSUMABLE else None
+    )
+
+    # Add children tools here too, they should be able to have a rate even though they are not visible
+    tools = list(Tool.objects.filter(Q(visible=True) | Q(parent_tool__isnull=False)))
+    # Because we are showing tool children, we cannot sort the queryset (child tool has no category)
+    tools.sort(key=lambda x: (x.category, x.name))
+    rate_types = get_rate_types(rate_type_choice)
 
     dictionary = {
+        "rate_types": rate_types,
         "rate_type_choice": rate_type_choice,
+        "item": tool or area or consumable,
         "rate_type_choices": get_rate_type_choices(),
-        "rate_id": rate_id,
         "rate_categories": RateCategory.objects.all(),
+        "rate_times": RateTime.objects.all(),
+        "tools": tools,
+        "areas": Area.objects.filter(area_children_set__isnull=True),
+        "consumables": Consumable.objects.all().order_by("category", "name"),
     }
-    rate_types = get_rate_types(rate_type_choice)
-    rate_forms = get_rate_forms(request, rate_types, rate)
-    dictionary["rate_types"] = rate_types
-    dictionary["forms"] = rate_forms
-    dictionary["form"] = list(rate_forms.values())[0] if rate_forms else None
 
-    if rate_type_choice == RateType.Type.TOOL:
-        dictionary["tools"] = Tool.objects.filter(visible=True).order_by("_category", "name")
-    elif rate_type_choice == RateType.Type.AREA:
-        dictionary["areas"] = Area.objects.filter(area_children_set__isnull=True)
-    elif rate_type_choice == RateType.Type.CONSUMABLE:
-        dictionary["consumables"] = Consumable.objects.all().order_by("category", "name")
-
-    forms_all_valid = all([form.is_valid() for form in rate_forms.values()]) if rate_forms else False
-    if request.method == "POST" and forms_all_valid:
-        # Don't commit since we want to save it using our own method
-        for rate_form in rate_forms.values():
-            form_rate: Rate = rate_form.save(commit=False)
-            form_rate.save_with_user(request.user)
-            rate_form.save_m2m()
-            message_item = f" for {form_rate.get_item()}" if isinstance(form_rate.get_item(), Model) else ""
-            message = f'Your {form_rate.type.get_type_display()} rate{message_item} was successfully {"updated" if rate_id else "created"}.'
-            messages.success(request, message=message)
-        return redirect("rates")
+    if request.method == "GET":
+        rate_forms = get_forms(request, rate_types, tool, area, consumable)
     else:
-        return render(request, "rates/rate.html", dictionary)
+        rate_forms = post_forms(request)
+        # We do a first pass to check that all forms are valid
+
+        forms_to_validate = rate_forms
+        forms_to_delete = []
+        allow_blank_rates = BillingRatesCustomization.get("allow_blank_rate") == "enabled"
+        if allow_blank_rates:
+            forms_to_validate = [form for form in rate_forms if form.has_rate_amount()]
+            forms_to_delete = [form for form in rate_forms if not form.has_rate_amount() and form.instance.id]
+        all_forms_valid = all([form.is_valid() for form in forms_to_validate]) if forms_to_validate else False
+        if all_forms_valid:
+            for rate_form in forms_to_validate:
+                # We have to check the form validity each time we save a rate, in case the next one breaks uniqueness for example
+                rate_form.full_clean()
+                if not rate_form.is_valid():
+                    dictionary["forms"] = rate_forms
+                    return render(request, "rates/rate.html", dictionary)
+                # Don't commit since we want to save it using our own method
+                form_rate: Rate = rate_form.save(commit=False)
+                form_rate.save_with_user(request.user)
+                rate_form.save_m2m()
+            for rate_form_delete in forms_to_delete:
+                rate_form_delete.instance.delete()
+            message = f"Your rates were successfully saved."
+            messages.success(request, message=message)
+            return redirect("rates")
+
+    dictionary["forms"] = rate_forms
+    return render(request, "rates/rate.html", dictionary)
 
 
 # We are building forms for each rate type, for each category.
 # The goal is to have all rate forms related to one group type (Tool, Area, Supply etc.) in one view.
-def get_rate_forms(request, rate_types: List[RateType], rate: Rate) -> Dict[str, RateAdminForm]:
-    forms = {}
+def get_forms(request, rate_types: List[RateType], tool, area, consumable) -> List[RateAdminForm]:
+    forms = []
     categories = RateCategory.objects.all()
+    missed_reservation_flat = getattr(settings, "DEFAULT_MISSED_RESERVATION_FLAT", True)
+    # Create a form for each rate type
+    count = 0
     for rate_type in rate_types:
+        missed_r_type = rate_type.type in [RateType.Type.TOOL_MISSED_RESERVATION, RateType.Type.AREA_MISSED_RESERVATION]
+        default_flat = missed_r_type and missed_reservation_flat or rate_type.type == RateType.Type.CONSUMABLE
         if rate_type.category_specific and categories:
+            # Add a form for each category
             for category in categories:
-                rate_type_name = rate_type.get_type_form_name(category)
-                data = get_data_from_request(request, rate_type, category)
-                instance = None
-                if rate:
-                    try:
-                        instance = Rate.objects.get(
-                            type=rate_type,
-                            category=category,
-                            tool_id=rate.tool_id,
-                            area_id=rate.area_id,
-                            consumable_id=rate.consumable_id,
-                        )
-                    except Rate.DoesNotExist:
-                        pass
-                forms[rate_type_name] = RateAdminForm(data=data, instance=instance)
+                count, n_forms = init_forms(request, count, rate_type, default_flat, tool, area, consumable, category)
+                forms.extend(n_forms)
         else:
-            rate_type_name = rate_type.get_type_form_name()
-            data = get_data_from_request(request, rate_type)
-            instance = None
-            if rate:
-                try:
-                    instance = Rate.objects.get(
-                        type=rate_type, tool_id=rate.tool_id, area_id=rate.area_id, consumable_id=rate.consumable_id
-                    )
-                except Rate.DoesNotExist:
-                    pass
-            forms[rate_type_name] = RateAdminForm(data=data, instance=instance)
+            count, n_forms = init_forms(request, count, rate_type, default_flat, tool, area, consumable)
+            forms.extend(n_forms)
     return forms
 
 
-def get_data_from_request(request, rate_type: RateType, category: RateCategory = None):
-    # Get data from request. We have common fields and type/category specific fields
-    if request.method != "POST":
-        return None
-    data = {
-        "type": rate_type.id,
-        "category": category.id if category else "",
-        "tool": request.POST.get("tool"),
-        "area": request.POST.get("area"),
-        "consumable": request.POST.get("consumable"),
-    }
-    type_form_name = rate_type.get_type_form_name(category)
-    data["id"] = request.POST.get(type_form_name + "_id")
-    data["amount"] = request.POST.get(type_form_name + "_amount")
-    data["flat"] = request.POST.get(type_form_name + "_flat")
-    data["minimum_charge"] = request.POST.get(type_form_name + "_minimum_charge")
-    return data
+def init_forms(request, count, rate_type, flat, tool=None, area=None, consumable=None, category=None):
+    forms = []
+    previous_rates = Rate.non_deleted().filter(type=rate_type, category=category, tool=tool, area=area, consumable=consumable)
+    if previous_rates.exists():
+        for prev_rate in previous_rates:
+            count = count + 1
+            forms.append(RateAdminForm(form_number=count, instance=prev_rate))
+    else:
+        count = count + 1
+        instance = Rate(type=rate_type, category=category, tool=tool, area=area, consumable=consumable, flat=flat)
+        forms.append(RateAdminForm(form_number=count, instance=instance))
+    return count, forms
+
+
+def post_forms(request) -> List[RateAdminForm]:
+    forms = []
+    form_numbers: List[str] = request.POST.getlist("form_numbers[]")
+    for form_number in form_numbers:
+        data = {}
+        for field in ["type", "category", "time", "tool", "area", "consumable", "amount", "flat", "minimum_charge"]:
+            data[field] = request.POST.get(form_number + "_" + field)
+        rate_id = request.POST.get(form_number + "_id")
+        instance = Rate.objects.get(pk=rate_id) if rate_id else None
+        forms.append(RateAdminForm(form_number=form_number, data=data, instance=instance))
+    return forms
 
 
 def get_rate_type_choices() -> List[Tuple[str, str]]:
     # Since we want to group all tool related types, we only have a subset here
     # Return a list of (value, display value) for use in a select
     rate_type_choices = set()
     for rate_type in RateType.objects.all():
@@ -155,15 +194,15 @@
         elif rate_type.is_consumable_rate() and rate_type.item_specific:
             rate_type_choices.add((rate_type.type, rate_type.get_type_display()))
         else:
             rate_type_choices.add((rate_type.type, rate_type.get_type_display()))
     return sorted(rate_type_choices)
 
 
-def get_rate_types(rate_type_choice: str):
+def get_rate_types(rate_type_choice: str) -> List[RateType]:
     rate_types = []
     if rate_type_choice:
         if rate_type_choice == RateType.Type.TOOL:
             rate_types = RateType.objects.filter(
                 type__in=[
                     RateType.Type.TOOL_USAGE,
                     RateType.Type.TOOL_MISSED_RESERVATION,
@@ -177,7 +216,42 @@
                 type__in=[RateType.Type.AREA_USAGE, RateType.Type.AREA_MISSED_RESERVATION], item_specific=True
             )
         elif rate_type_choice == RateType.Type.CONSUMABLE:
             rate_types = RateType.objects.filter(type=RateType.Type.CONSUMABLE)
         else:
             rate_types = RateType.objects.filter(type=rate_type_choice)
     return rate_types
+
+
+@accounting_or_manager_required
+@require_GET
+def new_time_rate_form(request):
+    rate_type = get_object_or_404(RateType, pk=int(request.GET["type"]))
+    category_id = request.GET.get("category", None) or None
+    tool_id = request.GET.get("tool", None) or None
+    area_id = request.GET.get("area", None) or None
+    consumable_id = request.GET.get("consumable", None) or None
+    count = request.GET["count"]
+    missed_reservation_flat = getattr(settings, "DEFAULT_MISSED_RESERVATION_FLAT", True)
+    missed_r_type = rate_type.type in [RateType.Type.TOOL_MISSED_RESERVATION, RateType.Type.AREA_MISSED_RESERVATION]
+    default_flat = missed_r_type and missed_reservation_flat or rate_type.type == RateType.Type.CONSUMABLE
+    instance = Rate(
+        type=rate_type,
+        category_id=category_id,
+        tool_id=tool_id,
+        area_id=area_id,
+        consumable_id=consumable_id,
+        flat=default_flat,
+    )
+    rate_form = RateAdminForm(form_number=count, instance=instance)
+    dictionary = {"rate_form": rate_form, "show_rate_time": True, "rate_times": RateTime.objects.all()}
+    return render(request, "rates/rate_form_details.html", dictionary)
+
+
+@accounting_or_manager_required
+@require_GET
+def delete_rate_time(request, rate_id):
+    rate = get_object_or_404(Rate, pk=rate_id)
+    if not rate.time:
+        return HttpResponseBadRequest("You can only delete rates with time")
+    rate.delete_with_user(request.user)
+    return HttpResponse()
```

## NEMO_billing/rates/templates/rates/rate.html

```diff
@@ -2,284 +2,377 @@
 00000010: 732f 6261 7365 2e68 746d 6c27 2025 7d0a  s/base.html' %}.
 00000020: 7b25 206c 6f61 6420 6375 7374 6f6d 5f74  {% load custom_t
 00000030: 6167 735f 616e 645f 6669 6c74 6572 7320  ags_and_filters 
 00000040: 257d 0a7b 2520 626c 6f63 6b20 7469 746c  %}.{% block titl
 00000050: 6520 257d 5261 7465 7b25 2065 6e64 626c  e %}Rate{% endbl
 00000060: 6f63 6b20 257d 0a7b 2520 626c 6f63 6b20  ock %}.{% block 
 00000070: 636f 6e74 656e 7420 257d 0a09 3c68 313e  content %}..<h1>
-00000080: 7b25 2069 6620 7261 7465 5f69 6420 257d  {% if rate_id %}
-00000090: 4564 6974 7b25 2065 6c73 6520 257d 4372  Edit{% else %}Cr
-000000a0: 6561 7465 7b25 2065 6e64 6966 2025 7d20  eate{% endif %} 
-000000b0: 7261 7465 3c2f 6831 3e0a 097b 2520 6966  rate</h1>..{% if
-000000c0: 2066 6f72 6d2e 6572 726f 7273 2025 7d0a   form.errors %}.
-000000d0: 0909 3c64 6976 2063 6c61 7373 3d22 616c  ..<div class="al
-000000e0: 6572 7420 616c 6572 742d 6461 6e67 6572  ert alert-danger
-000000f0: 223e 0a09 0909 4f6f 7073 2120 536f 6d65  ">....Oops! Some
-00000100: 7468 696e 6720 7765 6e74 2077 726f 6e67  thing went wrong
-00000110: 2e20 506c 6561 7365 2063 6f72 7265 6374  . Please correct
-00000120: 2074 6865 2065 7272 6f72 7320 6869 6768   the errors high
-00000130: 6c69 6768 7465 6420 6265 6c6f 772e 3c62  lighted below.<b
-00000140: 723e 0a09 0909 7b7b 2066 6f72 6d2e 6e6f  r>....{{ form.no
-00000150: 6e5f 6669 656c 645f 6572 726f 7273 207d  n_field_errors }
-00000160: 7d0a 0909 3c2f 6469 763e 0a09 7b25 2065  }...</div>..{% e
-00000170: 6e64 6966 2025 7d0a 097b 2520 6966 206e  ndif %}..{% if n
-00000180: 6f74 2072 6174 655f 6964 2025 7d0a 0909  ot rate_id %}...
-00000190: 3c70 3e0a 0909 0955 7365 2074 6869 7320  <p>....Use this 
-000001a0: 666f 726d 2074 6f20 7365 7420 7261 7465  form to set rate
-000001b0: 7320 666f 7220 746f 6f6c 732c 2061 7265  s for tools, are
-000001c0: 6173 2c20 7375 7070 6c69 6573 2061 6e64  as, supplies and
-000001d0: 2073 7461 6666 2063 6861 7267 6573 2e0a   staff charges..
-000001e0: 0909 3c2f 703e 0a09 7b25 2065 6e64 6966  ..</p>..{% endif
-000001f0: 2025 7d0a 093c 703e 5468 6520 7261 7465   %}..<p>The rate
-00000200: 7320 666f 7220 746f 6f6c 2075 7361 6765  s for tool usage
-00000210: 2026 2074 7261 696e 696e 672c 2061 7265   & training, are
-00000220: 6120 6163 6365 7373 2061 6e64 2073 7461  a access and sta
-00000230: 6666 2063 6861 7267 6573 2061 7265 2074  ff charges are t
-00000240: 6f20 6265 2065 7870 7265 7373 6564 203c  o be expressed <
-00000250: 7374 726f 6e67 3e70 6572 2068 6f75 723c  strong>per hour<
-00000260: 2f73 7472 6f6e 673e 2e3c 2f70 3e0a 093c  /strong>.</p>..<
-00000270: 666f 726d 2069 643d 2272 6174 655f 666f  form id="rate_fo
-00000280: 726d 2220 6d65 7468 6f64 3d22 706f 7374  rm" method="post
-00000290: 2220 636c 6173 733d 2266 6f72 6d2d 686f  " class="form-ho
-000002a0: 7269 7a6f 6e74 616c 2220 6163 7469 6f6e  rizontal" action
-000002b0: 3d22 7b25 2069 6620 7261 7465 5f69 6420  ="{% if rate_id 
-000002c0: 257d 7b25 2075 726c 2027 6564 6974 5f72  %}{% url 'edit_r
-000002d0: 6174 6527 2072 6174 655f 7479 7065 5f63  ate' rate_type_c
-000002e0: 686f 6963 6520 7261 7465 5f69 6420 257d  hoice rate_id %}
-000002f0: 7b25 2065 6c73 6520 257d 7b25 2075 726c  {% else %}{% url
-00000300: 2027 6372 6561 7465 5f72 6174 6527 2072   'create_rate' r
-00000310: 6174 655f 7479 7065 5f63 686f 6963 6520  ate_type_choice 
-00000320: 257d 7b25 2065 6e64 6966 2025 7d22 2073  %}{% endif %}" s
-00000330: 7479 6c65 3d22 6d61 7267 696e 2d74 6f70  tyle="margin-top
-00000340: 3a20 3235 7078 223e 0a09 097b 2520 6373  : 25px">...{% cs
-00000350: 7266 5f74 6f6b 656e 2025 7d0a 0909 3c64  rf_token %}...<d
-00000360: 6976 2063 6c61 7373 3d22 666f 726d 2d67  iv class="form-g
-00000370: 726f 7570 223e 0a09 0909 3c6c 6162 656c  roup">....<label
-00000380: 2063 6c61 7373 3d22 636f 6e74 726f 6c2d   class="control-
-00000390: 6c61 6265 6c20 636f 6c2d 736d 2d32 2220  label col-sm-2" 
-000003a0: 666f 723d 2272 6174 655f 7479 7065 223e  for="rate_type">
-000003b0: 3c73 7472 6f6e 673e 5261 7465 2074 7970  <strong>Rate typ
-000003c0: 653c 2f73 7472 6f6e 673e 3c2f 6c61 6265  e</strong></labe
-000003d0: 6c3e 0a09 0909 3c64 6976 2063 6c61 7373  l>....<div class
-000003e0: 3d22 636f 6c2d 736d 2d34 223e 0a09 0909  ="col-sm-4">....
-000003f0: 093c 7365 6c65 6374 2069 643d 2272 6174  .<select id="rat
-00000400: 655f 7479 7065 2220 6e61 6d65 3d22 7261  e_type" name="ra
-00000410: 7465 5f74 7970 6522 2063 6c61 7373 3d22  te_type" class="
-00000420: 666f 726d 2d63 6f6e 7472 6f6c 2220 6f6e  form-control" on
-00000430: 6368 616e 6765 3d22 7769 6e64 6f77 2e6c  change="window.l
-00000440: 6f63 6174 696f 6e20 3d20 277b 2520 7572  ocation = '{% ur
-00000450: 6c20 2763 7265 6174 655f 7261 7465 2720  l 'create_rate' 
-00000460: 2774 6f6f 6c27 2025 7d27 2e72 6570 6c61  'tool' %}'.repla
-00000470: 6365 2827 746f 6f6c 272c 2074 6869 732e  ce('tool', this.
-00000480: 7661 6c75 6529 223e 0a09 0909 0909 3c6f  value)">......<o
-00000490: 7074 696f 6e20 7661 6c75 653d 2222 3e53  ption value="">S
-000004a0: 656c 6563 7420 7261 7465 2074 7970 653c  elect rate type<
-000004b0: 2f6f 7074 696f 6e3e 0a09 0909 0909 7b25  /option>......{%
-000004c0: 2066 6f72 2076 616c 7565 2c20 6469 7370   for value, disp
-000004d0: 6c61 7920 696e 2072 6174 655f 7479 7065  lay in rate_type
-000004e0: 5f63 686f 6963 6573 2025 7d0a 0909 0909  _choices %}.....
-000004f0: 0909 7b25 2069 6620 7261 7465 5f69 6420  ..{% if rate_id 
-00000500: 257d 0a09 0909 0909 0909 7b25 2069 6620  %}........{% if 
-00000510: 7661 6c75 6520 3d3d 2072 6174 655f 7479  value == rate_ty
-00000520: 7065 5f63 686f 6963 6520 257d 0a09 0909  pe_choice %}....
-00000530: 0909 0909 093c 6f70 7469 6f6e 2076 616c  .....<option val
-00000540: 7565 3d22 7b7b 2076 616c 7565 207d 7d22  ue="{{ value }}"
-00000550: 2073 656c 6563 7465 643e 7b7b 2064 6973   selected>{{ dis
-00000560: 706c 6179 207d 7d3c 2f6f 7074 696f 6e3e  play }}</option>
-00000570: 0a09 0909 0909 0909 7b25 2065 6e64 6966  ........{% endif
-00000580: 2025 7d0a 0909 0909 0909 7b25 2065 6c73   %}.......{% els
-00000590: 6520 257d 0a09 0909 0909 0909 3c6f 7074  e %}........<opt
-000005a0: 696f 6e20 7661 6c75 653d 227b 7b20 7661  ion value="{{ va
-000005b0: 6c75 6520 7d7d 2220 7b25 2069 6620 7661  lue }}" {% if va
-000005c0: 6c75 6520 3d3d 2072 6174 655f 7479 7065  lue == rate_type
-000005d0: 5f63 686f 6963 6520 257d 7365 6c65 6374  _choice %}select
-000005e0: 6564 7b25 2065 6e64 6966 2025 7d3e 7b7b  ed{% endif %}>{{
-000005f0: 2064 6973 706c 6179 207d 7d3c 2f6f 7074   display }}</opt
-00000600: 696f 6e3e 0a09 0909 0909 097b 2520 656e  ion>.......{% en
-00000610: 6469 6620 257d 0a09 0909 0909 7b25 2065  dif %}......{% e
-00000620: 6e64 666f 7220 257d 0a09 0909 093c 2f73  ndfor %}.....</s
-00000630: 656c 6563 743e 0a09 0909 3c2f 6469 763e  elect>....</div>
-00000640: 0a09 0909 7b25 2069 6620 666f 726d 2e74  ....{% if form.t
-00000650: 7970 652e 6572 726f 7273 2025 7d0a 0909  ype.errors %}...
-00000660: 0909 3c64 6976 2063 6c61 7373 3d22 636f  ..<div class="co
-00000670: 6c2d 736d 2d36 2066 6f72 6d2d 636f 6e74  l-sm-6 form-cont
-00000680: 726f 6c2d 7374 6174 6963 2064 616e 6765  rol-static dange
-00000690: 722d 6869 6768 6c69 6768 7422 3e0a 0909  r-highlight">...
-000006a0: 0909 097b 7b20 666f 726d 2e74 7970 652e  ...{{ form.type.
-000006b0: 6572 726f 7273 7c73 7472 6970 7461 6773  errors|striptags
-000006c0: 207d 7d0a 0909 0909 3c2f 6469 763e 0a09   }}.....</div>..
-000006d0: 0909 7b25 2065 6e64 6966 2025 7d0a 0909  ..{% endif %}...
-000006e0: 3c2f 6469 763e 0a09 097b 2520 6966 2074  </div>...{% if t
-000006f0: 6f6f 6c73 2025 7d0a 0909 093c 6469 7620  ools %}....<div 
-00000700: 636c 6173 733d 2266 6f72 6d2d 6772 6f75  class="form-grou
-00000710: 7022 3e0a 0909 0909 3c6c 6162 656c 2063  p">.....<label c
-00000720: 6c61 7373 3d22 636f 6e74 726f 6c2d 6c61  lass="control-la
-00000730: 6265 6c20 636f 6c2d 736d 2d32 2220 666f  bel col-sm-2" fo
-00000740: 723d 2274 6f6f 6c22 3e3c 7374 726f 6e67  r="tool"><strong
-00000750: 3e54 6f6f 6c3c 2f73 7472 6f6e 673e 3c2f  >Tool</strong></
-00000760: 6c61 6265 6c3e 0a09 0909 093c 6469 7620  label>.....<div 
-00000770: 636c 6173 733d 2263 6f6c 2d73 6d2d 3422  class="col-sm-4"
-00000780: 3e0a 0909 0909 093c 7365 6c65 6374 2069  >......<select i
-00000790: 643d 2274 6f6f 6c22 206e 616d 653d 2274  d="tool" name="t
-000007a0: 6f6f 6c22 2063 6c61 7373 3d22 666f 726d  ool" class="form
-000007b0: 2d63 6f6e 7472 6f6c 2220 7265 7175 6972  -control" requir
-000007c0: 6564 3e0a 0909 0909 0909 3c6f 7074 696f  ed>.......<optio
-000007d0: 6e20 6469 7361 626c 6564 2073 656c 6563  n disabled selec
-000007e0: 7465 643e 266e 6273 703b 3c2f 6f70 7469  ted>&nbsp;</opti
-000007f0: 6f6e 3e0a 0909 0909 0909 7b25 2072 6567  on>.......{% reg
-00000800: 726f 7570 2074 6f6f 6c73 2062 7920 6361  roup tools by ca
-00000810: 7465 676f 7279 2061 7320 746f 6f6c 5f63  tegory as tool_c
-00000820: 6174 6567 6f72 6965 7320 257d 0a09 0909  ategories %}....
-00000830: 0909 097b 2520 666f 7220 6361 7465 676f  ...{% for catego
-00000840: 7279 2069 6e20 746f 6f6c 5f63 6174 6567  ry in tool_categ
-00000850: 6f72 6965 7320 257d 0a09 0909 0909 0909  ories %}........
-00000860: 7b25 2069 6620 746f 6f6c 5f63 6174 6567  {% if tool_categ
-00000870: 6f72 6965 737c 6c65 6e67 7468 203e 2031  ories|length > 1
-00000880: 206f 7220 6361 7465 676f 7279 2e67 726f   or category.gro
-00000890: 7570 6572 2025 7d0a 0909 0909 0909 093c  uper %}........<
-000008a0: 6f70 7467 726f 7570 206c 6162 656c 3d22  optgroup label="
-000008b0: 7b7b 2063 6174 6567 6f72 792e 6772 6f75  {{ category.grou
-000008c0: 7065 727c 6465 6661 756c 745f 6966 5f6e  per|default_if_n
-000008d0: 6f6e 653a 2755 6e63 6174 6567 6f72 697a  one:'Uncategoriz
-000008e0: 6564 2720 7d7d 223e 0a09 0909 0909 0909  ed' }}">........
-000008f0: 7b25 2065 6e64 6966 2025 7d0a 0909 0909  {% endif %}.....
-00000900: 0909 097b 2520 666f 7220 6974 656d 2069  ...{% for item i
-00000910: 6e20 6361 7465 676f 7279 2e6c 6973 7420  n category.list 
-00000920: 257d 0a09 0909 0909 0909 093c 6f70 7469  %}.........<opti
-00000930: 6f6e 2076 616c 7565 3d22 7b7b 2069 7465  on value="{{ ite
-00000940: 6d2e 6964 207d 7d22 207b 2520 6966 2066  m.id }}" {% if f
-00000950: 6f72 6d2e 746f 6f6c 2e76 616c 7565 7c74  orm.tool.value|t
-00000960: 6f5f 696e 7420 3d3d 2069 7465 6d2e 6964  o_int == item.id
-00000970: 2025 7d73 656c 6563 7465 647b 2520 656e   %}selected{% en
-00000980: 6469 6620 257d 3e7b 7b20 6974 656d 2e6e  dif %}>{{ item.n
-00000990: 616d 6520 7d7d 3c2f 6f70 7469 6f6e 3e0a  ame }}</option>.
-000009a0: 0909 0909 0909 097b 2520 656e 6466 6f72  .......{% endfor
-000009b0: 2025 7d0a 0909 0909 0909 097b 2520 6966   %}........{% if
-000009c0: 2074 6f6f 6c5f 6361 7465 676f 7269 6573   tool_categories
-000009d0: 7c6c 656e 6774 6820 3e20 3120 6f72 2063  |length > 1 or c
-000009e0: 6174 6567 6f72 792e 6772 6f75 7065 7220  ategory.grouper 
-000009f0: 257d 0a09 0909 0909 0909 3c2f 6f70 7467  %}........</optg
-00000a00: 726f 7570 3e0a 0909 0909 0909 097b 2520  roup>........{% 
-00000a10: 656e 6469 6620 257d 0a09 0909 0909 097b  endif %}.......{
-00000a20: 2520 656e 6466 6f72 2025 7d0a 0909 0909  % endfor %}.....
-00000a30: 093c 2f73 656c 6563 743e 0a09 0909 093c  .</select>.....<
-00000a40: 2f64 6976 3e0a 0909 093c 2f64 6976 3e0a  /div>....</div>.
-00000a50: 0909 7b25 2065 6c69 6620 6172 6561 7320  ..{% elif areas 
-00000a60: 257d 0a09 0909 3c64 6976 2063 6c61 7373  %}....<div class
-00000a70: 3d22 666f 726d 2d67 726f 7570 223e 0a09  ="form-group">..
-00000a80: 0909 093c 6c61 6265 6c20 636c 6173 733d  ...<label class=
-00000a90: 2263 6f6e 7472 6f6c 2d6c 6162 656c 2063  "control-label c
-00000aa0: 6f6c 2d73 6d2d 3222 2066 6f72 3d22 6172  ol-sm-2" for="ar
-00000ab0: 6561 223e 3c73 7472 6f6e 673e 4172 6561  ea"><strong>Area
-00000ac0: 3c2f 7374 726f 6e67 3e3c 2f6c 6162 656c  </strong></label
-00000ad0: 3e0a 0909 0909 3c64 6976 2063 6c61 7373  >.....<div class
-00000ae0: 3d22 636f 6c2d 736d 2d34 223e 0a09 0909  ="col-sm-4">....
-00000af0: 0909 3c73 656c 6563 7420 6964 3d22 6172  ..<select id="ar
-00000b00: 6561 2220 6e61 6d65 3d22 6172 6561 2220  ea" name="area" 
-00000b10: 636c 6173 733d 2266 6f72 6d2d 636f 6e74  class="form-cont
-00000b20: 726f 6c22 2072 6571 7569 7265 643e 0a09  rol" required>..
-00000b30: 0909 0909 097b 2520 6966 2061 7265 6173  .....{% if areas
-00000b40: 7c6c 656e 6774 6820 3d3d 2031 2025 7d0a  |length == 1 %}.
-00000b50: 0909 0909 0909 093c 6f70 7469 6f6e 2076  .......<option v
-00000b60: 616c 7565 3d22 7b7b 2061 7265 6173 2e30  alue="{{ areas.0
-00000b70: 2e69 6420 7d7d 223e 7b7b 2061 7265 6173  .id }}">{{ areas
-00000b80: 2e30 207d 7d3c 2f6f 7074 696f 6e3e 0a09  .0 }}</option>..
-00000b90: 0909 0909 097b 2520 656c 6966 2061 7265  .....{% elif are
-00000ba0: 6173 2025 7d0a 0909 0909 0909 093c 6f70  as %}........<op
-00000bb0: 7469 6f6e 2064 6973 6162 6c65 6420 7365  tion disabled se
-00000bc0: 6c65 6374 6564 2076 616c 7565 3d22 223e  lected value="">
-00000bd0: 4368 6f6f 7365 2061 6e20 6172 6561 3c2f  Choose an area</
-00000be0: 6f70 7469 6f6e 3e0a 0909 0909 0909 097b  option>........{
-00000bf0: 2520 666f 7220 6172 6561 2069 6e20 6172  % for area in ar
-00000c00: 6561 7320 257d 0a09 0909 0909 0909 093c  eas %}.........<
-00000c10: 6f70 7469 6f6e 2076 616c 7565 3d22 7b7b  option value="{{
-00000c20: 2061 7265 612e 6964 207d 7d22 207b 2520   area.id }}" {% 
-00000c30: 6966 2066 6f72 6d2e 6172 6561 2e76 616c  if form.area.val
-00000c40: 7565 7c74 6f5f 696e 7420 3d3d 2061 7265  ue|to_int == are
-00000c50: 612e 6964 2025 7d73 656c 6563 7465 647b  a.id %}selected{
-00000c60: 2520 656e 6469 6620 257d 3e7b 7b20 6172  % endif %}>{{ ar
-00000c70: 6561 2e6e 616d 6520 7d7d 3c2f 6f70 7469  ea.name }}</opti
-00000c80: 6f6e 3e0a 0909 0909 0909 097b 2520 656e  on>........{% en
-00000c90: 6466 6f72 2025 7d0a 0909 0909 0909 7b25  dfor %}.......{%
-00000ca0: 2065 6e64 6966 2025 7d0a 0909 0909 093c   endif %}......<
-00000cb0: 2f73 656c 6563 743e 0a09 0909 093c 2f64  /select>.....</d
-00000cc0: 6976 3e0a 0909 093c 2f64 6976 3e0a 0909  iv>....</div>...
-00000cd0: 7b25 2065 6c69 6620 636f 6e73 756d 6162  {% elif consumab
-00000ce0: 6c65 7320 257d 0a09 0909 3c64 6976 2063  les %}....<div c
-00000cf0: 6c61 7373 3d22 666f 726d 2d67 726f 7570  lass="form-group
-00000d00: 223e 0a09 0909 093c 6c61 6265 6c20 636c  ">.....<label cl
-00000d10: 6173 733d 2263 6f6e 7472 6f6c 2d6c 6162  ass="control-lab
-00000d20: 656c 2063 6f6c 2d73 6d2d 3222 2066 6f72  el col-sm-2" for
-00000d30: 3d22 636f 6e73 756d 6162 6c65 223e 3c73  ="consumable"><s
-00000d40: 7472 6f6e 673e 5375 7070 6c79 3c2f 7374  trong>Supply</st
-00000d50: 726f 6e67 3e3c 2f6c 6162 656c 3e0a 0909  rong></label>...
-00000d60: 0909 3c64 6976 2063 6c61 7373 3d22 636f  ..<div class="co
-00000d70: 6c2d 736d 2d34 223e 0a09 0909 0909 3c73  l-sm-4">......<s
-00000d80: 656c 6563 7420 6964 3d22 636f 6e73 756d  elect id="consum
-00000d90: 6162 6c65 2220 6e61 6d65 3d22 636f 6e73  able" name="cons
-00000da0: 756d 6162 6c65 2220 636c 6173 733d 2266  umable" class="f
-00000db0: 6f72 6d2d 636f 6e74 726f 6c22 2072 6571  orm-control" req
-00000dc0: 7569 7265 643e 0a09 0909 0909 093c 6f70  uired>.......<op
-00000dd0: 7469 6f6e 2064 6973 6162 6c65 6420 7365  tion disabled se
-00000de0: 6c65 6374 6564 2076 616c 7565 3d22 223e  lected value="">
-00000df0: 4368 6f6f 7365 2061 2073 7570 706c 793c  Choose a supply<
-00000e00: 2f6f 7074 696f 6e3e 0a09 0909 0909 097b  /option>.......{
-00000e10: 2520 7265 6772 6f75 7020 636f 6e73 756d  % regroup consum
-00000e20: 6162 6c65 7320 6279 2063 6174 6567 6f72  ables by categor
-00000e30: 7920 6173 2063 6f6e 7375 6d61 626c 655f  y as consumable_
-00000e40: 6361 7465 676f 7269 6573 2025 7d0a 0909  categories %}...
-00000e50: 0909 0909 7b25 2066 6f72 2063 6174 6567  ....{% for categ
-00000e60: 6f72 7920 696e 2063 6f6e 7375 6d61 626c  ory in consumabl
-00000e70: 655f 6361 7465 676f 7269 6573 2025 7d0a  e_categories %}.
-00000e80: 0909 0909 0909 097b 2520 6966 2063 6f6e  .......{% if con
-00000e90: 7375 6d61 626c 655f 6361 7465 676f 7269  sumable_categori
-00000ea0: 6573 7c6c 656e 6774 6820 3e20 3120 6f72  es|length > 1 or
-00000eb0: 2063 6174 6567 6f72 792e 6772 6f75 7065   category.groupe
-00000ec0: 7220 257d 0a09 0909 0909 0909 3c6f 7074  r %}........<opt
-00000ed0: 6772 6f75 7020 6c61 6265 6c3d 227b 7b20  group label="{{ 
-00000ee0: 6361 7465 676f 7279 2e67 726f 7570 6572  category.grouper
-00000ef0: 7c64 6566 6175 6c74 5f69 665f 6e6f 6e65  |default_if_none
-00000f00: 3a22 556e 6361 7465 676f 7269 7a65 6422  :"Uncategorized"
-00000f10: 207d 7d22 3e0a 0909 0909 0909 097b 2520   }}">........{% 
-00000f20: 656e 6469 6620 257d 0a09 0909 0909 0909  endif %}........
-00000f30: 7b25 2066 6f72 2069 7465 6d20 696e 2063  {% for item in c
-00000f40: 6174 6567 6f72 792e 6c69 7374 2025 7d0a  ategory.list %}.
-00000f50: 0909 0909 0909 0909 3c6f 7074 696f 6e20  ........<option 
-00000f60: 7661 6c75 653d 227b 7b20 6974 656d 2e69  value="{{ item.i
-00000f70: 6420 7d7d 2220 7b25 2069 6620 666f 726d  d }}" {% if form
-00000f80: 2e63 6f6e 7375 6d61 626c 652e 7661 6c75  .consumable.valu
-00000f90: 657c 746f 5f69 6e74 203d 3d20 6974 656d  e|to_int == item
-00000fa0: 2e69 6420 257d 7365 6c65 6374 6564 7b25  .id %}selected{%
-00000fb0: 2065 6e64 6966 2025 7d3e 7b7b 2069 7465   endif %}>{{ ite
-00000fc0: 6d2e 6e61 6d65 207d 7d3c 2f6f 7074 696f  m.name }}</optio
-00000fd0: 6e3e 0a09 0909 0909 0909 7b25 2065 6e64  n>........{% end
-00000fe0: 666f 7220 257d 0a09 0909 0909 0909 7b25  for %}........{%
-00000ff0: 2069 6620 636f 6e73 756d 6162 6c65 5f63   if consumable_c
-00001000: 6174 6567 6f72 6965 737c 6c65 6e67 7468  ategories|length
-00001010: 203e 2031 206f 7220 6361 7465 676f 7279   > 1 or category
-00001020: 2e67 726f 7570 6572 2025 7d0a 0909 0909  .grouper %}.....
-00001030: 0909 093c 2f6f 7074 6772 6f75 703e 0a09  ...</optgroup>..
-00001040: 0909 0909 0909 7b25 2065 6e64 6966 2025  ......{% endif %
-00001050: 7d0a 0909 0909 0909 7b25 2065 6e64 666f  }.......{% endfo
-00001060: 7220 257d 0a09 0909 0909 3c2f 7365 6c65  r %}......</sele
-00001070: 6374 3e0a 0909 0909 3c2f 6469 763e 0a09  ct>.....</div>..
-00001080: 0909 3c2f 6469 763e 0a09 097b 2520 656e  ..</div>...{% en
-00001090: 6469 6620 257d 0a09 097b 2520 666f 7220  dif %}...{% for 
-000010a0: 7261 7465 5f74 7970 6520 696e 2072 6174  rate_type in rat
-000010b0: 655f 7479 7065 7320 257d 0a09 0909 7b25  e_types %}....{%
-000010c0: 2069 6e63 6c75 6465 2022 7261 7465 732f   include "rates/
-000010d0: 7261 7465 5f66 6f72 6d5f 6465 7461 696c  rate_form_detail
-000010e0: 732e 6874 6d6c 2220 7769 7468 2072 6174  s.html" with rat
-000010f0: 655f 7479 7065 3d72 6174 655f 7479 7065  e_type=rate_type
-00001100: 2025 7d0a 0909 7b25 2065 6e64 666f 7220   %}...{% endfor 
-00001110: 257d 0a09 097b 2520 6966 2072 6174 655f  %}...{% if rate_
-00001120: 7479 7065 5f63 686f 6963 6520 257d 0a09  type_choice %}..
-00001130: 0909 3c64 6976 2063 6c61 7373 3d22 636f  ..<div class="co
-00001140: 6c2d 736d 2d36 2074 6578 742d 7269 6768  l-sm-6 text-righ
-00001150: 7422 3e0a 0909 0909 3c62 7574 746f 6e20  t">.....<button 
-00001160: 7479 7065 3d22 7375 626d 6974 2220 636c  type="submit" cl
-00001170: 6173 733d 2262 746e 2062 746e 2d73 7563  ass="btn btn-suc
-00001180: 6365 7373 223e 436f 6e66 6972 6d3c 2f62  cess">Confirm</b
-00001190: 7574 746f 6e3e 0a09 0909 3c2f 6469 763e  utton>....</div>
-000011a0: 0a09 097b 2520 656e 6469 6620 257d 0a09  ...{% endif %}..
-000011b0: 3c2f 666f 726d 3e0a 7b25 2065 6e64 626c  </form>.{% endbl
-000011c0: 6f63 6b20 257d                           ock %}
+00000080: 7b25 2069 6620 6974 656d 2025 7d7b 7b20  {% if item %}{{ 
+00000090: 6974 656d 207d 7d7b 2520 656c 6966 2066  item }}{% elif f
+000000a0: 6f72 6d73 2025 7d7b 7b20 666f 726d 732e  orms %}{{ forms.
+000000b0: 302e 696e 7374 616e 6365 2e74 7970 6520  0.instance.type 
+000000c0: 7d7d 7b25 2065 6c73 6520 257d 4372 6561  }}{% else %}Crea
+000000d0: 7465 7b25 2065 6e64 6966 2025 7d20 7261  te{% endif %} ra
+000000e0: 7465 3c2f 6831 3e0a 093c 703e 3c62 723e  te</h1>..<p><br>
+000000f0: 3c73 7061 6e20 636c 6173 733d 2270 7269  <span class="pri
+00000100: 6d61 7279 2d68 6967 686c 6967 6874 2067  mary-highlight g
+00000110: 6c79 7068 6963 6f6e 2067 6c79 7068 6963  lyphicon glyphic
+00000120: 6f6e 2d69 6e66 6f2d 7369 676e 223e 3c2f  on-info-sign"></
+00000130: 7370 616e 3e20 5468 6520 7261 7465 7320  span> The rates 
+00000140: 666f 7220 746f 6f6c 2075 7361 6765 2026  for tool usage &
+00000150: 2074 7261 696e 696e 672c 2061 7265 6120   training, area 
+00000160: 6163 6365 7373 2061 6e64 2073 7461 6666  access and staff
+00000170: 2063 6861 7267 6573 2061 7265 2074 6f20   charges are to 
+00000180: 6265 2065 7870 7265 7373 6564 203c 7374  be expressed <st
+00000190: 726f 6e67 3e70 6572 2068 6f75 723c 2f73  rong>per hour</s
+000001a0: 7472 6f6e 673e 2e3c 2f70 3e0a 093c 666f  trong>.</p>..<fo
+000001b0: 726d 2069 643d 2272 6174 655f 666f 726d  rm id="rate_form
+000001c0: 2220 6d65 7468 6f64 3d22 706f 7374 2220  " method="post" 
+000001d0: 636c 6173 733d 2266 6f72 6d2d 686f 7269  class="form-hori
+000001e0: 7a6f 6e74 616c 2220 6163 7469 6f6e 3d22  zontal" action="
+000001f0: 7b25 2069 6620 6974 656d 2025 7d7b 2520  {% if item %}{% 
+00000200: 7572 6c20 2763 7265 6174 655f 7261 7465  url 'create_rate
+00000210: 2720 7261 7465 5f74 7970 655f 6368 6f69  ' rate_type_choi
+00000220: 6365 2069 7465 6d2e 6964 2025 7d7b 2520  ce item.id %}{% 
+00000230: 656c 7365 2025 7d7b 2520 7572 6c20 2763  else %}{% url 'c
+00000240: 7265 6174 655f 7261 7465 2720 7261 7465  reate_rate' rate
+00000250: 5f74 7970 655f 6368 6f69 6365 2025 7d7b  _type_choice %}{
+00000260: 2520 656e 6469 6620 257d 2220 7374 796c  % endif %}" styl
+00000270: 653d 226d 6172 6769 6e2d 746f 703a 2032  e="margin-top: 2
+00000280: 3570 7822 3e0a 0909 7b25 2063 7372 665f  5px">...{% csrf_
+00000290: 746f 6b65 6e20 257d 0a09 097b 2520 6966  token %}...{% if
+000002a0: 206e 6f74 2066 6f72 6d73 2025 7d0a 0909   not forms %}...
+000002b0: 093c 6469 7620 636c 6173 733d 2266 6f72  .<div class="for
+000002c0: 6d2d 6772 6f75 7022 3e0a 0909 0909 3c6c  m-group">.....<l
+000002d0: 6162 656c 2063 6c61 7373 3d22 636f 6e74  abel class="cont
+000002e0: 726f 6c2d 6c61 6265 6c20 636f 6c2d 736d  rol-label col-sm
+000002f0: 2d32 2220 666f 723d 2272 6174 655f 7479  -2" for="rate_ty
+00000300: 7065 223e 3c73 7472 6f6e 673e 5261 7465  pe"><strong>Rate
+00000310: 2074 7970 653c 2f73 7472 6f6e 673e 3c2f   type</strong></
+00000320: 6c61 6265 6c3e 0a09 0909 093c 6469 7620  label>.....<div 
+00000330: 636c 6173 733d 2263 6f6c 2d73 6d2d 3422  class="col-sm-4"
+00000340: 3e0a 0909 0909 093c 7365 6c65 6374 2069  >......<select i
+00000350: 643d 2272 6174 655f 7479 7065 2220 6e61  d="rate_type" na
+00000360: 6d65 3d22 7261 7465 5f74 7970 6522 2063  me="rate_type" c
+00000370: 6c61 7373 3d22 666f 726d 2d63 6f6e 7472  lass="form-contr
+00000380: 6f6c 2220 6f6e 6368 616e 6765 3d22 7261  ol" onchange="ra
+00000390: 7465 5f74 7970 655f 7365 6c65 6374 696f  te_type_selectio
+000003a0: 6e28 7468 6973 2e76 616c 7565 2922 3e0a  n(this.value)">.
+000003b0: 0909 0909 0909 3c6f 7074 696f 6e20 7661  ......<option va
+000003c0: 6c75 653d 2222 3e53 656c 6563 7420 7261  lue="">Select ra
+000003d0: 7465 2074 7970 653c 2f6f 7074 696f 6e3e  te type</option>
+000003e0: 0a09 0909 0909 097b 2520 666f 7220 7661  .......{% for va
+000003f0: 6c75 652c 2064 6973 706c 6179 2069 6e20  lue, display in 
+00000400: 7261 7465 5f74 7970 655f 6368 6f69 6365  rate_type_choice
+00000410: 7320 257d 0a09 0909 0909 0909 3c6f 7074  s %}........<opt
+00000420: 696f 6e20 7661 6c75 653d 227b 7b20 7661  ion value="{{ va
+00000430: 6c75 6520 7d7d 2220 7b25 2069 6620 7661  lue }}" {% if va
+00000440: 6c75 6520 3d3d 2072 6174 655f 7479 7065  lue == rate_type
+00000450: 5f63 686f 6963 6520 257d 7365 6c65 6374  _choice %}select
+00000460: 6564 7b25 2065 6e64 6966 2025 7d3e 7b7b  ed{% endif %}>{{
+00000470: 2064 6973 706c 6179 207d 7d3c 2f6f 7074   display }}</opt
+00000480: 696f 6e3e 0a09 0909 0909 097b 2520 656e  ion>.......{% en
+00000490: 6466 6f72 2025 7d0a 0909 0909 093c 2f73  dfor %}......</s
+000004a0: 656c 6563 743e 0a09 0909 093c 2f64 6976  elect>.....</div
+000004b0: 3e0a 0909 093c 2f64 6976 3e0a 0909 093c  >....</div>....<
+000004c0: 6469 7620 6964 3d22 746f 6f6c 5f73 656c  div id="tool_sel
+000004d0: 6563 7422 2063 6c61 7373 3d22 666f 726d  ect" class="form
+000004e0: 2d67 726f 7570 2069 7465 6d5f 7365 6c65  -group item_sele
+000004f0: 6374 2220 7374 796c 653d 2264 6973 706c  ct" style="displ
+00000500: 6179 3a20 6e6f 6e65 223e 0a09 0909 093c  ay: none">.....<
+00000510: 6c61 6265 6c20 636c 6173 733d 2263 6f6e  label class="con
+00000520: 7472 6f6c 2d6c 6162 656c 2063 6f6c 2d73  trol-label col-s
+00000530: 6d2d 3222 2066 6f72 3d22 746f 6f6c 223e  m-2" for="tool">
+00000540: 3c73 7472 6f6e 673e 546f 6f6c 3c2f 7374  <strong>Tool</st
+00000550: 726f 6e67 3e3c 2f6c 6162 656c 3e0a 0909  rong></label>...
+00000560: 0909 3c64 6976 2063 6c61 7373 3d22 636f  ..<div class="co
+00000570: 6c2d 736d 2d34 223e 0a09 0909 0909 3c73  l-sm-4">......<s
+00000580: 656c 6563 7420 6964 3d22 746f 6f6c 2220  elect id="tool" 
+00000590: 6e61 6d65 3d22 746f 6f6c 2220 636c 6173  name="tool" clas
+000005a0: 733d 2266 6f72 6d2d 636f 6e74 726f 6c22  s="form-control"
+000005b0: 206f 6e63 6861 6e67 653d 2272 6174 655f   onchange="rate_
+000005c0: 7479 7065 5f73 656c 6563 7469 6f6e 2827  type_selection('
+000005d0: 546f 6f6c 272c 2074 6869 732e 7661 6c75  Tool', this.valu
+000005e0: 6529 223e 0a09 0909 0909 093c 6f70 7469  e)">.......<opti
+000005f0: 6f6e 2064 6973 6162 6c65 6420 7365 6c65  on disabled sele
+00000600: 6374 6564 3e43 686f 6f73 6520 6120 746f  cted>Choose a to
+00000610: 6f6c 3c2f 6f70 7469 6f6e 3e0a 0909 0909  ol</option>.....
+00000620: 0909 7b25 2072 6567 726f 7570 2074 6f6f  ..{% regroup too
+00000630: 6c73 2062 7920 6361 7465 676f 7279 2061  ls by category a
+00000640: 7320 746f 6f6c 5f63 6174 6567 6f72 6965  s tool_categorie
+00000650: 7320 257d 0a09 0909 0909 097b 2520 666f  s %}.......{% fo
+00000660: 7220 6361 7465 676f 7279 2069 6e20 746f  r category in to
+00000670: 6f6c 5f63 6174 6567 6f72 6965 7320 257d  ol_categories %}
+00000680: 0a09 0909 0909 0909 7b25 2069 6620 746f  ........{% if to
+00000690: 6f6c 5f63 6174 6567 6f72 6965 737c 6c65  ol_categories|le
+000006a0: 6e67 7468 203e 2031 206f 7220 6361 7465  ngth > 1 or cate
+000006b0: 676f 7279 2e67 726f 7570 6572 2025 7d0a  gory.grouper %}.
+000006c0: 0909 0909 0909 093c 6f70 7467 726f 7570  .......<optgroup
+000006d0: 206c 6162 656c 3d22 7b7b 2063 6174 6567   label="{{ categ
+000006e0: 6f72 792e 6772 6f75 7065 727c 6465 6661  ory.grouper|defa
+000006f0: 756c 745f 6966 5f6e 6f6e 653a 2755 6e63  ult_if_none:'Unc
+00000700: 6174 6567 6f72 697a 6564 2720 7d7d 223e  ategorized' }}">
+00000710: 0a09 0909 0909 0909 7b25 2065 6e64 6966  ........{% endif
+00000720: 2025 7d0a 0909 0909 0909 097b 2520 666f   %}........{% fo
+00000730: 7220 6974 656d 2069 6e20 6361 7465 676f  r item in catego
+00000740: 7279 2e6c 6973 7420 257d 0a09 0909 0909  ry.list %}......
+00000750: 0909 093c 6f70 7469 6f6e 2076 616c 7565  ...<option value
+00000760: 3d22 7b7b 2069 7465 6d2e 6964 207d 7d22  ="{{ item.id }}"
+00000770: 3e7b 7b20 6974 656d 2e6e 616d 6520 7d7d  >{{ item.name }}
+00000780: 3c2f 6f70 7469 6f6e 3e0a 0909 0909 0909  </option>.......
+00000790: 097b 2520 656e 6466 6f72 2025 7d0a 0909  .{% endfor %}...
+000007a0: 0909 0909 097b 2520 6966 2074 6f6f 6c5f  .....{% if tool_
+000007b0: 6361 7465 676f 7269 6573 7c6c 656e 6774  categories|lengt
+000007c0: 6820 3e20 3120 6f72 2063 6174 6567 6f72  h > 1 or categor
+000007d0: 792e 6772 6f75 7065 7220 257d 0a09 0909  y.grouper %}....
+000007e0: 0909 0909 3c2f 6f70 7467 726f 7570 3e0a  ....</optgroup>.
+000007f0: 0909 0909 0909 097b 2520 656e 6469 6620  .......{% endif 
+00000800: 257d 0a09 0909 0909 097b 2520 656e 6466  %}.......{% endf
+00000810: 6f72 2025 7d0a 0909 0909 093c 2f73 656c  or %}......</sel
+00000820: 6563 743e 0a09 0909 093c 2f64 6976 3e0a  ect>.....</div>.
+00000830: 0909 093c 2f64 6976 3e0a 0909 093c 6469  ...</div>....<di
+00000840: 7620 6964 3d22 6172 6561 5f73 656c 6563  v id="area_selec
+00000850: 7422 2063 6c61 7373 3d22 666f 726d 2d67  t" class="form-g
+00000860: 726f 7570 2069 7465 6d5f 7365 6c65 6374  roup item_select
+00000870: 2220 7374 796c 653d 2264 6973 706c 6179  " style="display
+00000880: 3a20 6e6f 6e65 223e 0a09 0909 093c 6c61  : none">.....<la
+00000890: 6265 6c20 636c 6173 733d 2263 6f6e 7472  bel class="contr
+000008a0: 6f6c 2d6c 6162 656c 2063 6f6c 2d73 6d2d  ol-label col-sm-
+000008b0: 3222 2066 6f72 3d22 6172 6561 223e 3c73  2" for="area"><s
+000008c0: 7472 6f6e 673e 4172 6561 3c2f 7374 726f  trong>Area</stro
+000008d0: 6e67 3e3c 2f6c 6162 656c 3e0a 0909 0909  ng></label>.....
+000008e0: 3c64 6976 2063 6c61 7373 3d22 636f 6c2d  <div class="col-
+000008f0: 736d 2d34 223e 0a09 0909 0909 3c73 656c  sm-4">......<sel
+00000900: 6563 7420 6964 3d22 6172 6561 2220 6e61  ect id="area" na
+00000910: 6d65 3d22 6172 6561 2220 636c 6173 733d  me="area" class=
+00000920: 2266 6f72 6d2d 636f 6e74 726f 6c22 206f  "form-control" o
+00000930: 6e63 6861 6e67 653d 2272 6174 655f 7479  nchange="rate_ty
+00000940: 7065 5f73 656c 6563 7469 6f6e 2827 4172  pe_selection('Ar
+00000950: 6561 272c 2074 6869 732e 7661 6c75 6529  ea', this.value)
+00000960: 223e 0a09 0909 0909 093c 6f70 7469 6f6e  ">.......<option
+00000970: 2064 6973 6162 6c65 6420 7365 6c65 6374   disabled select
+00000980: 6564 3e43 686f 6f73 6520 616e 2061 7265  ed>Choose an are
+00000990: 613c 2f6f 7074 696f 6e3e 0a09 0909 0909  a</option>......
+000009a0: 097b 2520 6966 2061 7265 6173 7c6c 656e  .{% if areas|len
+000009b0: 6774 6820 3d3d 2031 2025 7d0a 0909 0909  gth == 1 %}.....
+000009c0: 0909 093c 6f70 7469 6f6e 2076 616c 7565  ...<option value
+000009d0: 3d22 7b7b 2061 7265 6173 2e30 2e69 6420  ="{{ areas.0.id 
+000009e0: 7d7d 223e 7b7b 2061 7265 6173 2e30 207d  }}">{{ areas.0 }
+000009f0: 7d3c 2f6f 7074 696f 6e3e 0a09 0909 0909  }</option>......
+00000a00: 097b 2520 656c 6966 2061 7265 6173 2025  .{% elif areas %
+00000a10: 7d0a 0909 0909 0909 093c 6f70 7469 6f6e  }........<option
+00000a20: 2064 6973 6162 6c65 6420 7365 6c65 6374   disabled select
+00000a30: 6564 2076 616c 7565 3d22 223e 4368 6f6f  ed value="">Choo
+00000a40: 7365 2061 6e20 6172 6561 3c2f 6f70 7469  se an area</opti
+00000a50: 6f6e 3e0a 0909 0909 0909 097b 2520 666f  on>........{% fo
+00000a60: 7220 6172 6561 2069 6e20 6172 6561 7320  r area in areas 
+00000a70: 257d 0a09 0909 0909 0909 093c 6f70 7469  %}.........<opti
+00000a80: 6f6e 2076 616c 7565 3d22 7b7b 2061 7265  on value="{{ are
+00000a90: 612e 6964 207d 7d22 3e7b 7b20 6172 6561  a.id }}">{{ area
+00000aa0: 2e6e 616d 6520 7d7d 3c2f 6f70 7469 6f6e  .name }}</option
+00000ab0: 3e0a 0909 0909 0909 097b 2520 656e 6466  >........{% endf
+00000ac0: 6f72 2025 7d0a 0909 0909 0909 7b25 2065  or %}.......{% e
+00000ad0: 6e64 6966 2025 7d0a 0909 0909 093c 2f73  ndif %}......</s
+00000ae0: 656c 6563 743e 0a09 0909 093c 2f64 6976  elect>.....</div
+00000af0: 3e0a 0909 093c 2f64 6976 3e0a 0909 093c  >....</div>....<
+00000b00: 6469 7620 6964 3d22 636f 6e73 756d 6162  div id="consumab
+00000b10: 6c65 5f73 656c 6563 7422 2063 6c61 7373  le_select" class
+00000b20: 3d22 666f 726d 2d67 726f 7570 2069 7465  ="form-group ite
+00000b30: 6d5f 7365 6c65 6374 2220 7374 796c 653d  m_select" style=
+00000b40: 2264 6973 706c 6179 3a20 6e6f 6e65 223e  "display: none">
+00000b50: 0a09 0909 093c 6c61 6265 6c20 636c 6173  .....<label clas
+00000b60: 733d 2263 6f6e 7472 6f6c 2d6c 6162 656c  s="control-label
+00000b70: 2063 6f6c 2d73 6d2d 3222 2066 6f72 3d22   col-sm-2" for="
+00000b80: 636f 6e73 756d 6162 6c65 223e 3c73 7472  consumable"><str
+00000b90: 6f6e 673e 5375 7070 6c79 3c2f 7374 726f  ong>Supply</stro
+00000ba0: 6e67 3e3c 2f6c 6162 656c 3e0a 0909 0909  ng></label>.....
+00000bb0: 3c64 6976 2063 6c61 7373 3d22 636f 6c2d  <div class="col-
+00000bc0: 736d 2d34 223e 0a09 0909 0909 3c73 656c  sm-4">......<sel
+00000bd0: 6563 7420 6964 3d22 636f 6e73 756d 6162  ect id="consumab
+00000be0: 6c65 2220 6e61 6d65 3d22 636f 6e73 756d  le" name="consum
+00000bf0: 6162 6c65 2220 636c 6173 733d 2266 6f72  able" class="for
+00000c00: 6d2d 636f 6e74 726f 6c22 206f 6e63 6861  m-control" oncha
+00000c10: 6e67 653d 2272 6174 655f 7479 7065 5f73  nge="rate_type_s
+00000c20: 656c 6563 7469 6f6e 2827 434f 4e53 554d  election('CONSUM
+00000c30: 4142 4c45 272c 2074 6869 732e 7661 6c75  ABLE', this.valu
+00000c40: 6529 223e 0a09 0909 0909 093c 6f70 7469  e)">.......<opti
+00000c50: 6f6e 2064 6973 6162 6c65 6420 7365 6c65  on disabled sele
+00000c60: 6374 6564 2076 616c 7565 3d22 223e 4368  cted value="">Ch
+00000c70: 6f6f 7365 2061 2073 7570 706c 793c 2f6f  oose a supply</o
+00000c80: 7074 696f 6e3e 0a09 0909 0909 097b 2520  ption>.......{% 
+00000c90: 7265 6772 6f75 7020 636f 6e73 756d 6162  regroup consumab
+00000ca0: 6c65 7320 6279 2063 6174 6567 6f72 7920  les by category 
+00000cb0: 6173 2063 6f6e 7375 6d61 626c 655f 6361  as consumable_ca
+00000cc0: 7465 676f 7269 6573 2025 7d0a 0909 0909  tegories %}.....
+00000cd0: 0909 7b25 2066 6f72 2063 6174 6567 6f72  ..{% for categor
+00000ce0: 7920 696e 2063 6f6e 7375 6d61 626c 655f  y in consumable_
+00000cf0: 6361 7465 676f 7269 6573 2025 7d0a 0909  categories %}...
+00000d00: 0909 0909 097b 2520 6966 2063 6f6e 7375  .....{% if consu
+00000d10: 6d61 626c 655f 6361 7465 676f 7269 6573  mable_categories
+00000d20: 7c6c 656e 6774 6820 3e20 3120 6f72 2063  |length > 1 or c
+00000d30: 6174 6567 6f72 792e 6772 6f75 7065 7220  ategory.grouper 
+00000d40: 257d 0a09 0909 0909 0909 3c6f 7074 6772  %}........<optgr
+00000d50: 6f75 7020 6c61 6265 6c3d 227b 7b20 6361  oup label="{{ ca
+00000d60: 7465 676f 7279 2e67 726f 7570 6572 7c64  tegory.grouper|d
+00000d70: 6566 6175 6c74 5f69 665f 6e6f 6e65 3a22  efault_if_none:"
+00000d80: 556e 6361 7465 676f 7269 7a65 6422 207d  Uncategorized" }
+00000d90: 7d22 3e0a 0909 0909 0909 097b 2520 656e  }">........{% en
+00000da0: 6469 6620 257d 0a09 0909 0909 0909 7b25  dif %}........{%
+00000db0: 2066 6f72 2069 7465 6d20 696e 2063 6174   for item in cat
+00000dc0: 6567 6f72 792e 6c69 7374 2025 7d0a 0909  egory.list %}...
+00000dd0: 0909 0909 0909 3c6f 7074 696f 6e20 7661  ......<option va
+00000de0: 6c75 653d 227b 7b20 6974 656d 2e69 6420  lue="{{ item.id 
+00000df0: 7d7d 223e 7b7b 2069 7465 6d2e 6e61 6d65  }}">{{ item.name
+00000e00: 207d 7d3c 2f6f 7074 696f 6e3e 0a09 0909   }}</option>....
+00000e10: 0909 0909 7b25 2065 6e64 666f 7220 257d  ....{% endfor %}
+00000e20: 0a09 0909 0909 0909 7b25 2069 6620 636f  ........{% if co
+00000e30: 6e73 756d 6162 6c65 5f63 6174 6567 6f72  nsumable_categor
+00000e40: 6965 737c 6c65 6e67 7468 203e 2031 206f  ies|length > 1 o
+00000e50: 7220 6361 7465 676f 7279 2e67 726f 7570  r category.group
+00000e60: 6572 2025 7d0a 0909 0909 0909 093c 2f6f  er %}........</o
+00000e70: 7074 6772 6f75 703e 0a09 0909 0909 0909  ptgroup>........
+00000e80: 7b25 2065 6e64 6966 2025 7d0a 0909 0909  {% endif %}.....
+00000e90: 0909 7b25 2065 6e64 666f 7220 257d 0a09  ..{% endfor %}..
+00000ea0: 0909 0909 3c2f 7365 6c65 6374 3e0a 0909  ....</select>...
+00000eb0: 0909 3c2f 6469 763e 0a09 0909 3c2f 6469  ..</div>....</di
+00000ec0: 763e 0a09 097b 2520 656c 7365 2025 7d0a  v>...{% else %}.
+00000ed0: 0909 097b 2520 666f 7220 7261 7465 5f66  ...{% for rate_f
+00000ee0: 6f72 6d20 696e 2066 6f72 6d73 2025 7d0a  orm in forms %}.
+00000ef0: 0909 0909 7b25 2069 6e63 6c75 6465 2022  ....{% include "
+00000f00: 7261 7465 732f 7261 7465 5f66 6f72 6d5f  rates/rate_form_
+00000f10: 6465 7461 696c 732e 6874 6d6c 2220 7769  details.html" wi
+00000f20: 7468 2072 6174 655f 666f 726d 3d72 6174  th rate_form=rat
+00000f30: 655f 666f 726d 2025 7d0a 0909 097b 2520  e_form %}....{% 
+00000f40: 656e 6466 6f72 2025 7d0a 0909 093c 6469  endfor %}....<di
+00000f50: 7620 636c 6173 733d 2263 6f6c 2d73 6d2d  v class="col-sm-
+00000f60: 3620 7465 7874 2d72 6967 6874 223e 0a09  6 text-right">..
+00000f70: 0909 097b 2520 6275 7474 6f6e 2074 7970  ...{% button typ
+00000f80: 653d 2273 6176 6522 2076 616c 7565 3d22  e="save" value="
+00000f90: 436f 6e66 6972 6d22 2025 7d0a 0909 093c  Confirm" %}....<
+00000fa0: 2f64 6976 3e0a 0909 7b25 2065 6e64 6966  /div>...{% endif
+00000fb0: 2025 7d0a 093c 2f66 6f72 6d3e 0a09 3c73   %}..</form>..<s
+00000fc0: 6372 6970 743e 0a09 6675 6e63 7469 6f6e  cript>..function
+00000fd0: 2072 6174 655f 7479 7065 5f73 656c 6563   rate_type_selec
+00000fe0: 7469 6f6e 2872 6174 655f 7479 7065 2c20  tion(rate_type, 
+00000ff0: 6964 290a 2020 2020 7b0a 2020 2020 2020  id).    {.      
+00001000: 2020 6966 2028 7261 7465 5f74 7970 6529    if (rate_type)
+00001010: 0a20 2020 2020 2020 207b 0a09 0909 6966  .        {....if
+00001020: 2028 6964 290a 0909 097b 0a09 0909 0977   (id)....{.....w
+00001030: 696e 646f 772e 6c6f 6361 7469 6f6e 203d  indow.location =
+00001040: 2027 7b25 2075 726c 2027 6372 6561 7465   '{% url 'create
+00001050: 5f72 6174 6527 2027 746f 6f6c 2720 2739  _rate' 'tool' '9
+00001060: 3939 3927 2025 7d27 2e72 6570 6c61 6365  999' %}'.replace
+00001070: 2827 746f 6f6c 272c 2072 6174 655f 7479  ('tool', rate_ty
+00001080: 7065 292e 7265 706c 6163 6528 2739 3939  pe).replace('999
+00001090: 3927 2c20 6964 293b 0a09 0909 7d0a 0909  9', id);....}...
+000010a0: 0965 6c73 6520 6966 2028 7261 7465 5f74  .else if (rate_t
+000010b0: 7970 652e 746f 4c6f 7765 7243 6173 6528  ype.toLowerCase(
+000010c0: 2920 213d 3d20 2774 6f6f 6c27 2026 2620  ) !== 'tool' && 
+000010d0: 7261 7465 5f74 7970 652e 746f 4c6f 7765  rate_type.toLowe
+000010e0: 7243 6173 6528 2920 213d 3d20 2761 7265  rCase() !== 'are
+000010f0: 6127 2026 2620 7261 7465 5f74 7970 652e  a' && rate_type.
+00001100: 746f 4c6f 7765 7243 6173 6528 2920 213d  toLowerCase() !=
+00001110: 3d20 2763 6f6e 7375 6d61 626c 6527 290a  = 'consumable').
+00001120: 0909 097b 0a09 0909 0977 696e 646f 772e  ...{.....window.
+00001130: 6c6f 6361 7469 6f6e 203d 2027 7b25 2075  location = '{% u
+00001140: 726c 2027 6372 6561 7465 5f72 6174 6527  rl 'create_rate'
+00001150: 2027 746f 6f6c 2720 257d 272e 7265 706c   'tool' %}'.repl
+00001160: 6163 6528 2774 6f6f 6c27 2c20 7261 7465  ace('tool', rate
+00001170: 5f74 7970 6529 3b0a 0909 097d 0a09 0909  _type);....}....
+00001180: 656c 7365 0a09 0909 7b0a 2020 2020 2020  else....{.      
+00001190: 2020 2020 2020 2020 2020 2428 272e 6974            $('.it
+000011a0: 656d 5f73 656c 6563 7427 292e 6869 6465  em_select').hide
+000011b0: 2829 3b0a 0909 0909 2428 2723 272b 7261  ();.....$('#'+ra
+000011c0: 7465 5f74 7970 652e 746f 4c6f 7765 7243  te_type.toLowerC
+000011d0: 6173 6528 292b 225f 7365 6c65 6374 2229  ase()+"_select")
+000011e0: 2e73 686f 7728 293b 0a09 0909 7d0a 2020  .show();....}.  
+000011f0: 2020 2020 2020 7d0a 097d 0a20 2020 2066        }..}.    f
+00001200: 756e 6374 696f 6e20 6164 645f 7261 7465  unction add_rate
+00001210: 5f66 6f72 6d28 666f 726d 5f6e 756d 6265  _form(form_numbe
+00001220: 7229 0a20 2020 207b 0a20 2020 2020 2020  r).    {.       
+00001230: 207b 2320 4669 6775 7265 206f 7574 2074   {# Figure out t
+00001240: 6865 206d 6178 2066 6f72 6d20 6e75 6d62  he max form numb
+00001250: 6572 2074 6f20 7365 6e64 2069 7420 237d  er to send it #}
+00001260: 0a20 2020 2020 2020 206c 6574 2066 6f72  .        let for
+00001270: 6d5f 6e75 6d62 6572 5f69 6e70 7574 7320  m_number_inputs 
+00001280: 3d20 646f 6375 6d65 6e74 2e71 7565 7279  = document.query
+00001290: 5365 6c65 6374 6f72 416c 6c28 2769 6e70  SelectorAll('inp
+000012a0: 7574 5b6e 616d 653d 2266 6f72 6d5f 6e75  ut[name="form_nu
+000012b0: 6d62 6572 735b 5d22 5d27 293b 0a20 2020  mbers[]"]');.   
+000012c0: 2020 2020 206c 6574 206d 6178 5f66 6f72       let max_for
+000012d0: 6d5f 6e75 6d62 6572 203d 2030 3b0a 2020  m_number = 0;.  
+000012e0: 2020 2020 2020 666f 7220 286c 6574 2069        for (let i
+000012f0: 3d30 3b20 6920 3c20 666f 726d 5f6e 756d  =0; i < form_num
+00001300: 6265 725f 696e 7075 7473 2e6c 656e 6774  ber_inputs.lengt
+00001310: 683b 2069 2b2b 290a 2020 2020 2020 2020  h; i++).        
+00001320: 7b0a 2020 2020 2020 2020 2020 2020 6d61  {.            ma
+00001330: 785f 666f 726d 5f6e 756d 6265 7220 3d20  x_form_number = 
+00001340: 4d61 7468 2e6d 6178 286d 6178 5f66 6f72  Math.max(max_for
+00001350: 6d5f 6e75 6d62 6572 2c20 7061 7273 6549  m_number, parseI
+00001360: 6e74 2866 6f72 6d5f 6e75 6d62 6572 5f69  nt(form_number_i
+00001370: 6e70 7574 735b 695d 2e76 616c 7565 2929  nputs[i].value))
+00001380: 3b0a 0909 7d0a 2020 2020 2020 2020 6c65  ;...}.        le
+00001390: 7420 7261 7465 5f66 6f72 6d5f 7572 6c20  t rate_form_url 
+000013a0: 3d20 277b 2520 7572 6c20 276e 6577 5f74  = '{% url 'new_t
+000013b0: 696d 655f 7261 7465 5f66 6f72 6d27 2025  ime_rate_form' %
+000013c0: 7d3f 273b 0a20 2020 2020 2020 2072 6174  }?';.        rat
+000013d0: 655f 666f 726d 5f75 726c 202b 3d20 2726  e_form_url += '&
+000013e0: 636f 756e 743d 2720 2b20 286d 6178 5f66  count=' + (max_f
+000013f0: 6f72 6d5f 6e75 6d62 6572 202b 2031 293b  orm_number + 1);
+00001400: 0a20 2020 2020 2020 2066 6f72 2028 6c65  .        for (le
+00001410: 7420 6669 656c 6420 6f66 205b 2774 7970  t field of ['typ
+00001420: 6527 2c20 2763 6174 6567 6f72 7927 2c20  e', 'category', 
+00001430: 2774 6f6f 6c27 2c20 2761 7265 6127 2c20  'tool', 'area', 
+00001440: 2763 6f6e 7375 6d61 626c 6527 5d29 0a20  'consumable']). 
+00001450: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
+00001460: 2020 2020 206c 6574 2069 6e70 7574 5f6e       let input_n
+00001470: 616d 6520 3d20 666f 726d 5f6e 756d 6265  ame = form_numbe
+00001480: 7220 2b20 225f 2220 2b20 6669 656c 643b  r + "_" + field;
+00001490: 0a09 0909 7261 7465 5f66 6f72 6d5f 7572  ....rate_form_ur
+000014a0: 6c20 2b3d 2027 2627 202b 2066 6965 6c64  l += '&' + field
+000014b0: 202b 2027 3d27 202b 2024 2827 696e 7075   + '=' + $('inpu
+000014c0: 745b 6e61 6d65 3d22 272b 696e 7075 745f  t[name="'+input_
+000014d0: 6e61 6d65 2b27 225d 2729 2e76 616c 2829  name+'"]').val()
+000014e0: 3b0a 2020 2020 2020 2020 7d0a 2020 2020  ;.        }.    
+000014f0: 2020 2020 242e 6765 7428 7261 7465 5f66      $.get(rate_f
+00001500: 6f72 6d5f 7572 6c2c 2066 756e 6374 696f  orm_url, functio
+00001510: 6e20 2863 6f6e 7465 6e74 290a 2020 2020  n (content).    
+00001520: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
+00001530: 2020 2428 2723 272b 666f 726d 5f6e 756d    $('#'+form_num
+00001540: 6265 722b 275f 666f 726d 2729 2e61 6674  ber+'_form').aft
+00001550: 6572 2863 6f6e 7465 6e74 293b 0a20 2020  er(content);.   
+00001560: 2020 2020 207d 0a20 2020 2020 2020 2029       }.        )
+00001570: 3b0a 097d 0a20 2020 2066 756e 6374 696f  ;..}.    functio
+00001580: 6e20 6465 6c65 7465 5f72 6174 655f 666f  n delete_rate_fo
+00001590: 726d 2866 6f72 6d5f 6e75 6d62 6572 2c20  rm(form_number, 
+000015a0: 7261 7465 5f69 6429 0a20 2020 207b 0a20  rate_id).    {. 
+000015b0: 2020 2020 2020 206c 6574 2073 7563 6365         let succe
+000015c0: 7373 5f63 616c 6c62 6163 6b20 3d20 6675  ss_callback = fu
+000015d0: 6e63 7469 6f6e 2028 2920 7b20 2428 2723  nction () { $('#
+000015e0: 272b 666f 726d 5f6e 756d 6265 722b 275f  '+form_number+'_
+000015f0: 666f 726d 2729 2e72 656d 6f76 6528 293b  form').remove();
+00001600: 207d 0a20 2020 2020 2020 2069 6620 2872   }.        if (r
+00001610: 6174 655f 6964 290a 2020 2020 2020 2020  ate_id).        
+00001620: 7b0a 2020 2020 2020 2020 2020 2020 6966  {.            if
+00001630: 2028 636f 6e66 6972 6d28 2241 7265 2079   (confirm("Are y
+00001640: 6f75 2073 7572 6520 796f 7520 7761 6e74  ou sure you want
+00001650: 2074 6f20 6465 6c65 7465 2074 6869 7320   to delete this 
+00001660: 7261 7465 3f20 5468 6973 2063 616e 6e6f  rate? This canno
+00001670: 7420 6265 2075 6e64 6f6e 652e 2229 290a  t be undone.")).
+00001680: 2020 2020 2020 2020 2020 2020 7b0a 2020              {.  
+00001690: 2020 2020 2020 2020 2020 0961 6a61 785f            .ajax_
+000016a0: 6765 7428 277b 2520 7572 6c20 2764 656c  get('{% url 'del
+000016b0: 6574 655f 7261 7465 5f74 696d 6527 2027  ete_rate_time' '
+000016c0: 3939 3939 2720 257d 272e 7265 706c 6163  9999' %}'.replac
+000016d0: 6528 2739 3939 3927 2c20 7261 7465 5f69  e('9999', rate_i
+000016e0: 6429 2c20 756e 6465 6669 6e65 642c 2073  d), undefined, s
+000016f0: 7563 6365 7373 5f63 616c 6c62 6163 6b2c  uccess_callback,
+00001700: 2061 6a61 785f 6661 696c 7572 655f 6361   ajax_failure_ca
+00001710: 6c6c 6261 636b 2827 4572 726f 7220 6465  llback('Error de
+00001720: 6c65 7469 6e67 2072 6174 6527 2929 3b0a  leting rate'));.
+00001730: 2020 2020 2020 2020 2020 2020 7d0a 0909              }...
+00001740: 7d0a 2020 2020 2020 2020 656c 7365 0a20  }.        else. 
+00001750: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
+00001760: 2020 2020 2073 7563 6365 7373 5f63 616c       success_cal
+00001770: 6c62 6163 6b28 293b 0a20 2020 2020 2020  lback();.       
+00001780: 207d 0a09 7d0a 093c 2f73 6372 6970 743e   }..}..</script>
+00001790: 0a7b 2520 656e 6462 6c6f 636b 2025 7d    .{% endblock %}
```

## NEMO_billing/rates/templates/rates/rate_form_details.html

```diff
@@ -1,95 +1,88 @@
 {% load custom_tags_and_filters %}
-{% if rate_type.category_specific and rate_categories %}
-	{% for category in rate_categories %}
-		<div class="form-group">
-			<div class="col-sm-6">
-				<h4 class="tool-rate-section">{{ rate_type }} ({{ category }})</h4>
-			</div>
-		</div>
-		{% with type_name=rate_type.get_type_form_name|add:'_'|add:category.name|lower %}
-			{% with rate_form=forms|get_item:type_name %}
-				{% if rate_form.instance.id %}<input type="hidden" name="{{ type_name }}_id" value="{{ rate_form.instance.id }}">{% endif %}
-				<div class="form-group">
-					<label class="control-label col-sm-2" for="{{ type_name }}_amount"><strong>Amount</strong></label>
-					<div class="col-sm-4">
-						<input class="form-control" type="number" step=".01" id="{{ type_name }}_amount" name="{{ type_name }}_amount" value="{{ rate_form.amount.value }}" required>
-					</div>
-					{% if rate_form.amount.errors %}
-						<div class="col-sm-6 form-control-static danger-highlight">
-							{{ rate_form.amount.errors|striptags }}
-						</div>
-					{% endif %}
-				</div>
-				<div class="form-group">
-					<div class="col-sm-4 col-sm-offset-2">
-						<div class="checkbox">
-							<label><input type="checkbox" id="{{ type_name }}_flat" name="{{ type_name }}_flat" {% if rate_form.flat.value %}checked{% endif %}> Flat</label>
-						</div>
+{# Making this condition into number to use it more easily in the template #}
+{# This is equivalent to display_rate_time = rate_form.time.value or show_rate_time #}
+{% with form_has_time=rate_form.time.value|yesno:"1,0" show_time_var=show_rate_time|yesno:"1,0" %}
+	{% with display_rate_time=form_has_time|add:show_time_var %}
+		<div id="{{ rate_form.form_number }}_form">
+			<input type="hidden" name="form_numbers[]" value="{{ rate_form.form_number }}">
+			<input type="hidden" name="{{ rate_form.form_number }}_id" value="{{ rate_form.instance.id|default_if_none:'' }}">
+			<input type="hidden" name="{{ rate_form.form_number }}_type" value="{{ rate_form.instance.type.id }}">
+			<input type="hidden" name="{{ rate_form.form_number }}_category" value="{{ rate_form.instance.category.id }}">
+			<input type="hidden" name="{{ rate_form.form_number }}_tool" value="{{ rate_form.instance.tool.id }}">
+			<input type="hidden" name="{{ rate_form.form_number }}_area" value="{{ rate_form.instance.area.id }}">
+			<input type="hidden" name="{{ rate_form.form_number }}_consumable" value="{{ rate_form.instance.consumable.id }}">
+			<div class="form-group">
+				<div class="h4 col-sm-6 {% if not display_rate_time %}tool-rate-section{% else %}text-right{% endif %}" style="padding-left: 0; padding-right: 0">
+					<div class="col-sm-12">
+						<span style="margin-right: 10px">
+							{% if not display_rate_time %}{{ rate_form.display_title }}{% else %}{{ rate_form.instance.time.name|default:"New time" }}{% endif %}
+						</span>
+						{% if rate_times and not display_rate_time and rate_form.instance.type.can_have_rate_time %}
+							<button title="Click to add a different rate time" type="button" onclick="add_rate_form('{{ rate_form.form_number }}');" class="btn-success btn btn-xs pull-right"><i style="margin-right: 5px" class="glyphicon-plus-sign glyphicon"></i>Add new time</button>
+						{% endif %}
+						{% if display_rate_time %}
+							<button title="Delete this rate time" type="button" onclick="delete_rate_form('{{ rate_form.form_number }}', '{{ rate_form.instance.id|default_if_none:'' }}');" class="btn-danger btn btn-xs pull-right"><span class="glyphicon-trash glyphicon"></span></button>
+						{% endif %}
+					</div>
+				</div>
+				{% if rate_form.non_field_errors %}
+					<div class="col-sm-6 form-control-static danger-highlight tool-rate-section" style="border-top: none">
+						{{ rate_form.non_field_errors|striptags }}
 					</div>
-					{% if rate_form.flat.errors %}
-						<div class="col-sm-6 form-control-static danger-highlight">
-							{{ rate_form.flat.errors|striptags }}
-						</div>
-					{% endif %}
-				</div>
+				{% endif %}
+			</div>
+			{% if display_rate_time %}
 				<div class="form-group">
-					<label class="control-label col-sm-2" for="{{ type_name }}_minimum_charge">Minimum Charge</label>
+					<label class="control-label col-sm-2" for="{{ rate_form.form_number }}_time"><strong>Time</strong></label>
 					<div class="col-sm-4">
-						<input class="form-control" type="number" step=".01" id="{{ type_name }}_minimum_charge" name="{{ type_name }}_minimum_charge" value="{{ rate_form.minimum_charge.value }}">
+						<select class="form-control" id="{{ rate_form.form_number }}_time" name="{{ rate_form.form_number }}_time" required>
+							<option value="" disabled selected></option>
+							{% for rate_time in rate_times %}
+								<option value="{{ rate_time.id }}" {% if rate_form.time.value|to_int == rate_time.id %}selected{% endif %}>{{ rate_time }}</option>
+							{% endfor %}
+						</select>
 					</div>
-					{% if rate_form.minimum_charge.errors %}
+					{% if rate_form.time.errors %}
 						<div class="col-sm-6 form-control-static danger-highlight">
-							{{ rate_form.minimum_charge.errors|striptags }}
+							{{ rate_form.time.errors|striptags }}
 						</div>
 					{% endif %}
 				</div>
-			{% endwith %}
-		{% endwith %}
-	{% endfor %}
-{% else %}
-	{# this is the exact copy of the previous html, but with a different rate_form name #}
-	<div class="form-group">
-		<div class="col-sm-6">
-			<h4 class="tool-rate-section">{{ rate_type }}</h4>
-		</div>
-	</div>
-	{% with type_name=rate_type.get_type_form_name %}
-		{% with rate_form=forms|get_item:type_name %}
-			{% if rate_form.instance.id %}<input type="hidden" name="{{ type_name }}_id" value="{{ rate_form.instance.id }}">{% endif %}
+			{% endif %}
 			<div class="form-group">
-				<label class="control-label col-sm-2" for="{{ type_name }}_amount"><strong>Amount</strong></label>
+				<label class="control-label col-sm-2" for="{{ rate_form.form_number }}_amount"><strong>Amount</strong></label>
 				<div class="col-sm-4">
-					<input class="form-control" type="number" step=".01" id="{{ type_name }}_amount" name="{{ type_name }}_amount" value="{{ rate_form.amount.value }}" required>
+					<input class="form-control" type="number" step=".01" id="{{ rate_form.form_number }}_amount" name="{{ rate_form.form_number }}_amount" value="{{ rate_form.amount.value }}">
 				</div>
 				{% if rate_form.amount.errors %}
 					<div class="col-sm-6 form-control-static danger-highlight">
 						{{ rate_form.amount.errors|striptags }}
 					</div>
 				{% endif %}
 			</div>
 			<div class="form-group">
 				<div class="col-sm-4 col-sm-offset-2">
 					<div class="checkbox">
-						<label><input type="checkbox" id="{{ type_name }}_flat" name="{{ type_name }}_flat" {% if rate_form.flat.value %}checked{% endif %}> Flat</label>
+						<label><input type="checkbox" id="{{ rate_form.form_number }}_flat" name="{{ rate_form.form_number }}_flat" {% if rate_form.flat.value %}checked{% endif %}> Flat</label>
 					</div>
 				</div>
 				{% if rate_form.flat.errors %}
 					<div class="col-sm-6 form-control-static danger-highlight">
 						{{ rate_form.flat.errors|striptags }}
 					</div>
 				{% endif %}
 			</div>
 			<div class="form-group">
-				<label class="control-label col-sm-2" for="{{ type_name }}_minimum_charge">Minimum Charge</label>
+				<label class="control-label col-sm-2" for="{{ rate_form.form_number }}_minimum_charge">Minimum Charge</label>
 				<div class="col-sm-4">
-					<input class="form-control" type="number" step=".01" id="{{ type_name }}_minimum_charge" name="{{ type_name }}_minimum_charge" value="{{ rate_form.minimum_charge.value }}">
+					<input class="form-control" type="number" step=".01" id="{{ rate_form.form_number }}_minimum_charge" name="{{ rate_form.form_number }}_minimum_charge" value="{{ rate_form.minimum_charge.value }}">
 				</div>
 				{% if rate_form.minimum_charge.errors %}
 					<div class="col-sm-6 form-control-static danger-highlight">
 						{{ rate_form.minimum_charge.errors|striptags }}
 					</div>
 				{% endif %}
 			</div>
-		{% endwith %}
+		</div>
 	{% endwith %}
-{% endif %}
+{% endwith %}
```

## NEMO_billing/rates/templates/rates/rates.html

```diff
@@ -1,55 +1,104 @@
 {% extends 'pagination/pagination_base.html' %}
+{% block extrahead %}
+	<style>
+		.container .pagination {
+			margin: initial;
+		}
+		.nav-tabs > li.active > a, .nav-tabs > li.active > a:hover {
+			background-color: #e9ecef;
+		}
+	</style>
+{% endblock %}
+{% load custom_tags_and_filters %}
 {% block title %}Rates{% endblock %}
 {% block before_pagination %}
-	<h1>
-		Rates
-		<a class="btn btn-success pull-right" href="{% url 'create_rate' %}">New rate</a>
-	</h1>
-	{% if page %}
-	<div class="row" style="margin-bottom: 20px">
+	<div class="row">
+		<div class="col-xs-7">
+			<h1>Rates</h1>
+		</div>
+		<div class="col-sm-5 text-right">
+			<h1>{% button type="add" url="create_rate" value="New rate" %}</h1>
+		</div>
+	</div>
+	<div class="row" style="margin-bottom: 40px">
 		<div class="col-sm-4">
 			<input id="search" type="text" placeholder="Search for a rate" class="form-control" autofocus>
 		</div>
 	</div>
-	{% endif %}
+
+	<div class="pull-left">
+		<ul class="nav nav-tabs" id="tabs" style="border-bottom: none;">
+			<li {% if rate_type|lower == 'tool' %}class="active"{% endif %}><a href="{% url 'rates' 'Tool' %}">Tools</a></li>
+			<li {% if rate_type|lower == 'area' %}class="active"{% endif %}><a href="{% url 'rates' 'Area' %}">Areas</a></li>
+			<li {% if rate_type|lower == 'consumable' %}class="active"{% endif %}><a href="{% url 'rates' 'CONSUMABLE' %}">Supplies</a></li>
+			<li {% if rate_type|lower == 'other' %}class="active"{% endif %}><a href="{% url 'rates' 'other' %}">Other</a></li>
+		</ul>
+	</div>
 {% endblock %}
 {% block pagination_content %}
-	<table class="table table-bordered table-condensed table-striped table-hover thead-light">
-		<thead>
-			<tr>
-				<th>{% include 'pagination/pagination_column.html' with order_by='type' name='Type' %}</th>
-				<th>Item</th>
-				{% if rate_categories_exist %}<th>{% include 'pagination/pagination_column.html' with order_by='category' name='Category' %}</th>{% endif %}
-				<th>{% include 'pagination/pagination_column.html' with order_by='amount' name='Rate' %}</th>
-				<th class="button-column-minimum">{% include 'pagination/pagination_column.html' with order_by='flat' name='Flat Rate' align=True  %}</th>
-				<th>{% include 'pagination/pagination_column.html' with order_by='minimum_charge' name='Minimum Charge'%}</th>
-				<th class="text-center button-column-minimum"></th>
-			</tr>
-		</thead>
-		<tbody>
-			{% for rate in page %}
+	{% with 'tool area consumable' as rate_type_list %}
+		<table class="table table-align-middle table-bordered table-condensed table-striped table-hover thead-light">
+			<thead>
 				<tr>
-					<td>{{ rate.type }}</td>
-					<td>{{ rate.get_item|default_if_none:"" }}</td>
-					{% if rate_categories_exist %}<td>{{ rate.category|default_if_none:"" }}</td>{% endif %}
-					<td>{{ rate.amount }}</td>
-					<td class="text-center"><span class="glyphicon {% if rate.flat %}glyphicon-ok success-highlight{% endif %}"></span></td>
-					<td>{{ rate.minimum_charge|default_if_none:'' }}</td>
-					<td><button type="button" class="btn btn-xs btn-default" title="Edit rate" onclick="window.location = '{% url 'edit_rate' rate.type.get_rate_group_type rate.id %}'"><i class="glyphicon glyphicon-pencil"></i></button></td>
+					{% if rate_type|lower in rate_type_list.split %}
+						<th>{% include 'pagination/pagination_column.html' with order_by=rate_type|lower name=rate_type|lower|capfirst %}</th>
+					{% endif %}
+					{% if show_type %}<th>{% include 'pagination/pagination_column.html' with order_by='type' name='Type' %}</th>{% endif %}
+					{% if show_category %}<th>{% include 'pagination/pagination_column.html' with order_by='category' name='Category' %}</th>{% endif %}
+					{% if show_time %}<th>{% include 'pagination/pagination_column.html' with order_by='time' name='Time' %}</th>{% endif %}
+					<th>{% include 'pagination/pagination_column.html' with order_by='amount' name='Rate' %}</th>
+					<th class="button-column-minimum">{% include 'pagination/pagination_column.html' with order_by='flat' name='Flat Rate' %}</th>
+					<th>{% include 'pagination/pagination_column.html' with order_by='minimum_charge' name='Minimum Charge'%}</th>
+					<th class="text-center button-column-minimum"></th>
 				</tr>
-			{% endfor %}
-		</tbody>
-	</table>
+			</thead>
+			<tbody>
+				{% for rate in page %}
+					<tr>
+						{% if rate_type|lower in rate_type_list.split %}
+							<td>{{ rate.get_item|default_if_none:"" }}</td>
+						{% endif %}
+						{% if show_type %}<td>{{ rate.type }}</td>{% endif %}
+						{% if show_category %}<td>{{ rate.category|default_if_none:"" }}</td>{% endif %}
+						{% if show_time %}<td>{{ rate.time|default_if_none:"" }}</td>{% endif %}
+						<td>{{ rate.amount }}</td>
+						<td class="text-center"><span class="glyphicon {% if rate.flat %}glyphicon-ok success-highlight{% endif %}"></span></td>
+						<td>{{ rate.minimum_charge|default_if_none:'' }}</td>
+						<td>
+							{% if rate.get_item.id %}
+								{% url 'create_rate' rate.type.get_rate_group_type rate.get_item.id as edit_rate_url %}
+								{% button type="edit" size="small" url=edit_rate_url title="Edit rate" value="Edit" %}
+							{% else %}
+								{% url 'create_rate' rate.type.get_rate_group_type as edit_rate_url %}
+								{% button type="edit" size="small" url=edit_rate_url title="Edit rate" value="Edit" %}
+							{% endif %}
+						</td>
+					</tr>
+				{% endfor %}
+			</tbody>
+		</table>
+	{% endwith %}
 	<script>
-	function get_rate(jquery_event, search_selection, dataset_name)
+		function get_rate(jquery_event, search_selection, dataset_name)
 		{
-			window.location.href = "{% url 'edit_rate' 'tool' 999 %}".replace('tool', search_selection.type_value).replace('999', search_selection.id);
+			if (search_selection.id)
+			{
+				window.location.href = "{% url 'create_rate' 'tool' 999 %}".replace('tool', search_selection.type_value).replace('999', search_selection.id);
+			}
+            else
+            {
+                window.location.href = "{% url 'create_rate' 'tool' %}".replace('tool', search_selection.type_value);
+            }
 		}
 		function on_load()
 		{
 			$("#search").autocomplete('users', get_rate, {{ search_rates }}).focus();
 		}
 		window.addEventListener('load', on_load, true);
 	</script>
 {% endblock %}
-{% block table_empty_content %}No rates have been created yet.{% endblock %}
+{% block table_empty_content %}
+	<table class="table table-bordered table-condensed table-striped table-hover thead-light">
+		<tr><th style="clear: both; padding: 15px; font-weight: initial">No rates of this type have been created yet.</th></tr>
+	</table>
+{% endblock %}
```

### html2text {}

```diff
@@ -1,17 +1,36 @@
-{% extends 'pagination/pagination_base.html' %} {% block title %}Rates{%
+{% extends 'pagination/pagination_base.html' %} {% block extrahead %}
+ {% endblock %} {% load custom_tags_and_filters %} {% block title %}Rates{%
 endblock %} {% block before_pagination %}
-****** Rates New_rate ******
-{% if page %}
+****** Rates ******
+****** {% button type="add" url="create_rate" value="New rate" %} ******
 [                    ]
-{% endif %} {% endblock %} {% block pagination_content %}
-{% include 'pagination/                                {% include 'pagination/        {% include 'pagination/ {% include 'pagination/ {% include 'pagination/
-pagination_column.html'                                pagination_column.html' with   pagination_column.html' pagination_column.html' pagination_column.html' with
-with order_by='type'    Item                           order_by='category'            with order_by='amount'  with order_by='flat'    order_by='minimum_charge'
-name='Type' %}                                         name='Category' %}             name='Rate' %}          name='Flat Rate'        name='Minimum Charge'%}
-                                                                                                              align=True %}
-                        {                              {                                                                              {
-{{ rate.type }}         {                              {                              {{ rate.amount }}                               {
-                        rate.get_item|default_if_none: rate.category|default_if_none:                                                 rate.minimum_charge|default_if_none:
-                        "" }}                          "" }}                                                                          '' }}
- {% endblock %} {% block table_empty_content %}No rates have been created yet.
+    * % if rate_type|lower == 'tool' %}class="active"{% endif %}>Tools
+% if rate_type|lower == 'area' %}class="active"{% endif %}>Areas
+% if rate_type|lower == 'consumable' %}class="active"{% endif %}>Supplies
+% if rate_type|lower == 'other' %}class="active"{% endif %}>Other
+{% endblock %} {% block pagination_content %} {% with 'tool area consumable' as
+rate_type_list %}
+{% include 'pagination/        {% include 'pagination/ {% include 'pagination/        {% include 'pagination/    {% include 'pagination/ {% include 'pagination/ {% include 'pagination/
+pagination_column.html' with   pagination_column.html' pagination_column.html' with   pagination_column.html'    pagination_column.html' pagination_column.html' pagination_column.html' with
+order_by=rate_type|lower       with order_by='type'    order_by='category'            with order_by='time'       with order_by='amount'  with order_by='flat'    order_by='minimum_charge'
+name=rate_type|lower|capfirst  name='Type' %}          name='Category' %}             name='Time' %}             name='Rate' %}          name='Flat Rate' %}     name='Minimum Charge'%}
+%}
+                                                                                                                                                                                                      {% if rate.get_item.id %} {%
+                                                                                                                                                                                                      url 'create_rate'
+                                                                                                                                                                                                      rate.type.get_rate_group_type
+                                                                                                                                                                                                      rate.get_item.id as
+                                                                                                                                                                                                      edit_rate_url %} {% button
+{                                                      {                              {                                                                          {                                    type="edit" size="small"
+{                                                      {                              {                                                                          {                                    url=edit_rate_url title="Edit
+rate.get_item|default_if_none: {{ rate.type }}         rate.category|default_if_none: rate.time|default_if_none: {{ rate.amount }}                               rate.minimum_charge|default_if_none: rate" value="Edit" %} {% else
+"" }}                                                  "" }}                          "" }}                                                                      '' }}                                %} {% url 'create_rate'
+                                                                                                                                                                                                      rate.type.get_rate_group_type
+                                                                                                                                                                                                      as edit_rate_url %} {% button
+                                                                                                                                                                                                      type="edit" size="small"
+                                                                                                                                                                                                      url=edit_rate_url title="Edit
+                                                                                                                                                                                                      rate" value="Edit" %} {%
+                                                                                                                                                                                                      endif %}
+{% endwith %}
+ {% endblock %} {% block table_empty_content %}
+No rates of this type have been created yet.
 {% endblock %}
```

## NEMO_billing/templates/base/navbar.html

```diff
@@ -1,310 +1,12 @@
-00000000: 7b25 206c 6f61 6420 7374 6174 6963 2025  {% load static %
-00000010: 7d0a 7b25 206c 6f61 6420 6375 7374 6f6d  }.{% load custom
-00000020: 5f74 6167 735f 616e 645f 6669 6c74 6572  _tags_and_filter
-00000030: 7320 257d 0a3c 6e61 7620 636c 6173 733d  s %}.<nav class=
-00000040: 226e 6176 6261 7220 6e61 7662 6172 2d64  "navbar navbar-d
-00000050: 6566 6175 6c74 206e 6176 6261 722d 7374  efault navbar-st
-00000060: 6174 6963 2d74 6f70 223e 0a09 3c64 6976  atic-top">..<div
-00000070: 2063 6c61 7373 3d22 636f 6e74 6169 6e65   class="containe
-00000080: 7222 3e0a 0909 3c64 6976 2063 6c61 7373  r">...<div class
-00000090: 3d22 6e61 7662 6172 2d68 6561 6465 7222  ="navbar-header"
-000000a0: 3e0a 0909 093c 6275 7474 6f6e 2074 7970  >....<button typ
-000000b0: 653d 2262 7574 746f 6e22 2063 6c61 7373  e="button" class
-000000c0: 3d22 6e61 7662 6172 2d74 6f67 676c 6522  ="navbar-toggle"
-000000d0: 2064 6174 612d 746f 6767 6c65 3d22 636f   data-toggle="co
-000000e0: 6c6c 6170 7365 2220 6461 7461 2d74 6172  llapse" data-tar
-000000f0: 6765 743d 2223 7369 7465 2d6e 6176 6967  get="#site-navig
-00000100: 6174 696f 6e22 3e0a 0909 0909 3c73 7061  ation">.....<spa
-00000110: 6e20 636c 6173 733d 2269 636f 6e2d 6261  n class="icon-ba
-00000120: 7222 3e3c 2f73 7061 6e3e 0a09 0909 093c  r"></span>.....<
-00000130: 7370 616e 2063 6c61 7373 3d22 6963 6f6e  span class="icon
-00000140: 2d62 6172 223e 3c2f 7370 616e 3e0a 0909  -bar"></span>...
-00000150: 0909 3c73 7061 6e20 636c 6173 733d 2269  ..<span class="i
-00000160: 636f 6e2d 6261 7222 3e3c 2f73 7061 6e3e  con-bar"></span>
-00000170: 0a09 0909 3c2f 6275 7474 6f6e 3e0a 0909  ....</button>...
-00000180: 093c 6120 636c 6173 733d 226e 6176 6261  .<a class="navba
-00000190: 722d 6272 616e 6422 2068 7265 663d 227b  r-brand" href="{
-000001a0: 2520 7572 6c20 276c 616e 6469 6e67 2720  % url 'landing' 
-000001b0: 257d 223e 7b7b 2073 6974 655f 7469 746c  %}">{{ site_titl
-000001c0: 6520 7d7d 3c2f 613e 0a09 093c 2f64 6976  e }}</a>...</div
-000001d0: 3e0a 0909 3c64 6976 2063 6c61 7373 3d22  >...<div class="
-000001e0: 6e61 7662 6172 2d63 6f6c 6c61 7073 6520  navbar-collapse 
-000001f0: 636f 6c6c 6170 7365 2220 6964 3d22 7369  collapse" id="si
-00000200: 7465 2d6e 6176 6967 6174 696f 6e22 3e0a  te-navigation">.
-00000210: 0909 093c 756c 2063 6c61 7373 3d22 6e61  ...<ul class="na
-00000220: 7620 6e61 7662 6172 2d6e 6176 223e 0a09  v navbar-nav">..
-00000230: 0909 093c 6c69 3e3c 6120 6872 6566 3d22  ...<li><a href="
-00000240: 7b25 2075 726c 2027 6361 6c65 6e64 6172  {% url 'calendar
-00000250: 2720 257d 223e 4361 6c65 6e64 6172 3c2f  ' %}">Calendar</
-00000260: 613e 3c2f 6c69 3e0a 0909 0909 7b25 2069  a></li>.....{% i
-00000270: 6620 746f 6f6c 735f 6578 6973 7420 257d  f tools_exist %}
-00000280: 3c6c 693e 3c61 2068 7265 663d 227b 2520  <li><a href="{% 
-00000290: 7572 6c20 2774 6f6f 6c5f 636f 6e74 726f  url 'tool_contro
-000002a0: 6c27 2025 7d22 3e54 6f6f 6c20 636f 6e74  l' %}">Tool cont
-000002b0: 726f 6c3c 2f61 3e3c 2f6c 693e 7b25 2065  rol</a></li>{% e
-000002c0: 6e64 6966 2025 7d0a 0909 0909 7b25 2069  ndif %}.....{% i
-000002d0: 6620 746f 6f6c 735f 6578 6973 7420 6f72  f tools_exist or
-000002e0: 2061 7265 6173 5f65 7869 7374 2025 7d0a   areas_exist %}.
-000002f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000300: 2020 2020 7b25 2069 6620 6172 6561 735f      {% if areas_
-00000310: 6578 6973 7473 2025 7d0a 2020 2020 2020  exists %}.      
-00000320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000330: 2020 3c6c 693e 3c61 2068 7265 663d 227b    <li><a href="{
-00000340: 2520 7572 6c20 2773 7461 7475 735f 6461  % url 'status_da
-00000350: 7368 626f 6172 6427 2025 7d22 3e53 7461  shboard' %}">Sta
-00000360: 7475 7320 6461 7368 626f 6172 643c 2f61  tus dashboard</a
-00000370: 3e3c 2f6c 693e 0a20 2020 2020 2020 2020  ></li>.         
-00000380: 2020 2020 2020 2020 2020 207b 2520 656c             {% el
-00000390: 7365 2025 7d0a 2020 2020 2020 2020 2020  se %}.          
-000003a0: 2020 2020 2020 2020 2020 2020 2020 3c6c                <l
-000003b0: 693e 3c61 2068 7265 663d 227b 2520 7572  i><a href="{% ur
-000003c0: 6c20 2773 7461 7475 735f 6461 7368 626f  l 'status_dashbo
-000003d0: 6172 645f 7461 6227 2027 746f 6f6c 7327  ard_tab' 'tools'
-000003e0: 2025 7d22 3e53 7461 7475 7320 6461 7368   %}">Status dash
-000003f0: 626f 6172 643c 2f61 3e3c 2f6c 693e 0a20  board</a></li>. 
-00000400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000410: 2020 207b 2520 656e 6469 6620 257d 0a20     {% endif %}. 
-00000420: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-00000430: 2520 656e 6469 6620 257d 0a09 0909 097b  % endif %}.....{
-00000440: 2520 6966 2062 7564 6479 5f73 7973 7465  % if buddy_syste
-00000450: 6d5f 6172 6561 735f 6578 6973 7420 257d  m_areas_exist %}
-00000460: 0a09 0909 0909 3c6c 693e 3c61 2068 7265  ......<li><a hre
-00000470: 663d 227b 2520 7572 6c20 2762 7564 6479  f="{% url 'buddy
-00000480: 5f73 7973 7465 6d27 2025 7d22 3e0a 0909  _system' %}">...
-00000490: 0909 0909 4275 6464 7920 626f 6172 640a  ....Buddy board.
-000004a0: 0909 0909 0909 7b25 2069 6620 6275 6464  ......{% if budd
-000004b0: 795f 6e6f 7469 6669 6361 7469 6f6e 5f63  y_notification_c
-000004c0: 6f75 6e74 2025 7d0a 0909 0909 0909 093c  ount %}........<
-000004d0: 7370 616e 2063 6c61 7373 3d22 6261 6467  span class="badg
-000004e0: 6522 2073 7479 6c65 3d22 7665 7274 6963  e" style="vertic
-000004f0: 616c 2d61 6c69 676e 3a6d 6964 646c 653b  al-align:middle;
-00000500: 2062 6163 6b67 726f 756e 642d 636f 6c6f   background-colo
-00000510: 723a 7265 6422 3e7b 7b20 6275 6464 795f  r:red">{{ buddy_
-00000520: 6e6f 7469 6669 6361 7469 6f6e 5f63 6f75  notification_cou
-00000530: 6e74 207d 7d3c 2f73 7061 6e3e 0a09 0909  nt }}</span>....
-00000540: 0909 097b 2520 656e 6469 6620 257d 0a09  ...{% endif %}..
-00000550: 0909 0909 3c2f 613e 3c2f 6c69 3e0a 0909  ....</a></li>...
-00000560: 0909 7b25 2065 6e64 6966 2025 7d0a 0909  ..{% endif %}...
-00000570: 0909 7b25 2069 6620 7573 6572 2e69 735f  ..{% if user.is_
-00000580: 7374 6166 6620 6f72 2075 7365 722e 6973  staff or user.is
-00000590: 5f74 6f6f 6c5f 7375 7065 7275 7365 7220  _tool_superuser 
-000005a0: 6f72 2075 7365 722e 6973 5f70 726f 6a65  or user.is_proje
-000005b0: 6374 5f70 6920 257d 0a09 0909 0909 3c6c  ct_pi %}......<l
-000005c0: 6920 636c 6173 733d 2264 726f 7064 6f77  i class="dropdow
-000005d0: 6e22 3e0a 0909 0909 0909 3c61 2068 7265  n">.......<a hre
-000005e0: 663d 2223 2220 636c 6173 733d 2264 726f  f="#" class="dro
-000005f0: 7064 6f77 6e2d 746f 6767 6c65 2220 6461  pdown-toggle" da
-00000600: 7461 2d74 6f67 676c 653d 2264 726f 7064  ta-toggle="dropd
-00000610: 6f77 6e22 3e41 646d 696e 6973 7472 6174  own">Administrat
-00000620: 696f 6e20 3c62 2063 6c61 7373 3d22 6361  ion <b class="ca
-00000630: 7265 7422 3e3c 2f62 3e3c 2f61 3e0a 0909  ret"></b></a>...
-00000640: 0909 0909 3c75 6c20 636c 6173 733d 2264  ....<ul class="d
-00000650: 726f 7064 6f77 6e2d 6d65 6e75 223e 0a09  ropdown-menu">..
-00000660: 0909 0909 0909 7b23 2054 6865 206e 6176  ......{# The nav
-00000670: 6967 6174 696f 6e5f 7572 6c20 7461 6720  igation_url tag 
-00000680: 7769 6c6c 2064 6973 706c 6179 2074 6865  will display the
-00000690: 2069 7465 6d20 6966 2074 6865 2055 524c   item if the URL
-000006a0: 206e 616d 6520 6361 6e20 6265 2072 6576   name can be rev
-000006b0: 6572 7365 642e 2023 7d0a 0909 0909 0909  ersed. #}.......
-000006c0: 097b 2320 5468 6973 2061 6c6c 6f77 7320  .{# This allows 
-000006d0: 6974 656d 7320 746f 2062 6520 6561 7369  items to be easi
-000006e0: 6c79 2072 656d 6f76 6564 2066 726f 6d20  ly removed from 
-000006f0: 7468 6520 7075 626c 6963 2066 6163 696e  the public facin
-00000700: 6720 7665 7273 696f 6e2e 2023 7d0a 0909  g version. #}...
-00000710: 0909 0909 097b 2520 6966 2075 7365 722e  .....{% if user.
-00000720: 6973 5f73 7461 6666 2025 7d0a 0909 0909  is_staff %}.....
-00000730: 0909 0909 7b25 206e 6176 6967 6174 696f  ....{% navigatio
-00000740: 6e5f 7572 6c20 2761 6275 7365 2720 2741  n_url 'abuse' 'A
-00000750: 6275 7365 2720 257d 0a09 0909 0909 0909  buse' %}........
-00000760: 097b 2520 6e61 7669 6761 7469 6f6e 5f75  .{% navigation_u
-00000770: 726c 2027 6163 636f 756e 7473 5f61 6e64  rl 'accounts_and
-00000780: 5f70 726f 6a65 6374 7327 2027 4163 636f  _projects' 'Acco
-00000790: 756e 7473 2061 6e64 2070 726f 6a65 6374  unts and project
-000007a0: 7327 2025 7d0a 0909 0909 0909 0909 7b25  s' %}.........{%
-000007b0: 206e 6176 6967 6174 696f 6e5f 7572 6c20   navigation_url 
-000007c0: 2761 6c65 7274 7327 2027 416c 6572 7473  'alerts' 'Alerts
-000007d0: 2720 257d 0a09 0909 0909 0909 097b 2520  ' %}.........{% 
-000007e0: 6966 2061 7265 6173 5f65 7869 7374 2025  if areas_exist %
-000007f0: 7d7b 2520 6e61 7669 6761 7469 6f6e 5f75  }{% navigation_u
-00000800: 726c 2027 6172 6561 5f61 6363 6573 7327  rl 'area_access'
-00000810: 2027 4172 6561 2061 6363 6573 7327 2025   'Area access' %
-00000820: 7d7b 2520 656e 6469 6620 257d 0a09 0909  }{% endif %}....
-00000830: 0909 0909 097b 2520 6966 2074 6f6f 6c73  .....{% if tools
-00000840: 5f65 7869 7374 2025 7d7b 2520 6e61 7669  _exist %}{% navi
-00000850: 6761 7469 6f6e 5f75 726c 2027 636f 6e66  gation_url 'conf
-00000860: 6967 7572 6174 696f 6e5f 6167 656e 6461  iguration_agenda
-00000870: 2720 2743 6f6e 6669 6775 7261 7469 6f6e  ' 'Configuration
-00000880: 2061 6765 6e64 6127 2025 7d7b 2520 656e   agenda' %}{% en
-00000890: 6469 6620 257d 0a09 0909 0909 0909 097b  dif %}.........{
-000008a0: 2520 6e61 7669 6761 7469 6f6e 5f75 726c  % navigation_url
-000008b0: 2027 6375 7374 6f6d 5f63 6861 7267 6573   'custom_charges
-000008c0: 2720 2743 7573 746f 6d20 6368 6172 6765  ' 'Custom charge
-000008d0: 7327 2025 7d0a 0909 0909 0909 0909 7b25  s' %}.........{%
-000008e0: 206e 6176 6967 6174 696f 6e5f 7572 6c20   navigation_url 
-000008f0: 2763 7573 746f 6d69 7a61 7469 6f6e 2720  'customization' 
-00000900: 2743 7573 746f 6d69 7a61 7469 6f6e 2720  'Customization' 
-00000910: 257d 0a09 0909 0909 0909 097b 2520 6e61  %}.........{% na
-00000920: 7669 6761 7469 6f6e 5f75 726c 2027 6164  vigation_url 'ad
-00000930: 6d69 6e3a 696e 6465 7827 2027 4465 7461  min:index' 'Deta
-00000940: 696c 6564 2061 646d 696e 6973 7472 6174  iled administrat
-00000950: 696f 6e27 2025 7d0a 0909 0909 0909 0909  ion' %}.........
-00000960: 7b25 206e 6176 6967 6174 696f 6e5f 7572  {% navigation_ur
-00000970: 6c20 2765 6d61 696c 5f62 726f 6164 6361  l 'email_broadca
-00000980: 7374 2720 2745 6d61 696c 2720 257d 0a09  st' 'Email' %}..
-00000990: 0909 0909 0909 097b 2520 6966 2075 7365  .......{% if use
-000009a0: 722e 6973 5f73 7570 6572 7573 6572 2025  r.is_superuser %
-000009b0: 7d7b 2520 6e61 7669 6761 7469 6f6e 5f75  }{% navigation_u
-000009c0: 726c 2027 696d 7065 7273 6f6e 6174 6527  rl 'impersonate'
-000009d0: 2027 496d 7065 7273 6f6e 6174 6527 2025   'Impersonate' %
-000009e0: 7d7b 2520 656e 6469 6620 257d 0a09 0909  }{% endif %}....
-000009f0: 0909 0909 097b 2520 6e61 7669 6761 7469  .....{% navigati
-00000a00: 6f6e 5f75 726c 2027 696e 766f 6963 6573  on_url 'invoices
-00000a10: 2720 2749 6e76 6f69 6365 7327 2025 7d0a  ' 'Invoices' %}.
-00000a20: 0909 0909 0909 0909 7b25 2069 6620 746f  ........{% if to
-00000a30: 6f6c 735f 6578 6973 7420 257d 7b25 206e  ols_exist %}{% n
-00000a40: 6176 6967 6174 696f 6e5f 7572 6c20 276d  avigation_url 'm
-00000a50: 6169 6e74 656e 616e 6365 2720 274d 6169  aintenance' 'Mai
-00000a60: 6e74 656e 616e 6365 2720 257d 7b25 2065  ntenance' %}{% e
-00000a70: 6e64 6966 2025 7d0a 0909 0909 0909 0909  ndif %}.........
-00000a80: 7b25 206e 6176 6967 6174 696f 6e5f 7572  {% navigation_ur
-00000a90: 6c20 2770 726f 6a65 6374 5f62 696c 6c69  l 'project_billi
-00000aa0: 6e67 2720 2750 726f 6a65 6374 2062 696c  ng' 'Project bil
-00000ab0: 6c69 6e67 2720 257d 0a09 0909 0909 0909  ling' %}........
-00000ac0: 097b 2520 6966 2074 6f6f 6c73 5f65 7869  .{% if tools_exi
-00000ad0: 7374 2025 7d7b 2520 6e61 7669 6761 7469  st %}{% navigati
-00000ae0: 6f6e 5f75 726c 2027 7175 616c 6966 6963  on_url 'qualific
-00000af0: 6174 696f 6e73 2720 2751 7561 6c69 6669  ations' 'Qualifi
-00000b00: 6361 7469 6f6e 7327 2025 7d7b 2520 656e  cations' %}{% en
-00000b10: 6469 6620 257d 0a09 0909 0909 0909 097b  dif %}.........{
-00000b20: 2520 6e61 7669 6761 7469 6f6e 5f75 726c  % navigation_url
-00000b30: 2027 7261 7465 7327 2027 5261 7465 7327   'rates' 'Rates'
-00000b40: 2025 7d0a 0909 0909 0909 0909 7b25 206e   %}.........{% n
-00000b50: 6176 6967 6174 696f 6e5f 7572 6c20 2772  avigation_url 'r
-00000b60: 656d 6f74 655f 776f 726b 2720 2752 656d  emote_work' 'Rem
-00000b70: 6f74 6520 776f 726b 2720 257d 0a09 0909  ote work' %}....
-00000b80: 0909 0909 097b 2520 6e61 7669 6761 7469  .....{% navigati
-00000b90: 6f6e 5f75 726c 2027 7265 736f 7572 6365  on_url 'resource
-00000ba0: 7327 2027 5265 736f 7572 6365 7327 2025  s' 'Resources' %
-00000bb0: 7d0a 0909 0909 0909 0909 7b25 206e 6176  }.........{% nav
-00000bc0: 6967 6174 696f 6e5f 7572 6c20 2773 7461  igation_url 'sta
-00000bd0: 6666 5f63 6861 7267 6573 2720 2753 7461  ff_charges' 'Sta
-00000be0: 6666 2063 6861 7267 6573 2720 257d 0a09  ff charges' %}..
-00000bf0: 0909 0909 0909 097b 2520 6e61 7669 6761  .......{% naviga
-00000c00: 7469 6f6e 5f75 726c 2027 636f 6e73 756d  tion_url 'consum
-00000c10: 6162 6c65 7327 2027 5375 7070 6c69 6573  ables' 'Supplies
-00000c20: 2720 257d 0a09 0909 0909 0909 2020 2020  ' %}........    
-00000c30: 7b25 2069 6620 746f 6f6c 735f 6578 6973  {% if tools_exis
-00000c40: 7420 257d 7b25 206e 6176 6967 6174 696f  t %}{% navigatio
-00000c50: 6e5f 7572 6c20 2774 7261 696e 696e 6727  n_url 'training'
-00000c60: 2027 5472 6169 6e69 6e67 2720 257d 7b25   'Training' %}{%
-00000c70: 2065 6e64 6966 2025 7d0a 2020 2020 2020   endif %}.      
-00000c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000c90: 2020 2020 2020 2020 2020 7b25 206e 6176            {% nav
-00000ca0: 6967 6174 696f 6e5f 7572 6c20 2775 7365  igation_url 'use
-00000cb0: 7273 2720 2755 7365 7273 2720 257d 0a20  rs' 'Users' %}. 
-00000cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000cd0: 2020 2020 2020 2020 2020 207b 2520 656c             {% el
-00000ce0: 7365 2025 7d0a 2020 2020 2020 2020 2020  se %}.          
-00000cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d00: 2020 2020 2020 7b25 2069 6620 7573 6572        {% if user
-00000d10: 2e69 735f 7072 6f6a 6563 745f 7069 2025  .is_project_pi %
-00000d20: 7d0a 0909 0909 0909 0909 097b 2520 6e61  }..........{% na
-00000d30: 7669 6761 7469 6f6e 5f75 726c 2027 7072  vigation_url 'pr
-00000d40: 6f6a 6563 7473 2720 2750 726f 6a65 6374  ojects' 'Project
-00000d50: 7327 2025 7d0a 2020 2020 2020 2020 2020  s' %}.          
-00000d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d70: 2020 2020 2020 7b25 2065 6e64 6966 2025        {% endif %
-00000d80: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
-00000d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000da0: 2020 7b25 2069 6620 7573 6572 2e69 735f    {% if user.is_
-00000db0: 746f 6f6c 5f73 7570 6572 7573 6572 2025  tool_superuser %
-00000dc0: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
-00000dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000de0: 2020 2020 2020 7b25 2069 6620 746f 6f6c        {% if tool
-00000df0: 735f 6578 6973 7420 257d 7b25 206e 6176  s_exist %}{% nav
-00000e00: 6967 6174 696f 6e5f 7572 6c20 2774 7261  igation_url 'tra
-00000e10: 696e 696e 6727 2027 5472 6169 6e69 6e67  ining' 'Training
-00000e20: 2720 257d 7b25 2065 6e64 6966 2025 7d0a  ' %}{% endif %}.
-00000e30: 0909 0909 0909 0909 7b25 2065 6e64 6966  ........{% endif
-00000e40: 2025 7d0a 0909 0909 0909 097b 2520 656e   %}........{% en
-00000e50: 6469 6620 257d 0a09 0909 0909 093c 2f75  dif %}.......</u
-00000e60: 6c3e 0a09 0909 0909 3c2f 6c69 3e0a 0909  l>......</li>...
-00000e70: 0909 7b25 2065 6e64 6966 2025 7d0a 0909  ..{% endif %}...
-00000e80: 0909 3c6c 6920 636c 6173 733d 2276 6973  ..<li class="vis
-00000e90: 6962 6c65 2d78 7322 3e3c 6120 6872 6566  ible-xs"><a href
-00000ea0: 3d22 7b25 2020 7572 6c20 2775 7365 725f  ="{%  url 'user_
-00000eb0: 7072 6566 6572 656e 6365 7327 2025 7d22  preferences' %}"
-00000ec0: 3e50 7265 6665 7265 6e63 6573 3c2f 613e  >Preferences</a>
-00000ed0: 3c2f 6c69 3e0a 0909 0909 7b25 2069 6620  </li>.....{% if 
-00000ee0: 6c6f 676f 7574 5f61 6c6c 6f77 6564 2025  logout_allowed %
-00000ef0: 7d0a 0909 0909 093c 6c69 2063 6c61 7373  }......<li class
-00000f00: 3d22 7669 7369 626c 652d 7873 223e 3c61  ="visible-xs"><a
-00000f10: 2068 7265 663d 227b 2520 7572 6c20 276c   href="{% url 'l
-00000f20: 6f67 6f75 7427 2025 7d22 3e4c 6f67 6f75  ogout' %}">Logou
-00000f30: 743c 2f61 3e3c 2f6c 693e 0a09 0909 097b  t</a></li>.....{
-00000f40: 2520 656e 6469 6620 257d 0a09 0909 3c2f  % endif %}....</
-00000f50: 756c 3e0a 0909 093c 756c 2063 6c61 7373  ul>....<ul class
-00000f60: 3d22 6e61 7620 6e61 7662 6172 2d6e 6176  ="nav navbar-nav
-00000f70: 206e 6176 6261 722d 7269 6768 7420 6869   navbar-right hi
-00000f80: 6464 656e 2d78 7322 3e0a 0909 0909 7b25  dden-xs">.....{%
-00000f90: 2069 6620 7573 6572 2e69 735f 7374 6166   if user.is_staf
-00000fa0: 6620 616e 6420 7573 6572 2e63 6861 7267  f and user.charg
-00000fb0: 696e 675f 7374 6166 665f 7469 6d65 2025  ing_staff_time %
-00000fc0: 7d0a 0909 0909 093c 6c69 2063 6c61 7373  }......<li class
-00000fd0: 3d22 6869 6464 656e 2d73 6d22 3e0a 0909  ="hidden-sm">...
-00000fe0: 0909 0909 3c70 2063 6c61 7373 3d22 6e61  ....<p class="na
-00000ff0: 7662 6172 2d74 6578 7422 3e0a 0909 0909  vbar-text">.....
-00001000: 0909 093c 6120 6964 3d22 7374 6166 665f  ...<a id="staff_
-00001010: 6368 6172 6765 5f6c 696e 6b22 2068 7265  charge_link" hre
-00001020: 663d 227b 2520 7572 6c20 2773 7461 6666  f="{% url 'staff
-00001030: 5f63 6861 7267 6573 2720 257d 2220 7374  _charges' %}" st
-00001040: 796c 653d 2263 6f6c 6f72 3a72 6564 3b20  yle="color:red; 
-00001050: 7465 7874 2d64 6563 6f72 6174 696f 6e3a  text-decoration:
-00001060: 206e 6f6e 6522 2064 6174 612d 746f 6767   none" data-togg
-00001070: 6c65 3d22 746f 6f6c 7469 7022 2064 6174  le="tooltip" dat
-00001080: 612d 706c 6163 656d 656e 743d 2262 6f74  a-placement="bot
-00001090: 746f 6d22 2074 6974 6c65 3d22 7b25 2077  tom" title="{% w
-000010a0: 6974 6820 7573 6572 2e67 6574 5f73 7461  ith user.get_sta
-000010b0: 6666 5f63 6861 7267 6520 6173 2073 7461  ff_charge as sta
-000010c0: 6666 5f63 6861 7267 6520 257d 596f 7520  ff_charge %}You 
-000010d0: 6172 6520 6368 6172 6769 6e67 2073 7461  are charging sta
-000010e0: 6666 2074 696d 6520 746f 207b 7b20 7374  ff time to {{ st
-000010f0: 6166 665f 6368 6172 6765 2e63 7573 746f  aff_charge.custo
-00001100: 6d65 7220 7d7d 2066 6f72 2074 6865 2070  mer }} for the p
-00001110: 726f 6a65 6374 206e 616d 6564 207b 7b20  roject named {{ 
-00001120: 7374 6166 665f 6368 6172 6765 2e70 726f  staff_charge.pro
-00001130: 6a65 6374 207d 7d20 7369 6e63 6520 7b7b  ject }} since {{
-00001140: 2073 7461 6666 5f63 6861 7267 652e 7374   staff_charge.st
-00001150: 6172 7420 7d7d 2e7b 2520 656e 6477 6974  art }}.{% endwit
-00001160: 6820 257d 223e 0a09 0909 0909 0909 0943  h %}">.........C
-00001170: 6861 7267 696e 6720 7374 6166 6620 7469  harging staff ti
-00001180: 6d65 0a09 0909 0909 0909 3c2f 613e 0a09  me........</a>..
-00001190: 0909 0909 093c 2f70 3e0a 0909 0909 0909  .....</p>.......
-000011a0: 3c73 6372 6970 743e 0a09 0909 0909 0909  <script>........
-000011b0: 2428 2223 7374 6166 665f 6368 6172 6765  $("#staff_charge
-000011c0: 5f6c 696e 6b22 292e 746f 6f6c 7469 7028  _link").tooltip(
-000011d0: 293b 0a09 0909 0909 093c 2f73 6372 6970  );.......</scrip
-000011e0: 743e 0a09 0909 0909 3c2f 6c69 3e0a 0909  t>......</li>...
-000011f0: 0909 7b25 2065 6e64 6966 2025 7d0a 0909  ..{% endif %}...
-00001200: 0909 3c6c 6920 636c 6173 733d 2268 6964  ..<li class="hid
-00001210: 6465 6e2d 736d 223e 3c70 2063 6c61 7373  den-sm"><p class
-00001220: 3d22 6e61 7662 6172 2d74 6578 7422 3e57  ="navbar-text">W
-00001230: 656c 636f 6d65 2c20 7b7b 2075 7365 722e  elcome, {{ user.
-00001240: 6669 7273 745f 6e61 6d65 207d 7d3c 2f70  first_name }}</p
-00001250: 3e3c 2f6c 693e 0a09 0909 093c 6c69 2063  ></li>.....<li c
-00001260: 6c61 7373 3d22 6e61 7662 6172 2d70 7265  lass="navbar-pre
-00001270: 6665 7265 6e63 6573 223e 3c61 2068 7265  ferences"><a hre
-00001280: 663d 227b 2520 2075 726c 2027 7573 6572  f="{%  url 'user
-00001290: 5f70 7265 6665 7265 6e63 6573 2720 257d  _preferences' %}
-000012a0: 223e 3c69 6d67 2073 7263 3d22 7b25 2073  "><img src="{% s
-000012b0: 7461 7469 6320 2769 636f 6e73 2f70 7265  tatic 'icons/pre
-000012c0: 6665 7265 6e63 6573 2e70 6e67 2720 257d  ferences.png' %}
-000012d0: 222f 3e3c 2f61 3e3c 2f6c 693e 0a09 0909  "/></a></li>....
-000012e0: 097b 2520 6966 206c 6f67 6f75 745f 616c  .{% if logout_al
-000012f0: 6c6f 7765 6420 257d 0a09 0909 0909 3c6c  lowed %}......<l
-00001300: 693e 3c61 2068 7265 663d 227b 2520 7572  i><a href="{% ur
-00001310: 6c20 276c 6f67 6f75 7427 2025 7d22 3e4c  l 'logout' %}">L
-00001320: 6f67 6f75 743c 2f61 3e3c 2f6c 693e 0a09  ogout</a></li>..
-00001330: 0909 097b 2520 656e 6469 6620 257d 0a09  ...{% endif %}..
-00001340: 0909 3c2f 756c 3e0a 0909 3c2f 6469 763e  ..</ul>...</div>
-00001350: 0a09 3c2f 6469 763e 0a3c 2f6e 6176 3e    ..</div>.</nav>
+00000000: 7b25 2065 7874 656e 6473 2027 6261 7365  {% extends 'base
+00000010: 2f6e 6176 6261 725f 6261 7365 2e68 746d  /navbar_base.htm
+00000020: 6c27 2025 7d0a 7b25 206c 6f61 6420 7374  l' %}.{% load st
+00000030: 6174 6963 2025 7d0a 7b25 206c 6f61 6420  atic %}.{% load 
+00000040: 6375 7374 6f6d 5f74 6167 735f 616e 645f  custom_tags_and_
+00000050: 6669 6c74 6572 7320 257d 0a7b 2520 626c  filters %}.{% bl
+00000060: 6f63 6b20 6e61 7662 6172 5f61 646d 696e  ock navbar_admin
+00000070: 2025 7d0a 097b 7b20 626c 6f63 6b2e 7375   %}..{{ block.su
+00000080: 7065 7220 7d7d 0a09 7b25 2069 6e63 6c75  per }}..{% inclu
+00000090: 6465 2027 6261 7365 2f6e 6176 6261 725f  de 'base/navbar_
+000000a0: 6269 6c6c 696e 672e 6874 6d6c 2720 257d  billing.html' %}
+000000b0: 0a7b 2520 656e 6462 6c6f 636b 2025 7d0a  .{% endblock %}.
```

## NEMO_billing/templates/billing/custom_charge.html

```diff
@@ -1,10 +1,11 @@
 {% extends "base.html" %}
 {% load static %}
 {% load custom_tags_and_filters %}
+{% load billing_tags %}
 {% block extrahead %}
 	<script type="text/javascript" src="{% static "datetimepicker/bootstrap-datetimepicker.js" %}"></script>
 	<link rel="stylesheet" type="text/css" href="{% static "datetimepicker/bootstrap-datetimepicker.css" %}"/>
 {% endblock %}
 {% block title %}{% if form.instance.pk %}Edit{% else %}New{% endif %} Custom charge{% endblock %}
 {% block content %}
 	{% with edit=form.instance.pk %}
@@ -46,15 +47,15 @@
 						{{ form.additional_details.errors|striptags }}
 					</div>
 				{% endif %}
 			</div>
 			<div class="form-group">
 				<label class="control-label col-sm-2" for="date"><strong>Date</strong></label>
 				<div class="col-sm-4">
-					<input id="date" name="date" class="form-control" type="text" placeholder="Charge date" value="{% if edit %}{{ form.instance.date|date:"SHORT_DATETIME_FORMAT"|default_if_none:"" }}{% else %}{{ form.date.value|default_if_none:"" }}{% endif %}" required>
+					<input id="date" name="date" class="form-control" type="text" placeholder="Charge date" value="{{ form.date.value|input_date_format }}" required>
 				</div>
 				{% if form.date.errors %}
 					<div class="col-sm-6 form-control-static danger-highlight">
 						{{ form.date.errors|striptags }}
 					</div>
 				{% endif %}
 			</div>
@@ -118,16 +119,30 @@
 				</div>
 				{% if form.amount.errors %}
 					<div class="col-sm-6 form-control-static danger-highlight">
 						{{ form.amount.errors|striptags }}
 					</div>
 				{% endif %}
 			</div>
+			{% cap_discount_installed as cap_discount_installed %}
+			{% if cap_discount_installed %}
+				<div class="form-group">
+					<label class="control-label col-sm-2" for="cap_eligible">Cap eligible</label>
+					<div class="col-sm-4 checkbox">
+						<label><input id="cap_eligible" name="cap_eligible" type="checkbox" {% if form.cap_eligible.value %}checked{% endif %}> Check to make this charge count towards CAP</label>
+					</div>
+					{% if form.cap_eligible.errors %}
+						<div class="col-sm-6 form-control-static danger-highlight">
+							{{ form.cap_eligible.errors|striptags }}
+						</div>
+					{% endif %}
+				</div>
+			{% endif %}
 			<div class="col-sm-6 text-right">
-				<button type="submit" class="btn btn-success">Confirm</button>
+				{% button type="save" value="Confirm" %}
 			</div>
 		</form>
 
 		<script>
 		function clear_customer()
 		{
 			$("#chosen_customer").val('').hide();
@@ -136,15 +151,15 @@
 			$('#project').find('option').remove().end().attr('disabled', 'disabled');
 		}
 		function get_customer(jquery_event, search_selection, dataset_name)
 		{
 			$('#customer_search').prop('required', false).hide();
 			$('#chosen_customer').val(search_selection.name).show();
 			$('#customer').val(search_selection.id);
-			ajax_get("{% url 'get_projects' %}", {'user_id': search_selection.id}, update_projects);
+			ajax_get("{% url 'get_projects_for_custom_charges' %}", {'user_id': search_selection.id}, update_projects);
 		}
 		function update_projects(response, status, xml_http_request)
 		{
 			let project_selector = $('#project');
 			project_selector.find('option').remove().end().removeAttr('disabled');
 			let projects = response['projects'];
 
@@ -165,13 +180,15 @@
 					project_selector.append($('<option/>', {value: project.id, text: project.name}));
 				});
 			}
 		}
 		window.addEventListener('load', function()
 		{
 			$('#customer_search').autocomplete('customers', get_customer, {{ users|json_search_base }});
-			let time_picker_options = {'sideBySide': true};
-			$('#date').datetimepicker(time_picker_options);
+            let timepicker_properties = {
+                format: '{{ datetime_input_js_format }}', 'sideBySide': true
+            };
+			$('#date').datetimepicker(timepicker_properties);
 		}, true);
 		</script>
 	{% endwith %}
 {% endblock %}
```

### html2text {}

```diff
@@ -1,9 +1,9 @@
 {% extends "base.html" %} {% load static %} {% load custom_tags_and_filters %}
-{% block extrahead %}
+{% load billing_tags %} {% block extrahead %}
 ootstrap-datetimepicker.js" %}">
 ootstrap-datetimepicker.css" %}"/> {% endblock %} {% block title %}{% if
 form.instance.pk %}Edit{% else %}New{% endif %} Custom charge{% endblock %} {%
 block content %} {% with edit=form.instance.pk %}
 ****** {% if edit %}Edit{% else %}New{% endif %} custom charge ******
 {% if form.errors %}
 Oops! Something went wrong. Please correct the errors highlighted below.
@@ -20,16 +20,15 @@
 {% endif %}
 Description
  }}" autofocus>
 {% if form.additional_details.errors %}
 {{ form.additional_details.errors|striptags }}
 {% endif %}
 Date
-|default_if_none:"" }}{% else %}{{ form.date.value|default_if_none:"" }}{%
-endif %}" required>
+[{{ form.date.value|input_date_format }}]
 {% if form.date.errors %}
 {{ form.date.errors|striptags }}
 {% endif %}
 Customer {{ form.instance.customer }}
 % if not form.customer.value %}required{% endif %}>
  }}{% endif %}" style="{% if not form.customer.value %}display:none{% endif
 %}">
@@ -64,9 +63,18 @@
 {% endif %}
 {% endif %}
 Amount
 [Unknown INPUT type]
 {% if form.amount.errors %}
 {{ form.amount.errors|striptags }}
 {% endif %}
-Confirm
+{% cap_discount_installed as cap_discount_installed %} {% if
+cap_discount_installed %}
+Cap eligible
+% if form.cap_eligible.value %}checked{% endif %}> Check to make this charge
+count towards CAP
+{% if form.cap_eligible.errors %}
+{{ form.cap_eligible.errors|striptags }}
+{% endif %}
+{% endif %}
+{% button type="save" value="Confirm" %}
  {% endwith %} {% endblock %}
```

## NEMO_billing/templates/billing/custom_charges.html

```diff
@@ -1,14 +1,19 @@
 {% extends 'pagination/pagination_base.html' %}
+{% load custom_tags_and_filters %}
 {% block title %}Custom charges{% endblock %}
 {% block before_pagination %}
-	<h1>
-		Custom charges
-		<a class="btn btn-success pull-right" href="{% url 'create_custom_charge' %}">New custom charge</a>
-	</h1>
+	<div class="row">
+		<div class="col-xs-7">
+			<h1>Custom charges</h1>
+		</div>
+		<div class="col-sm-5 text-right">
+			<h1>{% button type="add" url="create_custom_charge" value="New custom charge" %}</h1>
+		</div>
+	</div>
 {% endblock %}
 {% block pagination_content %}
 	<table class="table table-bordered table-striped table-condensed thead-light">
 		<thead>
 			<tr>
 				<th>{% include 'pagination/pagination_column.html' with order_by="name" name='Name' %}</th>
 				<th>{% include 'pagination/pagination_column.html' with order_by="date" name='Date' %}</th>
```

### html2text {}

```diff
@@ -1,10 +1,12 @@
-{% extends 'pagination/pagination_base.html' %} {% block title %}Custom charges
-{% endblock %} {% block before_pagination %}
-****** Custom charges New_custom_charge ******
+{% extends 'pagination/pagination_base.html' %} {% load custom_tags_and_filters
+%} {% block title %}Custom charges{% endblock %} {% block before_pagination %}
+****** Custom charges ******
+****** {% button type="add" url="create_custom_charge" value="New custom
+charge" %} ******
 {% endblock %} {% block pagination_content %}
 {% include 'pagination/ {% include 'pagination/ {% include 'pagination/ {% include 'pagination/ {% include 'pagination/ {% include 'pagination/ {% include 'pagination/
 pagination_column.html' pagination_column.html' pagination_column.html' pagination_column.html' pagination_column.html' pagination_column.html' pagination_column.html' with
 with order_by="name"    with order_by="date"    with order_by="project" with                    with order_by="amount"  with order_by="creator" order_by="core_facility" name='Core
 name='Name' %}          name='Date' %}          name='Project' %}       order_by="customer"     name='Amount' %}        name='Created By' %}    Facility' %}
                                                                         name='Customer' %}
                                                 {                       {                                               {                       {
```

## NEMO_billing/templates/staff_charges/choose_project.html

```diff
@@ -1,8 +1,9 @@
 {% extends 'staff_charges/staff_charges_base.html' %}
+{% load custom_tags_and_filters %}
 {% block staff_charges_content %}
 	<div class="col-sm-12">
 		<form action="{% url 'begin_staff_charge' %}" class="form-horizontal" method="post">
 			{% csrf_token %}
 			<div class="form-group">
 				Customer: {{ customer }}<br>
 				<input type="hidden" name="customer" value="{{ customer.id }}">
@@ -12,18 +13,18 @@
 				{% if customer.active_project_count == 1 %}
 					Staff time will be billed to the customer's only project, &quot;{{ customer.active_projects.0 }}&quot;
 					<input type="hidden" name="project" value="{{ customer.active_projects.0.id }}">
 				{% else %}
 					Which of the customer's projects would you like to bill?
 					<div class="radio">
 						{% for p in customer.active_projects %}
-							<label class="control-label"><input type="radio" name="project" value="{{ p.id }}" required> {{ p }}</label><br>
+							<label class="control-label"><input type="radio" name="project" value="{{ p.id }}" required> {% project_selection_display p %}</label><br>
 						{% endfor %}
 					</div>
 				{% endif %}
 			</div>
 			<div class="form-group">
-				<input type="submit" class="btn btn-success" value="Begin billing staff time">
+                {% button type="save" value="Begin billing staff time" icon="glyphicon-time" %}
 			</div>
 		</form>
 	</div>
 {% endblock %}
```

## NEMO_billing/templates/staff_charges/new_custom_staff_charge.html

```diff
@@ -25,16 +25,16 @@
 							<option value="{{ core_facility.id }}">{{ core_facility.name }}</option>
 						{% endfor %}
 					</select>
 				</div>
 			</div>
 		{% endif %}
 		<div class="form-group">
-			<div class="col-sm-6">
-				<input type="submit" class="btn btn-success pull-right" value="Continue">
+			<div class="col-sm-6 text-right">
+				{% button type="save" value="Continue" icon="glyphicon-ok-circle" %}
 			</div>
 		</div>
 	</form>
 	<script>
 		function select_user(jquery_event, search_selection, dataset_name)
 		{
 			$("#customer").val(search_selection.id);
```

### html2text {}

```diff
@@ -12,9 +12,9 @@
 {% if core_facility_required %}Core Facility{% else %}Core Facility{% endif %}
 % if core_facility_required %}required{% endif %}>
 Select a core facility
 {% for core_facility in core_facilities %}
 {{ core_facility.name }}
 {% endfor %}
 {% endif %}
-[Continue]
+{% button type="save" value="Continue" icon="glyphicon-ok-circle" %}
  {% endblock %}
```

## Comparing `NEMO_billing/invoices/invoice_data_processor.py` & `NEMO_billing/cap_discount/processors.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,348 +1,384 @@
-from decimal import Decimal
-from typing import List, Optional
-
-from NEMO.models import (
-    UsageEvent,
-    AreaAccessRecord,
-    Reservation,
-    StaffCharge,
-    ConsumableWithdraw,
-    TrainingSession,
-    Consumable,
-    Area,
-    Tool,
-    User,
+from _decimal import Decimal
+from datetime import date, datetime, time
+from logging import getLogger
+from typing import Dict, Iterable, List, Optional, Union
+
+from NEMO.models import Account, Project
+from NEMO.utilities import get_month_timeframe
+from dateutil.relativedelta import relativedelta
+from django.contrib import messages
+from django.contrib.admin.utils import get_deleted_objects
+from django.db import transaction
+from django.db.models import Q
+from django.http import HttpRequest
+from django.utils import timezone
+
+from NEMO_billing.cap_discount.customization import CAPDiscountCustomization
+from NEMO_billing.cap_discount.exceptions import MissingCAPAmountException, NotLatestInvoiceException
+from NEMO_billing.cap_discount.models import CAPDiscount, CAPDiscountAmount, CAPDiscountConfiguration
+from NEMO_billing.invoices.models import (
+    BillableItemType,
+    Invoice,
+    InvoiceConfiguration,
+    InvoiceDetailItem,
+    InvoiceSummaryItem,
 )
-from NEMO.views.api_billing import get_minutes_between_dates
-from django.conf import settings
-from django.db.models import Sum, QuerySet, Q, F
-
-from NEMO_billing.invoices.exceptions import NoRateSetException, InvoiceItemsNotInFacilityException
-from NEMO_billing.invoices.models import ProjectBillingDetails, Invoice, InvoiceDetailItem, InvoiceSummaryItem
-from NEMO_billing.models import CustomCharge
-from NEMO_billing.rates.models import RateType, Rate
-
-
-def get_rate(
-    r_type: str,
-    project_details: ProjectBillingDetails,
-    tool: Tool = None,
-    area: Area = None,
-    consumable: Consumable = None,
-):
-    rate_type = RateType.objects.get(type=r_type)
-    kwargs = {"type_id": rate_type.id}
-    if rate_type.category_specific:
-        kwargs["category"] = project_details.category
-    if rate_type.item_specific:
-        if tool:
-            kwargs["tool_id"] = tool.id
-        elif area:
-            kwargs["area_id"] = area.id
-        elif consumable:
-            kwargs["consumable_id"] = consumable.id
-    try:
-        return Rate.objects.get(**kwargs)
-    except Rate.DoesNotExist:
-        raise NoRateSetException(rate_type.id, project_details.category, tool=tool, area=area, consumable=consumable)
-
-
-def get_rate_with_currency(invoice: Invoice, rate: str):
-    return f"{invoice.configuration.currency} {rate}"
-
-
-class InvoiceDataProcessor(object):
-    tool_usage_staff_filter = Q(operator__is_staff=True) & ~Q(operator=F("user"))
+from NEMO_billing.invoices.processors import (
+    FullInvoice,
+    InvoiceDataProcessor,
+    billable_to_invoice_detail_item,
+)
+from NEMO_billing.rates.models import RateCategory
 
-    def process_data(self, start, end, project_details, configuration, user: User) -> Optional[Invoice]:
-        invoice = self.create_invoice(start, end, project_details, configuration, user)
-        detail_items: List[InvoiceDetailItem] = []
-        detail_items.extend(self.tool_usages_invoice_details(invoice))
-        detail_items.extend(self.area_access_records_invoice_details(invoice))
-        detail_items.extend(self.missed_reservations_invoice_details(invoice))
-        detail_items.extend(self.staff_charges_invoice_details(invoice))
-        detail_items.extend(self.consumable_withdrawals_invoice_details(invoice))
-        detail_items.extend(self.training_sessions_invoice_details(invoice))
-        detail_items.extend(self.custom_charges_invoice_details(invoice))
-        if settings.INVOICE_ALL_ITEMS_MUST_BE_IN_FACILITY:
-            for detail_item in detail_items:
-                if not detail_item.core_facility:
-                    raise InvoiceItemsNotInFacilityException(detail_item)
-        if detail_items:
-            invoice.save()
-            for detail_item in detail_items:
-                detail_item.invoice = invoice
-                detail_item.save(force_insert=True)
-            self.add_invoice_summary_items(invoice)
-            return invoice
-
-    def create_invoice(self, start, end, project_details, configuration, user: User) -> Invoice:
-        invoice = Invoice()
-        invoice.start = start
-        invoice.end = end
-        invoice.project_details = project_details
-        invoice.configuration = configuration
-        invoice.created_by = user
-        invoice.total_amount = 0
-        return invoice
-
-    def tool_usages_invoice_details(self, invoice: Invoice) -> List[InvoiceDetailItem]:
-        start, end = invoice.start, invoice.end
-        usage_events = UsageEvent.objects.filter(start__gte=start, end__lte=end, start__lte=end, end__gte=start)
-        usage_events = usage_events.filter(project_id=invoice.project_details.project_id).order_by("start")
-        # Exclude usage events when operator is staff and different from user
-        usage_events = usage_events.exclude(self.tool_usage_staff_filter)
-        return [self.item_from_usage_event(invoice, usage_event) for usage_event in usage_events]
-
-    def area_access_records_invoice_details(self, invoice: Invoice) -> List[InvoiceDetailItem]:
-        start, end = invoice.start, invoice.end
-        access_records = AreaAccessRecord.objects.filter(
-            start__gte=start, end__lte=end, start__lte=end, end__gte=start, staff_charge=None
-        )
-        access_records = access_records.filter(project_id=invoice.project_details.project_id).order_by("start")
-        return [self.item_from_area_access_record(invoice, area_access) for area_access in access_records]
+processors_logger = getLogger(__name__)
 
-    def missed_reservations_invoice_details(self, invoice: Invoice) -> List[InvoiceDetailItem]:
-        start, end = invoice.start, invoice.end
-        missed_res = Reservation.objects.filter(
-            missed=True, start__gte=start, end__lte=end, start__lte=end, end__gte=start
-        )
-        missed_res = missed_res.filter(project_id=invoice.project_details.project_id).order_by("start")
-        return [self.item_from_missed_reservation(invoice, missed) for missed in missed_res]
 
-    def staff_charges_invoice_details(self, invoice: Invoice) -> List[InvoiceDetailItem]:
-        start, end = invoice.start, invoice.end
-        staff_charges = StaffCharge.objects.filter(start__gte=start, end__lte=end, start__lte=end, end__gte=start)
-        staff_charges = staff_charges.filter(project_id=invoice.project_details.project_id).order_by("start")
-        staff_charge_item_list = [self.item_from_staff_charge(invoice, staff_charge) for staff_charge in staff_charges]
-        # Add area access during staff charges
-        for area_access in AreaAccessRecord.objects.filter(staff_charge__in=staff_charges):
-            area_access_by_staff_item = self.item_from_area_access_record(invoice, area_access)
-            area_access_by_staff_item.item_type = InvoiceDetailItem.InvoiceDetailItemType.STAFF_CHARGE
-            staff_charge_item_list.append(area_access_by_staff_item)
-        # Add all tool usage by staff members
-        usages_by_staff = UsageEvent.objects.filter(start__gte=start, end__lte=end, start__lte=end, end__gte=start)
-        usages_by_staff = usages_by_staff.filter(project_id=invoice.project_details.project_id).order_by("start")
-        usages_by_staff = usages_by_staff.filter(self.tool_usage_staff_filter)
-        for usage_by_staff in usages_by_staff:
-            usages_by_staff_item = self.item_from_usage_event(invoice, usage_by_staff)
-            usages_by_staff_item.item_type = InvoiceDetailItem.InvoiceDetailItemType.STAFF_CHARGE
-            staff_charge_item_list.append(usages_by_staff_item)
-        return staff_charge_item_list
-
-    def consumable_withdrawals_invoice_details(self, invoice: Invoice) -> List[InvoiceDetailItem]:
-        start, end = invoice.start, invoice.end
-        withdrawals = ConsumableWithdraw.objects.filter(date__gte=start, date__lte=end)
-        withdrawals = withdrawals.filter(project_id=invoice.project_details.project_id).order_by("date")
-        return [self.item_from_consumable_withdrawal(invoice, withdrawal) for withdrawal in withdrawals]
-
-    def training_sessions_invoice_details(self, invoice: Invoice) -> List[InvoiceDetailItem]:
-        start, end = invoice.start, invoice.end
-        training_sessions = TrainingSession.objects.filter(date__gte=start, date__lte=end)
-        training_sessions = training_sessions.filter(project_id=invoice.project_details.project_id).order_by("date")
-        return [self.item_from_training(invoice, training) for training in training_sessions]
-
-    def custom_charges_invoice_details(self, invoice: Invoice) -> List[InvoiceDetailItem]:
-        start, end = invoice.start, invoice.end
-        custom_charges = CustomCharge.objects.filter(date__gte=start, date__lte=end)
-        custom_charges = custom_charges.filter(project_id=invoice.project_details.project_id).order_by("date")
-        return [self.item_from_custom_charge(invoice, custom_charge) for custom_charge in custom_charges]
-
-    def item_from_usage_event(self, invoice: Invoice, usage_event: UsageEvent) -> InvoiceDetailItem:
-        duration = get_minutes_between_dates(usage_event.start, usage_event.end)
-        item = InvoiceDetailItem(start=usage_event.start, end=usage_event.end, quantity=duration)
-        item.item_type = InvoiceDetailItem.InvoiceDetailItemType.TOOL_USAGE
-        item.name = usage_event.tool.name
-        item.user = usage_event.user.username
-        item.core_facility = usage_event.tool.core_facility
-        rate: Rate = get_rate(RateType.Type.TOOL_USAGE, invoice.project_details, tool=usage_event.tool)
-        item.amount = rate.calculate_amount(item.quantity)
-        item.rate = get_rate_with_currency(invoice, rate.display_rate())
-        return item
-
-    def item_from_area_access_record(self, invoice: Invoice, area_access_record: AreaAccessRecord):
-        duration = get_minutes_between_dates(area_access_record.start, area_access_record.end)
-        item = InvoiceDetailItem(start=area_access_record.start, end=area_access_record.end, quantity=duration)
-        item.item_type = InvoiceDetailItem.InvoiceDetailItemType.AREA_ACCESS
-        item.name = area_access_record.area.name
-        item.user = area_access_record.customer.username
-        item.core_facility = area_access_record.area.core_facility
-        rate: Rate = get_rate(RateType.Type.AREA_USAGE, invoice.project_details, area=area_access_record.area)
-        item.amount = rate.calculate_amount(item.quantity)
-        item.rate = get_rate_with_currency(invoice, rate.display_rate())
-        return item
-
-    def item_from_missed_reservation(self, invoice: Invoice, missed_reservation: Reservation) -> InvoiceDetailItem:
-        item = InvoiceDetailItem(start=missed_reservation.start, end=missed_reservation.end, quantity=1)
-        item.item_type = InvoiceDetailItem.InvoiceDetailItemType.MISSED_RESERVATION
-        item.user = missed_reservation.user.username
-        if missed_reservation.tool:
-            item.core_facility = missed_reservation.tool.core_facility
-            item.name = f"{missed_reservation.tool.name}"
-            rate = get_rate(
-                RateType.Type.TOOL_MISSED_RESERVATION, invoice.project_details, tool=missed_reservation.tool
+# Class to hold information about the discounts for an account, split by projects/users/core facilities
+class AccountDiscountCalculator:
+    def __init__(self, start_date: date):
+        self.start_date = start_date
+        # We are creating a dict of rate_category -> facility_name -> usernames -> cap discount objects
+        self.cap_discounts: Dict[str, Dict[str, Dict[str, CAPDiscount]]] = {}
+
+    def add_item(self, item: InvoiceDetailItem):
+        # This assumes we are getting the items in order of end date first, so we can add up amounts
+        project = item.invoice.project_details.project
+        cap_discount = self.get_or_create_cap(project, item)
+        if cap_discount and item_cap_discount_match(item, cap_discount):
+            if cap_discount.tmp_current_amount + item.amount > cap_discount.amount:
+                # apply discount to appropriate project
+                prj_id = item.invoice.project_details.project.id
+                project_discount = cap_discount.tmp_project_discounts.get(prj_id, Decimal(0))
+                # item - max (cap - current, 0) => item when current > cap otherwise item - (cap - current)
+                amount_for_discount = item.amount - max(cap_discount.amount-cap_discount.tmp_current_amount, Decimal(0))
+                # set the discount on the item and in the project total
+                item.discount = amount_for_discount * cap_discount.discount_amount()
+                cap_discount.tmp_project_discounts[prj_id] = project_discount + item.discount
+            cap_discount.tmp_current_amount += item.amount
+
+    def get_or_create_cap(self, project: Project, item: InvoiceDetailItem) -> Optional[CAPDiscount]:
+        core_facility = item.core_facility
+        username = item.user
+        rate_category = project.projectbillingdetails.category
+        rate_category_dict: Dict[str, Dict[str, CAPDiscount]] = self.cap_discounts.setdefault(rate_category.name, {})
+        facility_dict: Dict[str, CAPDiscount] = rate_category_dict.setdefault(core_facility, {})
+        try:
+            config = CAPDiscountConfiguration.objects.get(
+                rate_category=rate_category, core_facility__name=core_facility
             )
-            item.amount = rate.calculate_amount(item.quantity)
-            item.rate = get_rate_with_currency(invoice, rate.display_rate())
-        if missed_reservation.area:
-            item.core_facility = missed_reservation.area.core_facility
-            item.name = f"{missed_reservation.area.name}"
-            rate = get_rate(
-                RateType.Type.AREA_MISSED_RESERVATION, invoice.project_details, area=missed_reservation.area
+            username = username if config.split_by_user else None
+            if username in facility_dict:
+                return facility_dict.get(username)
+            # Only create if it is an eligible charge
+            elif item_cap_discount_match(item, config):
+                cap_discount: CAPDiscount = config.get_or_create_cap_discount(
+                    account=project.account, username=username, start=self.start_date
+                )
+                # Set tmp current amount
+                cap_discount.tmp_current_amount = CAPDiscountAmount.objects.get(
+                    cap_discount=cap_discount, month=self.start_date.month, year=self.start_date.year
+                ).start
+                return facility_dict.setdefault(username, cap_discount)
+        except CAPDiscountConfiguration.DoesNotExist:
+            processors_logger.debug(
+                f"No CAP configuration found for rate: {rate_category} and core facility: {core_facility}"
             )
-            item.amount = rate.calculate_amount(item.quantity)
-            item.rate = get_rate_with_currency(invoice, rate.display_rate())
-        return item
-
-    def item_from_staff_charge(self, invoice: Invoice, staff_charge: StaffCharge) -> InvoiceDetailItem:
-        duration = get_minutes_between_dates(staff_charge.start, staff_charge.end)
-        item = InvoiceDetailItem(start=staff_charge.start, end=staff_charge.end, quantity=duration)
-        item.item_type = InvoiceDetailItem.InvoiceDetailItemType.STAFF_CHARGE
-        item.name = "Staff time"
-        item.user = staff_charge.customer.username
-        rate = get_rate(RateType.Type.STAFF_CHARGE, invoice.project_details)
-        item.amount = rate.calculate_amount(item.quantity)
-        item.rate = get_rate_with_currency(invoice, rate.display_rate())
-        item.core_facility = staff_charge.core_facility
-        # If there is no core facility set on the staff charge itself, try to guess it
-        if not item.core_facility:
-            # We first check if there was an area access, in which case we will use the area's facility
-            area_charge: AreaAccessRecord = AreaAccessRecord.objects.filter(staff_charge_id=staff_charge.id).first()
-            if area_charge:
-                item.core_facility = area_charge.area.core_facility
-            else:
-                # Otherwise, check for tool usage on behalf of the same customer during the time
-                tool_usage: UsageEvent = UsageEvent.objects.filter(
-                    operator=staff_charge.staff_member, user=staff_charge.customer, start__gt=staff_charge.start
-                ).first()
-                if tool_usage:
-                    item.core_facility = tool_usage.tool.core_facility
-        return item
-
-    def item_from_consumable_withdrawal(self, invoice: Invoice, withdrawal: ConsumableWithdraw) -> InvoiceDetailItem:
-        item = InvoiceDetailItem(start=withdrawal.date, end=withdrawal.date, quantity=withdrawal.quantity)
-        item.item_type = InvoiceDetailItem.InvoiceDetailItemType.CONSUMABLE
-        item.core_facility = withdrawal.consumable.core_facility
-        item.name = withdrawal.consumable.name
-        item.user = withdrawal.customer.username
-        rate = get_rate(RateType.Type.CONSUMABLE, invoice.project_details, consumable=withdrawal.consumable)
-        item.amount = rate.calculate_amount(item.quantity)
-        item.rate = get_rate_with_currency(invoice, rate.display_rate())
-        return item
-
-    def item_from_training(self, invoice: Invoice, training: TrainingSession) -> InvoiceDetailItem:
-        item = InvoiceDetailItem(start=training.date, end=training.date, quantity=training.duration)
-        item.item_type = InvoiceDetailItem.InvoiceDetailItemType.TRAINING
-        item.core_facility = training.tool.core_facility
-        item.name = f"{training.tool.name} ({training.get_type_display()})"
-        item.user = training.trainee.username
-        if training.type == TrainingSession.Type.INDIVIDUAL:
-            rate = get_rate(RateType.Type.TOOL_TRAINING_INDIVIDUAL, invoice.project_details, tool=training.tool)
+
+    def get_discounts_for_project(self, rate_category: RateCategory, core_facility: str) -> List[CAPDiscount]:
+        # Returns the facility discounts for each user
+        return list(self.cap_discounts.get(rate_category.name, {}).get(core_facility, {}).values())
+
+    def all_cap_discounts(self) -> List[CAPDiscount]:
+        return [
+            value
+            for rate_category_dict in self.cap_discounts.values()
+            for facility_dict in rate_category_dict.values()
+            for value in facility_dict.values()
+            if rate_category_dict and facility_dict
+        ]
+
+
+class CAPDiscountInvoiceDataProcessor(InvoiceDataProcessor):
+    def generate_invoice_for_project(self, month, project, configuration, user, raise_if_exists=False) -> Invoice:
+        raise AttributeError("Generating invoices for projects is not supported. Select an account or 'All' instead")
+
+    # Do all this in a transaction so everything gets rolled back if an error happened
+    @transaction.atomic
+    def generate_invoice_for_account(self, month, account, configuration, user, raise_if_exists=False) -> List[Invoice]:
+        # Overriding this, so we can deal with discounts and save all invoices at the end
+        start, end = get_month_timeframe(month)
+        # First let's check that cap discounts have been correctly generated until now
+        # And initialize new amounts for this month
+        check_and_initialize_monthly_cap_amounts(account, start)
+
+        # Now create our cap calculator helper
+        discount_calculator = AccountDiscountCalculator(start.date())
+
+        # Go through the generation process, and add all items to account details list
+        all_account_details: List[InvoiceDetailItem] = []
+        invoices: List[FullInvoice] = []
+        for project in account.project_set.all():
+            invoice = self.generate_invoice(start, end, project, configuration, user, raise_if_exists)
+            if invoice:
+                invoices.append(invoice)
+                all_account_details.extend(invoice.detail_items)
+
+        if all_account_details:
+            # Sort account details by end date. This is very IMPORTANT to get discounts right
+            all_account_details.sort(key=lambda x: x.end)
+            # Go through all account charges to figure out the discounts
+            for detail in all_account_details:
+                discount_calculator.add_item(detail)
+            # Now let's update the CAP entities with the total charges for this account
+            for cap_discount in discount_calculator.all_cap_discounts():
+                amount = CAPDiscountAmount.objects.get(cap_discount=cap_discount, year=start.year, month=start.month)
+                amount.end = cap_discount.tmp_current_amount
+                amount.save(update_fields=["end"])
+
+        # Save all the invoices now
+        self.save_invoices(invoices, discount_calculator)
+        return [full_invoice.invoice for full_invoice in invoices]
+
+    def save_invoices(self, full_invoices: List[FullInvoice], discount_calculator: AccountDiscountCalculator = None):
+        for full_invoice in full_invoices:
+            # Pass calculator through the invoice, so we can retrieve it later
+            full_invoice.invoice.discount_calculator = discount_calculator
+            # Recalculate summaries with the discounts
+            full_invoice.summary_items = self.get_invoice_summary_items(full_invoice.invoice, full_invoice.detail_items)
+            full_invoice.save()
+
+    # Override this method, to check if we need to deal with discounts or not
+    def get_summary_items_for_facility(self, invoice: Invoice, core_facility: str, details) -> List[InvoiceSummaryItem]:
+        cap_discounts = []
+
+        calc: AccountDiscountCalculator = getattr(invoice, "discount_calculator", None)
+        if calc:
+            rate_category = invoice.project_details.category
+            cap_discounts: List[CAPDiscount] = calc.get_discounts_for_project(rate_category, core_facility)
+
+        if not cap_discounts:
+            # If we don't have any discounts, return original function
+            return super().get_summary_items_for_facility(invoice, core_facility, details)
         else:
-            rate = get_rate(RateType.Type.TOOL_TRAINING_GROUP, invoice.project_details, tool=training.tool)
-        item.amount = rate.calculate_amount(item.quantity)
-        item.rate = get_rate_with_currency(invoice, rate.display_rate())
-        return item
-
-    def item_from_custom_charge(self, invoice, custom_charge) -> InvoiceDetailItem:
-        item = InvoiceDetailItem(start=custom_charge.date, end=custom_charge.date, quantity=1)
-        item.item_type = InvoiceDetailItem.InvoiceDetailItemType.CUSTOM_CHARGE
-        item.core_facility = custom_charge.core_facility
-        item.name = custom_charge.name
-        item.user = custom_charge.customer.username
-        item.amount = custom_charge.amount
-        return item
-
-    def add_invoice_summary_items(self, invoice):
-        # Core facilities sorted alphabetically by non empty ones first
-        for core_facility in invoice.sorted_core_facilities():
-            self._add_summary_items_for_facility(invoice, core_facility)
-
-        # Recap of all charges
-        charges_amount = invoice.invoicesummaryitem_set.filter(
-            summary_item_type=InvoiceSummaryItem.InvoiceSummaryItemType.SUBTOTAL
-        ).aggregate(Sum("amount"))["amount__sum"]
-
-        # Tax
-        tax_amount = Decimal(0)
-        if invoice.configuration.tax and charges_amount > Decimal(0) and not invoice.project_details.no_tax:
-            tax = InvoiceSummaryItem(
-                invoice=invoice, name=f"{invoice.configuration.tax_name} ({invoice.configuration.tax_display()}%)"
-            )
-            tax.summary_item_type = InvoiceSummaryItem.InvoiceSummaryItemType.TAX
-            tax_amount = charges_amount * invoice.configuration.tax_amount()
-            tax.amount = tax_amount
-            tax.save(force_insert=True)
-
-        invoice.total_amount = charges_amount + tax_amount
-        invoice.save(update_fields=["total_amount"])
-
-    def _add_summary_items_for_facility(self, invoice: Invoice, core_facility: Optional[str]):
-        details = invoice.invoicedetailitem_set.filter(core_facility=core_facility)
-        self._add_aggregate_items_with_details(
-            invoice, core_facility, details, InvoiceDetailItem.InvoiceDetailItemType.TOOL_USAGE
-        )
-        self._add_aggregate_items_with_details(
-            invoice, core_facility, details, InvoiceDetailItem.InvoiceDetailItemType.AREA_ACCESS
-        )
-        self._add_aggregate_items_with_details(
-            invoice, core_facility, details, InvoiceDetailItem.InvoiceDetailItemType.CONSUMABLE
-        )
-        self._add_aggregate_items_with_details(
-            invoice, core_facility, details, InvoiceDetailItem.InvoiceDetailItemType.STAFF_CHARGE
-        )
-        self._add_aggregate_items_with_details(
-            invoice, core_facility, details, InvoiceDetailItem.InvoiceDetailItemType.TRAINING
-        )
-        self._add_aggregate_items_with_details(
-            invoice, core_facility, details, InvoiceDetailItem.InvoiceDetailItemType.MISSED_RESERVATION
-        )
-        self._add_aggregate_items_with_details(
-            invoice, core_facility, details, InvoiceDetailItem.InvoiceDetailItemType.CUSTOM_CHARGE
-        )
+            # Otherwise re-generate summary items with discounts
+            return self.get_summary_items_for_facility_with_discounts(invoice, core_facility, details, cap_discounts)
+
+    # This is our new version with the discount calculation
+    def get_summary_items_for_facility_with_discounts(
+        self, invoice: Invoice, core_facility: str, details, cap_discounts: List[CAPDiscount]
+    ) -> List[InvoiceSummaryItem]:
+        # Re-generate summary items
+        facility_summaries: List[InvoiceSummaryItem] = []
+        for billable_type in BillableItemType:
+            items = [item for item in details if item.item_type == billable_type.value]
+            facility_summaries.extend(self.get_recap_usage_summary(invoice, core_facility, items))
+
+        total_discount = Decimal(0)
+        for cap_discount in cap_discounts:
+            discount_amt = cap_discount.tmp_project_discounts.get(invoice.project_details.project.id)
+            if discount_amt and discount_amt != 0:
+                discount_name = f"{cap_discount.configuration.rate_category.name}{'/' + cap_discount.user.username if cap_discount.user else ''} CAP Discount"
+                f_discount = InvoiceSummaryItem(invoice=invoice, name=discount_name, core_facility=core_facility)
+                f_discount.summary_item_type = InvoiceSummaryItem.InvoiceSummaryItemType.DISCOUNT
+                f_discount.amount = discount_amt
+                facility_summaries.append(f_discount)
+                total_discount += discount_amt
 
         facility_subtotal = InvoiceSummaryItem(invoice=invoice, name="Subtotal", core_facility=core_facility)
         facility_subtotal.summary_item_type = InvoiceSummaryItem.InvoiceSummaryItemType.SUBTOTAL
-        facility_subtotal.amount = details.aggregate(Sum("amount"))["amount__sum"]
-        facility_subtotal.save(force_insert=True)
+        facility_subtotal.amount = sum(item.amount for item in details) + total_discount
+        facility_summaries.append(facility_subtotal)
+
+        return facility_summaries
 
-    def _add_aggregate_items_with_details(
-        self, invoice, core_facility: str, items: QuerySet, item_type: InvoiceDetailItem.InvoiceDetailItemType
-    ):
-        items = items.filter(item_type=item_type)
-        if items.exists():
-            item_names = list(items.values_list("name", flat=True).distinct())
-            item_names.sort()
-            for item_name in item_names:
-                item_name_qs = items.filter(name=item_name)
-                item_rate = item_name_qs.first().rate
-                total_q = item_name_qs.aggregate(Sum("quantity"))["quantity__sum"]
-                if InvoiceDetailItem.InvoiceDetailItemType.is_time_type(item_type):
-                    quantity_display = f" ({total_q/60:.2f} hours)"
-                elif item_type == InvoiceDetailItem.InvoiceDetailItemType.CUSTOM_CHARGE:
-                    quantity_display = ""
-                else:
-                    quantity_display = f" (x {total_q})"
-                summary_item_name = f"{item_name}{quantity_display}"
-                summary_item = InvoiceSummaryItem(invoice=invoice, name=summary_item_name, core_facility=core_facility)
-                summary_item.summary_item_type = InvoiceSummaryItem.InvoiceSummaryItemType.ITEM
-                summary_item.item_type = item_type
-                summary_item.details = item_rate
-                summary_item.amount = item_name_qs.aggregate(Sum("amount"))["amount__sum"]
-                summary_item.save(force_insert=True)
-
-    def category_name_for_item_type(self, item_type: InvoiceDetailItem.InvoiceDetailItemType):
-        if item_type == InvoiceDetailItem.InvoiceDetailItemType.TOOL_USAGE:
-            return "Tool Usage"
-        elif item_type == InvoiceDetailItem.InvoiceDetailItemType.AREA_ACCESS:
-            return "Area Access"
-        elif item_type == InvoiceDetailItem.InvoiceDetailItemType.CONSUMABLE:
-            return "Supplies/Materials"
-        elif item_type == InvoiceDetailItem.InvoiceDetailItemType.STAFF_CHARGE:
-            return "Technical Work"
-        elif item_type == InvoiceDetailItem.InvoiceDetailItemType.TRAINING:
-            return "Training"
-        elif item_type == InvoiceDetailItem.InvoiceDetailItemType.MISSED_RESERVATION:
-            return "Missed Reservations"
-        elif item_type == InvoiceDetailItem.InvoiceDetailItemType.CUSTOM_CHARGE:
-            return "Other"
+    @transaction.atomic
+    def delete_invoice(self, invoice: Invoice, request: HttpRequest):
+        # if this invoice has a CAP Discount associated with its account,
+        # delete all the other account invoices and CAP amounts for the month.
+        # This will force to re-generate all the invoices and CAP calculation.
+        invoice_account = invoice.project_details.project.account
+        invoice_year, invoice_month = invoice.start.year, invoice.start.month
+        invoices_to_delete: List[Invoice] = get_cap_related_invoices(invoice_account, invoice_year, invoice_month)
+        try:
+            delete_associated_amounts(invoice_account, invoice_year, invoice_month, request)
+        except NotLatestInvoiceException as e:
+            messages.error(request, e.msg)
+            return
+        for invoice in invoices_to_delete:
+            super().delete_invoice(invoice, request)
+
+    @transaction.atomic
+    def void_invoice(self, invoice: Invoice, request: HttpRequest):
+        invoice_account = invoice.project_details.project.account
+        invoice_year, invoice_month = invoice.start.year, invoice.start.month
+        invoices_to_void: List[Invoice] = get_cap_related_invoices(invoice_account, invoice_year, invoice_month)
+        try:
+            delete_associated_amounts(invoice_account, invoice_year, invoice_month, request)
+        except NotLatestInvoiceException as e:
+            messages.error(request, e.msg)
+            return
+        for invoice in invoices_to_void:
+            super().void_invoice(invoice, request)
+
+    def get_deleted_objects(self, invoices: Iterable[Invoice], request: HttpRequest, admin_site):
+        # gather all related objects to delete: other invoices, cap discounts, cap discount amounts
+        related_invoices = []
+        related_discounts = []
+        related_amounts = []
+        try:
+            for invoice in invoices:
+                invoice_account = invoice.project_details.project.account
+                invoice_year, invoice_month = invoice.start.year, invoice.start.month
+                related_invoices.extend(get_cap_related_invoices(invoice_account, invoice_year, invoice_month))
+                related_amounts.extend(get_amounts_to_delete(invoice_account, invoice_year, invoice_month))
+        except NotLatestInvoiceException as e:
+            return [], {}, set(), [e.msg]
+        invoice_deleted_objects = get_deleted_objects(related_invoices, request, admin_site)
+        # We might need to also delete some CAPDiscounts if the amount was the first
+        for cap_amount in related_amounts:
+            if cap_amount.cap_discount.earliest_amount() == cap_amount:
+                related_discounts.append(cap_amount.cap_discount)
+                related_amounts.remove(cap_amount)
+        amount_deleted_objects = get_deleted_objects(related_amounts, request, admin_site)
+        discount_deleted_objects = get_deleted_objects(related_discounts, request, admin_site)
+        return (
+            invoice_deleted_objects[0] + amount_deleted_objects[0] + discount_deleted_objects[0],
+            {**invoice_deleted_objects[1], **amount_deleted_objects[1], **discount_deleted_objects[1]},
+            invoice_deleted_objects[2],
+            invoice_deleted_objects[2],
+        )
+
+    def estimated_charges_since_last_update(self, cap_discount: CAPDiscount) -> Decimal:
+        latest_amount = cap_discount.latest_amount()
+        start_since_update = (
+            latest_amount.amount_date + relativedelta(months=1)
+            if latest_amount
+            else date(timezone.now().year, timezone.now().month, 1)
+        )
+        customer_filter = Q(project__account=cap_discount.account)
+        user_filter = Q(project__account=cap_discount.account)
+        trainee_filter = Q(project__account=cap_discount.account)
+        if cap_discount.user:
+            customer_filter = customer_filter & Q(customer=cap_discount.user)
+            user_filter = user_filter & Q(user=cap_discount.user)
+            trainee_filter = trainee_filter & Q(trainee=cap_discount.user)
+        config = InvoiceConfiguration.first_or_default()
+        items = self.get_billable_items(
+            datetime.combine(start_since_update, time()),
+            timezone.now(),
+            config,
+            customer_filter,
+            user_filter,
+            trainee_filter,
+            raise_no_rate=False,
+        )
+        detail_items: List[InvoiceDetailItem] = []
+        for item in items:
+            # exceptional case here where we need to create a "fake" invoice,
+            # so we can match items correctly
+            invoice = Invoice()
+            invoice.project_details = item.project.projectbillingdetails
+            detail_items.append(billable_to_invoice_detail_item(item, invoice=invoice))
+        return sum(item.amount for item in detail_items if item_cap_discount_match(item, cap_discount))
+
+
+def item_cap_discount_match(item: InvoiceDetailItem, cap: Union[CAPDiscount, CAPDiscountConfiguration]):
+    # function to check eligible/matching items for CAPDiscount or CAPDiscountConfiguration
+    configuration = cap
+    cap_match = True
+    if isinstance(cap, CAPDiscount):
+        cap_match = item.invoice.project_details.project.account == cap.account
+        if cap.configuration.split_by_user:
+            cap_match = cap_match and item.user == cap.user.username
+        configuration = cap.configuration
+
+    configuration_core_facility = configuration.core_facility.name if configuration.core_facility else None
+    item_type = BillableItemType(item.item_type)
+
+    # Check if tool is not excluded from CAP
+    tool_excluded = False
+    excluded_tool_ids = CAPDiscountCustomization.get_excluded_tool_ids()
+    if excluded_tool_ids:
+        if item_type in [BillableItemType.TOOL_USAGE, BillableItemType.MISSED_RESERVATION, BillableItemType.TRAINING]:
+            if item.content_object and item.content_object.tool:
+                tool_excluded = item.content_object.tool.id in excluded_tool_ids
+    if item_type == BillableItemType.STAFF_CHARGE:
+        # TODO: not sure here how to figure out if the tool is excluded since it's not set on the item
+        pass
+
+    # Only include cap eligible Custom Charges
+    custom_charge_included = True
+    if item_type == BillableItemType.CUSTOM_CHARGE:
+        custom_charge_included = item.content_object and item.content_object.cap_eligible
+
+    return (
+        item_type in cap.billable_charge_types
+        and not tool_excluded
+        and custom_charge_included
+        and item.invoice.project_details.category == configuration.rate_category
+        and item.core_facility == configuration_core_facility
+        and cap_match
+    )
+
+
+def check_and_initialize_monthly_cap_amounts(account: Account, start: date):
+    # Check that current discount amounts for the account have a previous value, otherwise raise an exception
+    caps = CAPDiscount.objects.filter(account=account).values_list("id", flat=True)
+    previous_month = start - relativedelta(months=1)
+    prev_cap_amounts = CAPDiscountAmount.objects.filter(
+        cap_discount__in=caps, year=previous_month.year, month=previous_month.month
+    )
+    if prev_cap_amounts.count() != caps.count():
+        raise MissingCAPAmountException(previous_month, account)
+
+    # Initialize all discounts for this account
+    for prev_cap_amount in prev_cap_amounts:
+        initialize_cap_discount_amount(prev_cap_amount, start)
+
+
+def initialize_cap_discount_amount(previous_amount: CAPDiscountAmount, start_date: date):
+    cap_discount = previous_amount.cap_discount
+    # Check if we need to reset the CAP
+    start_for_rec = datetime(year=start_date.year, month=start_date.month, day=start_date.day)
+    cap_reset = cap_discount.next_reset_date_after(start_date, inc=True)
+    amount = Decimal(0)
+    if start_for_rec == cap_reset:
+        cap_discount.reset()
+    # Only check previous amount if it's not a reset. Otherwise, it won't start over at 0
+    elif previous_amount:
+        amount = previous_amount.end
+    discount_amount, created = CAPDiscountAmount.objects.get_or_create(
+        cap_discount=cap_discount,
+        year=start_date.year,
+        month=start_date.month,
+        defaults={"start": amount, "end": amount},
+    )
+    cap_discount.tmp_current_amount = discount_amount.start
+
+
+def get_cap_related_invoices(account: Account, year, month) -> List[Invoice]:
+    return Invoice.objects.filter(start__year=year, start__month=month, project_details__project__account=account)
+
+
+def get_amounts_to_delete(account: Account, year, month) -> List[CAPDiscountAmount]:
+    cap_amounts_to_delete: List[CAPDiscountAmount] = []
+    # check to make sure they are all the latest invoices/amounts
+    for cap_discount in CAPDiscount.objects.filter(account=account):
+        latest_amount = cap_discount.latest_amount()
+        if not latest_amount or not latest_amount.year == year or not latest_amount.month == month:
+            msg = "You can only void/delete the latest invoices when a CAP is associated with it."
+            raise NotLatestInvoiceException(msg)
+        cap_amounts_to_delete.append(latest_amount)
+    return cap_amounts_to_delete
+
+
+def delete_associated_amounts(account: Account, year, month, request):
+    # delete associated CAP amounts for the year/month
+    for cap_amount in get_amounts_to_delete(account, year, month):
+        # If the amount was the first one, then delete the whole CAP discount
+        if cap_amount.cap_discount.earliest_amount() == cap_amount:
+            cap_amount.cap_discount.delete()
+            messages.success(request, f"{cap_amount.cap_discount} was successfully deleted.", "data-speed=30000")
+        else:
+            cap_amount.delete()
+            messages.success(request, f"{cap_amount} was successfully deleted.", "data-speed=30000")
```

## Comparing `NEMO_billing/invoices/invoice_generator.py` & `NEMO_billing/invoices/renderers.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,105 +1,86 @@
 import importlib
-import io
 from abc import ABC, abstractmethod
 from decimal import Decimal
-from typing import Optional, Tuple, List, Any
+from io import BytesIO, IOBase
+from typing import Any, List, Tuple
 
-from NEMO.models import User, Project
-from NEMO.utilities import get_month_timeframe
-from NEMO.views.customization import get_customization
+from NEMO.exceptions import InvalidCustomizationException
+from NEMO.utilities import BasicDisplayTable
+from NEMO.views.customization import ApplicationCustomization, ProjectsAccountsCustomization
 from django.conf import settings
-from django.core.files.base import ContentFile
 from django.db.models import Sum
 from django.utils import timezone
 
-from NEMO_billing.invoices.exceptions import NoProjectDetailsSetException, InvoiceAlreadyExistException
-from NEMO_billing.invoices.invoice_data_processor import InvoiceDataProcessor
-from NEMO_billing.invoices.models import Invoice, ProjectBillingDetails, InvoiceDetailItem, InvoiceSummaryItem
+from NEMO_billing.invoices.exceptions import (
+    InvoiceGenerationException,
+)
+from NEMO_billing.invoices.models import (
+    BillableItemType,
+    Invoice,
+    InvoiceDetailItem,
+    InvoiceSummaryItem,
+)
 from NEMO_billing.invoices.pdf_utilities import (
+    HEADING_FONT,
+    HEADING_FONT_CENTERED,
     InvoicePDFDocument,
     PDFPageSize,
     SMALL_FONT,
     SMALL_FONT_RIGHT,
-    HEADING_FONT,
-    HEADING_FONT_CENTERED,
 )
-from NEMO_billing.invoices.utilities import display_amount
-
-
-def generate_monthly_invoice(month, project, configuration, user: User, raise_if_exists=False) -> Optional[Invoice]:
-    start, end = get_month_timeframe(month)
-    return generate_invoice(start, end, project, configuration, user, raise_if_exists)
-
-
-def generate_invoice(start, end, project: Project, configuration, user, raise_if_exists=False) -> Optional[Invoice]:
-    # Start and end will be included in the results. So for example for September data, use: 09/01 to 09/30
-    try:
-        project_details = ProjectBillingDetails.objects.get(project_id=project.id)
-    except ProjectBillingDetails.DoesNotExist:
-        raise NoProjectDetailsSetException(project=project)
-    # If there is already a invoice for this project for those dates, don't regenerate it (unless void).
-    existing_invoices = Invoice.objects.filter(start=start, end=end, project_details=project_details, voided_date=None)
-    if existing_invoices.exists():
-        if raise_if_exists:
-            raise InvoiceAlreadyExistException(existing_invoices.first())
-    # No existing invoices, continue
-    elif not project_details.no_charge:
-        data_processor = invoice_generator_class.get_invoice_data_processor()
-        invoice = data_processor.process_data(start, end, project_details, configuration, user)
-        if invoice:
-            invoice_generator_class.render_invoice(invoice)
-            return invoice
+from NEMO_billing.invoices.utilities import category_name_for_item_type, display_amount
 
 
-class InvoiceGenerator(ABC):
+class InvoiceRenderer(ABC):
     def __init__(self):
         self.date_time_format = settings.INVOICE_DATETIME_FORMAT
         self.date_format = settings.INVOICE_DATE_FORMAT
 
-    def render_invoice(self, invoice: Invoice):
-        file_bytes = io.BytesIO()
-        document = self.init_document(invoice, file_bytes)
-        self.render_front_page(invoice, document)
-        self.render_summary(invoice, document)
-        if invoice.configuration.detailed_invoice:
-            self.render_details(invoice, document)
-        self.close_document(invoice, document, file_bytes)
-
-    def get_invoice_data_processor(self):
-        return InvoiceDataProcessor()
+    def render_invoice(self, invoice: Invoice) -> IOBase:
+        try:
+            file_bytes = BytesIO()
+            document = self.init_document(invoice, file_bytes)
+            self.render_front_page(invoice, document)
+            self.render_summary(invoice, document)
+            if invoice.configuration.detailed_invoice:
+                self.render_details(invoice, document)
+            return self.close_document(invoice, document, file_bytes)
+        except Exception as e:
+            raise InvoiceGenerationException(invoice, self, e)
 
     @abstractmethod
     def get_file_extension(self):
         pass
 
     @abstractmethod
-    def init_document(self, invoice: Invoice, file_bytes) -> Any:
+    def init_document(self, invoice: Invoice, file_bytes: IOBase) -> Any:
         pass
 
     @abstractmethod
     def render_front_page(self, invoice: Invoice, document):
         pass
 
     @abstractmethod
     def render_summary(self, invoice: Invoice, document):
         pass
 
     @abstractmethod
     def render_details(self, invoice: Invoice, document):
         pass
 
-    def close_document(self, invoice: Invoice, document, file_bytes):
-        file_bytes.seek(0)
-        invoice.file = ContentFile(file_bytes.read(), "invoice." + self.get_file_extension())
-        file_bytes.close()
-        invoice.save(update_fields=["file"])
+    def close_document(self, invoice: Invoice, document, file_bytes: IOBase) -> IOBase:
+        return file_bytes
+
+    def format_date_time(self, datetime, date_only: bool = False):
+        tz_datetime = datetime.astimezone(timezone.get_current_timezone())
+        return tz_datetime.strftime(self.date_format) if date_only else tz_datetime.strftime(self.date_time_format)
 
 
-class PDFInvoiceGenerator(InvoiceGenerator):
+class PDFInvoiceRenderer(InvoiceRenderer):
     def get_file_extension(self):
         return "pdf"
 
     def init_document(self, invoice: Invoice, file_bytes) -> InvoicePDFDocument:
         pdf = InvoicePDFDocument(
             buffer_bytes=file_bytes,
             pagesize=PDFPageSize.Letter,
@@ -121,157 +102,138 @@
         pdf.add_title("Invoice")
         key_value_col_width = [65, None]
         pdf.add_space(1, 30)
         details_data = [
             ("Date:", self.format_date_time(invoice.created_date, date_only=True)),
             ("Invoice:", invoice.invoice_number),
             ("Project:", invoice.project_details.name),
-            ("Ref/PO:", invoice.project_details.project.application_identifier),
+            (ProjectsAccountsCustomization.get("project_application_identifier_name")+":", invoice.project_details.project.application_identifier),
         ]
         pdf.add_table_key_value(details_data, key_value_col_width, details_key_style, default_style)
         pdf.add_space(1, 15)
-        pdf.add_table_key_value(
-            [("To:", invoice.project_details.addressee)], key_value_col_width, details_key_style, default_style
-        )
+        if invoice.project_details.addressee:
+            pdf.add_table_key_value(
+                [("To:", invoice.project_details.addressee)], key_value_col_width, details_key_style, default_style
+            )
         pdf.add_space(1, 50)
-        facility = get_customization("facility_name")
+        facility = ApplicationCustomization.get("facility_name")
         pdf.add_heading_paragraph(
             f"{facility} charges for {invoice.start.strftime(self.date_format)} to {invoice.end.strftime(self.date_format)}",
             heading_style_centered,
             fit=True,
             border=True,
         )
         pdf.add_space(1, 15)
         pdf.add_paragraph(
-            f"Total {facility} charges: <b>{display_amount(invoice.total_amount, invoice.configuration)}</b>",
-            style=total_charges_style,
+            f"Total {facility} charges: <b>{invoice.total_amount_display()}</b>", style=total_charges_style
         )
         pdf.add_space(1, 5)
         pdf.add_paragraph(f"Please refer to attached summary for details.", default_italic_style)
         if invoice.configuration.terms:
             pdf.add_space(1, 70)
             pdf.add_heading_paragraph("Terms and Conditions:", heading_style)
             pdf.add_paragraph(invoice.configuration.terms, default_style)
 
     def render_summary(self, invoice: Invoice, pdf: InvoicePDFDocument):
         header_name_style = pdf.styles[f"{SMALL_FONT}Bold10"]
         header_amount_style = pdf.styles[f"{SMALL_FONT_RIGHT}Bold10"]
         category_name_style = pdf.styles[f"{SMALL_FONT}Bold12"]
         category_amount_style = pdf.styles[f"{SMALL_FONT_RIGHT}Base12"]
-        discount_name_style = pdf.styles[f"{SMALL_FONT}Bold13"]
-        discount_amount_style = pdf.styles[f"{SMALL_FONT_RIGHT}Base13"]
         item_amount_style = pdf.styles[f"{SMALL_FONT_RIGHT}Base10"]
         other_name_style = pdf.styles[f"{SMALL_FONT}Bold10"]
         total_amount_style = pdf.styles[f"{SMALL_FONT_RIGHT}Bold12"]
         pdf.add_page_break()
         pdf.add_title("Summary")
         table_data = []
         # Separate type based on invoice configuration options
-        separate_item_types = []
-        facility_item_types = []
+        separate_item_types: List[BillableItemType] = []
+        facility_item_types: List[BillableItemType] = []
 
         if invoice.configuration.separate_tool_usage_charges:
-            separate_item_types.append(InvoiceDetailItem.InvoiceDetailItemType.TOOL_USAGE)
+            separate_item_types.append(BillableItemType.TOOL_USAGE)
         else:
-            facility_item_types.append(InvoiceDetailItem.InvoiceDetailItemType.TOOL_USAGE)
+            facility_item_types.append(BillableItemType.TOOL_USAGE)
         if invoice.configuration.separate_area_access_charges:
-            separate_item_types.append(InvoiceDetailItem.InvoiceDetailItemType.AREA_ACCESS)
+            separate_item_types.append(BillableItemType.AREA_ACCESS)
         else:
-            facility_item_types.append(InvoiceDetailItem.InvoiceDetailItemType.AREA_ACCESS)
+            facility_item_types.append(BillableItemType.AREA_ACCESS)
         if invoice.configuration.separate_consumable_charges:
-            separate_item_types.append(InvoiceDetailItem.InvoiceDetailItemType.CONSUMABLE)
+            separate_item_types.append(BillableItemType.CONSUMABLE)
         else:
-            facility_item_types.append(InvoiceDetailItem.InvoiceDetailItemType.CONSUMABLE)
+            facility_item_types.append(BillableItemType.CONSUMABLE)
         if invoice.configuration.separate_missed_reservation_charges:
-            separate_item_types.append(InvoiceDetailItem.InvoiceDetailItemType.MISSED_RESERVATION)
+            separate_item_types.append(BillableItemType.MISSED_RESERVATION)
         else:
-            facility_item_types.append(InvoiceDetailItem.InvoiceDetailItemType.MISSED_RESERVATION)
+            facility_item_types.append(BillableItemType.MISSED_RESERVATION)
         if invoice.configuration.separate_staff_charges:
-            separate_item_types.append(InvoiceDetailItem.InvoiceDetailItemType.STAFF_CHARGE)
+            separate_item_types.append(BillableItemType.STAFF_CHARGE)
         else:
-            facility_item_types.append(InvoiceDetailItem.InvoiceDetailItemType.STAFF_CHARGE)
+            facility_item_types.append(BillableItemType.STAFF_CHARGE)
         if invoice.configuration.separate_training_charges:
-            separate_item_types.append(InvoiceDetailItem.InvoiceDetailItemType.TRAINING)
+            separate_item_types.append(BillableItemType.TRAINING)
         else:
-            facility_item_types.append(InvoiceDetailItem.InvoiceDetailItemType.TRAINING)
+            facility_item_types.append(BillableItemType.TRAINING)
         if invoice.configuration.separate_custom_charges:
-            separate_item_types.append(InvoiceDetailItem.InvoiceDetailItemType.CUSTOM_CHARGE)
+            separate_item_types.append(BillableItemType.CUSTOM_CHARGE)
         else:
-            facility_item_types.append(InvoiceDetailItem.InvoiceDetailItemType.CUSTOM_CHARGE)
+            facility_item_types.append(BillableItemType.CUSTOM_CHARGE)
 
         # Deal first with non-empty core facilities
         for core_facility in invoice.sorted_core_facilities():
             if core_facility:
-                facility_summary_items = invoice.invoicesummaryitem_set.filter(core_facility=core_facility)
-                summary_items = facility_summary_items.filter(
+                facility_summaries = invoice.invoicesummaryitem_set.filter(core_facility=core_facility)
+                summary_items = facility_summaries.filter(
                     summary_item_type=InvoiceSummaryItem.InvoiceSummaryItemType.ITEM
                 )
-                facility_display_items = summary_items.filter(item_type__in=facility_item_types)
+                facility_display_items = summary_items.filter(item_type__in=[t.value for t in facility_item_types])
                 sub_total_amount = facility_display_items.aggregate(Sum("amount"))["amount__sum"]
                 # Don't show the facility if there are no items in it
                 if facility_display_items.exists():
                     table_data.append(["", "", ""])
                     table_data.append(
                         [(core_facility, category_name_style), ("", category_name_style), ("", category_amount_style)]
                     )
                     for item_type in facility_item_types:
-                        items = summary_items.filter(item_type=item_type)
+                        items = summary_items.filter(item_type=item_type.value)
                         self.add_items(invoice.configuration, table_data, items, pdf)
-                    facility_discount = facility_summary_items.filter(
-                        summary_item_type=InvoiceSummaryItem.InvoiceSummaryItemType.DISCOUNT
-                    ).first()
-                    facility_discount_amount = Decimal(0)
-                    if facility_discount:
-                        facility_discount_amount = facility_discount.amount
-                        table_data.append(
-                            [
-                                ("Discount", other_name_style),
-                                (facility_discount.details or ""),
-                                (display_amount(facility_discount_amount, invoice.configuration), item_amount_style),
-                            ]
-                        )
+                    discounts_amount = self.add_discounts(invoice.configuration, table_data, facility_summaries, pdf)
                     table_data.append(
                         [
                             ("Subtotal", other_name_style),
                             "",
                             (
-                                display_amount(sub_total_amount + facility_discount_amount, invoice.configuration),
+                                display_amount(sub_total_amount + discounts_amount, invoice.configuration),
                                 item_amount_style,
                             ),
                         ]
                     )
 
         # Add items not in any facilities (and items set as separate in configuration)
-        general_summary_items = invoice.invoicesummaryitem_set.filter(
-            core_facility=None, summary_item_type=InvoiceSummaryItem.InvoiceSummaryItemType.ITEM
+        general_summaries = invoice.invoicesummaryitem_set.filter(core_facility=None)
+        general_summary_items = general_summaries.filter(
+            summary_item_type=InvoiceSummaryItem.InvoiceSummaryItemType.ITEM
         )
         for item_type in facility_item_types + separate_item_types:
             if item_type in facility_item_types:
-                items = general_summary_items.filter(item_type=item_type)
+                items = general_summary_items.filter(item_type=item_type.value)
             else:
-                items = invoice.invoicesummaryitem_set.filter(item_type=item_type)
+                items = invoice.invoicesummaryitem_set.filter(item_type=item_type.value)
             if items.exists():
                 table_data.append(["", "", ""])
                 table_data.append(
-                    [
-                        (
-                            InvoiceDetailItem.InvoiceDetailItemType.category_name_for_item_type(item_type),
-                            category_name_style,
-                        ),
-                        "",
-                        ("", category_amount_style),
-                    ]
+                    [(category_name_for_item_type(item_type), category_name_style), "", ("", category_amount_style)]
                 )
                 self.add_items(invoice.configuration, table_data, items, pdf)
                 sub_total_amount = items.aggregate(Sum("amount"))["amount__sum"]
+                discounts_amount = self.add_discounts(invoice.configuration, table_data, general_summaries, pdf)
                 table_data.append(
                     [
                         ("Subtotal", other_name_style),
                         "",
-                        (display_amount(sub_total_amount, invoice.configuration), item_amount_style),
+                        (display_amount(sub_total_amount + discounts_amount, invoice.configuration), item_amount_style),
                     ]
                 )
 
         total_charges_amount = invoice.invoicesummaryitem_set.filter(
             summary_item_type=InvoiceSummaryItem.InvoiceSummaryItemType.SUBTOTAL
         ).aggregate(Sum("amount"))["amount__sum"]
         table_data.append(["", "", ""])
@@ -307,142 +269,281 @@
             table_data,
             headers=[("Item", header_name_style), ("Rate", header_name_style), ("Amount Due", header_amount_style)],
             col_width=summary_col_width,
             grid=False,
             border=True,
         )
 
+    def add_discounts(self, configuration, table_data, summaries_qs, pdf) -> Decimal:
+        discount_name_style = pdf.styles[f"{SMALL_FONT}Bold9"]
+        discounts_qs = summaries_qs.filter(summary_item_type=InvoiceSummaryItem.InvoiceSummaryItemType.DISCOUNT)
+        item_amount_style = pdf.styles[f"{SMALL_FONT_RIGHT}Base10"]
+        total_discounts_amount = Decimal(0)
+        for facility_discount in discounts_qs:
+            facility_discount_amount = facility_discount.amount
+            table_data.append(
+                [
+                    (facility_discount.name, discount_name_style),
+                    (facility_discount.details or ""),
+                    (display_amount(facility_discount_amount, configuration), item_amount_style),
+                ]
+            )
+            total_discounts_amount += facility_discount_amount
+        return total_discounts_amount
+
     def add_items(self, configuration, table_data, items_qs, pdf):
         item_amount_style = pdf.styles[f"{SMALL_FONT_RIGHT}Base10"]
         for item in items_qs:
             # Add prefix of category name only if we have a facility (otherwise it will be in the category with that name)
-            item_name = f"{item.category_name_for_item_type()} - {item.name}" if item.core_facility else f"{item.name}"
+            item_name = (
+                f"{category_name_for_item_type(item.item_type)} - {item.name}" if item.core_facility else f"{item.name}"
+            )
             table_data.append(
                 [item_name, item.details or "", (display_amount(item.amount, configuration), item_amount_style)]
             )
 
     def render_details(self, invoice: Invoice, pdf: InvoicePDFDocument):
         default_style = pdf.styles[f"{SMALL_FONT}Base12"]
         heading_style_centered = pdf.styles[f"{HEADING_FONT_CENTERED}Bold18"]
         pdf.add_page_break()
-        details_col_width = [None, None, 87, 87]
+        seven_col_width = [None, None, None, None, 65, 77, 50]
+        six_col_width = [None, None, None, 65, 77, 50]
+        four_col_width = [None, None, None, 50]
         for core_facility in invoice.sorted_core_facilities():
-            facility_name = core_facility if core_facility else "General Charges"
+            facility_name = core_facility or "General Charges"
             pdf.add_space(1, 20)
             pdf.add_heading_paragraph(facility_name, heading_style_centered, border=True)
             pdf.add_space(1, 20)
             tool_details = invoice.tool_usage_details(core_facility=core_facility)
             if tool_details.exists():
                 pdf.add_space(1, 10)
-                pdf.add_paragraph("Tool Usage", default_style)
+                pdf.add_paragraph(category_name_for_item_type(BillableItemType.TOOL_USAGE), default_style)
                 pdf.add_table(
-                    *self.duration_details_data(tool_details, "Tool"), col_width=details_col_width, grid=False
+                    *self.duration_details_data(tool_details, "Tool", pdf), col_width=seven_col_width, grid=False
                 )
             area_details = invoice.area_access_details(core_facility=core_facility)
             if area_details.exists():
                 pdf.add_space(1, 10)
-                pdf.add_paragraph("Area Access", default_style)
+                pdf.add_paragraph(category_name_for_item_type(BillableItemType.AREA_ACCESS), default_style)
                 pdf.add_table(
-                    *self.duration_details_data(area_details, "Area"), col_width=details_col_width, grid=False
+                    *self.duration_details_data(area_details, "Area", pdf), col_width=seven_col_width, grid=False
                 )
             staff_charges_details = invoice.staff_charge_details(core_facility=core_facility)
             if staff_charges_details.exists():
                 pdf.add_space(1, 10)
-                pdf.add_paragraph("Technical Work", default_style)
+                pdf.add_paragraph(category_name_for_item_type(BillableItemType.STAFF_CHARGE), default_style)
                 pdf.add_table(
-                    *self.duration_details_data(staff_charges_details, "Item"), col_width=details_col_width, grid=False
+                    *self.duration_details_data(staff_charges_details, "Item", pdf),
+                    col_width=seven_col_width,
+                    grid=False,
                 )
             consumable_withdrawals = invoice.consumable_withdrawal_details(core_facility=core_facility)
             if consumable_withdrawals.exists():
                 pdf.add_space(1, 10)
-                pdf.add_paragraph("Supplies/Materials", default_style)
+                pdf.add_paragraph(category_name_for_item_type(BillableItemType.CONSUMABLE), default_style)
                 pdf.add_table(
-                    *self.consumable_details_data(consumable_withdrawals, pdf), col_width=details_col_width, grid=False
+                    *self.consumable_details_data(consumable_withdrawals, pdf), col_width=six_col_width, grid=False
                 )
             training_details = invoice.training_details(core_facility=core_facility)
             if training_details.exists():
                 pdf.add_space(1, 10)
-                pdf.add_paragraph("Training", default_style)
-                pdf.add_table(
-                    *self.duration_details_data(training_details, "Tool"), col_width=details_col_width, grid=False
-                )
+                pdf.add_paragraph(category_name_for_item_type(BillableItemType.TRAINING), default_style)
+                pdf.add_table(*self.training_details_data(training_details, pdf), col_width=six_col_width, grid=False)
             missed_details = invoice.missed_reservation_details(core_facility=core_facility)
             if missed_details.exists():
                 pdf.add_space(1, 10)
-                pdf.add_paragraph("Missed Reservation", default_style)
+                pdf.add_paragraph(category_name_for_item_type(BillableItemType.MISSED_RESERVATION), default_style)
                 pdf.add_table(
-                    *self.duration_details_data(missed_details, "Reservation"), col_width=details_col_width, grid=False
+                    *self.duration_details_data(missed_details, "Reservation", pdf),
+                    col_width=seven_col_width,
+                    grid=False,
                 )
             custom_details = invoice.custom_charges_details(core_facility=core_facility)
             if custom_details.exists():
                 pdf.add_space(1, 10)
-                pdf.add_paragraph("Other Charges", default_style)
+                pdf.add_paragraph(category_name_for_item_type(BillableItemType.CUSTOM_CHARGE), default_style)
                 pdf.add_table(
-                    *self.custom_charge_details_data(custom_details, pdf), col_width=details_col_width, grid=False
+                    *self.custom_charge_details_data(custom_details, pdf), col_width=four_col_width, grid=False
                 )
 
-    def close_document(self, invoice: Invoice, pdf: InvoicePDFDocument, file_bytes):
+    def close_document(self, invoice: Invoice, pdf: InvoicePDFDocument, file_bytes: IOBase) -> IOBase:
         pdf.build()
-        super().close_document(invoice, pdf, file_bytes)
-
-    def format_date_time(self, datetime, date_only: bool = False):
-        tz_datetime = datetime.astimezone(timezone.get_current_timezone())
-        return tz_datetime.strftime(self.date_format) if date_only else tz_datetime.strftime(self.date_time_format)
+        return super().close_document(invoice, pdf, file_bytes)
 
-    def duration_details_data(self, items: List[InvoiceDetailItem], item_name: str) -> Tuple[List[List], List]:
+    def duration_details_data(self, items: List[InvoiceDetailItem], item_name: str, pdf) -> Tuple[List[List], List]:
+        last_item_style = pdf.styles[f"{SMALL_FONT_RIGHT}Base8"]
+        last_header_style = pdf.styles[f"{SMALL_FONT_RIGHT}Bold10"]
         return (
             [
                 [
                     str(item.user),
                     item.name,
                     self.format_date_time(item.start),
                     self.format_date_time(item.end),
+                    item.quantity_display(),
+                    item.rate,
+                    (item.amount_display(), last_item_style),
                 ]
                 for item in items
             ],
-            ["User", item_name, "Start Time", "End Time"],
+            ["User", item_name, "Start Time", "End Time", "Quantity", "Rate", ("Amount", last_header_style)],
         )
 
     def consumable_details_data(self, items: List[InvoiceDetailItem], pdf) -> Tuple[List[List], List]:
-        quantity_item_style = pdf.styles[f"{SMALL_FONT_RIGHT}Base8"]
-        quantity_header_style = pdf.styles[f"{SMALL_FONT_RIGHT}Bold10"]
+        last_item_style = pdf.styles[f"{SMALL_FONT_RIGHT}Base8"]
+        last_header_style = pdf.styles[f"{SMALL_FONT_RIGHT}Bold10"]
         return (
             [
                 [
                     str(item.user),
                     item.name,
                     self.format_date_time(item.start),
-                    (item.quantity_display(), quantity_item_style),
+                    item.quantity_display(),
+                    item.rate,
+                    (item.amount_display(), last_item_style),
                 ]
                 for item in items
             ],
-            ["User", "Supply", "Date", ("Quantity", quantity_header_style)],
+            ["User", "Supply", "Date", "Quantity", "Rate", ("Amount", last_header_style)],
         )
 
-    def custom_charge_details_data(self, items: List[InvoiceDetailItem], pdf) -> Tuple[List[List], List]:
-        amount_item_style = pdf.styles[f"{SMALL_FONT_RIGHT}Base8"]
-        amount_header_style = pdf.styles[f"{SMALL_FONT_RIGHT}Bold10"]
+    def training_details_data(self, items: List[InvoiceDetailItem], pdf) -> Tuple[List[List], List]:
+        last_item_style = pdf.styles[f"{SMALL_FONT_RIGHT}Base8"]
+        last_header_style = pdf.styles[f"{SMALL_FONT_RIGHT}Bold10"]
         return (
             [
                 [
                     str(item.user),
-                    item.name,
+                    "Tool",
                     self.format_date_time(item.start),
-                    (item.amount_display(), amount_item_style),
+                    item.quantity_display(),
+                    item.rate,
+                    (item.amount_display(), last_item_style),
                 ]
                 for item in items
             ],
-            ["User", "Charge", "Date", ("Amount", amount_header_style)],
+            ["User", "Tool", "Date", "Duration", "Rate", ("Amount", last_header_style)],
+        )
+
+    def custom_charge_details_data(self, items: List[InvoiceDetailItem], pdf) -> Tuple[List[List], List]:
+        last_item_style = pdf.styles[f"{SMALL_FONT_RIGHT}Base8"]
+        last_header_style = pdf.styles[f"{SMALL_FONT_RIGHT}Bold10"]
+        return (
+            [
+                [str(item.user), item.name, self.format_date_time(item.start), (item.amount_display(), last_item_style)]
+                for item in items
+            ],
+            ["User", "Charge", "Date", ("Amount", last_header_style)],
         )
 
 
-def get_invoice_generator_class() -> InvoiceGenerator:
-    rates_class = getattr(
-        settings, "INVOICE_GENERATOR_CLASS", "NEMO_billing.invoices.invoice_generator.PDFInvoiceGenerator"
-    )
-    assert isinstance(rates_class, str)
-    pkg, attr = rates_class.rsplit(".", 1)
+class CSVInvoiceRenderer(InvoiceRenderer):
+    PROJECT_ID_KEY = "application_identifier"
+    FACILITY_KEY = "facility"
+    USER_KEY = "user"
+    ITEM_TYPE_KEY = "item_type"
+    ITEM_KEY = "item"
+    START_KEY = "start"
+    END_KEY = "end"
+    QUANTITY_KEY = "quantity"
+    RATE_KEY = "rate"
+    DISCOUNT_KEY = "discount"
+    AMOUNT_KEY = "amount"
+
+    def __init__(self):
+        super().__init__()
+        self.document = BasicDisplayTable()
+
+    def get_file_extension(self):
+        return "csv"
+
+    def init_document(self, invoice: Invoice, file_bytes) -> Any:
+        self.document.add_header((self.PROJECT_ID_KEY, ProjectsAccountsCustomization.get("project_application_identifier_name")))
+        if invoice.invoicedetailitem_set.filter(core_facility__isempty=False).exists():
+            self.document.add_header((self.FACILITY_KEY, "Facility"))
+        self.document.add_header((self.USER_KEY, "User"))
+        self.document.add_header((self.ITEM_TYPE_KEY, "Item Type"))
+        self.document.add_header((self.ITEM_KEY, "Item"))
+        self.document.add_header((self.START_KEY, "Start Time"))
+        self.document.add_header((self.END_KEY, "End Time"))
+        self.document.add_header((self.QUANTITY_KEY, "Quantity"))
+        self.document.add_header((self.RATE_KEY, "Rate"))
+        self.document.add_header((self.DISCOUNT_KEY, "Discount"))
+        self.document.add_header((self.AMOUNT_KEY, "Amount"))
+        return self.document
+
+    def render_front_page(self, invoice: Invoice, document):
+        pass
+
+    def render_summary(self, invoice: Invoice, document):
+        pass
+
+    def render_details(self, invoice: Invoice, document: BasicDisplayTable):
+        for item in invoice.invoice_details().order_by("-start"):
+            self.document.add_row(
+                {
+                    self.PROJECT_ID_KEY: invoice.project_details.project.application_identifier,
+                    self.FACILITY_KEY: item.core_facility,
+                    self.USER_KEY: item.user,
+                    self.ITEM_TYPE_KEY: item.get_item_type_display(),
+                    self.ITEM_KEY: item.name,
+                    self.START_KEY: self.format_date_time(item.start),
+                    self.END_KEY: self.format_date_time(item.end),
+                    self.QUANTITY_KEY: item.quantity,
+                    self.RATE_KEY: item.rate,
+                    self.DISCOUNT_KEY: item.discount,
+                    self.AMOUNT_KEY: item.amount,
+                }
+            )
+        for discount in invoice.invoicesummaryitem_set.filter(
+            summary_item_type=InvoiceSummaryItem.InvoiceSummaryItemType.DISCOUNT
+        ):
+            self.document.add_row(
+                {
+                    self.PROJECT_ID_KEY: invoice.project_details.project.application_identifier,
+                    self.FACILITY_KEY: discount.core_facility,
+                    self.ITEM_TYPE_KEY: discount.get_item_type_display(),
+                    self.ITEM_KEY: discount.name,
+                    self.AMOUNT_KEY: discount.amount,
+                }
+            )
+        for other in invoice.invoicesummaryitem_set.filter(
+            summary_item_type=InvoiceSummaryItem.InvoiceSummaryItemType.OTHER
+        ):
+            self.document.add_row(
+                {
+                    self.PROJECT_ID_KEY: invoice.project_details.project.application_identifier,
+                    self.FACILITY_KEY: other.core_facility,
+                    self.ITEM_TYPE_KEY: other.get_item_type_display(),
+                    self.ITEM_KEY: other.name,
+                    self.AMOUNT_KEY: other.amount,
+                }
+            )
+        for tax in invoice.invoicesummaryitem_set.filter(
+            summary_item_type=InvoiceSummaryItem.InvoiceSummaryItemType.TAX
+        ):
+            self.document.add_row(
+                {
+                    self.PROJECT_ID_KEY: invoice.project_details.project.application_identifier,
+                    self.FACILITY_KEY: tax.core_facility,
+                    self.ITEM_TYPE_KEY: tax.get_item_type_display(),
+                    self.ITEM_KEY: tax.name,
+                    self.AMOUNT_KEY: tax.amount,
+                }
+            )
+        self.document.add_row({self.ITEM_KEY: "Total", self.AMOUNT_KEY: invoice.total_amount})
+
+    def close_document(self, invoice: Invoice, document: BasicDisplayTable, file_bytes: IOBase):
+        # write the bytes and let the parent class return it
+        file_bytes = BytesIO(document.to_csv().content)
+        return super().close_document(invoice, document, file_bytes)
+
+
+def get_invoice_renderer_class() -> InvoiceRenderer:
+    renderer_class = getattr(settings, "INVOICE_RENDERER_CLASS", "NEMO_billing.invoices.renderers.PDFInvoiceRenderer")
+    assert isinstance(renderer_class, str)
+    pkg, attr = renderer_class.rsplit(".", 1)
     ret = getattr(importlib.import_module(pkg), attr)
     return ret()
 
 
-invoice_generator_class = get_invoice_generator_class()
+invoice_renderer_class = get_invoice_renderer_class()
```

## Comparing `NEMO_billing-1.9.1.dist-info/LICENSE` & `NEMO_billing-2.0.0.dist-info/LICENSE`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2019 Prometheus Computing LLC
+Copyright (c) 2023 Atlantis Labs LLC
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

