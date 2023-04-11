# Comparing `tmp/LocalResolver-0.0.3.tar.gz` & `tmp/LocalResolver-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LocalResolver-0.0.3.tar", last modified: Sun Apr  9 15:25:30 2023, max compression
+gzip compressed data, was "LocalResolver-1.0.0.tar", last modified: Tue Apr 11 17:28:14 2023, max compression
```

## Comparing `LocalResolver-0.0.3.tar` & `LocalResolver-1.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-09 15:25:30.393651 LocalResolver-0.0.3/
--rw-r--r--   0 kali      (1000) kali      (1000)    35149 2023-04-06 19:27:34.000000 LocalResolver-0.0.3/LICENSE.txt
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-09 15:25:30.393651 LocalResolver-0.0.3/LocalResolver.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)     2371 2023-04-09 15:25:30.000000 LocalResolver-0.0.3/LocalResolver.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      293 2023-04-09 15:25:30.000000 LocalResolver-0.0.3/LocalResolver.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-04-09 15:25:30.000000 LocalResolver-0.0.3/LocalResolver.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       59 2023-04-09 15:25:30.000000 LocalResolver-0.0.3/LocalResolver.egg-info/entry_points.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        6 2023-04-09 15:25:30.000000 LocalResolver-0.0.3/LocalResolver.egg-info/requires.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       14 2023-04-09 15:25:30.000000 LocalResolver-0.0.3/LocalResolver.egg-info/top_level.txt
--rw-r--r--   0 kali      (1000) kali      (1000)     7561 2023-04-09 15:25:13.000000 LocalResolver-0.0.3/LocalResolver.py
--rw-r--r--   0 kali      (1000) kali      (1000)       27 2023-04-06 19:27:34.000000 LocalResolver-0.0.3/MANIFEST.in
--rw-r--r--   0 kali      (1000) kali      (1000)     2371 2023-04-09 15:25:30.393651 LocalResolver-0.0.3/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)     1174 2023-04-06 20:12:08.000000 LocalResolver-0.0.3/README.md
--rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-04-09 15:25:30.393651 LocalResolver-0.0.3/setup.cfg
--rw-r--r--   0 kali      (1000) kali      (1000)     1619 2023-04-09 15:25:18.000000 LocalResolver-0.0.3/setup.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-11 17:28:14.629609 LocalResolver-1.0.0/
+-rw-r--r--   0 kali      (1000) kali      (1000)    35149 2023-04-07 01:27:34.000000 LocalResolver-1.0.0/LICENSE.txt
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-11 17:28:14.629609 LocalResolver-1.0.0/LocalResolver.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)     2791 2023-04-11 17:28:14.000000 LocalResolver-1.0.0/LocalResolver.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      283 2023-04-11 17:28:14.000000 LocalResolver-1.0.0/LocalResolver.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-04-11 17:28:14.000000 LocalResolver-1.0.0/LocalResolver.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       53 2023-04-11 17:28:14.000000 LocalResolver-1.0.0/LocalResolver.egg-info/entry_points.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       21 2023-04-11 17:28:14.000000 LocalResolver-1.0.0/LocalResolver.egg-info/requires.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       14 2023-04-11 17:28:14.000000 LocalResolver-1.0.0/LocalResolver.egg-info/top_level.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)    41489 2023-04-11 23:26:24.000000 LocalResolver-1.0.0/LocalResolver.py
+-rw-r--r--   0 kali      (1000) kali      (1000)       27 2023-04-07 01:27:34.000000 LocalResolver-1.0.0/MANIFEST.in
+-rw-r--r--   0 kali      (1000) kali      (1000)     2791 2023-04-11 17:28:14.629609 LocalResolver-1.0.0/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)     1626 2023-04-11 23:24:00.000000 LocalResolver-1.0.0/README.md
+-rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-04-11 17:28:14.629609 LocalResolver-1.0.0/setup.cfg
+-rw-r--r--   0 kali      (1000) kali      (1000)     1556 2023-04-11 23:23:52.000000 LocalResolver-1.0.0/setup.py
```

### Comparing `LocalResolver-0.0.3/LICENSE.txt` & `LocalResolver-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `LocalResolver-0.0.3/LocalResolver.egg-info/PKG-INFO` & `LocalResolver-1.0.0/LocalResolver.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: LocalResolver
-Version: 0.0.3
-Summary: This package implements local hostname resolver tool with scapy (using netbios and LLMNR query).
+Version: 1.0.0
+Summary: This package implements local hostname resolver tool with scapy.
 Home-page: https://github.com/mauricelambert/LocalResolver
 Author: Maurice Lambert
 Author-email: mauricelambert434@gmail.com
 Maintainer: Maurice Lambert
 Maintainer-email: mauricelambert434@gmail.com
 License: GPL-3.0 License
 Project-URL: Executable, https://mauricelambert.github.io/info/python/code/LocalResolver.pyz
@@ -38,39 +38,43 @@
 ## Requirements
 
 This package require: 
 
  - python3
  - python3 Standard Library
  - Scapy
+ - PythonToolsKit
 
 ## Installation
 
 ```bash
 pip install LocalResolver 
 ```
 
 ## Examples
 
 ### Command lines
 
 ```bash
