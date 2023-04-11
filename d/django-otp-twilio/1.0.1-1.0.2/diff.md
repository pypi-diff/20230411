# Comparing `tmp/django-otp-twilio-1.0.1.tar.gz` & `tmp/django-otp-twilio-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-otp-twilio-1.0.1.tar", last modified: Mon Nov 29 19:11:12 2021, max compression
+gzip compressed data, was "dist/django-otp-twilio-1.0.2.tar", last modified: Tue Apr 11 17:57:02 2023, max compression
```

## Comparing `django-otp-twilio-1.0.1.tar` & `django-otp-twilio-1.0.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 psagers    (502) staff       (20)        0 2021-11-29 19:11:12.000000 django-otp-twilio-1.0.1/
--rw-r--r--   0 psagers    (502) staff       (20)     4442 2021-11-29 19:08:15.000000 django-otp-twilio-1.0.1/CHANGES.rst
--rw-r--r--   0 psagers    (502) staff       (20)     1297 2019-08-22 18:26:39.000000 django-otp-twilio-1.0.1/LICENSE
--rw-r--r--   0 psagers    (502) staff       (20)      100 2019-08-26 17:57:03.000000 django-otp-twilio-1.0.1/MANIFEST.in
--rw-r--r--   0 psagers    (502) staff       (20)     1549 2021-11-29 19:11:12.000000 django-otp-twilio-1.0.1/PKG-INFO
--rw-r--r--   0 psagers    (502) staff       (20)      710 2020-05-06 19:43:58.000000 django-otp-twilio-1.0.1/README.rst
-drwxr-xr-x   0 psagers    (502) staff       (20)        0 2021-11-29 19:11:12.000000 django-otp-twilio-1.0.1/docs/
--rw-r--r--   0 psagers    (502) staff       (20)     5709 2019-08-22 18:26:39.000000 django-otp-twilio-1.0.1/docs/Makefile
-drwxr-xr-x   0 psagers    (502) staff       (20)        0 2021-11-29 19:11:12.000000 django-otp-twilio-1.0.1/docs/ext/
--rw-r--r--   0 psagers    (502) staff       (20)      217 2019-08-26 20:14:44.000000 django-otp-twilio-1.0.1/docs/ext/otpdocs.py
-drwxr-xr-x   0 psagers    (502) staff       (20)        0 2021-11-29 19:11:12.000000 django-otp-twilio-1.0.1/docs/source/
--rw-r--r--   0 psagers    (502) staff       (20)       54 2019-08-26 17:35:13.000000 django-otp-twilio-1.0.1/docs/source/changes.rst
--rw-r--r--   0 psagers    (502) staff       (20)     8876 2021-11-29 19:08:15.000000 django-otp-twilio-1.0.1/docs/source/conf.py
--rw-r--r--   0 psagers    (502) staff       (20)     2643 2020-05-06 19:26:34.000000 django-otp-twilio-1.0.1/docs/source/index.rst
--rw-r--r--   0 psagers    (502) staff       (20)      147 2021-11-29 19:11:12.000000 django-otp-twilio-1.0.1/setup.cfg
--rwxr-xr-x   0 psagers    (502) staff       (20)     1087 2021-11-29 19:08:59.000000 django-otp-twilio-1.0.1/setup.py
-drwxr-xr-x   0 psagers    (502) staff       (20)        0 2021-11-29 19:11:12.000000 django-otp-twilio-1.0.1/src/
-drwxr-xr-x   0 psagers    (502) staff       (20)        0 2021-11-29 19:11:12.000000 django-otp-twilio-1.0.1/src/django_otp_twilio.egg-info/
--rw-r--r--   0 psagers    (502) staff       (20)     1549 2021-11-29 19:11:12.000000 django-otp-twilio-1.0.1/src/django_otp_twilio.egg-info/PKG-INFO
--rw-r--r--   0 psagers    (502) staff       (20)      752 2021-11-29 19:11:12.000000 django-otp-twilio-1.0.1/src/django_otp_twilio.egg-info/SOURCES.txt
--rw-r--r--   0 psagers    (502) staff       (20)        1 2021-11-29 19:11:12.000000 django-otp-twilio-1.0.1/src/django_otp_twilio.egg-info/dependency_links.txt
--rw-r--r--   0 psagers    (502) staff       (20)       27 2021-11-29 19:11:12.000000 django-otp-twilio-1.0.1/src/django_otp_twilio.egg-info/requires.txt
--rw-r--r--   0 psagers    (502) staff       (20)       11 2021-11-29 19:11:12.000000 django-otp-twilio-1.0.1/src/django_otp_twilio.egg-info/top_level.txt
-drwxr-xr-x   0 psagers    (502) staff       (20)        0 2021-11-29 19:11:12.000000 django-otp-twilio-1.0.1/src/otp_twilio/
--rw-r--r--   0 psagers    (502) staff       (20)        0 2021-11-29 18:39:10.000000 django-otp-twilio-1.0.1/src/otp_twilio/__init__.py
--rw-r--r--   0 psagers    (502) staff       (20)      667 2020-05-06 19:28:33.000000 django-otp-twilio-1.0.1/src/otp_twilio/admin.py
--rw-r--r--   0 psagers    (502) staff       (20)      146 2021-11-29 18:29:47.000000 django-otp-twilio-1.0.1/src/otp_twilio/apps.py
--rw-r--r--   0 psagers    (502) staff       (20)      965 2020-05-06 18:01:36.000000 django-otp-twilio-1.0.1/src/otp_twilio/conf.py
-drwxr-xr-x   0 psagers    (502) staff       (20)        0 2021-11-29 19:11:12.000000 django-otp-twilio-1.0.1/src/otp_twilio/migrations/
--rw-r--r--   0 psagers    (502) staff       (20)     1411 2020-05-06 18:53:59.000000 django-otp-twilio-1.0.1/src/otp_twilio/migrations/0001_initial.py
--rw-r--r--   0 psagers    (502) staff       (20)      540 2019-08-26 17:20:36.000000 django-otp-twilio-1.0.1/src/otp_twilio/migrations/0002_last_t.py
--rw-r--r--   0 psagers    (502) staff       (20)      463 2019-08-22 18:26:39.000000 django-otp-twilio-1.0.1/src/otp_twilio/migrations/0003_longer_number.py
--rw-r--r--   0 psagers    (502) staff       (20)     1465 2020-05-06 17:59:54.000000 django-otp-twilio-1.0.1/src/otp_twilio/migrations/0004_sidechanneldevice.py
--rw-r--r--   0 psagers    (502) staff       (20)        0 2019-08-22 18:26:39.000000 django-otp-twilio-1.0.1/src/otp_twilio/migrations/__init__.py
--rw-r--r--   0 psagers    (502) staff       (20)     4010 2021-04-07 15:38:02.000000 django-otp-twilio-1.0.1/src/otp_twilio/models.py
--rw-r--r--   0 psagers    (502) staff       (20)     3209 2020-05-06 18:53:59.000000 django-otp-twilio-1.0.1/src/otp_twilio/tests.py
+drwxr-xr-x   0 psagers   (1000) psagers   (1000)        0 2023-04-11 17:57:02.000000 django-otp-twilio-1.0.2/
+-rw-rw-r--   0 psagers   (1000) psagers   (1000)     4623 2023-04-11 17:56:33.000000 django-otp-twilio-1.0.2/CHANGES.rst
+-rw-rw-r--   0 psagers   (1000) psagers   (1000)     1297 2022-01-13 18:26:54.000000 django-otp-twilio-1.0.2/LICENSE
+-rw-rw-r--   0 psagers   (1000) psagers   (1000)      100 2022-01-13 18:26:54.000000 django-otp-twilio-1.0.2/MANIFEST.in
+-rw-r--r--   0 psagers   (1000) psagers   (1000)     1549 2023-04-11 17:57:02.000000 django-otp-twilio-1.0.2/PKG-INFO
+-rw-rw-r--   0 psagers   (1000) psagers   (1000)      710 2022-01-13 18:26:54.000000 django-otp-twilio-1.0.2/README.rst
+drwxr-xr-x   0 psagers   (1000) psagers   (1000)        0 2023-04-11 17:57:02.000000 django-otp-twilio-1.0.2/docs/
+-rw-rw-r--   0 psagers   (1000) psagers   (1000)     5709 2022-01-13 18:26:54.000000 django-otp-twilio-1.0.2/docs/Makefile
+drwxr-xr-x   0 psagers   (1000) psagers   (1000)        0 2023-04-11 17:57:02.000000 django-otp-twilio-1.0.2/docs/ext/
+-rw-rw-r--   0 psagers   (1000) psagers   (1000)      217 2022-01-13 18:26:54.000000 django-otp-twilio-1.0.2/docs/ext/otpdocs.py
+drwxr-xr-x   0 psagers   (1000) psagers   (1000)        0 2023-04-11 17:57:02.000000 django-otp-twilio-1.0.2/docs/source/
+-rw-rw-r--   0 psagers   (1000) psagers   (1000)       54 2022-01-13 18:26:54.000000 django-otp-twilio-1.0.2/docs/source/changes.rst
+-rw-rw-r--   0 psagers   (1000) psagers   (1000)     8876 2023-04-11 17:56:33.000000 django-otp-twilio-1.0.2/docs/source/conf.py
+-rw-r--r--   0 psagers   (1000) psagers   (1000)     3029 2023-04-11 17:51:34.000000 django-otp-twilio-1.0.2/docs/source/index.rst
+-rw-rw-r--   0 psagers   (1000) psagers   (1000)      147 2023-04-11 17:57:02.000000 django-otp-twilio-1.0.2/setup.cfg
+-rwxrwxr-x   0 psagers   (1000) psagers   (1000)     1087 2023-04-11 17:56:33.000000 django-otp-twilio-1.0.2/setup.py
+drwxr-xr-x   0 psagers   (1000) psagers   (1000)        0 2023-04-11 17:57:02.000000 django-otp-twilio-1.0.2/src/
+drwxr-xr-x   0 psagers   (1000) psagers   (1000)        0 2023-04-11 17:57:02.000000 django-otp-twilio-1.0.2/src/django_otp_twilio.egg-info/
+-rw-r--r--   0 psagers   (1000) psagers   (1000)     1549 2023-04-11 17:57:02.000000 django-otp-twilio-1.0.2/src/django_otp_twilio.egg-info/PKG-INFO
+-rw-r--r--   0 psagers   (1000) psagers   (1000)      752 2023-04-11 17:57:02.000000 django-otp-twilio-1.0.2/src/django_otp_twilio.egg-info/SOURCES.txt
+-rw-r--r--   0 psagers   (1000) psagers   (1000)        1 2023-04-11 17:57:02.000000 django-otp-twilio-1.0.2/src/django_otp_twilio.egg-info/dependency_links.txt
+-rw-r--r--   0 psagers   (1000) psagers   (1000)       27 2023-04-11 17:57:02.000000 django-otp-twilio-1.0.2/src/django_otp_twilio.egg-info/requires.txt
+-rw-r--r--   0 psagers   (1000) psagers   (1000)       11 2023-04-11 17:57:02.000000 django-otp-twilio-1.0.2/src/django_otp_twilio.egg-info/top_level.txt
+drwxr-xr-x   0 psagers   (1000) psagers   (1000)        0 2023-04-11 17:57:02.000000 django-otp-twilio-1.0.2/src/otp_twilio/
+-rw-rw-r--   0 psagers   (1000) psagers   (1000)        0 2022-01-13 18:26:54.000000 django-otp-twilio-1.0.2/src/otp_twilio/__init__.py
+-rw-rw-r--   0 psagers   (1000) psagers   (1000)      667 2022-01-13 18:26:54.000000 django-otp-twilio-1.0.2/src/otp_twilio/admin.py
+-rw-rw-r--   0 psagers   (1000) psagers   (1000)      146 2022-01-13 18:26:54.000000 django-otp-twilio-1.0.2/src/otp_twilio/apps.py
+-rw-r--r--   0 psagers   (1000) psagers   (1000)     1053 2023-04-11 17:51:34.000000 django-otp-twilio-1.0.2/src/otp_twilio/conf.py
+drwxr-xr-x   0 psagers   (1000) psagers   (1000)        0 2023-04-11 17:57:02.000000 django-otp-twilio-1.0.2/src/otp_twilio/migrations/
+-rw-rw-r--   0 psagers   (1000) psagers   (1000)     1411 2022-01-13 18:26:54.000000 django-otp-twilio-1.0.2/src/otp_twilio/migrations/0001_initial.py
+-rw-rw-r--   0 psagers   (1000) psagers   (1000)      540 2022-01-13 18:26:54.000000 django-otp-twilio-1.0.2/src/otp_twilio/migrations/0002_last_t.py
+-rw-rw-r--   0 psagers   (1000) psagers   (1000)      463 2022-01-13 18:26:54.000000 django-otp-twilio-1.0.2/src/otp_twilio/migrations/0003_longer_number.py
+-rw-rw-r--   0 psagers   (1000) psagers   (1000)     1465 2022-01-13 18:26:54.000000 django-otp-twilio-1.0.2/src/otp_twilio/migrations/0004_sidechanneldevice.py
+-rw-rw-r--   0 psagers   (1000) psagers   (1000)        0 2022-01-13 18:26:54.000000 django-otp-twilio-1.0.2/src/otp_twilio/migrations/__init__.py
+-rw-r--r--   0 psagers   (1000) psagers   (1000)     4072 2023-04-11 17:51:34.000000 django-otp-twilio-1.0.2/src/otp_twilio/models.py
+-rw-rw-r--   0 psagers   (1000) psagers   (1000)     3209 2022-01-13 18:26:54.000000 django-otp-twilio-1.0.2/src/otp_twilio/tests.py
```

### Comparing `django-otp-twilio-1.0.1/CHANGES.rst` & `django-otp-twilio-1.0.2/CHANGES.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,19 @@
+v1.0.2 - April 11, 2023 - New configuration options
+--------------------------------------------------------------------------------
+
+- Allow configuration of API URL and API key.
+
+
 v1.0.1 - November 29, 2021 - Forward compatibility
 --------------------------------------------------------------------------------
 
 Default to AutoField to avoid spurious migrations.
 
 
