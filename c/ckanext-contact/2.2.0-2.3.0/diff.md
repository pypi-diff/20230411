# Comparing `tmp/ckanext-contact-2.2.0.tar.gz` & `tmp/ckanext-contact-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-contact-2.2.0.tar", last modified: Mon Apr  3 13:15:31 2023, max compression
+gzip compressed data, was "ckanext-contact-2.3.0.tar", last modified: Tue Apr 11 08:14:57 2023, max compression
```

## Comparing `ckanext-contact-2.2.0.tar` & `ckanext-contact-2.3.0.tar`

### file list

```diff
@@ -1,51 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 13:15:31.912742 ckanext-contact-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-03 13:15:20.000000 ckanext-contact-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-04-03 13:15:31.912742 ckanext-contact-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-04-03 13:15:20.000000 ckanext-contact-2.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 13:15:31.912742 ckanext-contact-2.2.0/ckanext/
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-03 13:15:20.000000 ckanext-contact-2.2.0/ckanext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 13:15:31.912742 ckanext-contact-2.2.0/ckanext/contact/
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-03 13:15:20.000000 ckanext-contact-2.2.0/ckanext/contact/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-03 13:15:20.000000 ckanext-contact-2.2.0/ckanext/contact/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-03 13:15:20.000000 ckanext-contact-2.2.0/ckanext/contact/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-04-03 13:15:20.000000 ckanext-contact-2.2.0/ckanext/contact/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-03 13:15:20.000000 ckanext-contact-2.2.0/ckanext/contact/recaptcha.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 13:15:31.912742 ckanext-contact-2.2.0/ckanext/contact/routes/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-03 13:15:20.000000 ckanext-contact-2.2.0/ckanext/contact/routes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-04-03 13:15:20.000000 ckanext-contact-2.2.0/ckanext/contact/routes/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-04-03 13:15:20.000000 ckanext-contact-2.2.0/ckanext/contact/routes/contact.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 13:15:31.908742 ckanext-contact-2.2.0/ckanext/contact/theme/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 13:15:31.912742 ckanext-contact-2.2.0/ckanext/contact/theme/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 13:15:31.912742 ckanext-contact-2.2.0/ckanext/contact/theme/assets/modules/
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-04-03 13:15:20.000000 ckanext-contact-2.2.0/ckanext/contact/theme/assets/modules/form-contact.js
--rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-04-03 13:15:20.000000 ckanext-contact-2.2.0/ckanext/contact/theme/assets/modules/modal-contact.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 13:15:31.912742 ckanext-contact-2.2.0/ckanext/contact/theme/assets/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-04-03 13:15:20.000000 ckanext-contact-2.2.0/ckanext/contact/theme/assets/scripts/recaptcha_helpers.js
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-03 13:15:20.000000 ckanext-contact-2.2.0/ckanext/contact/theme/assets/webassets.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 13:15:31.912742 ckanext-contact-2.2.0/ckanext/contact/theme/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 13:15:31.912742 ckanext-contact-2.2.0/ckanext/contact/theme/templates/ajax_snippets/
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-03 13:15:20.000000 ckanext-contact-2.2.0/ckanext/contact/theme/templates/ajax_snippets/contact_form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 13:15:31.912742 ckanext-contact-2.2.0/ckanext/contact/theme/templates/contact/
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-04-03 13:15:20.000000 ckanext-contact-2.2.0/ckanext/contact/theme/templates/contact/form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 13:15:31.912742 ckanext-contact-2.2.0/ckanext/contact/theme/templates/contact/snippets/
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-04-03 13:15:20.000000 ckanext-contact-2.2.0/ckanext/contact/theme/templates/contact/snippets/form.html
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-03 13:15:20.000000 ckanext-contact-2.2.0/ckanext/contact/theme/templates/contact/snippets/modal_link.html
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-03 13:15:20.000000 ckanext-contact-2.2.0/ckanext/contact/theme/templates/contact/success.html
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-03 13:15:20.000000 ckanext-contact-2.2.0/ckanext/contact/theme/templates/header.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 13:15:31.912742 ckanext-contact-2.2.0/ckanext_contact.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-04-03 13:15:31.000000 ckanext-contact-2.2.0/ckanext_contact.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-03 13:15:31.000000 ckanext-contact-2.2.0/ckanext_contact.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 13:15:31.000000 ckanext-contact-2.2.0/ckanext_contact.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-03 13:15:31.000000 ckanext-contact-2.2.0/ckanext_contact.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 13:15:31.000000 ckanext-contact-2.2.0/ckanext_contact.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-03 13:15:31.000000 ckanext-contact-2.2.0/ckanext_contact.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-03 13:15:31.000000 ckanext-contact-2.2.0/ckanext_contact.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 13:15:31.908742 ckanext-contact-2.2.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 13:15:31.912742 ckanext-contact-2.2.0/docs/_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-04-03 13:15:20.000000 ckanext-contact-2.2.0/docs/_scripts/gen_api_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-03 13:15:20.000000 ckanext-contact-2.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 13:15:31.912742 ckanext-contact-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-03 13:15:20.000000 ckanext-contact-2.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 13:15:31.912742 ckanext-contact-2.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-03 13:15:20.000000 ckanext-contact-2.2.0/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-04-03 13:15:20.000000 ckanext-contact-2.2.0/tests/test_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:14:57.304059 ckanext-contact-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-11 08:14:39.000000 ckanext-contact-2.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-04-11 08:14:57.304059 ckanext-contact-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-04-11 08:14:39.000000 ckanext-contact-2.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:14:57.300058 ckanext-contact-2.3.0/ckanext/
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-11 08:14:39.000000 ckanext-contact-2.3.0/ckanext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:14:57.300058 ckanext-contact-2.3.0/ckanext/contact/
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-11 08:14:39.000000 ckanext-contact-2.3.0/ckanext/contact/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-11 08:14:39.000000 ckanext-contact-2.3.0/ckanext/contact/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-11 08:14:39.000000 ckanext-contact-2.3.0/ckanext/contact/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-04-11 08:14:39.000000 ckanext-contact-2.3.0/ckanext/contact/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-11 08:14:39.000000 ckanext-contact-2.3.0/ckanext/contact/recaptcha.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:14:57.300058 ckanext-contact-2.3.0/ckanext/contact/routes/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-11 08:14:39.000000 ckanext-contact-2.3.0/ckanext/contact/routes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5452 2023-04-11 08:14:39.000000 ckanext-contact-2.3.0/ckanext/contact/routes/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-04-11 08:14:39.000000 ckanext-contact-2.3.0/ckanext/contact/routes/contact.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:14:57.296059 ckanext-contact-2.3.0/ckanext/contact/theme/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:14:57.300058 ckanext-contact-2.3.0/ckanext/contact/theme/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:14:57.300058 ckanext-contact-2.3.0/ckanext/contact/theme/assets/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-04-11 08:14:39.000000 ckanext-contact-2.3.0/ckanext/contact/theme/assets/modules/form-contact.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-04-11 08:14:39.000000 ckanext-contact-2.3.0/ckanext/contact/theme/assets/modules/modal-contact.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:14:57.300058 ckanext-contact-2.3.0/ckanext/contact/theme/assets/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-04-11 08:14:39.000000 ckanext-contact-2.3.0/ckanext/contact/theme/assets/scripts/recaptcha_helpers.js
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-11 08:14:39.000000 ckanext-contact-2.3.0/ckanext/contact/theme/assets/webassets.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:14:57.300058 ckanext-contact-2.3.0/ckanext/contact/theme/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:14:57.300058 ckanext-contact-2.3.0/ckanext/contact/theme/templates/ajax_snippets/
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-11 08:14:39.000000 ckanext-contact-2.3.0/ckanext/contact/theme/templates/ajax_snippets/contact_form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:14:57.300058 ckanext-contact-2.3.0/ckanext/contact/theme/templates/contact/
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-04-11 08:14:39.000000 ckanext-contact-2.3.0/ckanext/contact/theme/templates/contact/form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:14:57.300058 ckanext-contact-2.3.0/ckanext/contact/theme/templates/contact/snippets/
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-04-11 08:14:39.000000 ckanext-contact-2.3.0/ckanext/contact/theme/templates/contact/snippets/form.html
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-11 08:14:39.000000 ckanext-contact-2.3.0/ckanext/contact/theme/templates/contact/snippets/modal_link.html
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-11 08:14:39.000000 ckanext-contact-2.3.0/ckanext/contact/theme/templates/contact/success.html
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-11 08:14:39.000000 ckanext-contact-2.3.0/ckanext/contact/theme/templates/header.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:14:57.304059 ckanext-contact-2.3.0/ckanext_contact.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-04-11 08:14:57.000000 ckanext-contact-2.3.0/ckanext_contact.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-11 08:14:57.000000 ckanext-contact-2.3.0/ckanext_contact.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 08:14:57.000000 ckanext-contact-2.3.0/ckanext_contact.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-11 08:14:57.000000 ckanext-contact-2.3.0/ckanext_contact.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 08:14:57.000000 ckanext-contact-2.3.0/ckanext_contact.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-11 08:14:57.000000 ckanext-contact-2.3.0/ckanext_contact.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-11 08:14:57.000000 ckanext-contact-2.3.0/ckanext_contact.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:14:57.300058 ckanext-contact-2.3.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:14:57.304059 ckanext-contact-2.3.0/docs/_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-04-11 08:14:39.000000 ckanext-contact-2.3.0/docs/_scripts/gen_api_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-11 08:14:39.000000 ckanext-contact-2.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 08:14:57.304059 ckanext-contact-2.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-11 08:14:39.000000 ckanext-contact-2.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:14:57.300058 ckanext-contact-2.3.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:14:57.304059 ckanext-contact-2.3.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:14:39.000000 ckanext-contact-2.3.0/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-11 08:14:39.000000 ckanext-contact-2.3.0/tests/unit/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-04-11 08:14:39.000000 ckanext-contact-2.3.0/tests/unit/test_helpers.py
```

### Comparing `ckanext-contact-2.2.0/LICENSE` & `ckanext-contact-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-contact-2.2.0/PKG-INFO` & `ckanext-contact-2.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-contact
-Version: 2.2.0
+Version: 2.3.0
 Summary: A CKAN extension for adding popup contact forms to pages.
 Author-email: Natural History Museum <data@nhm.ac.uk>
 License: GPL-3.0-or-later
 Project-URL: repository, https://github.com/NaturalHistoryMuseum/ckanext-contact
 Project-URL: changelog, https://github.com/NaturalHistoryMuseum/ckanext-contact/blob/main/CHANGELOG.md
 Keywords: CKAN,data,contact
 Classifier: Development Status :: 5 - Production/Stable
