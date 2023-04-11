# Comparing `tmp/berlin-appointment-finder-1.0.1.tar.gz` & `tmp/berlin-appointment-finder-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "berlin-appointment-finder-1.0.1.tar", last modified: Wed Apr  5 13:14:17 2023, max compression
+gzip compressed data, was "berlin-appointment-finder-1.0.2.tar", last modified: Tue Apr 11 08:51:13 2023, max compression
```

## Comparing `berlin-appointment-finder-1.0.1.tar` & `berlin-appointment-finder-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2023-04-05 13:14:17.804482 berlin-appointment-finder-1.0.1/
--rw-------   0 nicolas    (501) staff       (20)     1073 2022-01-25 21:16:12.000000 berlin-appointment-finder-1.0.1/LICENSE
--rw-r--r--   0 nicolas    (501) staff       (20)     2358 2023-04-05 13:14:17.803909 berlin-appointment-finder-1.0.1/PKG-INFO
--rw-------   0 nicolas    (501) staff       (20)     1965 2023-04-05 11:56:10.000000 berlin-appointment-finder-1.0.1/README.md
-drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2023-04-05 13:14:17.802501 berlin-appointment-finder-1.0.1/berlin_appointment_finder.egg-info/
--rw-r--r--   0 nicolas    (501) staff       (20)     2358 2023-04-05 13:14:17.000000 berlin-appointment-finder-1.0.1/berlin_appointment_finder.egg-info/PKG-INFO
--rw-r--r--   0 nicolas    (501) staff       (20)      335 2023-04-05 13:14:17.000000 berlin-appointment-finder-1.0.1/berlin_appointment_finder.egg-info/SOURCES.txt
--rw-r--r--   0 nicolas    (501) staff       (20)        1 2023-04-05 13:14:17.000000 berlin-appointment-finder-1.0.1/berlin_appointment_finder.egg-info/dependency_links.txt
--rw-r--r--   0 nicolas    (501) staff       (20)        1 2023-04-05 11:21:55.000000 berlin-appointment-finder-1.0.1/berlin_appointment_finder.egg-info/not-zip-safe
--rw-r--r--   0 nicolas    (501) staff       (20)       87 2023-04-05 13:14:17.000000 berlin-appointment-finder-1.0.1/berlin_appointment_finder.egg-info/requires.txt
--rw-r--r--   0 nicolas    (501) staff       (20)        1 2023-04-05 13:14:17.000000 berlin-appointment-finder-1.0.1/berlin_appointment_finder.egg-info/top_level.txt
-drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2023-04-05 13:14:17.803172 berlin-appointment-finder-1.0.1/bin/
--rwxr-xr-x   0 nicolas    (501) staff       (20)     2259 2023-04-05 12:26:04.000000 berlin-appointment-finder-1.0.1/bin/appointments
--rw-r--r--   0 nicolas    (501) staff       (20)       38 2023-04-05 13:14:17.804623 berlin-appointment-finder-1.0.1/setup.cfg
--rw-r--r--   0 nicolas    (501) staff       (20)      859 2023-04-05 12:25:30.000000 berlin-appointment-finder-1.0.1/setup.py
+drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2023-04-11 08:51:13.929165 berlin-appointment-finder-1.0.2/
+-rw-------   0 nicolas    (501) staff       (20)     1073 2022-01-25 21:16:12.000000 berlin-appointment-finder-1.0.2/LICENSE
+-rw-r--r--   0 nicolas    (501) staff       (20)     2358 2023-04-11 08:51:13.928381 berlin-appointment-finder-1.0.2/PKG-INFO
+-rw-------   0 nicolas    (501) staff       (20)     1965 2023-04-05 11:56:10.000000 berlin-appointment-finder-1.0.2/README.md
+drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2023-04-11 08:51:13.879540 berlin-appointment-finder-1.0.2/appointments/
+-rw-r--r--   0 nicolas    (501) staff       (20)        0 2023-04-11 08:41:36.000000 berlin-appointment-finder-1.0.2/appointments/__init__.py
+-rw-r--r--   0 nicolas    (501) staff       (20)     6729 2023-04-05 14:58:26.000000 berlin-appointment-finder-1.0.2/appointments/appointments.py
+drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2023-04-11 08:51:13.926106 berlin-appointment-finder-1.0.2/berlin_appointment_finder.egg-info/
+-rw-r--r--   0 nicolas    (501) staff       (20)     2358 2023-04-11 08:51:13.000000 berlin-appointment-finder-1.0.2/berlin_appointment_finder.egg-info/PKG-INFO
+-rw-r--r--   0 nicolas    (501) staff       (20)      389 2023-04-11 08:51:13.000000 berlin-appointment-finder-1.0.2/berlin_appointment_finder.egg-info/SOURCES.txt
+-rw-r--r--   0 nicolas    (501) staff       (20)        1 2023-04-11 08:51:13.000000 berlin-appointment-finder-1.0.2/berlin_appointment_finder.egg-info/dependency_links.txt
+-rw-r--r--   0 nicolas    (501) staff       (20)        1 2023-04-05 11:21:55.000000 berlin-appointment-finder-1.0.2/berlin_appointment_finder.egg-info/not-zip-safe
+-rw-r--r--   0 nicolas    (501) staff       (20)       85 2023-04-11 08:51:13.000000 berlin-appointment-finder-1.0.2/berlin_appointment_finder.egg-info/requires.txt
+-rw-r--r--   0 nicolas    (501) staff       (20)       13 2023-04-11 08:51:13.000000 berlin-appointment-finder-1.0.2/berlin_appointment_finder.egg-info/top_level.txt
+drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2023-04-11 08:51:13.926954 berlin-appointment-finder-1.0.2/bin/
+-rwxr-xr-x   0 nicolas    (501) staff       (20)     2259 2023-04-05 12:26:04.000000 berlin-appointment-finder-1.0.2/bin/appointments
+-rw-r--r--   0 nicolas    (501) staff       (20)       38 2023-04-11 08:51:13.929367 berlin-appointment-finder-1.0.2/setup.cfg
+-rw-r--r--   0 nicolas    (501) staff       (20)      857 2023-04-11 08:49:57.000000 berlin-appointment-finder-1.0.2/setup.py
```

### Comparing `berlin-appointment-finder-1.0.1/LICENSE` & `berlin-appointment-finder-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `berlin-appointment-finder-1.0.1/PKG-INFO` & `berlin-appointment-finder-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: berlin-appointment-finder
-Version: 1.0.1
+Version: 1.0.2
 Summary: Finds appointments at the Berlin Bürgeramt, broadcasts them via websockets
 Home-page: https://github.com/nicbou/burgeramt-appointments-websockets
 Author: Nicolas Bouliane
 Author-email: contact@nicolasbouliane.com
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `berlin-appointment-finder-1.0.1/README.md` & `berlin-appointment-finder-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `berlin-appointment-finder-1.0.1/berlin_appointment_finder.egg-info/PKG-INFO` & `berlin-appointment-finder-1.0.2/berlin_appointment_finder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: berlin-appointment-finder
-Version: 1.0.1
+Version: 1.0.2
 Summary: Finds appointments at the Berlin Bürgeramt, broadcasts them via websockets
 Home-page: https://github.com/nicbou/burgeramt-appointments-websockets
 Author: Nicolas Bouliane
 Author-email: contact@nicolasbouliane.com
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `berlin-appointment-finder-1.0.1/bin/appointments` & `berlin-appointment-finder-1.0.2/bin/appointments`

 * *Files identical despite different names*

### Comparing `berlin-appointment-finder-1.0.1/setup.py` & `berlin-appointment-finder-1.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 long_description = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name='berlin-appointment-finder',
-    version='1.0.1',
+    version='1.0.2',
     description='Finds appointments at the Berlin Bürgeramt, broadcasts them via websockets',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/nicbou/burgeramt-appointments-websockets',
     author='Nicolas Bouliane',
     author_email='contact@nicolasbouliane.com',
     license='MIT',
     packages=find_packages(),
     scripts=['bin/appointments'],
     python_requires='>=3.10',
     install_requires=[
+        'aiohttp==3.8.4',
         'beautifulsoup4==4.10.0',
         'chime==0.7.0',
         'pytz',
-        'requests==2.27.1',
         'websockets==10.1',
         'lxml==4.7.1',
     ],
     zip_safe=False,
 )
```