-
 v1.0.0 - August 13, 2020 - Update test matrix
 ------------------------------------------------------------
 
 - Added Django 3.1 to the test environments and fixed deprecation warnings.
 
 - Version bumped to align with the core django-otp project.
```

### Comparing `django-otp-twilio-1.0.1/LICENSE` & `django-otp-twilio-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-otp-twilio-1.0.1/PKG-INFO` & `django-otp-twilio-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-otp-twilio
-Version: 1.0.1
+Version: 1.0.2
 Summary: A django-otp plugin that delivers tokens via Twilio's SMS service.
 Home-page: https://github.com/django-otp/django-otp-twilio
 Author: Peter Sagerson
 Author-email: psagers@ignorare.net
 License: BSD
 Project-URL: Documentation, https://django-otp-twilio.readthedocs.io/
 Project-URL: Source, https://github.com/django-otp/django-otp-twilio
```

### Comparing `django-otp-twilio-1.0.1/README.rst` & `django-otp-twilio-1.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `django-otp-twilio-1.0.1/docs/Makefile` & `django-otp-twilio-1.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-otp-twilio-1.0.1/docs/source/conf.py` & `django-otp-twilio-1.0.2/docs/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 copyright = u'2012, Peter Sagerson'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The full version, including alpha/beta/rc tags.
-release = '1.0.1'
+release = '1.0.2'
 
 # The short X.Y version.
 version = '.'.join(release.split('.')[:2])
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 # language = None
```