@@ -100,14 +100,15 @@
 
 | Name                                       | Description                                       | Default                         |
 |--------------------------------------------|---------------------------------------------------|---------------------------------|
 | `ckanext.contact.mail_to`                  | Email address to submit to                        | `email_to`                      |
 | `ckanext.contact.recipient_name`           | Name of the recipient                             | `ckan.site_title`               |
 | `ckanext.contact.subject`                  | Email subject for the submitted form              | 'Contact/Question from visitor' |
 | `ckanext.contact.add_timestamp_to_subject` | Whether to append a timestamp to the subject line | `false`                         |
+| `ckanext.contact.subject_prefix`           | A prefix to add to the subject before sending     | ''                              |
 
 ## Recaptcha
 
 | Name                                  | Description                              | Default               |
 |---------------------------------------|------------------------------------------|-----------------------|
 | `ckanext.contact.recaptcha_v3_key`    | API key for the reCAPTCHA service.       | False (i.e. disabled) |
 | `ckanext.contact.recaptcha_v3_secret` | API secret for the reCAPTCHA service.    | False (i.e. disabled) |
```

### Comparing `ckanext-contact-2.2.0/README.md` & `ckanext-contact-2.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -79,14 +79,15 @@
 
 | Name                                       | Description                                       | Default                         |
 |--------------------------------------------|---------------------------------------------------|---------------------------------|
 | `ckanext.contact.mail_to`                  | Email address to submit to                        | `email_to`                      |
 | `ckanext.contact.recipient_name`           | Name of the recipient                             | `ckan.site_title`               |
 | `ckanext.contact.subject`                  | Email subject for the submitted form              | 'Contact/Question from visitor' |
 | `ckanext.contact.add_timestamp_to_subject` | Whether to append a timestamp to the subject line | `false`                         |
