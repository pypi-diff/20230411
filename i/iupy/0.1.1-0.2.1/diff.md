# Comparing `tmp/iupy-0.1.1.tar.gz` & `tmp/iupy-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iupy-0.1.1.tar", last modified: Wed Dec 15 01:37:05 2021, max compression
+gzip compressed data, was "iupy-0.2.1.tar", last modified: Thu Apr  6 00:38:23 2023, max compression
```

## Comparing `iupy-0.1.1.tar` & `iupy-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,21 @@
-drwxr-xr-x   0 ch191256   (501) staff       (20)        0 2021-12-15 01:37:05.058472 iupy-0.1.1/
--rw-r--r--   0 ch191256   (501) staff       (20)     1073 2021-10-23 21:30:44.000000 iupy-0.1.1/LICENSE
--rw-r--r--   0 ch191256   (501) staff       (20)     2731 2021-12-15 01:37:05.058572 iupy-0.1.1/PKG-INFO
--rw-r--r--   0 ch191256   (501) staff       (20)     2004 2021-11-02 12:56:05.000000 iupy-0.1.1/README.md
--rw-r--r--   0 ch191256   (501) staff       (20)      106 2021-10-25 15:52:39.000000 iupy-0.1.1/pyproject.toml
--rw-r--r--   0 ch191256   (501) staff       (20)      781 2021-12-15 01:37:05.059099 iupy-0.1.1/setup.cfg
-drwxr-xr-x   0 ch191256   (501) staff       (20)        0 2021-12-15 01:37:05.053895 iupy-0.1.1/src/
-drwxr-xr-x   0 ch191256   (501) staff       (20)        0 2021-12-15 01:37:05.056939 iupy-0.1.1/src/iupy/
--rw-r--r--   0 ch191256   (501) staff       (20)       67 2021-11-29 22:15:36.000000 iupy-0.1.1/src/iupy/__init__.py
--rw-r--r--   0 ch191256   (501) staff       (20)     1111 2021-11-29 22:15:36.000000 iupy-0.1.1/src/iupy/misc.py
--rw-r--r--   0 ch191256   (501) staff       (20)     4001 2021-11-29 22:15:36.000000 iupy-0.1.1/src/iupy/myconfig.py
--rw-r--r--   0 ch191256   (501) staff       (20)     5648 2021-11-29 22:15:36.000000 iupy-0.1.1/src/iupy/network.py
-drwxr-xr-x   0 ch191256   (501) staff       (20)        0 2021-12-15 01:37:05.058232 iupy-0.1.1/src/iupy.egg-info/
--rw-r--r--   0 ch191256   (501) staff       (20)     2731 2021-12-15 01:37:05.000000 iupy-0.1.1/src/iupy.egg-info/PKG-INFO
--rw-r--r--   0 ch191256   (501) staff       (20)      249 2021-12-15 01:37:05.000000 iupy-0.1.1/src/iupy.egg-info/SOURCES.txt
--rw-r--r--   0 ch191256   (501) staff       (20)        1 2021-12-15 01:37:05.000000 iupy-0.1.1/src/iupy.egg-info/dependency_links.txt
--rw-r--r--   0 ch191256   (501) staff       (20)        5 2021-12-15 01:37:05.000000 iupy-0.1.1/src/iupy.egg-info/top_level.txt
+drwxr-xr-x   0 ch191256   (501) staff       (20)        0 2023-04-06 00:38:23.015311 iupy-0.2.1/
+-rw-r--r--   0 ch191256   (501) staff       (20)     1073 2022-09-11 21:20:10.000000 iupy-0.2.1/LICENSE
+-rw-r--r--   0 ch191256   (501) staff       (20)     3673 2023-04-06 00:38:23.015364 iupy-0.2.1/PKG-INFO
+-rw-r--r--   0 ch191256   (501) staff       (20)     2845 2023-04-03 13:05:15.000000 iupy-0.2.1/README.md
+-rw-r--r--   0 ch191256   (501) staff       (20)      106 2022-09-11 21:20:10.000000 iupy-0.2.1/pyproject.toml
+-rw-r--r--   0 ch191256   (501) staff       (20)      861 2023-04-06 00:38:23.015580 iupy-0.2.1/setup.cfg
+drwxr-xr-x   0 ch191256   (501) staff       (20)        0 2023-04-06 00:38:23.012148 iupy-0.2.1/src/
+drwxr-xr-x   0 ch191256   (501) staff       (20)        0 2023-04-06 00:38:23.014353 iupy-0.2.1/src/iupy/
+-rw-r--r--   0 ch191256   (501) staff       (20)       67 2022-09-11 21:20:10.000000 iupy-0.2.1/src/iupy/__init__.py
+-rw-r--r--   0 ch191256   (501) staff       (20)     1691 2023-04-03 13:05:15.000000 iupy-0.2.1/src/iupy/misc.py
+-rw-r--r--   0 ch191256   (501) staff       (20)     4001 2023-03-31 23:16:00.000000 iupy-0.2.1/src/iupy/myconfig.py
+-rw-r--r--   0 ch191256   (501) staff       (20)    10862 2023-04-06 00:32:03.000000 iupy-0.2.1/src/iupy/network.py
+drwxr-xr-x   0 ch191256   (501) staff       (20)        0 2023-04-06 00:38:23.014821 iupy-0.2.1/src/iupy.egg-info/
+-rw-r--r--   0 ch191256   (501) staff       (20)     3673 2023-04-06 00:38:23.000000 iupy-0.2.1/src/iupy.egg-info/PKG-INFO
+-rw-r--r--   0 ch191256   (501) staff       (20)      312 2023-04-06 00:38:23.000000 iupy-0.2.1/src/iupy.egg-info/SOURCES.txt
+-rw-r--r--   0 ch191256   (501) staff       (20)        1 2023-04-06 00:38:23.000000 iupy-0.2.1/src/iupy.egg-info/dependency_links.txt
+-rw-r--r--   0 ch191256   (501) staff       (20)        5 2023-04-06 00:38:23.000000 iupy-0.2.1/src/iupy.egg-info/top_level.txt
+drwxr-xr-x   0 ch191256   (501) staff       (20)        0 2023-04-06 00:38:23.015215 iupy-0.2.1/tests/
+-rw-r--r--   0 ch191256   (501) staff       (20)     1299 2022-09-11 21:20:10.000000 iupy-0.2.1/tests/test_myconfig.py
+-rw-r--r--   0 ch191256   (501) staff       (20)     2771 2022-09-11 21:20:10.000000 iupy-0.2.1/tests/test_network.py
+-rw-r--r--   0 ch191256   (501) staff       (20)     1841 2023-04-06 00:32:03.000000 iupy-0.2.1/tests/test_sap.py
```

### Comparing `iupy-0.1.1/LICENSE` & `iupy-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `iupy-0.1.1/PKG-INFO` & `iupy-0.2.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,54 +1,69 @@
 Metadata-Version: 2.1
 Name: iupy
-Version: 0.1.1
+Version: 0.2.1
 Summary: Ian Underwood Python kit
 Home-page: https://github.com/iunderwood/iupy
 Author: Ian A. Underwood
 Author-email: ian@underwood-hq.org
 License: MIT License
 Platform: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # iupy
-Ian Underwood Python Kit
+Ian Underwood Python Kit (IUPY)
 
 ## About
 This package is a set of Python functions that I have built out and found useful in my travels as a network engineer.  This is the base package for all iupy additional packages to follow.
 
 This functions in this package are meant to be standalone packages and have no other package dependencies beyond a base Python installation.  These functions are designed to be light on requirements.
 
-This package has been built and tested against Python 3.9, and may work in earlier versions.
+This package has been built and tested against Python 3.9, and should work down to 3.7 but I can't guarantee that.
 
 ## Function Summary
 
 ### misc.py
 
 iupy.text_header : Returns a text header returning the time, user, and system a given output was generated on.  Additional options allow for identifying a source, as well as another user if specified.  A footer may also be defined.
 
+iupy.merge_dict : Returns a combined dictionary given two dictionary inputs.
+
 ### myconfig.py
 
 iupy.get_file_handle_ro : Returns a file handle given a name, or None if the file cannot be found or is inaccessible.  Exceptions are logged to DEBUG.
 
 iupy.get_my_config : Moves through a series of directories looking for a configuration file needed by a script.  This returns a data dictionary containing the data, the filename used, and the file's timestamp.  Useful for baking portable CLI utilities and automated scripts.
 
 ### network.py
 
-iupy.get_my_ip : Returns a string, the source IP given a remote IP address or destination.  Returns None if there is a SocketError which prevents the source from being determined.
+#### Host Information
+
+iupy.get_my_ip : Returns a string, the source IP given a remote IP address or destination.  Returns None if there is a SocketError which prevents the source from being determined.  If no destination is specified, the function assumes well-known DNS server 4.2.2.1
+
+#### ACL and Bitmask Tools
 
 iupy.v4_bits_to_mask : Returns a string,  a netmask based upon the number of bits in relation to 0.0.0.0/bits.  Returns None if the mask is out of range.
 
 ippy.v4_mask_to_bits : Returns a string, as the largest number of consecutive bits given an IP address.  This is far more forgiving than the ipaddress library, which may be useful to some.
 
 iupy.v4_wildcard : This function returns a compliant wildcard for a given IP address.  This is similar to, but different than a host mask as a wildcard does not need to have a series of consecutive bits in order to be valid.
 
+iupy.aclv4_hostmask : Takes an IPv4 host or host/mask and returns a Cisco-compatible string for use in ACL generation.
+
+iupy.routev4_hostmask : Takes an IPv4 host or host/mask and returns a cisco-compatible string for use in generating static route statements.
+
+#### Session Announcement Protocol
+
+iupy.sap_segment : This function generates the segment portion of an RFC-2974 Session Announcement Protocol packet.  The segment still needs to but put on the wire with a UDP socket.  The keywords cover the fields the segment requires.  Returns None if any of the keywords are invalid or incomplete.
```

