# Comparing `tmp/lti-consumer-xblock-9.0.0.tar.gz` & `tmp/lti-consumer-xblock-9.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lti-consumer-xblock-9.0.0.tar", last modified: Mon Mar  6 17:07:01 2023, max compression
+gzip compressed data, was "lti-consumer-xblock-9.0.1.tar", last modified: Tue Apr 11 14:25:01 2023, max compression
```

## Comparing `lti-consumer-xblock-9.0.0.tar` & `lti-consumer-xblock-9.0.1.tar`

### file list

```diff
@@ -1,213 +1,213 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 17:07:01.256144 lti-consumer-xblock-9.0.0/
--rw-r--r--   0 runner    (1001) docker     (122)    34520 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       97 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      694 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (122)    14196 2023-03-06 17:07:01.256144 lti-consumer-xblock-9.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    13412 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 17:07:01.240144 lti-consumer-xblock-9.0.0/lti_consumer/
--rw-r--r--   0 runner    (1001) docker     (122)      152 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1317 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/admin.py
--rw-r--r--   0 runner    (1001) docker     (122)    11820 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/api.py
--rw-r--r--   0 runner    (1001) docker     (122)      672 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/apps.py
--rw-r--r--   0 runner    (1001) docker     (122)     5845 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/data.py
--rw-r--r--   0 runner    (1001) docker     (122)      134 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     1531 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/filters.py
--rw-r--r--   0 runner    (1001) docker     (122)      666 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 17:07:01.240144 lti-consumer-xblock-9.0.0/lti_consumer/lti_1p1/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/lti_1p1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14958 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/lti_1p1/consumer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 17:07:01.240144 lti-consumer-xblock-9.0.0/lti_consumer/lti_1p1/contrib/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/lti_1p1/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5551 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/lti_1p1/contrib/django.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 17:07:01.240144 lti-consumer-xblock-9.0.0/lti_consumer/lti_1p1/contrib/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/lti_1p1/contrib/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6923 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/lti_1p1/contrib/tests/test_django.py
--rw-r--r--   0 runner    (1001) docker     (122)      143 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/lti_1p1/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     5976 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/lti_1p1/oauth.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 17:07:01.240144 lti-consumer-xblock-9.0.0/lti_consumer/lti_1p1/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/lti_1p1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13817 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/lti_1p1/tests/test_consumer.py
--rw-r--r--   0 runner    (1001) docker     (122)     3674 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/lti_1p1/tests/test_oauth.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 17:07:01.240144 lti-consumer-xblock-9.0.0/lti_consumer/lti_1p3/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/lti_1p3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2256 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/lti_1p3/ags.py
--rw-r--r--   0 runner    (1001) docker     (122)     2773 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/lti_1p3/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    32216 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/lti_1p3/consumer.py
--rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/lti_1p3/deep_linking.py
--rw-r--r--   0 runner    (1001) docker     (122)     1996 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/lti_1p3/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 17:07:01.240144 lti-consumer-xblock-9.0.0/lti_consumer/lti_1p3/extensions/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/lti_1p3/extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 17:07:01.244144 lti-consumer-xblock-9.0.0/lti_consumer/lti_1p3/extensions/rest_framework/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/lti_1p3/extensions/rest_framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3499 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/lti_1p3/extensions/rest_framework/authentication.py
--rw-r--r--   0 runner    (1001) docker     (122)      388 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/lti_1p3/extensions/rest_framework/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)      554 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/lti_1p3/extensions/rest_framework/parsers.py
--rw-r--r--   0 runner    (1001) docker     (122)     3298 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/lti_1p3/extensions/rest_framework/permissions.py
--rw-r--r--   0 runner    (1001) docker     (122)     1759 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/lti_1p3/extensions/rest_framework/renderers.py
--rw-r--r--   0 runner    (1001) docker     (122)    14353 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/lti_1p3/extensions/rest_framework/serializers.py
--rw-r--r--   0 runner    (1001) docker     (122)      775 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/lti_1p3/extensions/rest_framework/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     7491 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/lti_1p3/key_handlers.py
--rw-r--r--   0 runner    (1001) docker     (122)     1101 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/lti_1p3/nprs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 17:07:01.244144 lti-consumer-xblock-9.0.0/lti_consumer/lti_1p3/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/lti_1p3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 17:07:01.244144 lti-consumer-xblock-9.0.0/lti_consumer/lti_1p3/tests/extensions/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/lti_1p3/tests/extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 17:07:01.244144 lti-consumer-xblock-9.0.0/lti_consumer/lti_1p3/tests/extensions/rest_framework/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/lti_1p3/tests/extensions/rest_framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4234 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/lti_1p3/tests/extensions/rest_framework/test_authentication.py
--rw-r--r--   0 runner    (1001) docker     (122)     9039 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/lti_1p3/tests/extensions/rest_framework/test_permissions.py
--rw-r--r--   0 runner    (1001) docker     (122)     2240 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/lti_1p3/tests/test_ags.py
--rw-r--r--   0 runner    (1001) docker     (122)    39510 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/lti_1p3/tests/test_consumer.py
--rw-r--r--   0 runner    (1001) docker     (122)     2361 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/lti_1p3/tests/test_deep_linking.py
--rw-r--r--   0 runner    (1001) docker     (122)     9305 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/lti_1p3/tests/test_key_handlers.py
--rw-r--r--   0 runner    (1001) docker     (122)     1264 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/lti_1p3/tests/test_nrps.py
--rw-r--r--   0 runner    (1001) docker     (122)      226 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/lti_1p3/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    69931 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/lti_xblock.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 17:07:01.248144 lti-consumer-xblock-9.0.0/lti_consumer/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)      940 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)     1256 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/migrations/0002_ltiagslineitem.py
--rw-r--r--   0 runner    (1001) docker     (122)     1677 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/migrations/0003_ltiagsscore.py
--rw-r--r--   0 runner    (1001) docker     (122)     1237 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/migrations/0004_keyset_mgmt_to_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     1808 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/migrations/0005_migrate_keyset_to_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     2361 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/migrations/0006_add_on_model_config_for_lti_1p1.py
--rw-r--r--   0 runner    (1001) docker     (122)     1105 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/migrations/0007_ltidlcontentitem.py
--rw-r--r--   0 runner    (1001) docker     (122)      924 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/migrations/0008_fix_uuid_backfill.py
--rw-r--r--   0 runner    (1001) docker     (122)     1403 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/migrations/0009_backfill-empty-string-config-id.py
--rw-r--r--   0 runner    (1001) docker     (122)     1298 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/migrations/0010_backfill-empty-string-lti-config.py
--rw-r--r--   0 runner    (1001) docker     (122)     2510 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/migrations/0011_courseeditltifieldsenabledflag.py
--rw-r--r--   0 runner    (1001) docker     (122)      496 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/migrations/0012_rename_courseeditltifieldsenabledflag_model.py
--rw-r--r--   0 runner    (1001) docker     (122)      669 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/migrations/0013_auto_20210712_1352.py
--rw-r--r--   0 runner    (1001) docker     (122)      821 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/migrations/0014_adds_external_id.py
--rw-r--r--   0 runner    (1001) docker     (122)     3641 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/migrations/0015_add_additional_1p3_fields.py
--rw-r--r--   0 runner    (1001) docker     (122)      521 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/migrations/0016_lticonfiguration_lti_1p3_proctoring_enabled.py
--rw-r--r--   0 runner    (1001) docker     (122)      844 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/migrations/0017_lticonfiguration_lti_1p3_redirect_uris.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    32021 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/models.py
--rw-r--r--   0 runner    (1001) docker     (122)     8078 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/outcomes.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 17:07:01.248144 lti-consumer-xblock-9.0.0/lti_consumer/plugin/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11681 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/plugin/compat.py
--rw-r--r--   0 runner    (1001) docker     (122)     2404 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/plugin/urls.py
--rw-r--r--   0 runner    (1001) docker     (122)    35136 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/plugin/views.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 17:07:01.248144 lti-consumer-xblock-9.0.0/lti_consumer/signals/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/signals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3800 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/signals/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 17:07:01.232144 lti-consumer-xblock-9.0.0/lti_consumer/static/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 17:07:01.248144 lti-consumer-xblock-9.0.0/lti_consumer/static/css/
--rw-r--r--   0 runner    (1001) docker     (122)     4091 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/static/css/student.css
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 17:07:01.248144 lti-consumer-xblock-9.0.0/lti_consumer/static/js/
--rw-r--r--   0 runner    (1001) docker     (122)    10549 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/static/js/xblock_lti_consumer.js
--rw-r--r--   0 runner    (1001) docker     (122)     6043 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/static/js/xblock_studio_view.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 17:07:01.248144 lti-consumer-xblock-9.0.0/lti_consumer/static/sass/
--rw-r--r--   0 runner    (1001) docker     (122)     4751 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/static/sass/student.scss
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 17:07:01.232144 lti-consumer-xblock-9.0.0/lti_consumer/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 17:07:01.248144 lti-consumer-xblock-9.0.0/lti_consumer/templates/html/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 17:07:01.248144 lti-consumer-xblock-9.0.0/lti_consumer/templates/html/lti-dl/
--rw-r--r--   0 runner    (1001) docker     (122)      405 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/templates/html/lti-dl/dl_response_error.html
--rw-r--r--   0 runner    (1001) docker     (122)      434 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/templates/html/lti-dl/dl_response_saved.html
--rw-r--r--   0 runner    (1001) docker     (122)     1048 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/templates/html/lti-dl/render_dl_content.html
--rw-r--r--   0 runner    (1001) docker     (122)      168 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/templates/html/lti-dl/render_html.html
--rw-r--r--   0 runner    (1001) docker     (122)      890 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/templates/html/lti-dl/render_image.html
--rw-r--r--   0 runner    (1001) docker     (122)      709 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/templates/html/lti-dl/render_link.html
--rw-r--r--   0 runner    (1001) docker     (122)      355 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/templates/html/lti-dl/render_lti_resource_link.html
--rw-r--r--   0 runner    (1001) docker     (122)      893 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/templates/html/lti_1p3_launch.html
--rw-r--r--   0 runner    (1001) docker     (122)      405 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/templates/html/lti_1p3_permission_error.html
--rw-r--r--   0 runner    (1001) docker     (122)     1435 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/templates/html/lti_1p3_studio.html
--rw-r--r--   0 runner    (1001) docker     (122)      364 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/templates/html/lti_iframe.html
--rw-r--r--   0 runner    (1001) docker     (122)     1148 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/templates/html/lti_launch.html
--rw-r--r--   0 runner    (1001) docker     (122)      429 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/templates/html/lti_launch_error.html
--rw-r--r--   0 runner    (1001) docker     (122)      445 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/templates/html/lti_proctoring_start_error.html
--rw-r--r--   0 runner    (1001) docker     (122)     3849 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/templates/html/student.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 17:07:01.248144 lti-consumer-xblock-9.0.0/lti_consumer/templates/xml/
--rw-r--r--   0 runner    (1001) docker     (122)      798 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/templates/xml/outcome_service_response.xml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 17:07:01.248144 lti-consumer-xblock-9.0.0/lti_consumer/templatetags/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      780 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/templatetags/get_dl_lti_launch_url.py
--rw-r--r--   0 runner    (1001) docker     (122)      566 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/templatetags/lti_sanitize.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 17:07:01.252144 lti-consumer-xblock-9.0.0/lti_consumer/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       56 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2807 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 17:07:01.252144 lti-consumer-xblock-9.0.0/lti_consumer/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 17:07:01.252144 lti-consumer-xblock-9.0.0/lti_consumer/tests/unit/plugin/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/tests/unit/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11288 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/tests/unit/plugin/test_proctoring.py
--rw-r--r--   0 runner    (1001) docker     (122)    25574 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/tests/unit/plugin/test_views.py
--rw-r--r--   0 runner    (1001) docker     (122)    38579 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/tests/unit/plugin/test_views_lti_ags.py
--rw-r--r--   0 runner    (1001) docker     (122)    26203 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/tests/unit/plugin/test_views_lti_deep_linking.py
--rw-r--r--   0 runner    (1001) docker     (122)    10559 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/tests/unit/plugin/test_views_lti_nrps.py
--rw-r--r--   0 runner    (1001) docker     (122)    26379 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/tests/unit/test_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     2866 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/tests/unit/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (122)    82946 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/tests/unit/test_lti_xblock.py
--rw-r--r--   0 runner    (1001) docker     (122)    24054 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/tests/unit/test_models.py
--rw-r--r--   0 runner    (1001) docker     (122)    16718 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/tests/unit/test_outcomes.py
--rw-r--r--   0 runner    (1001) docker     (122)     3573 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/tests/unit/test_signals.py
--rw-r--r--   0 runner    (1001) docker     (122)     4743 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/tests/unit/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      366 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/track.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 17:07:01.252144 lti-consumer-xblock-9.0.0/lti_consumer/translations/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 17:07:01.236144 lti-consumer-xblock-9.0.0/lti_consumer/translations/ar/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 17:07:01.252144 lti-consumer-xblock-9.0.0/lti_consumer/translations/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    10720 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/translations/ar/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    11737 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/translations/ar/LC_MESSAGES/text.po
--rw-r--r--   0 runner    (1001) docker     (122)      359 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/translations/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 17:07:01.236144 lti-consumer-xblock-9.0.0/lti_consumer/translations/en/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 17:07:01.252144 lti-consumer-xblock-9.0.0/lti_consumer/translations/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      380 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/translations/en/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    14641 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/translations/en/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 17:07:01.236144 lti-consumer-xblock-9.0.0/lti_consumer/translations/es_419/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 17:07:01.252144 lti-consumer-xblock-9.0.0/lti_consumer/translations/es_419/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     9197 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/translations/es_419/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    10322 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/translations/es_419/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 17:07:01.236144 lti-consumer-xblock-9.0.0/lti_consumer/translations/fr/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 17:07:01.252144 lti-consumer-xblock-9.0.0/lti_consumer/translations/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1404 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/translations/fr/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)     6171 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/translations/fr/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 17:07:01.236144 lti-consumer-xblock-9.0.0/lti_consumer/translations/fr_CA/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 17:07:01.252144 lti-consumer-xblock-9.0.0/lti_consumer/translations/fr_CA/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     9166 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/translations/fr_CA/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    10186 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/translations/fr_CA/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 17:07:01.236144 lti-consumer-xblock-9.0.0/lti_consumer/translations/he/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 17:07:01.252144 lti-consumer-xblock-9.0.0/lti_consumer/translations/he/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    10080 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/translations/he/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    11097 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/translations/he/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 17:07:01.236144 lti-consumer-xblock-9.0.0/lti_consumer/translations/hi/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 17:07:01.252144 lti-consumer-xblock-9.0.0/lti_consumer/translations/hi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      461 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/translations/hi/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5766 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/translations/hi/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 17:07:01.236144 lti-consumer-xblock-9.0.0/lti_consumer/translations/ja_JP/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 17:07:01.256144 lti-consumer-xblock-9.0.0/lti_consumer/translations/ja_JP/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     9838 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/translations/ja_JP/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    10907 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/translations/ja_JP/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 17:07:01.236144 lti-consumer-xblock-9.0.0/lti_consumer/translations/ko_KR/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 17:07:01.256144 lti-consumer-xblock-9.0.0/lti_consumer/translations/ko_KR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      469 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/translations/ko_KR/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5774 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/translations/ko_KR/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 17:07:01.236144 lti-consumer-xblock-9.0.0/lti_consumer/translations/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 17:07:01.256144 lti-consumer-xblock-9.0.0/lti_consumer/translations/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1349 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/translations/pt_BR/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)     6216 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/translations/pt_BR/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 17:07:01.236144 lti-consumer-xblock-9.0.0/lti_consumer/translations/pt_PT/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 17:07:01.256144 lti-consumer-xblock-9.0.0/lti_consumer/translations/pt_PT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    10221 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/translations/pt_PT/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    18852 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/translations/pt_PT/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 17:07:01.236144 lti-consumer-xblock-9.0.0/lti_consumer/translations/ru/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 17:07:01.256144 lti-consumer-xblock-9.0.0/lti_consumer/translations/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      601 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/translations/ru/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5906 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/translations/ru/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 17:07:01.236144 lti-consumer-xblock-9.0.0/lti_consumer/translations/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 17:07:01.256144 lti-consumer-xblock-9.0.0/lti_consumer/translations/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      495 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/translations/zh_CN/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5835 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/translations/zh_CN/LC_MESSAGES/text.po
--rw-r--r--   0 runner    (1001) docker     (122)    10931 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/lti_consumer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 17:07:01.256144 lti-consumer-xblock-9.0.0/lti_consumer_xblock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    14196 2023-03-06 17:07:01.000000 lti-consumer-xblock-9.0.0/lti_consumer_xblock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6826 2023-03-06 17:07:01.000000 lti-consumer-xblock-9.0.0/lti_consumer_xblock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)      106 2023-03-06 17:07:01.000000 lti-consumer-xblock-9.0.0/lti_consumer_xblock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      199 2023-03-06 17:07:01.000000 lti-consumer-xblock-9.0.0/lti_consumer_xblock.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      171 2023-03-06 17:07:01.000000 lti-consumer-xblock-9.0.0/lti_consumer_xblock.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-03-06 17:07:01.000000 lti-consumer-xblock-9.0.0/lti_consumer_xblock.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 17:07:01.256144 lti-consumer-xblock-9.0.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      325 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      493 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)      120 2023-03-06 17:07:01.256144 lti-consumer-xblock-9.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     5875 2023-03-06 17:06:57.000000 lti-consumer-xblock-9.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.502351 lti-consumer-xblock-9.0.1/
+-rw-r--r--   0 runner    (1001) docker     (122)    34520 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       97 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      694 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (122)    14196 2023-04-11 14:25:01.502351 lti-consumer-xblock-9.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    13412 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.478351 lti-consumer-xblock-9.0.1/lti_consumer/
+-rw-r--r--   0 runner    (1001) docker     (122)      152 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1317 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11820 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      672 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5845 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)      134 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1531 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)      666 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.482351 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p1/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14958 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p1/consumer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.482351 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p1/contrib/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p1/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5551 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p1/contrib/django.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.482351 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p1/contrib/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p1/contrib/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6923 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p1/contrib/tests/test_django.py
+-rw-r--r--   0 runner    (1001) docker     (122)      143 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p1/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5976 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p1/oauth.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.482351 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p1/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13817 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p1/tests/test_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3674 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p1/tests/test_oauth.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.482351 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2256 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/ags.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2773 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32216 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/deep_linking.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1996 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.482351 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/extensions/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.482351 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/extensions/rest_framework/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/extensions/rest_framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3499 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/extensions/rest_framework/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (122)      388 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/extensions/rest_framework/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)      554 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/extensions/rest_framework/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3298 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/extensions/rest_framework/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1759 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/extensions/rest_framework/renderers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14353 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/extensions/rest_framework/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      775 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/extensions/rest_framework/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7491 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/key_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1101 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/nprs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.486351 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.486351 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/tests/extensions/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/tests/extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.486351 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/tests/extensions/rest_framework/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/tests/extensions/rest_framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4234 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/tests/extensions/rest_framework/test_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9039 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/tests/extensions/rest_framework/test_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2240 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/tests/test_ags.py
+-rw-r--r--   0 runner    (1001) docker     (122)    39510 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/tests/test_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2361 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/tests/test_deep_linking.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9305 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/tests/test_key_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1264 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/tests/test_nrps.py
+-rw-r--r--   0 runner    (1001) docker     (122)      226 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    69931 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/lti_xblock.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.490351 lti-consumer-xblock-9.0.1/lti_consumer/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)      940 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1256 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/migrations/0002_ltiagslineitem.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1677 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/migrations/0003_ltiagsscore.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1237 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/migrations/0004_keyset_mgmt_to_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1808 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/migrations/0005_migrate_keyset_to_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2361 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/migrations/0006_add_on_model_config_for_lti_1p1.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1105 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/migrations/0007_ltidlcontentitem.py
+-rw-r--r--   0 runner    (1001) docker     (122)      924 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/migrations/0008_fix_uuid_backfill.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1403 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/migrations/0009_backfill-empty-string-config-id.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1298 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/migrations/0010_backfill-empty-string-lti-config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2510 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/migrations/0011_courseeditltifieldsenabledflag.py
+-rw-r--r--   0 runner    (1001) docker     (122)      496 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/migrations/0012_rename_courseeditltifieldsenabledflag_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)      669 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/migrations/0013_auto_20210712_1352.py
+-rw-r--r--   0 runner    (1001) docker     (122)      821 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/migrations/0014_adds_external_id.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3641 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/migrations/0015_add_additional_1p3_fields.py
+-rw-r--r--   0 runner    (1001) docker     (122)      521 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/migrations/0016_lticonfiguration_lti_1p3_proctoring_enabled.py
+-rw-r--r--   0 runner    (1001) docker     (122)      844 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/migrations/0017_lticonfiguration_lti_1p3_redirect_uris.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32021 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8078 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/outcomes.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.490351 lti-consumer-xblock-9.0.1/lti_consumer/plugin/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11681 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/plugin/compat.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2404 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/plugin/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35136 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/plugin/views.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.490351 lti-consumer-xblock-9.0.1/lti_consumer/signals/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/signals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3800 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/signals/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.474351 lti-consumer-xblock-9.0.1/lti_consumer/static/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.490351 lti-consumer-xblock-9.0.1/lti_consumer/static/css/
+-rw-r--r--   0 runner    (1001) docker     (122)     4091 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/static/css/student.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.490351 lti-consumer-xblock-9.0.1/lti_consumer/static/js/
+-rw-r--r--   0 runner    (1001) docker     (122)    10549 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/static/js/xblock_lti_consumer.js
+-rw-r--r--   0 runner    (1001) docker     (122)     6043 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/static/js/xblock_studio_view.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.490351 lti-consumer-xblock-9.0.1/lti_consumer/static/sass/
+-rw-r--r--   0 runner    (1001) docker     (122)     4751 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/static/sass/student.scss
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.474351 lti-consumer-xblock-9.0.1/lti_consumer/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.490351 lti-consumer-xblock-9.0.1/lti_consumer/templates/html/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.490351 lti-consumer-xblock-9.0.1/lti_consumer/templates/html/lti-dl/
+-rw-r--r--   0 runner    (1001) docker     (122)      405 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/templates/html/lti-dl/dl_response_error.html
+-rw-r--r--   0 runner    (1001) docker     (122)      434 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/templates/html/lti-dl/dl_response_saved.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1048 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/templates/html/lti-dl/render_dl_content.html
+-rw-r--r--   0 runner    (1001) docker     (122)      168 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/templates/html/lti-dl/render_html.html
+-rw-r--r--   0 runner    (1001) docker     (122)      890 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/templates/html/lti-dl/render_image.html
+-rw-r--r--   0 runner    (1001) docker     (122)      709 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/templates/html/lti-dl/render_link.html
+-rw-r--r--   0 runner    (1001) docker     (122)      355 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/templates/html/lti-dl/render_lti_resource_link.html
+-rw-r--r--   0 runner    (1001) docker     (122)      893 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/templates/html/lti_1p3_launch.html
+-rw-r--r--   0 runner    (1001) docker     (122)      405 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/templates/html/lti_1p3_permission_error.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1435 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/templates/html/lti_1p3_studio.html
+-rw-r--r--   0 runner    (1001) docker     (122)      364 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/templates/html/lti_iframe.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1148 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/templates/html/lti_launch.html
+-rw-r--r--   0 runner    (1001) docker     (122)      429 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/templates/html/lti_launch_error.html
+-rw-r--r--   0 runner    (1001) docker     (122)      445 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/templates/html/lti_proctoring_start_error.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3849 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/templates/html/student.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.494351 lti-consumer-xblock-9.0.1/lti_consumer/templates/xml/
+-rw-r--r--   0 runner    (1001) docker     (122)      798 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/templates/xml/outcome_service_response.xml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.494351 lti-consumer-xblock-9.0.1/lti_consumer/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      780 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/templatetags/get_dl_lti_launch_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)      566 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/templatetags/lti_sanitize.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.494351 lti-consumer-xblock-9.0.1/lti_consumer/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2807 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.494351 lti-consumer-xblock-9.0.1/lti_consumer/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.494351 lti-consumer-xblock-9.0.1/lti_consumer/tests/unit/plugin/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/tests/unit/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11288 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/tests/unit/plugin/test_proctoring.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25574 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/tests/unit/plugin/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (122)    38579 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/tests/unit/plugin/test_views_lti_ags.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26203 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/tests/unit/plugin/test_views_lti_deep_linking.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10559 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/tests/unit/plugin/test_views_lti_nrps.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26379 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/tests/unit/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2866 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/tests/unit/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)    82946 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/tests/unit/test_lti_xblock.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24054 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/tests/unit/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16718 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/tests/unit/test_outcomes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3573 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/tests/unit/test_signals.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4743 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/tests/unit/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      366 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/track.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.494351 lti-consumer-xblock-9.0.1/lti_consumer/translations/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.474351 lti-consumer-xblock-9.0.1/lti_consumer/translations/ar/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.494351 lti-consumer-xblock-9.0.1/lti_consumer/translations/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    10720 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/translations/ar/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    20385 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/translations/ar/LC_MESSAGES/text.po
+-rw-r--r--   0 runner    (1001) docker     (122)      359 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/translations/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.474351 lti-consumer-xblock-9.0.1/lti_consumer/translations/en/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.498351 lti-consumer-xblock-9.0.1/lti_consumer/translations/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      380 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/translations/en/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    14641 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/translations/en/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.474351 lti-consumer-xblock-9.0.1/lti_consumer/translations/es_419/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.498351 lti-consumer-xblock-9.0.1/lti_consumer/translations/es_419/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     9197 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/translations/es_419/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    24997 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/translations/es_419/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.474351 lti-consumer-xblock-9.0.1/lti_consumer/translations/fr/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.498351 lti-consumer-xblock-9.0.1/lti_consumer/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1404 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/translations/fr/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    24275 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/translations/fr/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.474351 lti-consumer-xblock-9.0.1/lti_consumer/translations/fr_CA/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.498351 lti-consumer-xblock-9.0.1/lti_consumer/translations/fr_CA/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     9166 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/translations/fr_CA/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    10186 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/translations/fr_CA/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.474351 lti-consumer-xblock-9.0.1/lti_consumer/translations/he/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.498351 lti-consumer-xblock-9.0.1/lti_consumer/translations/he/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    10080 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/translations/he/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    19741 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/translations/he/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.474351 lti-consumer-xblock-9.0.1/lti_consumer/translations/hi/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.498351 lti-consumer-xblock-9.0.1/lti_consumer/translations/hi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      461 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/translations/hi/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    14649 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/translations/hi/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.474351 lti-consumer-xblock-9.0.1/lti_consumer/translations/ja_JP/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.498351 lti-consumer-xblock-9.0.1/lti_consumer/translations/ja_JP/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     9838 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/translations/ja_JP/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    10907 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/translations/ja_JP/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.474351 lti-consumer-xblock-9.0.1/lti_consumer/translations/ko_KR/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.498351 lti-consumer-xblock-9.0.1/lti_consumer/translations/ko_KR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      469 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/translations/ko_KR/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    14719 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/translations/ko_KR/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.474351 lti-consumer-xblock-9.0.1/lti_consumer/translations/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.498351 lti-consumer-xblock-9.0.1/lti_consumer/translations/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1349 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/translations/pt_BR/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    15126 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/translations/pt_BR/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.474351 lti-consumer-xblock-9.0.1/lti_consumer/translations/pt_PT/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.498351 lti-consumer-xblock-9.0.1/lti_consumer/translations/pt_PT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    10221 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/translations/pt_PT/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    18852 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/translations/pt_PT/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.478351 lti-consumer-xblock-9.0.1/lti_consumer/translations/ru/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.498351 lti-consumer-xblock-9.0.1/lti_consumer/translations/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      601 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/translations/ru/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    14789 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/translations/ru/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.478351 lti-consumer-xblock-9.0.1/lti_consumer/translations/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.498351 lti-consumer-xblock-9.0.1/lti_consumer/translations/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      495 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/translations/zh_CN/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    14700 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/translations/zh_CN/LC_MESSAGES/text.po
+-rw-r--r--   0 runner    (1001) docker     (122)    10931 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.502351 lti-consumer-xblock-9.0.1/lti_consumer_xblock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    14196 2023-04-11 14:25:01.000000 lti-consumer-xblock-9.0.1/lti_consumer_xblock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6826 2023-04-11 14:25:01.000000 lti-consumer-xblock-9.0.1/lti_consumer_xblock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      106 2023-04-11 14:25:01.000000 lti-consumer-xblock-9.0.1/lti_consumer_xblock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      199 2023-04-11 14:25:01.000000 lti-consumer-xblock-9.0.1/lti_consumer_xblock.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      171 2023-04-11 14:25:01.000000 lti-consumer-xblock-9.0.1/lti_consumer_xblock.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-04-11 14:25:01.000000 lti-consumer-xblock-9.0.1/lti_consumer_xblock.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.502351 lti-consumer-xblock-9.0.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      325 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      493 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      120 2023-04-11 14:25:01.502351 lti-consumer-xblock-9.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     5875 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/setup.py
```

### Comparing `lti-consumer-xblock-9.0.0/LICENSE` & `lti-consumer-xblock-9.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/NOTICE` & `lti-consumer-xblock-9.0.1/NOTICE`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/PKG-INFO` & `lti-consumer-xblock-9.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lti-consumer-xblock
-Version: 9.0.0
+Version: 9.0.1
 Summary: This XBlock implements the consumer side of the LTI specification.
 Home-page: https://github.com/openedx/xblock-lti-consumer
 Author: Open edX project
 Author-email: oscm@edx.org
 Keywords: lti consumer xblock
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
```