+| `ckanext.contact.subject_prefix`           | A prefix to add to the subject before sending     | ''                              |
 
 ## Recaptcha
 
 | Name                                  | Description                              | Default               |
 |---------------------------------------|------------------------------------------|-----------------------|
 | `ckanext.contact.recaptcha_v3_key`    | API key for the reCAPTCHA service.       | False (i.e. disabled) |
 | `ckanext.contact.recaptcha_v3_secret` | API secret for the reCAPTCHA service.    | False (i.e. disabled) |
```

### Comparing `ckanext-contact-2.2.0/ckanext/contact/interfaces.py` & `ckanext-contact-2.3.0/ckanext/contact/interfaces.py`

 * *Files identical despite different names*

### Comparing `ckanext-contact-2.2.0/ckanext/contact/plugin.py` & `ckanext-contact-2.3.0/ckanext/contact/plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext-contact-2.2.0/ckanext/contact/recaptcha.py` & `ckanext-contact-2.3.0/ckanext/contact/recaptcha.py`

 * *Files identical despite different names*

### Comparing `ckanext-contact-2.2.0/ckanext/contact/routes/_helpers.py` & `ckanext-contact-2.3.0/ckanext/contact/routes/_helpers.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,21 +23,25 @@
 
     :param data_dict: the request params as a dict
     :return: a 3-tuple of errors, error summaries and a recaptcha error, in the event where no
              issues occur the return is ({}, {}, None)
     """
     errors = {}
     error_summary = {}
+    optional_fields = {'subject'}
     recaptcha_error = None
 
     # check each field to see if it has a value and if not, show and error
     for field, value in data_dict.items():
         # we know the save field is not necessary and may be empty so ignore it
         if field == 'save':
             continue
+        # ignore optionals
+        if field in optional_fields:
+            continue
         if value is None or value == '':
             errors[field] = ['Missing Value']
             error_summary[field] = 'Missing value'
 
     # only check the recaptcha if there are no errors
     if not errors:
         try:
@@ -50,32 +54,40 @@
             log.info(f'Recaptcha failed due to "{e}"')
             recaptcha_error = toolkit._('Recaptcha check failed, please try again.')
 
     return errors, error_summary, recaptcha_error
 
 
 def build_subject(
-    subject_default='Contact/Question from visitor', timestamp_default=False
+    subject=None, default='Contact/Question from visitor', timestamp_default=False
 ):
     """
