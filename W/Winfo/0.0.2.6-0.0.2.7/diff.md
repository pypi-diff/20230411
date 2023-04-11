# Comparing `tmp/Winfo-0.0.2.6.tar.gz` & `tmp/Winfo-0.0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Winfo-0.0.2.6.tar", last modified: Mon Apr 10 14:42:47 2023, max compression
+gzip compressed data, was "Winfo-0.0.2.7.tar", last modified: Tue Apr 11 12:23:18 2023, max compression
```

## Comparing `Winfo-0.0.2.6.tar` & `Winfo-0.0.2.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 14:42:47.312823 Winfo-0.0.2.6/
--rw-rw-rw-   0        0        0     1156 2023-04-07 10:35:15.000000 Winfo-0.0.2.6/LICENSE
--rw-rw-rw-   0        0        0     5360 2023-04-10 14:42:47.310824 Winfo-0.0.2.6/PKG-INFO
--rw-rw-rw-   0        0        0     4912 2023-04-10 14:17:51.000000 Winfo-0.0.2.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-10 14:42:47.291824 Winfo-0.0.2.6/Winfo/
--rw-rw-rw-   0        0        0     2658 2023-04-10 14:29:58.000000 Winfo-0.0.2.6/Winfo/__init__.py
--rw-rw-rw-   0        0        0     1300 2023-04-09 16:56:37.000000 Winfo-0.0.2.6/Winfo/cpu.py
--rw-rw-rw-   0        0        0      967 2023-04-09 16:58:02.000000 Winfo-0.0.2.6/Winfo/disk.py
--rw-rw-rw-   0        0        0      680 2023-04-09 16:58:55.000000 Winfo-0.0.2.6/Winfo/ethernet.py
--rw-rw-rw-   0        0        0      522 2023-04-09 16:57:11.000000 Winfo-0.0.2.6/Winfo/gpu.py
--rw-rw-rw-   0        0        0      972 2023-04-10 14:20:06.000000 Winfo-0.0.2.6/Winfo/memory.py
--rw-rw-rw-   0        0        0      479 2023-04-09 16:59:58.000000 Winfo-0.0.2.6/Winfo/motherboard.py
--rw-rw-rw-   0        0        0     1197 2023-04-10 14:38:42.000000 Winfo-0.0.2.6/Winfo/software.py
-drwxrwxrwx   0        0        0        0 2023-04-10 14:42:47.309823 Winfo-0.0.2.6/Winfo.egg-info/
--rw-rw-rw-   0        0        0     5360 2023-04-10 14:42:47.000000 Winfo-0.0.2.6/Winfo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2023-04-10 14:42:47.000000 Winfo-0.0.2.6/Winfo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 14:42:47.000000 Winfo-0.0.2.6/Winfo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-10 14:42:47.000000 Winfo-0.0.2.6/Winfo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-10 14:42:47.312823 Winfo-0.0.2.6/setup.cfg
--rw-rw-rw-   0        0        0      677 2023-04-10 14:42:21.000000 Winfo-0.0.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 12:23:18.224991 Winfo-0.0.2.7/
+-rw-rw-rw-   0        0        0     1156 2023-04-07 10:35:15.000000 Winfo-0.0.2.7/LICENSE
+-rw-rw-rw-   0        0        0     5833 2023-04-11 12:23:18.223994 Winfo-0.0.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0     5385 2023-04-11 12:19:53.000000 Winfo-0.0.2.7/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 12:23:18.210994 Winfo-0.0.2.7/Winfo/
+-rw-rw-rw-   0        0        0     2658 2023-04-10 14:29:58.000000 Winfo-0.0.2.7/Winfo/__init__.py
+-rw-rw-rw-   0        0        0     1300 2023-04-09 16:56:37.000000 Winfo-0.0.2.7/Winfo/cpu.py
+-rw-rw-rw-   0        0        0      967 2023-04-09 16:58:02.000000 Winfo-0.0.2.7/Winfo/disk.py
+-rw-rw-rw-   0        0        0      680 2023-04-09 16:58:55.000000 Winfo-0.0.2.7/Winfo/ethernet.py
+-rw-rw-rw-   0        0        0      522 2023-04-09 16:57:11.000000 Winfo-0.0.2.7/Winfo/gpu.py
+-rw-rw-rw-   0        0        0     1339 2023-04-11 12:16:05.000000 Winfo-0.0.2.7/Winfo/memory.py
+-rw-rw-rw-   0        0        0      479 2023-04-09 16:59:58.000000 Winfo-0.0.2.7/Winfo/motherboard.py
+-rw-rw-rw-   0        0        0     1197 2023-04-10 14:38:42.000000 Winfo-0.0.2.7/Winfo/software.py
+drwxrwxrwx   0        0        0        0 2023-04-11 12:23:18.222992 Winfo-0.0.2.7/Winfo.egg-info/
+-rw-rw-rw-   0        0        0     5833 2023-04-11 12:23:18.000000 Winfo-0.0.2.7/Winfo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2023-04-11 12:23:18.000000 Winfo-0.0.2.7/Winfo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 12:23:18.000000 Winfo-0.0.2.7/Winfo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-11 12:23:18.000000 Winfo-0.0.2.7/Winfo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 12:23:18.224991 Winfo-0.0.2.7/setup.cfg
+-rw-rw-rw-   0        0        0      677 2023-04-11 12:22:23.000000 Winfo-0.0.2.7/setup.py
```

### Comparing `Winfo-0.0.2.6/LICENSE` & `Winfo-0.0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `Winfo-0.0.2.6/PKG-INFO` & `Winfo-0.0.2.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Winfo
-Version: 0.0.2.6
+Version: 0.0.2.7
 Summary: Get information about your windows system
 Author: BLUEAMETHYST Studios
 Keywords: python,windows,util,information,system
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
@@ -56,14 +56,42 @@
 
 ```Python
 import Winfo
 
 print("My Memory is from " + Winfo.memory.getmanufacturer())
 print("I've " + Winfo.memory.getcapacityMB() + " of memory or in GB: " + Winfo.memory.getcapacityGB())
 print("My memory works at " + Winfo.memory.getSpeed() + " Mhz")