### Comparing `iupy-0.1.1/README.md` & `iupy-0.2.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,45 @@
 # iupy
-Ian Underwood Python Kit
+Ian Underwood Python Kit (IUPY)
 
 ## About
 This package is a set of Python functions that I have built out and found useful in my travels as a network engineer.  This is the base package for all iupy additional packages to follow.
 
 This functions in this package are meant to be standalone packages and have no other package dependencies beyond a base Python installation.  These functions are designed to be light on requirements.
 
-This package has been built and tested against Python 3.9, and may work in earlier versions.
+This package has been built and tested against Python 3.9, and should work down to 3.7 but I can't guarantee that.
 
 ## Function Summary
 
 ### misc.py
 
 iupy.text_header : Returns a text header returning the time, user, and system a given output was generated on.  Additional options allow for identifying a source, as well as another user if specified.  A footer may also be defined.
 
+iupy.merge_dict : Returns a combined dictionary given two dictionary inputs.
+
 ### myconfig.py
 
 iupy.get_file_handle_ro : Returns a file handle given a name, or None if the file cannot be found or is inaccessible.  Exceptions are logged to DEBUG.
 
 iupy.get_my_config : Moves through a series of directories looking for a configuration file needed by a script.  This returns a data dictionary containing the data, the filename used, and the file's timestamp.  Useful for baking portable CLI utilities and automated scripts.
 
 ### network.py
 