-    Creates the subject line for the contact email using the config or the defaults.
+    Creates the subject line for the contact email using the config or the provided
+    subject.
 
-    :param subject_default: the default str to use if ckanext.contact.subject isn't specified
-    :param timestamp_default: the default bool to use if add_timestamp_to_subject isn't specified
+    :param subject: a user defined subject line
+    :param default: the default str to use if the user didn't provide a subject or
+                    ckanext.contact.subject isn't specified
+    :param timestamp_default: the default bool to use if add_timestamp_to_subject isn't
+                              specified
     :return: the subject line
     """
-    subject = toolkit.config.get('ckanext.contact.subject', toolkit._(subject_default))
+    if not subject:
+        subject = toolkit.config.get('ckanext.contact.subject', toolkit._(default))
     if asbool(
         toolkit.config.get(
             'ckanext.contact.add_timestamp_to_subject', timestamp_default
         )
     ):
         timestamp = datetime.now(timezone.utc).strftime('%Y-%m-%d %H:%M:%S %Z')
         subject = f'{subject} [{timestamp}]'
-    return subject
+
+    prefix = toolkit.config.get('ckanext.contact.subject_prefix', '')
+
+    return f'{prefix}{" " if prefix else ""}{subject}'
 
 
 def submit():
     """
     Take the data in the request params and send an email using them. If the data is
     invalid or a recaptcha is setup and it fails, don't send the email.
 
@@ -103,15 +115,15 @@
         mail_dict = {
             'recipient_email': toolkit.config.get(
                 'ckanext.contact.mail_to', toolkit.config.get('email_to')
             ),
             'recipient_name': toolkit.config.get(
                 'ckanext.contact.recipient_name', toolkit.config.get('ckan.site_title')
             ),
-            'subject': build_subject(),
+            'subject': build_subject(subject=data_dict.get('subject')),
             'body': '\n'.join(body_parts),
             'headers': {'reply-to': data_dict['email']},
         }
 
         # allow other plugins to modify the mail_dict
         for plugin in PluginImplementations(IContact):
             plugin.mail_alter(mail_dict, data_dict)