+print("All my memory's Speed in a Python list: " + Winfo.memory.getSpeedAll())
+```
+
+- If you want to list all Speed values in a prettier way, try this:
+
+```Python
+import Winfo
+
+prettylist = ""
+
+for i in Winfo.memory.getSpeedAll():
+    prettylist = prettylist + i + "\n"
+
+print(prettylist)
+```
+
+- Instead of looking like this when printed:
+
+```
+[3000, 3000]
+```
+
+- It would now look like this:
+
+```
+3000
+3000
+
 ```
 
 ### Disk Information
 
 - List all connected disks (Returns them in a Python list)
 - Get Disk Size (Capacity) of disk 0, if you want to get the size of another disks set it's number as the index argument in the function
 
@@ -71,15 +99,15 @@
 import Winfo
 
 print("Here's a list of all my disks as a Python List: " + str(Winfo.disk.listall()))
 print("The size of my primary disk is: " + Winfo.disk.getsize())
 print("The size of my secondary disk is: " + Winfo.disk.getsize(1))
 ```
 
-- BONUS TIP! If you want to list all disks in a prettier way try this:
+- Like with the getSpeedAll, if you want to list all disks in a prettier way try this:
 
 ```Python
 import Winfo
 
 prettylist = ""
 
 for i in Winfo.disk.listall():
@@ -110,15 +138,15 @@
 ```Python
 import Winfo
 
 print("My MAC Address is: " + Winfo.ethernet.macaddr())
 print("List of all Network Adapters as a Python list: " + Winfo.ethernet.listadapters())
 ```
 
-- Like with the Disklist, you can make the list returned from Winfo.ethernet.listadapters() way prettier by doing this:
+- Like with the Disklist and the getSpeedAll, you can make the list returned from Winfo.ethernet.listadapters() way prettier by doing this:
 
 ```Python
 import Winfo
 
 prettylist = ""
 
 for i in Winfo.ethernet.listadapters():
