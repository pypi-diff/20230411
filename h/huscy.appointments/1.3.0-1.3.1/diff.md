# Comparing `tmp/huscy.appointments-1.3.0.tar.gz` & `tmp/huscy.appointments-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huscy.appointments-1.3.0.tar", last modified: Tue Dec  6 19:02:26 2022, max compression
+gzip compressed data, was "huscy.appointments-1.3.1.tar", last modified: Tue Apr 11 14:02:49 2023, max compression
```

## Comparing `huscy.appointments-1.3.0.tar` & `huscy.appointments-1.3.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-06 19:02:26.123607 huscy.appointments-1.3.0/
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1030 2022-12-06 19:02:26.123607 huscy.appointments-1.3.0/PKG-INFO
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1496 2022-12-06 11:58:45.000000 huscy.appointments-1.3.0/README.md
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-06 19:02:26.111607 huscy.appointments-1.3.0/huscy/
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-06 19:02:26.115607 huscy.appointments-1.3.0/huscy/appointments/
--rw-r--r--   0 jenkins    (111) jenkins    (115)       89 2022-12-06 17:32:43.000000 huscy.appointments-1.3.0/huscy/appointments/__init__.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      226 2020-04-27 18:13:51.000000 huscy.appointments-1.3.0/huscy/appointments/admin.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      277 2022-12-06 17:32:43.000000 huscy.appointments-1.3.0/huscy/appointments/api_urls.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      190 2022-06-23 09:02:55.000000 huscy.appointments-1.3.0/huscy/appointments/apps.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1472 2020-04-27 18:13:51.000000 huscy.appointments-1.3.0/huscy/appointments/feed.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      577 2020-04-27 18:13:51.000000 huscy.appointments-1.3.0/huscy/appointments/filters.py
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-06 19:02:26.123607 huscy.appointments-1.3.0/huscy/appointments/migrations/
--rw-r--r--   0 jenkins    (111) jenkins    (115)     2834 2020-04-27 18:13:51.000000 huscy.appointments-1.3.0/huscy/appointments/migrations/0001_initial.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     4178 2020-04-27 18:13:51.000000 huscy.appointments-1.3.0/huscy/appointments/migrations/0002_auto_20200226_0735.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      453 2020-04-27 18:13:51.000000 huscy.appointments-1.3.0/huscy/appointments/migrations/0003_auto_20200226_0756.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1251 2021-10-26 09:34:30.000000 huscy.appointments-1.3.0/huscy/appointments/migrations/0004_auto_20211026_0424.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)        0 2020-04-27 18:13:51.000000 huscy.appointments-1.3.0/huscy/appointments/migrations/__init__.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     2947 2020-04-27 18:13:51.000000 huscy.appointments-1.3.0/huscy/appointments/models.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     2164 2020-04-27 18:13:51.000000 huscy.appointments-1.3.0/huscy/appointments/serializers.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     5220 2022-06-23 09:02:55.000000 huscy.appointments-1.3.0/huscy/appointments/services.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      266 2022-12-06 17:32:43.000000 huscy.appointments-1.3.0/huscy/appointments/urls.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      424 2020-04-27 18:13:51.000000 huscy.appointments-1.3.0/huscy/appointments/validators.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     2206 2020-04-27 18:13:51.000000 huscy.appointments-1.3.0/huscy/appointments/views.py
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-06 19:02:26.111607 huscy.appointments-1.3.0/huscy.appointments.egg-info/
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1030 2022-12-06 19:02:25.000000 huscy.appointments-1.3.0/huscy.appointments.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (111) jenkins    (115)      842 2022-12-06 19:02:25.000000 huscy.appointments-1.3.0/huscy.appointments.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)        1 2022-12-06 19:02:25.000000 huscy.appointments-1.3.0/huscy.appointments.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)      129 2022-12-06 19:02:25.000000 huscy.appointments-1.3.0/huscy.appointments.egg-info/requires.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)        6 2022-12-06 19:02:25.000000 huscy.appointments-1.3.0/huscy.appointments.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)       38 2022-12-06 19:02:26.123607 huscy.appointments-1.3.0/setup.cfg
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1358 2022-12-06 11:58:45.000000 huscy.appointments-1.3.0/setup.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-11 14:02:49.864089 huscy.appointments-1.3.1/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1036 2023-04-11 14:02:49.864089 huscy.appointments-1.3.1/PKG-INFO
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1496 2023-04-11 10:53:38.000000 huscy.appointments-1.3.1/README.md
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-11 14:02:49.856089 huscy.appointments-1.3.1/huscy/
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-11 14:02:49.864089 huscy.appointments-1.3.1/huscy/appointments/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       89 2023-04-11 10:53:38.000000 huscy.appointments-1.3.1/huscy/appointments/__init__.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      226 2020-04-27 18:13:51.000000 huscy.appointments-1.3.1/huscy/appointments/admin.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      277 2022-12-06 17:32:43.000000 huscy.appointments-1.3.1/huscy/appointments/api_urls.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      190 2022-06-23 09:02:55.000000 huscy.appointments-1.3.1/huscy/appointments/apps.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1472 2020-04-27 18:13:51.000000 huscy.appointments-1.3.1/huscy/appointments/feed.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      577 2020-04-27 18:13:51.000000 huscy.appointments-1.3.1/huscy/appointments/filters.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-11 14:02:49.864089 huscy.appointments-1.3.1/huscy/appointments/migrations/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     2834 2020-04-27 18:13:51.000000 huscy.appointments-1.3.1/huscy/appointments/migrations/0001_initial.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     4178 2020-04-27 18:13:51.000000 huscy.appointments-1.3.1/huscy/appointments/migrations/0002_auto_20200226_0735.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      453 2020-04-27 18:13:51.000000 huscy.appointments-1.3.1/huscy/appointments/migrations/0003_auto_20200226_0756.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1251 2021-10-26 09:34:30.000000 huscy.appointments-1.3.1/huscy/appointments/migrations/0004_auto_20211026_0424.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        0 2020-04-27 18:13:51.000000 huscy.appointments-1.3.1/huscy/appointments/migrations/__init__.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     2765 2023-04-11 10:53:38.000000 huscy.appointments-1.3.1/huscy/appointments/models.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     2164 2020-04-27 18:13:51.000000 huscy.appointments-1.3.1/huscy/appointments/serializers.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     5194 2023-04-11 10:53:38.000000 huscy.appointments-1.3.1/huscy/appointments/services.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      266 2022-12-06 17:32:43.000000 huscy.appointments-1.3.1/huscy/appointments/urls.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      424 2020-04-27 18:13:51.000000 huscy.appointments-1.3.1/huscy/appointments/validators.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     2206 2020-04-27 18:13:51.000000 huscy.appointments-1.3.1/huscy/appointments/views.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-11 14:02:49.860089 huscy.appointments-1.3.1/huscy.appointments.egg-info/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1036 2023-04-11 14:02:49.000000 huscy.appointments-1.3.1/huscy.appointments.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      842 2023-04-11 14:02:49.000000 huscy.appointments-1.3.1/huscy.appointments.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        1 2023-04-11 14:02:49.000000 huscy.appointments-1.3.1/huscy.appointments.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      129 2023-04-11 14:02:49.000000 huscy.appointments-1.3.1/huscy.appointments.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        6 2023-04-11 14:02:49.000000 huscy.appointments-1.3.1/huscy.appointments.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       38 2023-04-11 14:02:49.864089 huscy.appointments-1.3.1/setup.cfg
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1364 2023-04-11 10:53:38.000000 huscy.appointments-1.3.1/setup.py
```

### Comparing `huscy.appointments-1.3.0/PKG-INFO` & `huscy.appointments-1.3.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: huscy.appointments
-Version: 1.3.0
+Version: 1.3.1
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Alexander Tyapkov, Mathias Goldau, Stefan Bunde
 Author-email: tyapkov@gmail.com, goldau@cbs.mpg.de, stefanbunde+git@posteo.de
 License: AGPLv3+
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Provides-Extra: development
 Provides-Extra: testing