-HostnameResolver -h
-HostnameResolver 192.168.1.2
-HostnameResolver 192.168.1.3,192.168.1.2,WIN10,HOMEPC,example.com
+LocalResolver -h
+LocalResolver --retry 5 --timeout 5 --interval 2 192.168.1.2   # very long
+LocalResolver 192.168.1.3 192.168.1.2 WIN10 HOMEPC test.local
+LocalResolver --no-netbios --no-dns fe80::3317:f73e:2166:bbd8/64
+LocalResolver --no-llmnr --no-mdns fe80::3317:f73e:2166:bbd8/64
 ```
 
 ### Python3
 
 ```python
-from LocalResolver import LocalResolver
+from LocalResolver import LocalResolver, resolve_local_name, resolve_local_ip
 
-localResolver = LocalResolver("192.168.1.45", timeout=3)
-hostname = localResolver.resolve_NBTNS()
-hostname = localResolver.resolve_LLMNR()
+[r.hostname for r in resolve_local_ip("192.168.5.2")]
+[r.ip for r in resolve_local_ip("192.168.5.2", retry=2, inter=1, timeout=3, netbios=True, llmnr=True, mdns=True, dns=True)]
+[(r.ip, r.source) for r in resolve_local_name("WIN10")]
+[(r.ip, r.source) for r in resolve_local_name("HOMEPC", retry=2, inter=1, timeout=3, netbios=True, llmnr=True, mdns=True, dns=True)]
 ```
 
 ## Links
 
  - [Github Page](https://github.com/mauricelambert/LocalResolver)
  - [Documentation](https://mauricelambert.github.io/info/python/code/LocalResolver.html)
  - [Download as python executable](https://mauricelambert.github.io/info/python/code/LocalResolver.pyz)
```

### Comparing `LocalResolver-0.0.3/PKG-INFO` & `LocalResolver-1.0.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: LocalResolver
-Version: 0.0.3
-Summary: This package implements local hostname resolver tool with scapy (using netbios and LLMNR query).
+Version: 1.0.0
+Summary: This package implements local hostname resolver tool with scapy.
 Home-page: https://github.com/mauricelambert/LocalResolver
 Author: Maurice Lambert
 Author-email: mauricelambert434@gmail.com
 Maintainer: Maurice Lambert
 Maintainer-email: mauricelambert434@gmail.com
 License: GPL-3.0 License
 Project-URL: Executable, https://mauricelambert.github.io/info/python/code/LocalResolver.pyz
@@ -38,39 +38,43 @@
 ## Requirements
 
 This package require: 
 
  - python3
  - python3 Standard Library
  - Scapy