-iupy.get_my_ip : Returns a string, the source IP given a remote IP address or destination.  Returns None if there is a SocketError which prevents the source from being determined.
+#### Host Information
+
+iupy.get_my_ip : Returns a string, the source IP given a remote IP address or destination.  Returns None if there is a SocketError which prevents the source from being determined.  If no destination is specified, the function assumes well-known DNS server 4.2.2.1
+
+#### ACL and Bitmask Tools
 
 iupy.v4_bits_to_mask : Returns a string,  a netmask based upon the number of bits in relation to 0.0.0.0/bits.  Returns None if the mask is out of range.
 
 ippy.v4_mask_to_bits : Returns a string, as the largest number of consecutive bits given an IP address.  This is far more forgiving than the ipaddress library, which may be useful to some.
 
-iupy.v4_wildcard : This function returns a compliant wildcard for a given IP address.  This is similar to, but different than a host mask as a wildcard does not need to have a series of consecutive bits in order to be valid.
+iupy.v4_wildcard : This function returns a compliant wildcard for a given IP address.  This is similar to, but different than a host mask as a wildcard does not need to have a series of consecutive bits in order to be valid.
+
+iupy.aclv4_hostmask : Takes an IPv4 host or host/mask and returns a Cisco-compatible string for use in ACL generation.
+
+iupy.routev4_hostmask : Takes an IPv4 host or host/mask and returns a cisco-compatible string for use in generating static route statements.
+
+#### Session Announcement Protocol
+
+iupy.sap_segment : This function generates the segment portion of an RFC-2974 Session Announcement Protocol packet.  The segment still needs to but put on the wire with a UDP socket.  The keywords cover the fields the segment requires.  Returns None if any of the keywords are invalid or incomplete.
```

### Comparing `iupy-0.1.1/src/iupy/myconfig.py` & `iupy-0.2.1/src/iupy/myconfig.py`

 * *Files identical despite different names*

### Comparing `iupy-0.1.1/src/iupy.egg-info/PKG-INFO` & `iupy-0.2.1/src/iupy.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,54 +1,69 @@
 Metadata-Version: 2.1
 Name: iupy