```

### Comparing `huscy.appointments-1.3.0/README.md` & `huscy.appointments-1.3.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 ![Django Versions](https://img.shields.io/pypi/djversions/huscy-appointments)
 
 
 
 Requirements
 ------
 
-- Python 3.7+
+- Python 3.8+
 - A supported version of Django
 
-Tox tests on Django versions 3.2, 4.0 and 4.1.
+Tox tests on Django versions 3.2, 4.1 and 4.2.
 
 
 
 Installation
 ------
 
 To install `husy.appointments` simply run:
```

### Comparing `huscy.appointments-1.3.0/huscy/appointments/feed.py` & `huscy.appointments-1.3.1/huscy/appointments/feed.py`

 * *Files identical despite different names*

### Comparing `huscy.appointments-1.3.0/huscy/appointments/filters.py` & `huscy.appointments-1.3.1/huscy/appointments/filters.py`

 * *Files identical despite different names*

### Comparing `huscy.appointments-1.3.0/huscy/appointments/migrations/0001_initial.py` & `huscy.appointments-1.3.1/huscy/appointments/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `huscy.appointments-1.3.0/huscy/appointments/migrations/0002_auto_20200226_0735.py` & `huscy.appointments-1.3.1/huscy/appointments/migrations/0002_auto_20200226_0735.py`

 * *Files identical despite different names*

### Comparing `huscy.appointments-1.3.0/huscy/appointments/migrations/0004_auto_20211026_0424.py` & `huscy.appointments-1.3.1/huscy/appointments/migrations/0004_auto_20211026_0424.py`

 * *Files identical despite different names*

### Comparing `huscy.appointments-1.3.0/huscy/appointments/models.py` & `huscy.appointments-1.3.1/huscy/appointments/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-from enum import Enum
 import secrets
 
 from django.conf import settings
+from django.db import models
 from django.db.models import CASCADE
 from django.db.models import CharField
 from django.db.models import DateTimeField
 from django.db.models import ForeignKey
 from django.db.models import Model
-from django.db.models import PositiveSmallIntegerField
 from django.db.models import TextField
 from django.utils.translation import gettext_lazy as _
 
 
 class Appointment(Model):
     owner = ForeignKey(settings.AUTH_USER_MODEL, on_delete=CASCADE, verbose_name=_('Owner'))
     title = CharField(max_length=255, blank=True, default=_('New appointment'),
@@ -25,30 +24,25 @@
         return str(self.title)
 
     class Meta:
         verbose_name = _('Appointment')
         verbose_name_plural = _('Appointments')
 
 
-class Invitation(Model):
-    class STATUS(Enum):
-        pending = (0, _('Pending'))
-        accepted = (1, _('Accepted'))
-        declined = (2, _('Declined'))
-
-        @classmethod
-        def get_value(cls, member):
-            return cls[member].value[0]
-
-    appointment = ForeignKey(Appointment, on_delete=CASCADE, related_name='invitations',
-                             verbose_name=_('Appointment'))
-    participant = CharField(max_length=128, verbose_name=_('Participant'))
-    status = PositiveSmallIntegerField(choices=[x.value for x in STATUS],
-                                       default=STATUS.get_value('pending'),
-                                       verbose_name=_('Status'))
+class Invitation(models.Model):
+    class STATUS(models.IntegerChoices):
+        pending = 0, _('Pending')
+        accepted = 1, _('Accepted')
+        declined = 2, _('Declined')
+
+    appointment = models.ForeignKey(Appointment, on_delete=CASCADE, related_name='invitations',
+                                    verbose_name=_('Appointment'))
+    participant = models.CharField(_('Participant'), max_length=128)
+    status = models.PositiveSmallIntegerField(_('Status'), choices=STATUS.choices,
+                                              default=STATUS.pending)
 
     def __str__(self):
         return f'{self.appointment.title} -- {self.participant} ({self.get_status_display()})'
 
     class Meta:
         verbose_name = _('Invitation')
         verbose_name_plural = _('Invitations')
```

### Comparing `huscy.appointments-1.3.0/huscy/appointments/serializers.py` & `huscy.appointments-1.3.1/huscy/appointments/serializers.py`

 * *Files identical despite different names*

### Comparing `huscy.appointments-1.3.0/huscy/appointments/services.py` & `huscy.appointments-1.3.1/huscy/appointments/services.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,29 +118,29 @@
     else:
         invitation = (models.Invitation.objects
                                        .select_related('appointment')
                                        .get(appointment_id=appointment, participant=participant))
         warnings.warn('Passing the appointment id to accept_appointment is marked as deprecated. '
                       'Please use appointment object instead.', DeprecationWarning)
 
-    invitation.status = models.Invitation.STATUS.get_value('accepted')
+    invitation.status = models.Invitation.STATUS.accepted
     invitation.save()
     return invitation.appointment
 
 
 def decline_appointment(appointment, participant):
     if isinstance(appointment, models.Appointment):
         invitation = appointment.invitations.get(participant=participant)
     else:
         invitation = (models.Invitation.objects
                                        .select_related('appointment')
                                        .get(appointment_id=appointment, participant=participant))
         warnings.warn('Passing the appointment id to decline_appointment is marked as deprecated. '
                       'Please use appointment object instead.', DeprecationWarning)
 
-    invitation.status = models.Invitation.STATUS.get_value('declined')
+    invitation.status = models.Invitation.STATUS.declined
     invitation.save()
     return invitation.appointment
 
 
 def get_resources():
     return models.Resource.objects.all()
```

### Comparing `huscy.appointments-1.3.0/huscy/appointments/views.py` & `huscy.appointments-1.3.1/huscy/appointments/views.py`

 * *Files identical despite different names*

### Comparing `huscy.appointments-1.3.0/huscy.appointments.egg-info/PKG-INFO` & `huscy.appointments-1.3.1/huscy.appointments.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: huscy.appointments
-Version: 1.3.0
+Version: 1.3.1
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Alexander Tyapkov, Mathias Goldau, Stefan Bunde
 Author-email: tyapkov@gmail.com, goldau@cbs.mpg.de, stefanbunde+git@posteo.de
 License: AGPLv3+
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Provides-Extra: development
 Provides-Extra: testing
```

### Comparing `huscy.appointments-1.3.0/huscy.appointments.egg-info/SOURCES.txt` & `huscy.appointments-1.3.1/huscy.appointments.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `huscy.appointments-1.3.0/setup.py` & `huscy.appointments-1.3.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,18 +26,18 @@
 
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3 :: Only',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Framework :: Django',
         'Framework :: Django :: 3.2',
-        'Framework :: Django :: 4.0',
         'Framework :: Django :: 4.1',
+        'Framework :: Django :: 4.2',
     ],
 )
```