+ - PythonToolsKit
 
 ## Installation
 
 ```bash
 pip install LocalResolver 
 ```
 
 ## Examples
 
 ### Command lines
 
 ```bash
-HostnameResolver -h
-HostnameResolver 192.168.1.2
-HostnameResolver 192.168.1.3,192.168.1.2,WIN10,HOMEPC,example.com
+LocalResolver -h
+LocalResolver --retry 5 --timeout 5 --interval 2 192.168.1.2   # very long
+LocalResolver 192.168.1.3 192.168.1.2 WIN10 HOMEPC test.local
+LocalResolver --no-netbios --no-dns fe80::3317:f73e:2166:bbd8/64
+LocalResolver --no-llmnr --no-mdns fe80::3317:f73e:2166:bbd8/64
 ```
 
 ### Python3
 
 ```python
-from LocalResolver import LocalResolver
+from LocalResolver import LocalResolver, resolve_local_name, resolve_local_ip
 
-localResolver = LocalResolver("192.168.1.45", timeout=3)
-hostname = localResolver.resolve_NBTNS()
-hostname = localResolver.resolve_LLMNR()
+[r.hostname for r in resolve_local_ip("192.168.5.2")]
+[r.ip for r in resolve_local_ip("192.168.5.2", retry=2, inter=1, timeout=3, netbios=True, llmnr=True, mdns=True, dns=True)]
+[(r.ip, r.source) for r in resolve_local_name("WIN10")]
+[(r.ip, r.source) for r in resolve_local_name("HOMEPC", retry=2, inter=1, timeout=3, netbios=True, llmnr=True, mdns=True, dns=True)]
 ```
 
 ## Links
 
  - [Github Page](https://github.com/mauricelambert/LocalResolver)
  - [Documentation](https://mauricelambert.github.io/info/python/code/LocalResolver.html)
  - [Download as python executable](https://mauricelambert.github.io/info/python/code/LocalResolver.pyz)
```

### Comparing `LocalResolver-0.0.3/setup.py` & `LocalResolver-1.0.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,43 +1,41 @@
 from setuptools import setup, find_packages
 
 setup(
-    name = 'LocalResolver',
-    version = "0.0.3",
+    name="LocalResolver",
+    version="1.0.0",
     py_modules=["LocalResolver"],
-    install_requires = ['scapy'],
-    author = "Maurice Lambert", 
-    author_email = "mauricelambert434@gmail.com",
+    install_requires=["scapy", "PythonToolsKit"],
+    author="Maurice Lambert",
+    author_email="mauricelambert434@gmail.com",
     maintainer="Maurice Lambert",
     maintainer_email="mauricelambert434@gmail.com",
-    description = "This package implements local hostname resolver tool with scapy (using netbios and LLMNR query).",
-    long_description = open('README.md').read(),
+    description="This package implements local hostname resolver tool with scapy.",
+    long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
-    url = 'https://github.com/mauricelambert/LocalResolver',
+    url="https://github.com/mauricelambert/LocalResolver",
     project_urls={
         "Executable": "https://mauricelambert.github.io/info/python/code/LocalResolver.pyz",
         "Documentation": "https://mauricelambert.github.io/info/python/code/LocalResolver.html",
     },
-    classifiers = [
+    classifiers=[
         "Environment :: Console",
         "Natural Language :: English",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.9",
         "Operating System :: MacOS",
         "Operating System :: POSIX :: Linux",
         "Operating System :: Microsoft :: Windows",
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     ],
-    entry_points = {
-        'console_scripts': [
-            'HostnameResolver = LocalResolver:resolve'
-        ],
+    entry_points={
+        "console_scripts": ["LocalResolver = LocalResolver:main"],
     },
-    python_requires='>=3.8',
+    python_requires=">=3.8",
     keywords=[
         "Resolve",
         "Hostname",
         "LLMNR",
         "Netbios",
     ],
     platforms=["Windows", "Linux", "MacOS"],
```