### Comparing `django-otp-twilio-1.0.1/docs/source/index.rst` & `django-otp-twilio-1.0.2/docs/source/index.rst`

 * *Files 10% similar despite different names*

```diff
@@ -41,30 +41,46 @@
 
 .. autoclass:: otp_twilio.admin.TwilioSMSDeviceAdmin
 
 
 Settings
 --------
 
+.. setting:: OTP_TWILIO_URL
+
+**OTP_TWILIO_URL**
+
+Default: ``"https://api.twilio.com""``
+
+Twilio API URL. This can be used to change edge location
+
 .. setting:: OTP_TWILIO_ACCOUNT
 
 **OTP_TWILIO_ACCOUNT**
 
 Default: ``None``
 
 Your Twilio account ID.
 
+.. setting:: OTP_TWILIO_API_KEY
+
+**OTP_TWILIO_API_KEY**
+
+Default: ``None``
+
+Your Twilio API key, if no API key is specified requests are made using the Twilio Account ID.
+
 
 .. setting:: OTP_TWILIO_AUTH
 
 **OTP_TWILIO_AUTH**
 
 Default: ``None``
 
-Your Twilio auth token.
+Your Twilio auth token used for API requests. (Either API Key token or account auth token)
 
 
 .. setting:: OTP_TWILIO_CHALLENGE_MESSAGE
 
 **OTP_TWILIO_CHALLENGE_MESSAGE**
 
 Default: ``"Sent by SMS"``
```