```

### Comparing `Winfo-0.0.2.6/README.md` & `Winfo-0.0.2.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -43,14 +43,42 @@
 
 ```Python
 import Winfo
 
 print("My Memory is from " + Winfo.memory.getmanufacturer())
 print("I've " + Winfo.memory.getcapacityMB() + " of memory or in GB: " + Winfo.memory.getcapacityGB())
 print("My memory works at " + Winfo.memory.getSpeed() + " Mhz")
+print("All my memory's Speed in a Python list: " + Winfo.memory.getSpeedAll())
+```
+
+- If you want to list all Speed values in a prettier way, try this:
+
+```Python
+import Winfo
+
+prettylist = ""
+
+for i in Winfo.memory.getSpeedAll():
+    prettylist = prettylist + i + "\n"
+
+print(prettylist)
+```
+
+- Instead of looking like this when printed:
+
+```
+[3000, 3000]
+```
+
+- It would now look like this:
+
+```
+3000
+3000
+
 ```
 
 ### Disk Information
 
 - List all connected disks (Returns them in a Python list)
 - Get Disk Size (Capacity) of disk 0, if you want to get the size of another disks set it's number as the index argument in the function
 
@@ -58,15 +86,15 @@
 import Winfo
 
 print("Here's a list of all my disks as a Python List: " + str(Winfo.disk.listall()))
 print("The size of my primary disk is: " + Winfo.disk.getsize())
 print("The size of my secondary disk is: " + Winfo.disk.getsize(1))
 ```
 
-- BONUS TIP! If you want to list all disks in a prettier way try this:
+- Like with the getSpeedAll, if you want to list all disks in a prettier way try this:
 
 ```Python
 import Winfo
 
 prettylist = ""
 
 for i in Winfo.disk.listall():
@@ -97,15 +125,15 @@
 ```Python
 import Winfo
 
 print("My MAC Address is: " + Winfo.ethernet.macaddr())
 print("List of all Network Adapters as a Python list: " + Winfo.ethernet.listadapters())
 ```
 
-- Like with the Disklist, you can make the list returned from Winfo.ethernet.listadapters() way prettier by doing this:
+- Like with the Disklist and the getSpeedAll, you can make the list returned from Winfo.ethernet.listadapters() way prettier by doing this:
 
 ```Python
 import Winfo
 
 prettylist = ""
 
 for i in Winfo.ethernet.listadapters():
```

### Comparing `Winfo-0.0.2.6/Winfo/__init__.py` & `Winfo-0.0.2.7/Winfo/__init__.py`

 * *Files identical despite different names*

### Comparing `Winfo-0.0.2.6/Winfo/cpu.py` & `Winfo-0.0.2.7/Winfo/cpu.py`

 * *Files identical despite different names*

### Comparing `Winfo-0.0.2.6/Winfo/disk.py` & `Winfo-0.0.2.7/Winfo/disk.py`

 * *Files identical despite different names*

### Comparing `Winfo-0.0.2.6/Winfo/ethernet.py` & `Winfo-0.0.2.7/Winfo/ethernet.py`

 * *Files identical despite different names*

### Comparing `Winfo-0.0.2.6/Winfo/gpu.py` & `Winfo-0.0.2.7/Winfo/gpu.py`

 * *Files identical despite different names*

### Comparing `Winfo-0.0.2.6/Winfo/memory.py` & `Winfo-0.0.2.7/Winfo/memory.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,10 +16,22 @@
     raw = check_output(["wmic", "computersystem", "get", "totalphysicalmemory"])
     rawdecoded = raw.decode().lstrip("TotalPhysicalMemory").rstrip("\n")
     getcapGB = int(rawdecoded) / 1024 ** 3
     return float(getcapGB)
 
 def getSpeed():
     raw = check_output(["wmic", "memorychip", "get", "Speed"])
