# Comparing `tmp/whois-rdap-0.0.8.tar.gz` & `tmp/whois-rdap-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/srv/storage/projects/scripts/whois/dist/tmpol10q83c/whois-rdap-0.0.8.tar", last modified: Mon Mar 13 18:22:31 2023, max compression
+gzip compressed data, was "/srv/storage/projects/scripts/whois/dist/tmpibako9ju/whois-rdap-0.0.9.tar", last modified: Fri Mar 17 14:54:06 2023, max compression
```

## Comparing `whois-rdap-0.0.8.tar` & `whois-rdap-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-03-13 18:22:31.000000 whois-rdap-0.0.8/
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      104 2022-03-11 04:31:03.000000 whois-rdap-0.0.8/pyproject.toml
-drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-03-13 18:22:31.000000 whois-rdap-0.0.8/whois_rdap.egg-info/
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       14 2023-03-13 18:22:31.000000 whois-rdap-0.0.8/whois_rdap.egg-info/requires.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)        1 2023-03-13 18:22:31.000000 whois-rdap-0.0.8/whois_rdap.egg-info/dependency_links.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)        6 2023-03-13 18:22:31.000000 whois-rdap-0.0.8/whois_rdap.egg-info/top_level.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      229 2023-03-13 18:22:31.000000 whois-rdap-0.0.8/whois_rdap.egg-info/SOURCES.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      636 2023-03-13 18:22:31.000000 whois-rdap-0.0.8/whois_rdap.egg-info/PKG-INFO
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       56 2021-09-13 01:54:57.000000 whois-rdap-0.0.8/README.md
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)     1070 2021-09-13 01:54:57.000000 whois-rdap-0.0.8/LICENSE
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       66 2022-03-13 06:05:14.000000 whois-rdap-0.0.8/setup.py
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      636 2023-03-13 18:22:31.000000 whois-rdap-0.0.8/PKG-INFO
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      681 2023-03-13 18:22:31.000000 whois-rdap-0.0.8/setup.cfg
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)    10347 2023-03-13 18:21:16.000000 whois-rdap-0.0.8/whois.py
+drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-03-17 14:54:06.000000 whois-rdap-0.0.9/
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      104 2022-03-11 04:31:03.000000 whois-rdap-0.0.9/pyproject.toml
+drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-03-17 14:54:06.000000 whois-rdap-0.0.9/whois_rdap.egg-info/
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       14 2023-03-17 14:54:06.000000 whois-rdap-0.0.9/whois_rdap.egg-info/requires.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)        1 2023-03-17 14:54:06.000000 whois-rdap-0.0.9/whois_rdap.egg-info/dependency_links.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)        6 2023-03-17 14:54:06.000000 whois-rdap-0.0.9/whois_rdap.egg-info/top_level.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      229 2023-03-17 14:54:06.000000 whois-rdap-0.0.9/whois_rdap.egg-info/SOURCES.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      636 2023-03-17 14:54:06.000000 whois-rdap-0.0.9/whois_rdap.egg-info/PKG-INFO
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       56 2021-09-13 01:54:57.000000 whois-rdap-0.0.9/README.md
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)     1070 2021-09-13 01:54:57.000000 whois-rdap-0.0.9/LICENSE
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       66 2022-03-13 06:05:14.000000 whois-rdap-0.0.9/setup.py
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      636 2023-03-17 14:54:06.000000 whois-rdap-0.0.9/PKG-INFO
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      681 2023-03-17 14:54:06.000000 whois-rdap-0.0.9/setup.cfg
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)    10466 2023-03-17 14:52:31.000000 whois-rdap-0.0.9/whois.py
```

### Comparing `whois-rdap-0.0.8/whois_rdap.egg-info/PKG-INFO` & `whois-rdap-0.0.9/whois_rdap.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whois-rdap
-Version: 0.0.8
+Version: 0.0.9
 Summary: A small library for using the WHOIS (arin.net) RDAP protocol for whois lookups
 Home-page: https://github.com/ejohnfel/whois
 Author: Eric Johnfelt
 Author-email: ejohnfel@hotmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ejohnfel/whois/issues
 Platform: UNKNOWN
```

### Comparing `whois-rdap-0.0.8/LICENSE` & `whois-rdap-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `whois-rdap-0.0.8/PKG-INFO` & `whois-rdap-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whois-rdap
-Version: 0.0.8
+Version: 0.0.9
 Summary: A small library for using the WHOIS (arin.net) RDAP protocol for whois lookups
 Home-page: https://github.com/ejohnfel/whois
 Author: Eric Johnfelt
 Author-email: ejohnfel@hotmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ejohnfel/whois/issues
 Platform: UNKNOWN
```

### Comparing `whois-rdap-0.0.8/setup.cfg` & `whois-rdap-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = whois-rdap
-version = 0.0.8
+version = 0.0.9
 author = Eric Johnfelt
 author_email = ejohnfel@hotmail.com
 description = A small library for using the WHOIS (arin.net) RDAP protocol for whois lookups
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ejohnfel/whois
 project_urls =
```

### Comparing `whois-rdap-0.0.8/whois.py` & `whois-rdap-0.0.9/whois.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,25 +12,25 @@
 import random
 import json
 import ipaddress
 import time
 from collections import namedtuple
 
 import py_helper as ph
-from py_helper import DebugMode, CmdLineMode, ModuleMode, Msg, DbgMsg
+from py_helper import DebugMode, CmdLineMode, ModuleMode, Msg, DbgMsg, ValidIP, IsNetwork
 
 # Init Random
 random.seed()
 
 #
 # Variables
 #
 
 # Version
-VERSION=(0,0,8)
+VERSION=(0,0,9)
 Version = __version__ = ".".join([ str(x) for x in VERSION ])
 
 # Parser
 __Parser__ = None
 
 # Email Addess Expression
 loose_emailaddr_exp = "(?P<username>[\w_-]+)@(?P<domain>([\w\-]+\.)+([\w\-]*))"
@@ -261,14 +261,20 @@
 	# Init these
 	response = payload = None
 
 	# Format :
 	# RDAP-Exit-Code, Rec-Name, Rec-Handle, StartAddr, EndAddr, CIDR, parentHandle, abuse, payload, country
 	result = WhoisResult(404, None, None, None, None, None, None, None, None, None)
 
+	if IsNetwork(ipaddr):
+		ipaddr = ipaddr.rsplit("/")[0]
+
+	if not ValidIP(ipaddr):
+		return result
+
 	while retry_count < retry_limit:
 		response = payload = None
 
 		try:
 			response, payload = whois_rdap(MkUrl(ip,ipaddr))
 		except requests.ConnectionError:
 			time.sleep(retry_in)			# Most likely a rate limit hit
```