### Comparing `lti-consumer-xblock-9.0.0/README.rst` & `lti-consumer-xblock-9.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/admin.py` & `lti-consumer-xblock-9.0.1/lti_consumer/admin.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/api.py` & `lti-consumer-xblock-9.0.1/lti_consumer/api.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/apps.py` & `lti-consumer-xblock-9.0.1/lti_consumer/apps.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/data.py` & `lti-consumer-xblock-9.0.1/lti_consumer/data.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/filters.py` & `lti-consumer-xblock-9.0.1/lti_consumer/filters.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/forms.py` & `lti-consumer-xblock-9.0.1/lti_consumer/forms.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/lti_1p1/consumer.py` & `lti-consumer-xblock-9.0.1/lti_consumer/lti_1p1/consumer.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/lti_1p1/contrib/django.py` & `lti-consumer-xblock-9.0.1/lti_consumer/lti_1p1/contrib/django.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/lti_1p1/contrib/tests/test_django.py` & `lti-consumer-xblock-9.0.1/lti_consumer/lti_1p1/contrib/tests/test_django.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/lti_1p1/oauth.py` & `lti-consumer-xblock-9.0.1/lti_consumer/lti_1p1/oauth.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/lti_1p1/tests/test_consumer.py` & `lti-consumer-xblock-9.0.1/lti_consumer/lti_1p1/tests/test_consumer.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/lti_1p1/tests/test_oauth.py` & `lti-consumer-xblock-9.0.1/lti_consumer/lti_1p1/tests/test_oauth.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/lti_1p3/ags.py` & `lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/ags.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/lti_1p3/constants.py` & `lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/constants.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/lti_1p3/consumer.py` & `lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/consumer.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/lti_1p3/deep_linking.py` & `lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/deep_linking.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/lti_1p3/exceptions.py` & `lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/exceptions.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/lti_1p3/extensions/rest_framework/authentication.py` & `lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/extensions/rest_framework/authentication.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/lti_1p3/extensions/rest_framework/parsers.py` & `lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/extensions/rest_framework/parsers.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/lti_1p3/extensions/rest_framework/permissions.py` & `lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/extensions/rest_framework/permissions.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/lti_1p3/extensions/rest_framework/renderers.py` & `lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/extensions/rest_framework/renderers.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/lti_1p3/extensions/rest_framework/serializers.py` & `lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/extensions/rest_framework/serializers.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/lti_1p3/extensions/rest_framework/utils.py` & `lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/extensions/rest_framework/utils.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/lti_1p3/key_handlers.py` & `lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/key_handlers.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/lti_1p3/nprs.py` & `lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/nprs.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/lti_1p3/tests/extensions/rest_framework/test_authentication.py` & `lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/tests/extensions/rest_framework/test_authentication.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/lti_1p3/tests/extensions/rest_framework/test_permissions.py` & `lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/tests/extensions/rest_framework/test_permissions.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/lti_1p3/tests/test_ags.py` & `lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/tests/test_ags.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/lti_1p3/tests/test_consumer.py` & `lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/tests/test_consumer.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/lti_1p3/tests/test_deep_linking.py` & `lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/tests/test_deep_linking.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/lti_1p3/tests/test_key_handlers.py` & `lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/tests/test_key_handlers.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/lti_1p3/tests/test_nrps.py` & `lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/tests/test_nrps.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/lti_xblock.py` & `lti-consumer-xblock-9.0.1/lti_consumer/lti_xblock.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/migrations/0001_initial.py` & `lti-consumer-xblock-9.0.1/lti_consumer/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/migrations/0002_ltiagslineitem.py` & `lti-consumer-xblock-9.0.1/lti_consumer/migrations/0002_ltiagslineitem.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/migrations/0003_ltiagsscore.py` & `lti-consumer-xblock-9.0.1/lti_consumer/migrations/0003_ltiagsscore.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/migrations/0004_keyset_mgmt_to_model.py` & `lti-consumer-xblock-9.0.1/lti_consumer/migrations/0004_keyset_mgmt_to_model.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/migrations/0005_migrate_keyset_to_model.py` & `lti-consumer-xblock-9.0.1/lti_consumer/migrations/0005_migrate_keyset_to_model.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/migrations/0006_add_on_model_config_for_lti_1p1.py` & `lti-consumer-xblock-9.0.1/lti_consumer/migrations/0006_add_on_model_config_for_lti_1p1.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/migrations/0007_ltidlcontentitem.py` & `lti-consumer-xblock-9.0.1/lti_consumer/migrations/0007_ltidlcontentitem.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/migrations/0008_fix_uuid_backfill.py` & `lti-consumer-xblock-9.0.1/lti_consumer/migrations/0008_fix_uuid_backfill.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/migrations/0009_backfill-empty-string-config-id.py` & `lti-consumer-xblock-9.0.1/lti_consumer/migrations/0009_backfill-empty-string-config-id.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/migrations/0010_backfill-empty-string-lti-config.py` & `lti-consumer-xblock-9.0.1/lti_consumer/migrations/0010_backfill-empty-string-lti-config.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/migrations/0011_courseeditltifieldsenabledflag.py` & `lti-consumer-xblock-9.0.1/lti_consumer/migrations/0011_courseeditltifieldsenabledflag.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/migrations/0013_auto_20210712_1352.py` & `lti-consumer-xblock-9.0.1/lti_consumer/migrations/0013_auto_20210712_1352.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/migrations/0014_adds_external_id.py` & `lti-consumer-xblock-9.0.1/lti_consumer/migrations/0014_adds_external_id.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/migrations/0015_add_additional_1p3_fields.py` & `lti-consumer-xblock-9.0.1/lti_consumer/migrations/0015_add_additional_1p3_fields.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/migrations/0016_lticonfiguration_lti_1p3_proctoring_enabled.py` & `lti-consumer-xblock-9.0.1/lti_consumer/migrations/0016_lticonfiguration_lti_1p3_proctoring_enabled.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/migrations/0017_lticonfiguration_lti_1p3_redirect_uris.py` & `lti-consumer-xblock-9.0.1/lti_consumer/migrations/0017_lticonfiguration_lti_1p3_redirect_uris.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/models.py` & `lti-consumer-xblock-9.0.1/lti_consumer/models.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/outcomes.py` & `lti-consumer-xblock-9.0.1/lti_consumer/outcomes.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/plugin/compat.py` & `lti-consumer-xblock-9.0.1/lti_consumer/plugin/compat.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/plugin/urls.py` & `lti-consumer-xblock-9.0.1/lti_consumer/plugin/urls.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/plugin/views.py` & `lti-consumer-xblock-9.0.1/lti_consumer/plugin/views.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/signals/signals.py` & `lti-consumer-xblock-9.0.1/lti_consumer/signals/signals.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/static/css/student.css` & `lti-consumer-xblock-9.0.1/lti_consumer/static/css/student.css`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/static/js/xblock_lti_consumer.js` & `lti-consumer-xblock-9.0.1/lti_consumer/static/js/xblock_lti_consumer.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/static/js/xblock_studio_view.js` & `lti-consumer-xblock-9.0.1/lti_consumer/static/js/xblock_studio_view.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/static/sass/student.scss` & `lti-consumer-xblock-9.0.1/lti_consumer/static/sass/student.scss`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/templates/html/lti-dl/render_dl_content.html` & `lti-consumer-xblock-9.0.1/lti_consumer/templates/html/lti-dl/render_dl_content.html`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/templates/html/lti-dl/render_image.html` & `lti-consumer-xblock-9.0.1/lti_consumer/templates/html/lti-dl/render_image.html`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/templates/html/lti-dl/render_link.html` & `lti-consumer-xblock-9.0.1/lti_consumer/templates/html/lti-dl/render_link.html`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/templates/html/lti_1p3_launch.html` & `lti-consumer-xblock-9.0.1/lti_consumer/templates/html/lti_1p3_launch.html`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/templates/html/lti_1p3_studio.html` & `lti-consumer-xblock-9.0.1/lti_consumer/templates/html/lti_1p3_studio.html`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/templates/html/lti_launch.html` & `lti-consumer-xblock-9.0.1/lti_consumer/templates/html/lti_launch.html`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/templates/html/student.html` & `lti-consumer-xblock-9.0.1/lti_consumer/templates/html/student.html`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/templates/xml/outcome_service_response.xml` & `lti-consumer-xblock-9.0.1/lti_consumer/templates/xml/outcome_service_response.xml`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/templatetags/get_dl_lti_launch_url.py` & `lti-consumer-xblock-9.0.1/lti_consumer/templatetags/get_dl_lti_launch_url.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/templatetags/lti_sanitize.py` & `lti-consumer-xblock-9.0.1/lti_consumer/templatetags/lti_sanitize.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/tests/test_utils.py` & `lti-consumer-xblock-9.0.1/lti_consumer/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/tests/unit/plugin/test_proctoring.py` & `lti-consumer-xblock-9.0.1/lti_consumer/tests/unit/plugin/test_proctoring.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/tests/unit/plugin/test_views.py` & `lti-consumer-xblock-9.0.1/lti_consumer/tests/unit/plugin/test_views.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/tests/unit/plugin/test_views_lti_ags.py` & `lti-consumer-xblock-9.0.1/lti_consumer/tests/unit/plugin/test_views_lti_ags.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/tests/unit/plugin/test_views_lti_deep_linking.py` & `lti-consumer-xblock-9.0.1/lti_consumer/tests/unit/plugin/test_views_lti_deep_linking.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/tests/unit/plugin/test_views_lti_nrps.py` & `lti-consumer-xblock-9.0.1/lti_consumer/tests/unit/plugin/test_views_lti_nrps.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/tests/unit/test_api.py` & `lti-consumer-xblock-9.0.1/lti_consumer/tests/unit/test_api.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/tests/unit/test_filters.py` & `lti-consumer-xblock-9.0.1/lti_consumer/tests/unit/test_filters.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/tests/unit/test_lti_xblock.py` & `lti-consumer-xblock-9.0.1/lti_consumer/tests/unit/test_lti_xblock.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/tests/unit/test_models.py` & `lti-consumer-xblock-9.0.1/lti_consumer/tests/unit/test_models.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/tests/unit/test_outcomes.py` & `lti-consumer-xblock-9.0.1/lti_consumer/tests/unit/test_outcomes.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/tests/unit/test_signals.py` & `lti-consumer-xblock-9.0.1/lti_consumer/tests/unit/test_signals.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/tests/unit/test_utils.py` & `lti-consumer-xblock-9.0.1/lti_consumer/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/translations/ar/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.0.1/lti_consumer/translations/ar/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/translations/en/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.0.1/lti_consumer/translations/en/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/translations/es_419/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.0.1/lti_consumer/translations/es_419/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/translations/es_419/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.0.1/lti_consumer/translations/fr_CA/LC_MESSAGES/text.po`

 * *Files 26% similar despite different names*