```

### Comparing `ckanext-contact-2.2.0/ckanext/contact/routes/contact.py` & `ckanext-contact-2.3.0/ckanext/contact/routes/contact.py`

 * *Files identical despite different names*

### Comparing `ckanext-contact-2.2.0/ckanext/contact/theme/assets/modules/form-contact.js` & `ckanext-contact-2.3.0/ckanext/contact/theme/assets/modules/form-contact.js`

 * *Files identical despite different names*

### Comparing `ckanext-contact-2.2.0/ckanext/contact/theme/assets/modules/modal-contact.js` & `ckanext-contact-2.3.0/ckanext/contact/theme/assets/modules/modal-contact.js`

 * *Files identical despite different names*

### Comparing `ckanext-contact-2.2.0/ckanext/contact/theme/assets/scripts/recaptcha_helpers.js` & `ckanext-contact-2.3.0/ckanext/contact/theme/assets/scripts/recaptcha_helpers.js`

 * *Files identical despite different names*

### Comparing `ckanext-contact-2.2.0/ckanext/contact/theme/templates/ajax_snippets/contact_form.html` & `ckanext-contact-2.3.0/ckanext/contact/theme/templates/ajax_snippets/contact_form.html`

 * *Files identical despite different names*

### Comparing `ckanext-contact-2.2.0/ckanext/contact/theme/templates/contact/form.html` & `ckanext-contact-2.3.0/ckanext/contact/theme/templates/contact/form.html`

 * *Files identical despite different names*

### Comparing `ckanext-contact-2.2.0/ckanext/contact/theme/templates/contact/snippets/form.html` & `ckanext-contact-2.3.0/ckanext/contact/theme/templates/contact/snippets/form.html`

 * *Files 12% similar despite different names*

```diff
@@ -22,14 +22,18 @@
                 {{ form.input('name', label=_('Contact Name'), id='field-name', value=data.name,
                               error=errors.name, classes=['control-medium'], is_required=true) }}
 
                 {{ form.input('email', label=_('Email'), id='field-email', type='email',
                               value=data.email, error=errors.email, classes=['control-medium'],
                               is_required=true) }}
 
+                {{ form.input('subject', label=_('Subject'), id='field-subject',
+                              value=data.subject, error=errors.subject, classes=['control-medium'],
+                              is_required=false, placeholder=_('Optional subject')) }}
+
                 {{ form.markdown('content', label=_('Your Request'), id='field-content',
                                  value=data.content, error=errors.content,
                                  placeholder=_('What do you have to tell us?'), is_required=true) }}
             {% endblock %}
         </fieldset>
 
         <div class="form-actions">
```

### Comparing `ckanext-contact-2.2.0/ckanext/contact/theme/templates/contact/success.html` & `ckanext-contact-2.3.0/ckanext/contact/theme/templates/contact/success.html`

 * *Files identical despite different names*

### Comparing `ckanext-contact-2.2.0/ckanext_contact.egg-info/PKG-INFO` & `ckanext-contact-2.3.0/ckanext_contact.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-contact
-Version: 2.2.0
+Version: 2.3.0
 Summary: A CKAN extension for adding popup contact forms to pages.
 Author-email: Natural History Museum <data@nhm.ac.uk>
 License: GPL-3.0-or-later
 Project-URL: repository, https://github.com/NaturalHistoryMuseum/ckanext-contact
 Project-URL: changelog, https://github.com/NaturalHistoryMuseum/ckanext-contact/blob/main/CHANGELOG.md
 Keywords: CKAN,data,contact
 Classifier: Development Status :: 5 - Production/Stable
@@ -100,14 +100,15 @@
 
 | Name                                       | Description                                       | Default                         |
 |--------------------------------------------|---------------------------------------------------|---------------------------------|
 | `ckanext.contact.mail_to`                  | Email address to submit to                        | `email_to`                      |
 | `ckanext.contact.recipient_name`           | Name of the recipient                             | `ckan.site_title`               |
 | `ckanext.contact.subject`                  | Email subject for the submitted form              | 'Contact/Question from visitor' |
 | `ckanext.contact.add_timestamp_to_subject` | Whether to append a timestamp to the subject line | `false`                         |
+| `ckanext.contact.subject_prefix`           | A prefix to add to the subject before sending     | ''                              |
 
 ## Recaptcha
 
 | Name                                  | Description                              | Default               |
 |---------------------------------------|------------------------------------------|-----------------------|
 | `ckanext.contact.recaptcha_v3_key`    | API key for the reCAPTCHA service.       | False (i.e. disabled) |
 | `ckanext.contact.recaptcha_v3_secret` | API secret for the reCAPTCHA service.    | False (i.e. disabled) |
```

### Comparing `ckanext-contact-2.2.0/ckanext_contact.egg-info/SOURCES.txt` & `ckanext-contact-2.3.0/ckanext_contact.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -25,9 +25,10 @@
 ckanext_contact.egg-info/SOURCES.txt
 ckanext_contact.egg-info/dependency_links.txt
 ckanext_contact.egg-info/entry_points.txt
 ckanext_contact.egg-info/not-zip-safe
 ckanext_contact.egg-info/requires.txt
 ckanext_contact.egg-info/top_level.txt
 docs/_scripts/gen_api_pages.py
