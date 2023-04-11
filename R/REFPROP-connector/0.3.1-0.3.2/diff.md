# Comparing `tmp/REFPROP_connector-0.3.1.tar.gz` & `tmp/REFPROP_connector-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "REFPROP_connector-0.3.1.tar", last modified: Thu Mar 23 10:15:44 2023, max compression
+gzip compressed data, was "REFPROP_connector-0.3.2.tar", last modified: Tue Apr 11 17:38:50 2023, max compression
```

## Comparing `REFPROP_connector-0.3.1.tar` & `REFPROP_connector-0.3.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-03-23 10:15:44.231943 REFPROP_connector-0.3.1/
--rw-rw-rw-   0        0        0       26 2022-06-23 09:23:17.000000 REFPROP_connector-0.3.1/.gitignore
--rw-rw-rw-   0        0        0    35823 2021-12-10 08:32:10.000000 REFPROP_connector-0.3.1/LICENSE
--rw-rw-rw-   0        0        0     6186 2023-03-23 10:15:44.232943 REFPROP_connector-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     4376 2021-12-10 10:47:30.000000 REFPROP_connector-0.3.1/README.md
-drwxrwxrwx   0        0        0        0 2023-03-23 10:15:44.206943 REFPROP_connector-0.3.1/REFPROPConnector/
--rwxrwxrwx   0        0        0  5280688 2021-12-10 08:32:10.000000 REFPROP_connector-0.3.1/REFPROPConnector/NIST2310.EXE
-drwxrwxrwx   0        0        0        0 2023-03-23 10:15:44.210942 REFPROP_connector-0.3.1/REFPROPConnector/Support/
--rw-rw-rw-   0        0        0        0 2022-02-03 11:33:25.000000 REFPROP_connector-0.3.1/REFPROPConnector/Support/__init__.py
--rw-rw-rw-   0        0        0     1558 2022-02-03 16:21:28.000000 REFPROP_connector-0.3.1/REFPROPConnector/Support/constants.py
--rw-rw-rw-   0        0        0    10679 2022-02-03 16:47:42.000000 REFPROP_connector-0.3.1/REFPROPConnector/Support/refprop_names_tree.py
-drwxrwxrwx   0        0        0        0 2023-03-23 10:15:44.213942 REFPROP_connector-0.3.1/REFPROPConnector/Support/resources/
--rw-rw-rw-   0        0        0       30 2023-03-23 10:02:54.000000 REFPROP_connector-0.3.1/REFPROPConnector/Support/resources/REFPROP_exec.dat
--rw-rw-rw-   0        0        0    15641 2023-03-23 09:58:41.000000 REFPROP_connector-0.3.1/REFPROPConnector/Support/resources/REFPROP_names.xml
--rw-rw-rw-   0        0        0        0 2022-02-03 11:35:20.000000 REFPROP_connector-0.3.1/REFPROPConnector/Support/resources/__init__.py
--rw-rw-rw-   0        0        0     2906 2023-03-23 09:57:25.000000 REFPROP_connector-0.3.1/REFPROPConnector/Support/resources/file_handler.py
--rw-rw-rw-   0        0        0    15902 2023-03-23 09:58:40.000000 REFPROP_connector-0.3.1/REFPROPConnector/Support/resources/rp_names_file_generator.py
--rw-rw-rw-   0        0        0      190 2022-02-03 11:47:19.000000 REFPROP_connector-0.3.1/REFPROPConnector/__init__.py
--rw-rw-rw-   0        0        0    27241 2023-01-27 16:53:10.000000 REFPROP_connector-0.3.1/REFPROPConnector/refprop_calculator.py
-drwxrwxrwx   0        0        0        0 2023-03-23 10:15:44.208943 REFPROP_connector-0.3.1/REFPROPConnectorTest/
--rw-rw-rw-   0        0        0        0 2021-12-10 10:12:18.000000 REFPROP_connector-0.3.1/REFPROPConnectorTest/__init__.py
--rw-rw-rw-   0        0        0     2828 2022-09-28 08:16:54.000000 REFPROP_connector-0.3.1/REFPROPConnectorTest/test_file.py
-drwxrwxrwx   0        0        0        0 2023-03-23 10:15:44.230961 REFPROP_connector-0.3.1/REFPROP_connector.egg-info/
--rw-rw-rw-   0        0        0     6186 2023-03-23 10:15:44.000000 REFPROP_connector-0.3.1/REFPROP_connector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      847 2023-03-23 10:15:44.000000 REFPROP_connector-0.3.1/REFPROP_connector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-23 10:15:44.000000 REFPROP_connector-0.3.1/REFPROP_connector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-03-23 10:15:44.000000 REFPROP_connector-0.3.1/REFPROP_connector.egg-info/requires.txt
--rw-rw-rw-   0        0        0       38 2023-03-23 10:15:44.000000 REFPROP_connector-0.3.1/REFPROP_connector.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       87 2023-03-23 10:11:51.000000 REFPROP_connector-0.3.1/requirements.txt
--rw-rw-rw-   0        0        0       86 2023-03-23 10:15:44.236942 REFPROP_connector-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0     2228 2023-03-23 10:13:27.000000 REFPROP_connector-0.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-23 10:15:44.231943 REFPROP_connector-0.3.1/twine_upload/
--rw-rw-rw-   0        0        0     1089 2022-06-21 16:26:22.000000 REFPROP_connector-0.3.1/twine_upload/pip_upload.py
+drwxrwxrwx   0        0        0        0 2023-04-11 17:38:50.816597 REFPROP_connector-0.3.2/
+-rw-rw-rw-   0        0        0       26 2022-06-23 09:23:17.000000 REFPROP_connector-0.3.2/.gitignore
+-rw-rw-rw-   0        0        0    35823 2021-12-10 08:32:10.000000 REFPROP_connector-0.3.2/LICENSE
+-rw-rw-rw-   0        0        0     6186 2023-04-11 17:38:50.816597 REFPROP_connector-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4376 2021-12-10 10:47:30.000000 REFPROP_connector-0.3.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 17:38:50.783423 REFPROP_connector-0.3.2/REFPROPConnector/
+-rwxrwxrwx   0        0        0  5280688 2021-12-10 08:32:10.000000 REFPROP_connector-0.3.2/REFPROPConnector/NIST2310.EXE
+drwxrwxrwx   0        0        0        0 2023-04-11 17:38:50.786471 REFPROP_connector-0.3.2/REFPROPConnector/Support/
+-rw-rw-rw-   0        0        0        0 2022-02-03 11:33:25.000000 REFPROP_connector-0.3.2/REFPROPConnector/Support/__init__.py
+-rw-rw-rw-   0        0        0     1558 2022-02-03 16:21:28.000000 REFPROP_connector-0.3.2/REFPROPConnector/Support/constants.py
+-rw-rw-rw-   0        0        0    10679 2022-02-03 16:47:42.000000 REFPROP_connector-0.3.2/REFPROPConnector/Support/refprop_names_tree.py
+drwxrwxrwx   0        0        0        0 2023-04-11 17:38:50.798484 REFPROP_connector-0.3.2/REFPROPConnector/Support/resources/
+-rw-rw-rw-   0        0        0       30 2023-04-11 17:32:53.000000 REFPROP_connector-0.3.2/REFPROPConnector/Support/resources/REFPROP_exec.dat
+-rw-rw-rw-   0        0        0    16788 2023-04-11 17:29:02.000000 REFPROP_connector-0.3.2/REFPROPConnector/Support/resources/REFPROP_names.xml
+-rw-rw-rw-   0        0        0        0 2022-02-03 11:35:20.000000 REFPROP_connector-0.3.2/REFPROPConnector/Support/resources/__init__.py
+-rw-rw-rw-   0        0        0     2906 2023-03-23 09:57:25.000000 REFPROP_connector-0.3.2/REFPROPConnector/Support/resources/file_handler.py
+-rw-rw-rw-   0        0        0    17049 2023-04-11 17:29:02.000000 REFPROP_connector-0.3.2/REFPROPConnector/Support/resources/rp_names_file_generator.py
+-rw-rw-rw-   0        0        0      190 2022-02-03 11:47:19.000000 REFPROP_connector-0.3.2/REFPROPConnector/__init__.py
+-rw-rw-rw-   0        0        0    27241 2023-01-27 16:53:10.000000 REFPROP_connector-0.3.2/REFPROPConnector/refprop_calculator.py
+drwxrwxrwx   0        0        0        0 2023-04-11 17:38:50.785436 REFPROP_connector-0.3.2/REFPROPConnectorTest/
+-rw-rw-rw-   0        0        0        0 2021-12-10 10:12:18.000000 REFPROP_connector-0.3.2/REFPROPConnectorTest/__init__.py
+-rw-rw-rw-   0        0        0     2828 2023-04-11 17:32:51.000000 REFPROP_connector-0.3.2/REFPROPConnectorTest/test_file.py
+drwxrwxrwx   0        0        0        0 2023-04-11 17:38:50.815597 REFPROP_connector-0.3.2/REFPROP_connector.egg-info/
+-rw-rw-rw-   0        0        0     6186 2023-04-11 17:38:50.000000 REFPROP_connector-0.3.2/REFPROP_connector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      847 2023-04-11 17:38:50.000000 REFPROP_connector-0.3.2/REFPROP_connector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 17:38:50.000000 REFPROP_connector-0.3.2/REFPROP_connector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-04-11 17:38:50.000000 REFPROP_connector-0.3.2/REFPROP_connector.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       38 2023-04-11 17:38:50.000000 REFPROP_connector-0.3.2/REFPROP_connector.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       87 2023-03-23 10:11:51.000000 REFPROP_connector-0.3.2/requirements.txt
+-rw-rw-rw-   0        0        0       86 2023-04-11 17:38:50.817580 REFPROP_connector-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     2228 2023-04-11 17:37:39.000000 REFPROP_connector-0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 17:38:50.816597 REFPROP_connector-0.3.2/twine_upload/
+-rw-rw-rw-   0        0        0     1089 2022-06-21 16:26:22.000000 REFPROP_connector-0.3.2/twine_upload/pip_upload.py
```

### Comparing `REFPROP_connector-0.3.1/LICENSE` & `REFPROP_connector-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `REFPROP_connector-0.3.1/PKG-INFO` & `REFPROP_connector-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: REFPROP_connector
-Version: 0.3.1
+Version: 0.3.2
 Summary: Tools for launching REFPROP calculation and retrieving results from python
 Home-page: https://www.dief.unifi.it/vp-177-serg-group-english-version.html
 Author: Pietro Ungar
 Author-email: pietro.ungar@unifi.it
 License: GNU GPLv3
-Download-URL: https://github.com/SERGGroup/REFPROPConnector/archive/refs/tags/0.3.1.tar.gz
+Download-URL: https://github.com/SERGGroup/REFPROPConnector/archive/refs/tags/0.3.2.tar.gz
 Project-URL: Source, https://github.com/SERGGroup/REFPROPConnector
 Project-URL: Tracker, https://github.com/SERGGroup/REFPROPConnector/issues
 Description: # REFPROP connector
         
         __REFPROP connector__ is a tools developed by the [SERG research group](https://www.dief.unifi.it/vp-177-serg-group-english-version.html) 
         of the [University of Florence](https://www.unifi.it/changelang-eng.html) for launching [REFPROP](https://www.nist.gov/srd/refprop) 
         calculation and retrieving results from python.
```

