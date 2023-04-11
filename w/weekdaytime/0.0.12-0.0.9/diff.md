# Comparing `tmp/weekdaytime-0.0.12.tar.gz` & `tmp/weekdaytime-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\weekdaytime-0.0.12.tar", last modified: Tue Apr 11 13:40:08 2023, max compression
+gzip compressed data, was "dist\weekdaytime-0.0.9.tar", last modified: Mon Apr 10 10:57:09 2023, max compression
```

## Comparing `weekdaytime-0.0.12.tar` & `weekdaytime-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 13:40:08.000000 weekdaytime-0.0.12/
--rw-rw-rw-   0        0        0     1091 2023-04-05 09:07:45.000000 weekdaytime-0.0.12/LICENSE
--rw-rw-rw-   0        0        0       34 2023-04-10 10:38:24.000000 weekdaytime-0.0.12/MANIFEST.in
--rw-rw-rw-   0        0        0     4850 2023-04-11 13:40:08.000000 weekdaytime-0.0.12/PKG-INFO
--rw-rw-rw-   0        0        0     4520 2023-04-10 11:34:39.000000 weekdaytime-0.0.12/README.md
--rw-rw-rw-   0        0        0      148 2023-04-11 13:40:08.000000 weekdaytime-0.0.12/setup.cfg
--rw-rw-rw-   0        0        0      516 2023-04-11 13:40:00.000000 weekdaytime-0.0.12/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-11 13:40:08.000000 weekdaytime-0.0.12/weekdaytime/
--rw-rw-rw-   0        0        0     7205 2023-04-11 13:34:57.000000 weekdaytime-0.0.12/weekdaytime/period.py
--rw-rw-rw-   0        0        0     2345 2023-04-08 14:41:13.000000 weekdaytime-0.0.12/weekdaytime/weekdaytime.py
--rw-rw-rw-   0        0        0       90 2023-04-11 13:40:06.000000 weekdaytime-0.0.12/weekdaytime/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 13:40:08.000000 weekdaytime-0.0.12/weekdaytime.egg-info/
--rw-rw-rw-   0        0        0        1 2023-04-11 13:40:08.000000 weekdaytime-0.0.12/weekdaytime.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-10 10:57:09.000000 weekdaytime-0.0.12/weekdaytime.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     4850 2023-04-11 13:40:08.000000 weekdaytime-0.0.12/weekdaytime.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       14 2023-04-11 13:40:08.000000 weekdaytime-0.0.12/weekdaytime.egg-info/requires.txt
--rw-rw-rw-   0        0        0      329 2023-04-11 13:40:08.000000 weekdaytime-0.0.12/weekdaytime.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       12 2023-04-11 13:40:08.000000 weekdaytime-0.0.12/weekdaytime.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-10 10:57:09.000000 weekdaytime-0.0.9/
+-rw-rw-rw-   0        0        0     1091 2023-04-05 09:07:45.000000 weekdaytime-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0       34 2023-04-10 10:38:24.000000 weekdaytime-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     5018 2023-04-10 10:57:09.000000 weekdaytime-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4689 2023-04-10 10:50:15.000000 weekdaytime-0.0.9/README.md
+-rw-rw-rw-   0        0        0      148 2023-04-10 10:57:09.000000 weekdaytime-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      515 2023-04-10 10:50:49.000000 weekdaytime-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 10:57:09.000000 weekdaytime-0.0.9/weekdaytime/
+-rw-rw-rw-   0        0        0     7096 2023-04-10 09:20:43.000000 weekdaytime-0.0.9/weekdaytime/period.py
+-rw-rw-rw-   0        0        0     2345 2023-04-08 14:41:13.000000 weekdaytime-0.0.9/weekdaytime/weekdaytime.py
+-rw-rw-rw-   0        0        0       89 2023-04-10 10:50:53.000000 weekdaytime-0.0.9/weekdaytime/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 10:57:09.000000 weekdaytime-0.0.9/weekdaytime.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-04-10 10:57:09.000000 weekdaytime-0.0.9/weekdaytime.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-10 10:57:09.000000 weekdaytime-0.0.9/weekdaytime.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     5018 2023-04-10 10:57:09.000000 weekdaytime-0.0.9/weekdaytime.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       14 2023-04-10 10:57:09.000000 weekdaytime-0.0.9/weekdaytime.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      329 2023-04-10 10:57:09.000000 weekdaytime-0.0.9/weekdaytime.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       12 2023-04-10 10:57:09.000000 weekdaytime-0.0.9/weekdaytime.egg-info/top_level.txt
```

### Comparing `weekdaytime-0.0.12/LICENSE` & `weekdaytime-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `weekdaytime-0.0.12/PKG-INFO` & `weekdaytime-0.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weekdaytime
-Version: 0.0.12
+Version: 0.0.9
 Summary: Python library that models available periods in a week
 Home-page: https://github.com/AaronTHCheung/weekdaytime
 Author: Aaron Cheung
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -21,18 +21,23 @@
     evaluates to True if and only if ```visit_period``` is within ```available_period```.
 - Manipulate period objects with bitwise operators (```|, &, ~, ^```)
 - Convert period string into a period object, and vise versa (e.g., `'09:00~15:00,17:00~21:00;15:00~02:00(Fri,Sat)'`)
 
 ## Installation
 1. Python version must not be less than 3.6.
 2. The dependent library `bitarray` requires Microsoft Visual C++ 14.0. Get it with "Microsoft Visual C++ Build Tools": https://visualstudio.microsoft.com/downloads/
-3. Install with pip using the command
-    ```
-    pip install weekdaytime
-    ```
+3. 
+    - Install with pip using the command
+        ```
+        pip install weekdaytime
+        ```
+    - Alternatively, the library can also be installed with anaconda using the command
+        ```
+        conda install weekdaytime
+        ```
 
 ## Usage
 ### weekdaytime class
 A weekdaytime instance specifies a point in time in a week.
 ```
 from weekdaytime import weekdaytime as wdt