-    rawdecoded = raw.decode().lstrip("Speed").rstrip("\n")
-    getspeed = rawdecoded.replace("\n", "")
-    return float(rawdecoded)
+    rawdecoded = raw.decode().replace("Speed", "").strip()
+    speedlist = [int(speed) for speed in rawdecoded.split("\n") if speed.isdigit()]
+    if not speedlist:
+        return None
+    else:
+        return max(speedlist)
+    
+def getSpeedAll():
+    raw = check_output(["wmic", "memorychip", "get", "Speed"])
+    rawdecoded = raw.decode().strip().split('\r\n')
+    speeds = [int(speed) for speed in rawdecoded[1:] if speed.strip().isdigit()]
+    return speeds
+    
+
+print(getSpeed())
```

### Comparing `Winfo-0.0.2.6/Winfo/software.py` & `Winfo-0.0.2.7/Winfo/software.py`

 * *Files identical despite different names*

### Comparing `Winfo-0.0.2.6/Winfo.egg-info/PKG-INFO` & `Winfo-0.0.2.7/Winfo.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Winfo
-Version: 0.0.2.6
+Version: 0.0.2.7
 Summary: Get information about your windows system
 Author: BLUEAMETHYST Studios
 Keywords: python,windows,util,information,system
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
@@ -56,14 +56,42 @@
 
 ```Python
 import Winfo
 
 print("My Memory is from " + Winfo.memory.getmanufacturer())
 print("I've " + Winfo.memory.getcapacityMB() + " of memory or in GB: " + Winfo.memory.getcapacityGB())
 print("My memory works at " + Winfo.memory.getSpeed() + " Mhz")
+print("All my memory's Speed in a Python list: " + Winfo.memory.getSpeedAll())
+```
+
+- If you want to list all Speed values in a prettier way, try this:
+
+```Python
+import Winfo
+
+prettylist = ""
+
+for i in Winfo.memory.getSpeedAll():
+    prettylist = prettylist + i + "\n"
+
+print(prettylist)
+```
+
+- Instead of looking like this when printed:
+
+```
+[3000, 3000]
+```
+
+- It would now look like this:
+
+```
+3000
+3000
+
 ```
 
 ### Disk Information
 
 - List all connected disks (Returns them in a Python list)
 - Get Disk Size (Capacity) of disk 0, if you want to get the size of another disks set it's number as the index argument in the function
 
@@ -71,15 +99,15 @@
 import Winfo
 
 print("Here's a list of all my disks as a Python List: " + str(Winfo.disk.listall()))
 print("The size of my primary disk is: " + Winfo.disk.getsize())
 print("The size of my secondary disk is: " + Winfo.disk.getsize(1))
 ```
 
-- BONUS TIP! If you want to list all disks in a prettier way try this:
+- Like with the getSpeedAll, if you want to list all disks in a prettier way try this:
 
 ```Python
 import Winfo
 
 prettylist = ""
 
 for i in Winfo.disk.listall():
@@ -110,15 +138,15 @@
 ```Python
 import Winfo
 
 print("My MAC Address is: " + Winfo.ethernet.macaddr())
 print("List of all Network Adapters as a Python list: " + Winfo.ethernet.listadapters())
 ```
 
-- Like with the Disklist, you can make the list returned from Winfo.ethernet.listadapters() way prettier by doing this:
+- Like with the Disklist and the getSpeedAll, you can make the list returned from Winfo.ethernet.listadapters() way prettier by doing this:
 
 ```Python
 import Winfo
 
 prettylist = ""
 
 for i in Winfo.ethernet.listadapters():
```

### Comparing `Winfo-0.0.2.6/setup.py` & `Winfo-0.0.2.7/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as f:
     readme = f.read()
     f.close()
     
 setup(
     name="Winfo",
-    version="0.0.2.6",
+    version="0.0.2.7",
     author="BLUEAMETHYST Studios",
     description="Get information about your windows system",
     long_description_content_type="text/markdown",
     long_description=readme,
     packages=find_packages(),
     keywords=['python', 'windows', 'util', 'information', 'system'],
     classifiers=[
```