### Comparing `django-otp-twilio-1.0.1/setup.py` & `django-otp-twilio-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 
 from setuptools import setup, find_packages
 
 
 setup(
     name='django-otp-twilio',
-    version='1.0.1',
+    version='1.0.2',
     description="A django-otp plugin that delivers tokens via Twilio's SMS service.",
     author="Peter Sagerson",
     author_email='psagers@ignorare.net',
     url='https://github.com/django-otp/django-otp-twilio',
     project_urls={
         "Documentation": 'https://django-otp-twilio.readthedocs.io/',
         "Source": 'https://github.com/django-otp/django-otp-twilio',
```

### Comparing `django-otp-twilio-1.0.1/src/django_otp_twilio.egg-info/PKG-INFO` & `django-otp-twilio-1.0.2/src/django_otp_twilio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-otp-twilio
-Version: 1.0.1
+Version: 1.0.2
 Summary: A django-otp plugin that delivers tokens via Twilio's SMS service.
 Home-page: https://github.com/django-otp/django-otp-twilio
 Author: Peter Sagerson
 Author-email: psagers@ignorare.net
 License: BSD
 Project-URL: Documentation, https://django-otp-twilio.readthedocs.io/
 Project-URL: Source, https://github.com/django-otp/django-otp-twilio
```

### Comparing `django-otp-twilio-1.0.1/src/django_otp_twilio.egg-info/SOURCES.txt` & `django-otp-twilio-1.0.2/src/django_otp_twilio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-otp-twilio-1.0.1/src/otp_twilio/admin.py` & `django-otp-twilio-1.0.2/src/otp_twilio/admin.py`

 * *Files identical despite different names*

### Comparing `django-otp-twilio-1.0.1/src/otp_twilio/conf.py` & `django-otp-twilio-1.0.2/src/otp_twilio/conf.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 class Settings(object):
     """
     This is a simple class to take the place of the global settings object. An
     instance will contain all of our settings as attributes, with default
     values if they are not specified by the configuration.
     """
     _defaults = {
+        'OTP_TWILIO_URL': "https://api.twilio.com",
         'OTP_TWILIO_ACCOUNT': None,
+        'OTP_TWILIO_API_KEY': None,
         'OTP_TWILIO_AUTH': None,
         'OTP_TWILIO_CHALLENGE_MESSAGE': "Sent by SMS",
         'OTP_TWILIO_FROM': None,
         'OTP_TWILIO_NO_DELIVERY': False,
         'OTP_TWILIO_THROTTLE_FACTOR': 1,
         'OTP_TWILIO_TOKEN_TEMPLATE': '{token}',
         'OTP_TWILIO_TOKEN_VALIDITY': 30,
```

### Comparing `django-otp-twilio-1.0.1/src/otp_twilio/migrations/0001_initial.py` & `django-otp-twilio-1.0.2/src/otp_twilio/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-otp-twilio-1.0.1/src/otp_twilio/migrations/0002_last_t.py` & `django-otp-twilio-1.0.2/src/otp_twilio/migrations/0002_last_t.py`

 * *Files identical despite different names*

### Comparing `django-otp-twilio-1.0.1/src/otp_twilio/migrations/0004_sidechanneldevice.py` & `django-otp-twilio-1.0.2/src/otp_twilio/migrations/0004_sidechanneldevice.py`

 * *Files identical despite different names*

### Comparing `django-otp-twilio-1.0.1/src/otp_twilio/models.py` & `django-otp-twilio-1.0.2/src/otp_twilio/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,24 +73,24 @@
         challenge = settings.OTP_TWILIO_CHALLENGE_MESSAGE.format(token=self.token)
 
         return challenge
 
     def _deliver_token(self, token):
         self._validate_config()
 
-        url = 'https://api.twilio.com/2010-04-01/Accounts/{0}/Messages.json'.format(settings.OTP_TWILIO_ACCOUNT)
+        url = '{0}/2010-04-01/Accounts/{1}/Messages.json'.format(settings.OTP_TWILIO_URL, settings.OTP_TWILIO_ACCOUNT)
         data = {
             'From': settings.OTP_TWILIO_FROM,
             'To': self.number,
             'Body': str(token),
         }
 
         response = requests.post(
             url, data=data,
-            auth=(settings.OTP_TWILIO_ACCOUNT, settings.OTP_TWILIO_AUTH)
+            auth=(settings.TWILIO_API_KEY if settings.TWILIO_API_KEY else settings.OTP_TWILIO_ACCOUNT, settings.OTP_TWILIO_AUTH)
         )
 
         try:
             response.raise_for_status()
         except Exception as e:
             logger.exception('Error sending token by Twilio SMS: {0}'.format(e))
             raise
```

### Comparing `django-otp-twilio-1.0.1/src/otp_twilio/tests.py` & `django-otp-twilio-1.0.2/src/otp_twilio/tests.py`

 * *Files identical despite different names*