-Version: 0.1.1
+Version: 0.2.1
 Summary: Ian Underwood Python kit
 Home-page: https://github.com/iunderwood/iupy
 Author: Ian A. Underwood
 Author-email: ian@underwood-hq.org
 License: MIT License
 Platform: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # iupy
-Ian Underwood Python Kit
+Ian Underwood Python Kit (IUPY)
 
 ## About
 This package is a set of Python functions that I have built out and found useful in my travels as a network engineer.  This is the base package for all iupy additional packages to follow.
 
 This functions in this package are meant to be standalone packages and have no other package dependencies beyond a base Python installation.  These functions are designed to be light on requirements.
 
-This package has been built and tested against Python 3.9, and may work in earlier versions.
+This package has been built and tested against Python 3.9, and should work down to 3.7 but I can't guarantee that.
 
 ## Function Summary
 
 ### misc.py
 
 iupy.text_header : Returns a text header returning the time, user, and system a given output was generated on.  Additional options allow for identifying a source, as well as another user if specified.  A footer may also be defined.
 
+iupy.merge_dict : Returns a combined dictionary given two dictionary inputs.
+
 ### myconfig.py
 
 iupy.get_file_handle_ro : Returns a file handle given a name, or None if the file cannot be found or is inaccessible.  Exceptions are logged to DEBUG.
 
 iupy.get_my_config : Moves through a series of directories looking for a configuration file needed by a script.  This returns a data dictionary containing the data, the filename used, and the file's timestamp.  Useful for baking portable CLI utilities and automated scripts.
 
 ### network.py
 
-iupy.get_my_ip : Returns a string, the source IP given a remote IP address or destination.  Returns None if there is a SocketError which prevents the source from being determined.
+#### Host Information
+
+iupy.get_my_ip : Returns a string, the source IP given a remote IP address or destination.  Returns None if there is a SocketError which prevents the source from being determined.  If no destination is specified, the function assumes well-known DNS server 4.2.2.1
+
+#### ACL and Bitmask Tools
 
 iupy.v4_bits_to_mask : Returns a string,  a netmask based upon the number of bits in relation to 0.0.0.0/bits.  Returns None if the mask is out of range.
 
 ippy.v4_mask_to_bits : Returns a string, as the largest number of consecutive bits given an IP address.  This is far more forgiving than the ipaddress library, which may be useful to some.
 
 iupy.v4_wildcard : This function returns a compliant wildcard for a given IP address.  This is similar to, but different than a host mask as a wildcard does not need to have a series of consecutive bits in order to be valid.
 
+iupy.aclv4_hostmask : Takes an IPv4 host or host/mask and returns a Cisco-compatible string for use in ACL generation.
+
+iupy.routev4_hostmask : Takes an IPv4 host or host/mask and returns a cisco-compatible string for use in generating static route statements.
+
+#### Session Announcement Protocol
+
+iupy.sap_segment : This function generates the segment portion of an RFC-2974 Session Announcement Protocol packet.  The segment still needs to but put on the wire with a UDP socket.  The keywords cover the fields the segment requires.  Returns None if any of the keywords are invalid or incomplete.
```