```diff
@@ -1,229 +1,227 @@
 # 
 # Translators:
-# Albeiro Gonzalez <albeiro.gonzalez@edunext.co>, 2018
-# Juan Camilo Montoya Franco <juan.montoya@edunext.co>, 2017
-# Laura Silva <lingison@edx.org>, 2016
+# Pierre Mailhot <pierre.mailhot@gmail.com>, 2019
 msgid ""
 msgstr ""
 "Project-Id-Version: XBlocks\n"
 "POT-Creation-Date: 2016-03-18 15:09+0500\n"
-"PO-Revision-Date: 2018-02-16 21:43+0000\n"
-"Last-Translator: Albeiro Gonzalez <albeiro.gonzalez@edunext.co>\n"
-"Language-Team: Spanish (Latin America) (http://www.transifex.com/open-edx/xblocks/language/es_419/)\n"
+"PO-Revision-Date: 2019-08-26 22:01+0000\n"
+"Last-Translator: Pierre Mailhot <pierre.mailhot@gmail.com>\n"
+"Language-Team: French (Canada) (http://www.transifex.com/open-edx/xblocks/language/fr_CA/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: es_419\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Language: fr_CA\n"
+"Plural-Forms: nplurals=2; plural=(n > 1);\n"
 "X-Generator: Poedit 1.8.7\n"
 "X-Poedit-Basepath: ../../..\n"
 "X-Poedit-SearchPath-0: lti_consumer.py\n"
 
 #: lti_consumer.py
 msgid "No valid user id found in endpoint URL"
-msgstr "No se encontró un id de usuario válido en el URL del endpoint"
+msgstr "Aucun ID utilisateur valide trouvé dans l'URL cible"
 
 #: lti_consumer.py
 msgid "Display Name"
-msgstr "Nombre a mostrar"
+msgstr "Nom d'affichage"
 
 #: lti_consumer.py
 msgid ""
 "Enter the name that students see for this component. Analytics reports may "
 "also use the display name to identify this component."
-msgstr "Ingrese el nombre que los estudiantes verán para este componente. Los reportes de Analytics también pueden utilizar el nombre para mostrar para identificar este componente."
+msgstr "Entrez le nom que les étudiants voient pour ce composant. Les rapports d'analyse peuvent également utiliser le nom d'affichage pour identifier ce composant."
 
 #: lti_consumer.py
 msgid "LTI Consumer"
-msgstr "Consumidor LTI"
+msgstr "Consommateur LTI"
 
 #: lti_consumer.py:256
 msgid "LTI Application Information"
-msgstr "Información sobre la aplicación LTI"
+msgstr "Information à propos de l'application LTI"
 
 #: lti_consumer.py
 msgid ""
 "Enter a description of the third party application. If requesting username "
 "and/or email, use this text box to inform users why their username and/or "
 "email will be forwarded to a third party application."
-msgstr "Provea una descripción de la aplicación de un tercero. Si se solicita el nombre del usuario o su correo, use este cuadro de texto para informar al usuario que su nombre de usuario y su correo serán redireccionados a una aplicación de un tercero."
+msgstr "Entrer une description de l'application tierce. Si vous demandez le nom d'utilisateur et/ou courriel, utilisez cette boîte de dialogue pour informer les utilisateurs pourquoi leur nom d'utilisateur et/ou courriel seront transmis à une application tierce."
 
 #: lti_consumer.py
 msgid "LTI ID"
-msgstr "ID de LTI"
+msgstr "Identifiant LTI"
 
 #: lti_consumer.py
 #, python-brace-format
 msgid ""
 "Enter the LTI ID for the external LTI provider. This value must be the same "
 "LTI ID that you entered in the LTI Passports setting on the Advanced "
 "Settings page.<br />See the {docs_anchor_open}edX LTI "
 "documentation{anchor_close} for more details on this setting."
-msgstr "Introduzca el ID LTI para el proveedor LTI externo. Este valor debe ser el mismo ID LTI que ingresó en la configuración de Pasaportes LTI en la página Configuración avanzada.<br />Consulte la {docs_anchor_open} documentación de edX LTI {anchor_close} para obtener más detalles sobre esta configuración."
+msgstr "Entrez l'ID LTI du fournisseur LTI externe. Cette valeur doit être identique à l'ID LTI que vous avez entré dans le paramètre LTI Passports de la page des paramètres avancés.<br />Voir {docs_anchor_open}edX LTI documentation{anchor_close} pour plus de détails sur ce paramètre."
 
 #: lti_consumer.py
 msgid "LTI URL"
-msgstr "URL de LTI"
+msgstr "URL LTI"
 
 #: lti_consumer.py
 #, python-brace-format
 msgid ""
 "Enter the URL of the external tool that this component launches. This "
 "setting is only used when Hide External Tool is set to False.<br />See the "
 "{docs_anchor_open}edX LTI documentation{anchor_close} for more details on "
 "this setting."
-msgstr "Ingrese la URL de la herramienta externa que este componente inicia. Esta configuración sólo se utiliza cuando Ocultar herramienta externa se establece en Falso.<br />Consulte la {docs_anchor_open} documentación de edX LTI {anchor_close} para obtener más detalles sobre esta configuración."
+msgstr "Entrez l'URL de l'outil externe que ce composant lance. Ce paramètre est uniquement utilisé lorsque l'option Masquer l'outil externe est définie sur False.<br />Voir {docs_anchor_open}edX LTI documentation{anchor_close} pour plus de détails sur ce paramètre."
 
 #: lti_consumer.py
 msgid "Custom Parameters"
-msgstr "Parámetros personalizados"
+msgstr "Paramètres personnalisés"
 
 #: lti_consumer.py
 #, python-brace-format
 msgid ""
 "Add the key/value pair for any custom parameters, such as the page your "
 "e-book should open to or the background color for this component. Ex. "
 "[\"page=1\", \"color=white\"]<br />See the {docs_anchor_open}edX LTI "
 "documentation{anchor_close} for more details on this setting."
-msgstr "Agregue el par clave / valor para cualquier parámetro personalizado, como la página a la que su libro electrónico debe abrirse o el color de fondo para este componente. Ej. [\"page=1\", \"color=white\"]<br />Consulte la {docs_anchor_open} documentación de edX LTI {anchor_close} para obtener más detalles sobre esta configuración"
+msgstr "Ajoutez la paire clé / valeur pour tous les paramètres personnalisés, tels que la page que votre livre électronique doit ouvrir ou la couleur d'arrière-plan de ce composant. Ex. [\"page=1\", \"color=white\"]<br />Voir {docs_anchor_open}edX LTI documentation{anchor_close} pour plus de détails sur ce paramètre."
 
 #: lti_consumer.py
 msgid "LTI Launch Target"
-msgstr "Target para el LTI"
+msgstr "Cible de lancement LTI"
 
 #: lti_consumer.py
 msgid ""
 "Select Inline if you want the LTI content to open in an IFrame in the "
 "current page. Select Modal if you want the LTI content to open in a modal "
 "window in the current page. Select New Window if you want the LTI content to"
 " open in a new browser window. This setting is only used when Hide External "
 "Tool is set to False."
-msgstr "Seleccione Inline si desea que el contenido LTI se abra en un IFrame en la página actual. Seleccione Modal si desea que el contenido LTI se abra en una ventana modal en la página actual. Seleccione Nueva ventana si desea que el contenido LTI se abra en una nueva ventana del navegador. Esta configuración sólo se utiliza cuando Ocultar herramienta externa se establece en Falso."
+msgstr "Sélectionnez Inline si vous souhaitez que le contenu LTI s'ouvre dans un IFrame de la page en cours. Sélectionnez Modal si vous souhaitez que le contenu LTI s'ouvre dans une fenêtre modale de la page en cours. Sélectionnez Nouvelle Fenêtre si vous souhaitez que le contenu LTI s'ouvre dans une nouvelle fenêtre du navigateur. Ce paramètre est uniquement utilisé lorsque l'option masquer l'outil externe est définie sur False."
 
 #: lti_consumer.py
 msgid "Button Text"
-msgstr "Texto para el botón"
+msgstr "Texte du bouton"
 
 #: lti_consumer.py
 msgid ""
 "Enter the text on the button used to launch the third party application. "
 "This setting is only used when Hide External Tool is set to False and LTI "
 "Launch Target is set to Modal or New Window."
-msgstr "Ingrese el texto en el botón usado para iniciar la aplicación de terceros. Esta opción sólo se utiliza cuando Ocultar herramienta externa se establece en Falso y el Target para el LTI se establece en Modal o Nueva Ventana."
+msgstr "Entrez le texte du bouton qui sera utilisé pour lancer l'application tierce. Ce paramètre est utilisé uniquement lorsque masquer l'outil externe est défini sur False et que LTI Launch Target est défini sur Modal ou Nouvelle fenêtre."
 
 #: lti_consumer.py
 msgid "Inline Height"
-msgstr "Altura Inline"
+msgstr "Hauteur intégré"
 
 #: lti_consumer.py
 msgid ""
 "Enter the desired pixel height of the iframe which will contain the LTI "
 "tool. This setting is only used when Hide External Tool is set to False and "
 "LTI Launch Target is set to Inline."
-msgstr "Introduzca la altura en píxeles deseada del iframe que contendrá la herramienta LTI. Esta opción sólo se utiliza cuando Ocultar herramienta externa se establece en False y Target para el LTI se establece en Inline."
+msgstr "Entrez la hauteur de pixel souhaitée de l'iframe qui contiendra l'outil LTI. Ce paramètre est uniquement utilisé lorsque masquer l'outil externe est défini sur False et que LTI Launch Target est défini sur Inline."
 
 #: lti_consumer.py
 msgid "Modal Height"
-msgstr "Altura del modal"
+msgstr "Hauteur modale"
 
 #: lti_consumer.py
 msgid ""
 "Enter the desired viewport percentage height of the modal overlay which will"
 " contain the LTI tool. This setting is only used when Hide External Tool is "
 "set to False and LTI Launch Target is set to Modal."
-msgstr "Ingrese la altura de porcentaje de visualización deseada de la superposición modal que contendrá la herramienta LTI. Esta opción sólo se utiliza cuando Ocultar herramienta externa se establece en False y Target para el LTI se establece en Modal."
+msgstr "Entrez le pourcentage de hauteur de la fenêtre de visualisation de la superposition modale qui contiendra l’outil LTI. Ce paramètre est uniquement utilisé lorsque masquer l'outil externe est défini sur False et que LTI Launch Target est défini sur Modal."
 
 #: lti_consumer.py
 msgid "Modal Width"
-msgstr "Ancho del modal"
+msgstr "Largeur modale"
 
 #: lti_consumer.py
 msgid ""
 "Enter the desired viewport percentage width of the modal overlay which will "
 "contain the LTI tool. This setting is only used when Hide External Tool is "
 "set to False and LTI Launch Target is set to Modal."
-msgstr "Ingrese el ancho de porcentaje de la ventana de visualización de la superposición modal que contendrá la herramienta LTI. Esta opción sólo se utiliza cuando Ocultar herramienta externa se establece en False y Target para el LTI se establece en Modal."
+msgstr "Entrez le pourcentage de largeur de la fenêtre de superposition modale qui contiendra l’outil LTI. Ce paramètre est uniquement utilisé lorsque masquer l'outil externe est défini sur False et que LTI Launch Target est défini sur Modal."
 
 #: lti_consumer.py
 msgid "Scored"
-msgstr "Puntuado"
+msgstr "Noté"
 
 #: lti_consumer.py
 msgid ""
 "Select True if this component will receive a numerical score from the "
 "external LTI system."
-msgstr "Seleccione True si este componente recibirá una puntuación numérica desde un sistema LTI externo."
+msgstr "Sélectionner vrai (true) si ce composant va recevoir une note numérique de la part du système externe LTI."
 
 #: lti_consumer.py
 msgid ""
 "Enter the number of points possible for this component.  The default value "
 "is 1.0.  This setting is only used when Scored is set to True."
-msgstr "Ingrese el número de puntos posibles para este componente. El valor por defecto es 1.0. Este valor solo se utiliza cuando el parámetro de calificación está definido como True."
+msgstr "Entrer le nombre de points possible pour ce composant. La valeur de défaut est 1.0. Ce paramètre est uniquement utilisé quand Noté est initialisé à Vrai (True)."
 
 #: lti_consumer.py
 msgid ""
 "The score kept in the xblock KVS -- duplicate of the published score in "
 "django DB"
-msgstr "La calificación almacenada en xblock KVS -- un duplicado de la calificación publicada en django DB"
+msgstr "La note conservée dans le xblock KVS -- duplicat de la note publiée dans django DB"
 
 #: lti_consumer.py
 msgid "Comment as returned from grader, LTI2.0 spec"
-msgstr "El comentario tal y como fue enviado por el evaluador, LTI2.0 spec"
+msgstr "Commentaire comme retourné par l'évaluateur, spécification LTI2.0"
 
 #: lti_consumer.py
 msgid "Hide External Tool"
-msgstr "Ocultar la herramienta externa"
+msgstr "Cacher les outils externes"
 
 #: lti_consumer.py
 msgid ""
 "Select True if you want to use this component as a placeholder for syncing "
 "with an external grading  system rather than launch an external tool.  This "
 "setting hides the Launch button and any IFrames for this component."
-msgstr "Seleccione True si desea usar este componente como marcador para sincronizarse con un servicio externo en lugar de lanzar una herramienta externa. Esta opción oculta el botón de Lanzar y cualquier iframe para este componente."
+msgstr "Sélectionner vrai (true) si vous voulez utiliser ce composant comme un espace réservé pour synchroniser avec un système d'évaluation externe au lieu de démarrer un outil externe.  Ce paramètre cache le bouton Démarrage et tout IFrames pour ce composant."
 
 #: lti_consumer.py
 msgid "Accept grades past deadline"
-msgstr "Aceptar notas después de la fecha límite"
+msgstr "Accepter les notes après la date limite"
 
 #: lti_consumer.py
 msgid ""
 "Select True to allow third party systems to post grades past the deadline."
-msgstr "Seleccione True para permitir que sistemas de terceros publiquen calificaciones después de la fecha límite."
+msgstr "Sélectionner vrai (true) pour permettre aux systèmes tierces de poster des notes après la date limite."
 
 #: lti_consumer.py
 msgid "Request user's username"
-msgstr "Solicite el nombre público del usuario"
+msgstr "Demander le nom d'utilisateur"
 
 #: lti_consumer.py
 msgid "Select True to request the user's username."
-msgstr "Seleccione True para solicitar el nombre de usuario."
+msgstr "Choisir vrai (true) afin de demander le nom d'utilisateur."
 
 #: lti_consumer.py
 msgid "Request user's email"
-msgstr "Solicitar la dirección de correo del usuario"
+msgstr "Demander l'adresse courriel de l'utilisateur"
 
 #: lti_consumer.py
 msgid "Select True to request the user's email address."
-msgstr "Seleccione True para solicitar el correo electrónico del usuario."
+msgstr "Choisir vrai (true) afin de demander l'adresse courriel de l'utilisateur."
 
 #: lti_consumer.py
 #, python-brace-format
 msgid ""
 "Could not parse LTI passport: {lti_passport}. Should be \"id:key:secret\" "
 "string."
-msgstr "No ha sido posible leer el pasaporte LTI: {lti_passport}. Debería ser una cadena \"id:key:secret\"."
+msgstr "Impossible d'analyser le passeport LTI: {lti_passport}. Devrait être une chaîne \"id:key:secret\"."
 
 #: lti_consumer.py
 msgid "Could not get user id for current request"
-msgstr "No se pudo obtener el id de usuario para esta petición"
+msgstr "Impossible d'obtenir l'ID utilisateur pour la demande en cours"
 
 #: lti_consumer.py
 #, python-brace-format
 msgid ""
 "Could not parse custom parameter: {custom_parameter}. Should be \"x=y\" "
 "string."
-msgstr "No se pudo leer el parámetro personalizado: {custom_parameter}. Debería ser una cadena \"x=y\"."
+msgstr "Impossible d'analyser le paramètre personnalisé: {custom_parameter}. Devrait être une chaîne \"x=y\"."
 
 #: lti_consumer.py
 msgid "[LTI]: Real user not found against anon_id: {}"
-msgstr "[LTI]: No se encontró un usuario que coincidiera con anon_id: {}"
+msgstr "[LTI]: Utilisateur réel non trouvé pour anon_id: {}"
```

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/translations/fr/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.0.1/lti_consumer/translations/fr/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/translations/fr_CA/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.0.1/lti_consumer/translations/fr_CA/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/translations/he/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.0.1/lti_consumer/translations/he/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/translations/ja_JP/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.0.1/lti_consumer/translations/ja_JP/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/translations/ja_JP/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.0.1/lti_consumer/translations/ja_JP/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/translations/pt_BR/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.0.1/lti_consumer/translations/pt_BR/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/translations/pt_PT/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.0.1/lti_consumer/translations/pt_PT/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/translations/pt_PT/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.0.1/lti_consumer/translations/pt_PT/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/translations/ru/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.0.1/lti_consumer/translations/ru/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer/utils.py` & `lti-consumer-xblock-9.0.1/lti_consumer/utils.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer_xblock.egg-info/PKG-INFO` & `lti-consumer-xblock-9.0.1/lti_consumer_xblock.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lti-consumer-xblock
-Version: 9.0.0
+Version: 9.0.1
 Summary: This XBlock implements the consumer side of the LTI specification.
 Home-page: https://github.com/openedx/xblock-lti-consumer
 Author: Open edX project
 Author-email: oscm@edx.org
 Keywords: lti consumer xblock
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
```

### Comparing `lti-consumer-xblock-9.0.0/lti_consumer_xblock.egg-info/SOURCES.txt` & `lti-consumer-xblock-9.0.1/lti_consumer_xblock.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.0/setup.py` & `lti-consumer-xblock-9.0.1/setup.py`

 * *Files identical despite different names*