### Comparing `REFPROP_connector-0.3.1/README.md` & `REFPROP_connector-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `REFPROP_connector-0.3.1/REFPROPConnector/NIST2310.EXE` & `REFPROP_connector-0.3.2/REFPROPConnector/NIST2310.EXE`

 * *Files identical despite different names*

### Comparing `REFPROP_connector-0.3.1/REFPROPConnector/Support/constants.py` & `REFPROP_connector-0.3.2/REFPROPConnector/Support/constants.py`

 * *Files identical despite different names*

### Comparing `REFPROP_connector-0.3.1/REFPROPConnector/Support/refprop_names_tree.py` & `REFPROP_connector-0.3.2/REFPROPConnector/Support/refprop_names_tree.py`

 * *Files identical despite different names*

### Comparing `REFPROP_connector-0.3.1/REFPROPConnector/Support/resources/REFPROP_names.xml` & `REFPROP_connector-0.3.2/REFPROPConnector/Support/resources/REFPROP_names.xml`

 * *Files 1% similar despite different names*

#### Comparing `REFPROP_connector-0.3.1/REFPROPConnector/Support/resources/REFPROP_names.xml` & `REFPROP_connector-0.3.2/REFPROPConnector/Support/resources/REFPROP_names.xml`

```diff
@@ -199,14 +199,34 @@
         <unit name="MOLAR ENGLISH" unit="BTU/(lbmol * R)"/>
         <unit name="MKS" unit="J/(g * K)"/>
         <unit name="CGS" unit="J/(g * K)"/>
         <unit name="MIXED" unit="J/(g * K)"/>
         <unit name="MEUNITS" unit="J/(g * K)"/>
       </units>
     </refprop_name>
+    <refprop_name name="CP0">
+      <std_names>
+        <std_name name="cp0"/>
+        <std_name name="ideal_isochoric_heat_capacity"/>
+      </std_names>
+      <units>
+        <unit name="DEFAULT" unit="J/(mol * K)"/>
+        <unit name="MOLE SI" unit="J/(mol * K)"/>
+        <unit name="MASS SI" unit="J/(g * K)"/>
+        <unit name="SI WITH C" unit="J/(g * K)"/>
+        <unit name="MOLAR BASE SI" unit="J/(mol * K)"/>
+        <unit name="MASS BASE SI" unit="J/(kg * K)"/>
+        <unit name="ENGLISH" unit="BTU/(lbm * R)"/>
+        <unit name="MOLAR ENGLISH" unit="BTU/(lbmol * R)"/>
+        <unit name="MKS" unit="J/(g * K)"/>
+        <unit name="CGS" unit="J/(g * K)"/>
+        <unit name="MIXED" unit="J/(g * K)"/>
+        <unit name="MEUNITS" unit="J/(g * K)"/>
+      </units>
+    </refprop_name>
     <refprop_name name="CV">
       <std_names>
         <std_name name="cv"/>
         <std_name name="isobaric_heat_capacity"/>
       </std_names>
       <units>
         <unit name="DEFAULT" unit="J/(mol * K)"/>
```