```

### Comparing `weekdaytime-0.0.12/README.md` & `weekdaytime-0.0.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -9,18 +9,23 @@
     evaluates to True if and only if ```visit_period``` is within ```available_period```.
 - Manipulate period objects with bitwise operators (```|, &, ~, ^```)
 - Convert period string into a period object, and vise versa (e.g., `'09:00~15:00,17:00~21:00;15:00~02:00(Fri,Sat)'`)
 
 ## Installation
 1. Python version must not be less than 3.6.
 2. The dependent library `bitarray` requires Microsoft Visual C++ 14.0. Get it with "Microsoft Visual C++ Build Tools": https://visualstudio.microsoft.com/downloads/
-3. Install with pip using the command
-    ```
-    pip install weekdaytime
-    ```
+3. 
+    - Install with pip using the command
+        ```
+        pip install weekdaytime
+        ```
+    - Alternatively, the library can also be installed with anaconda using the command
+        ```
+        conda install weekdaytime
+        ```
 
 ## Usage
 ### weekdaytime class
 A weekdaytime instance specifies a point in time in a week.
 ```
 from weekdaytime import weekdaytime as wdt
```

### Comparing `weekdaytime-0.0.12/setup.py` & `weekdaytime-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 from pathlib import Path
 
 long_description = (Path(__file__).parent/'README.md').read_text()
 setup(
     name='weekdaytime',
-    version='0.0.12',
+    version='0.0.9',
     description='Python library that models available periods in a week',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Aaron Cheung',
     packages=['weekdaytime'],
     python_requires='>=3.6',
     install_requires=[
```

### Comparing `weekdaytime-0.0.12/weekdaytime/period.py` & `weekdaytime-0.0.9/weekdaytime/period.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     @staticmethod
     def strpperiod(string: str):
         # string example: 09:00~15:00,17:00~20:00;14:00~02:00(Fri);12:00~20:00(Sat,Sun)
         ba = bitarray(60*24*7)
         ba.setall(0)
 
         generic_string = ''
-        m = re.search(';|^([0-9:~,]+)(;|$)', string)
+        m = re.search(';|^([0-9:~,]+);|$', string)
         if m.group(0) != '' and m.groups()[0] is not None:
             # there is a weekday-generic part
             generic_string = m.group(1)
             specific_string = string[:m.span()[0]] + ';' + string[m.span()[1]:]
         else:
             # all parts are weekday-specific
             specific_string = string
@@ -64,23 +64,20 @@
                 end_minute_of_day = end_hour * 60 + end_minute
                 if end_minute_of_day < start_minute_of_day: end_minute_of_day += 60 * 24  # across midnight
 
                 starts_minute_of_day.append(start_minute_of_day)
                 ends_minute_of_day.append(end_minute_of_day)
                 
             for weekdayAbbrev in weekdayAbbrev_string.split(','):
-                try:
-                    start_weekday = weekdaytime.intfweekday(weekdayAbbrev)
-                    specific_predicates[start_weekday] = 1
-                    for s, e in zip(starts_minute_of_day, ends_minute_of_day):
-                        start_weekdaytime = weekdaytime.from_min_of_week(start_weekday * 24 * 60 + s)
-                        end_weekdaytime = weekdaytime.from_min_of_week(start_weekday * 24 * 60 + e)
-                        ba |= period(start_weekdaytime, end_weekdaytime)._fba
-                except Exception:
-                    pass
+                start_weekday = weekdaytime.intfweekday(weekdayAbbrev)
+                specific_predicates[start_weekday] = 1
+                for s, e in zip(starts_minute_of_day, ends_minute_of_day):
+                    start_weekdaytime = weekdaytime.from_min_of_week(start_weekday * 24 * 60 + s)
+                    end_weekdaytime = weekdaytime.from_min_of_week(start_weekday * 24 * 60 + e)
+                    ba |= period(start_weekdaytime, end_weekdaytime)._fba
 
         # remaining days are filled with weekday-generic information
         for time_substring in generic_string.split(','):
             if len(time_substring) != 11: continue
             start_hour, start_minute, end_hour, end_minute = [int(x) for x in re.split(':|~', time_substring)]
 
             start_minute_of_day = start_hour * 60 + start_minute
```

### Comparing `weekdaytime-0.0.12/weekdaytime/weekdaytime.py` & `weekdaytime-0.0.9/weekdaytime/weekdaytime.py`

 * *Files identical despite different names*

### Comparing `weekdaytime-0.0.12/weekdaytime.egg-info/PKG-INFO` & `weekdaytime-0.0.9/weekdaytime.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weekdaytime
-Version: 0.0.12
+Version: 0.0.9
 Summary: Python library that models available periods in a week
 Home-page: https://github.com/AaronTHCheung/weekdaytime
 Author: Aaron Cheung
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -21,18 +21,23 @@
     evaluates to True if and only if ```visit_period``` is within ```available_period```.
 - Manipulate period objects with bitwise operators (```|, &, ~, ^```)
 - Convert period string into a period object, and vise versa (e.g., `'09:00~15:00,17:00~21:00;15:00~02:00(Fri,Sat)'`)
 
 ## Installation
 1. Python version must not be less than 3.6.
 2. The dependent library `bitarray` requires Microsoft Visual C++ 14.0. Get it with "Microsoft Visual C++ Build Tools": https://visualstudio.microsoft.com/downloads/
-3. Install with pip using the command
-    ```
-    pip install weekdaytime
-    ```
+3. 
+    - Install with pip using the command
+        ```
+        pip install weekdaytime
+        ```
+    - Alternatively, the library can also be installed with anaconda using the command
+        ```
+        conda install weekdaytime
+        ```
 
 ## Usage
 ### weekdaytime class
 A weekdaytime instance specifies a point in time in a week.
 ```
 from weekdaytime import weekdaytime as wdt
```