-tests/test_auth.py
-tests/test_helpers.py
+tests/unit/__init__.py
+tests/unit/test_auth.py
+tests/unit/test_helpers.py
```

### Comparing `ckanext-contact-2.2.0/docs/_scripts/gen_api_pages.py` & `ckanext-contact-2.3.0/docs/_scripts/gen_api_pages.py`

 * *Files identical despite different names*

### Comparing `ckanext-contact-2.2.0/pyproject.toml` & `ckanext-contact-2.3.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ckanext-contact"
-version = "2.2.0"
+version = "2.3.0"
 description = "A CKAN extension for adding popup contact forms to pages."
 readme = "README.md"
 requires-python = ">=3.6"
 license = { text = "GPL-3.0-or-later" }
 authors = [
     { name = "Natural History Museum", email = "data@nhm.ac.uk" }
 ]
@@ -51,15 +51,15 @@
 exclude = ["tests", "docs"]
 
 [tool.setuptools.package-data]
 "ckanext.contact.theme" = ["*", "**/*"]
 
 [tool.commitizen]
 name = "cz_nhm"
-version = "2.2.0"
+version = "2.3.0"
 tag_format = "v$version"
 update_changelog_on_bump = true
 changelog_incremental = true
 version_files = [
     "pyproject.toml:version"
 ]
```

### Comparing `ckanext-contact-2.2.0/tests/test_auth.py` & `ckanext-contact-2.3.0/tests/unit/test_auth.py`

 * *Files identical despite different names*

### Comparing `ckanext-contact-2.2.0/tests/test_helpers.py` & `ckanext-contact-2.3.0/tests/unit/test_helpers.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,18 +7,28 @@
 
 class TestBuildSubject:
     def test_no_config_all_defaults(self):
         subject = build_subject()
         assert subject == 'Contact/Question from visitor'
 
     def test_no_config_pass_default_subject(self):
-        subject_default = 'TEST SUBJECT'
+        default = 'TEST SUBJECT'
+
+        subject = build_subject(default=default)
+        assert subject == default
 
-        subject = build_subject(subject_default=subject_default)
-        assert subject == subject_default
+    def test_user_specified(self):
+        subject = 'YES PLEASE EMAIL'
+        assert build_subject(subject=subject) == subject
+
+    @pytest.mark.ckan_config('ckanext.contact.subject', 'TEST SUBJECT')
+    def test_user_specified_and_defaults(self):
+        subject = 'YES PLEASE EMAIL'
+
+        assert build_subject(subject=subject) == subject
 
     def test_no_config_pass_default_timestamp_false(self):
         timestamp_default = False
 
         subject = build_subject(timestamp_default=timestamp_default)
         assert subject == 'Contact/Question from visitor'
 
@@ -34,15 +44,17 @@
         assert subject == f'Contact/Question from visitor [{timestamp}]'
 
     @freeze_time("2021-01-01")
     def test_no_config_pass_both(self):
         subject_default = 'TEST SUBJECT'
         timestamp_default = True
 
-        subject = build_subject(subject_default, timestamp_default)
+        subject = build_subject(
+            default=subject_default, timestamp_default=timestamp_default
+        )
 
         timestamp = datetime(2021, 1, 1, tzinfo=timezone.utc).strftime(
             '%Y-%m-%d %H:%M:%S %Z'
         )
         assert subject == f'{subject_default} [{timestamp}]'
 
     @freeze_time("2021-01-01")
@@ -57,7 +69,16 @@
         assert subject == f'TEST SUBJECT [{timestamp}]'
 
     @pytest.mark.ckan_config('ckanext.contact.subject', 'TEST SUBJECT')
     @pytest.mark.ckan_config('ckanext.contact.add_timestamp_to_subject', 'false')
     def test_config_with_timestamp(self):
         subject = build_subject()
         assert subject == 'TEST SUBJECT'
+
+    def test_prefix_not_provided(self):
+        subject = build_subject(subject='TEST')
+        assert subject == 'TEST'
+
+    @pytest.mark.ckan_config('ckanext.contact.subject_prefix', 'PREFIX:')
+    def test_prefix_provided(self):
+        subject = build_subject(subject='TEST')
+        assert subject == 'PREFIX: TEST'
```