### Comparing `REFPROP_connector-0.3.1/REFPROPConnector/Support/resources/file_handler.py` & `REFPROP_connector-0.3.2/REFPROPConnector/Support/resources/file_handler.py`

 * *Files identical despite different names*

### Comparing `REFPROP_connector-0.3.1/REFPROPConnector/Support/resources/rp_names_file_generator.py` & `REFPROP_connector-0.3.2/REFPROPConnector/Support/resources/rp_names_file_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -284,14 +284,42 @@
                 <unit name = "CGS"              unit = "J/(g * K)" />
                 <unit name = "MIXED"            unit = "J/(g * K)" />
                 <unit name = "MEUNITS"          unit = "J/(g * K)" />
 
             </units>
 
         </refprop_name>
+        <refprop_name name = "CP0">
+
+            <std_names>
+
+                <std_name name="cp0"/>
+                <std_name name="ideal_isochoric_heat_capacity"/>
+
+            </std_names>
+            <units>
+
+                <unit name = "DEFAULT"          unit = "J/(mol * K)" />
+                <unit name = "MOLE SI"          unit = "J/(mol * K)" />
+                <unit name = "MASS SI"          unit = "J/(g * K)" />
+                <unit name = "SI WITH C"        unit = "J/(g * K)" />
+
+                <unit name = "MOLAR BASE SI"    unit = "J/(mol * K)" />
+                <unit name = "MASS BASE SI"     unit = "J/(kg * K)" />
+                <unit name = "ENGLISH"          unit = "BTU/(lbm * R)" />
+                <unit name = "MOLAR ENGLISH"    unit = "BTU/(lbmol * R)" />
+
+                <unit name = "MKS"              unit = "J/(g * K)" />
+                <unit name = "CGS"              unit = "J/(g * K)" />
+                <unit name = "MIXED"            unit = "J/(g * K)" />
+                <unit name = "MEUNITS"          unit = "J/(g * K)" />
+
+            </units>
+
+        </refprop_name>
         <refprop_name name = "CV">
 
             <std_names>
 
                 <std_name name="cv"/>
                 <std_name name="isobaric_heat_capacity"/>
```

### Comparing `REFPROP_connector-0.3.1/REFPROPConnector/refprop_calculator.py` & `REFPROP_connector-0.3.2/REFPROPConnector/refprop_calculator.py`

 * *Files identical despite different names*

### Comparing `REFPROP_connector-0.3.1/REFPROPConnectorTest/test_file.py` & `REFPROP_connector-0.3.2/REFPROPConnectorTest/test_file.py`

 * *Files identical despite different names*

### Comparing `REFPROP_connector-0.3.1/REFPROP_connector.egg-info/PKG-INFO` & `REFPROP_connector-0.3.2/REFPROP_connector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: REFPROP-connector
-Version: 0.3.1
+Version: 0.3.2
 Summary: Tools for launching REFPROP calculation and retrieving results from python
 Home-page: https://www.dief.unifi.it/vp-177-serg-group-english-version.html
 Author: Pietro Ungar
 Author-email: pietro.ungar@unifi.it
 License: GNU GPLv3
-Download-URL: https://github.com/SERGGroup/REFPROPConnector/archive/refs/tags/0.3.1.tar.gz
+Download-URL: https://github.com/SERGGroup/REFPROPConnector/archive/refs/tags/0.3.2.tar.gz
 Project-URL: Source, https://github.com/SERGGroup/REFPROPConnector
 Project-URL: Tracker, https://github.com/SERGGroup/REFPROPConnector/issues
 Description: # REFPROP connector
         
         __REFPROP connector__ is a tools developed by the [SERG research group](https://www.dief.unifi.it/vp-177-serg-group-english-version.html) 
         of the [University of Florence](https://www.unifi.it/changelang-eng.html) for launching [REFPROP](https://www.nist.gov/srd/refprop) 
         calculation and retrieving results from python.
```

### Comparing `REFPROP_connector-0.3.1/REFPROP_connector.egg-info/SOURCES.txt` & `REFPROP_connector-0.3.2/REFPROP_connector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `REFPROP_connector-0.3.1/setup.py` & `REFPROP_connector-0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 from os import path, listdir
 
-VERSION = "0.3.1"
+VERSION = "0.3.2"
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
 
     long_description = f.read()
```

### Comparing `REFPROP_connector-0.3.1/twine_upload/pip_upload.py` & `REFPROP_connector-0.3.2/twine_upload/pip_upload.py`

 * *Files identical despite different names*

