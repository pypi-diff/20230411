# Comparing `tmp/coscine-0.9.0.tar.gz` & `tmp/coscine-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/coscine-0.9.0.tar", last modified: Thu Mar  9 04:08:47 2023, max compression
+gzip compressed data, was "dist/coscine-0.9.1.tar", last modified: Tue Apr 11 13:21:26 2023, max compression
```

## Comparing `coscine-0.9.0.tar` & `coscine-0.9.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 04:08:47.000000 coscine-0.9.0/
--rw-rw-rw-   0 root         (0) root         (0)     1084 2023-03-09 03:41:36.000000 coscine-0.9.0/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     7001 2023-03-09 04:08:47.000000 coscine-0.9.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5471 2023-03-09 03:41:36.000000 coscine-0.9.0/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-09 04:08:47.000000 coscine-0.9.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3905 2023-03-09 03:41:36.000000 coscine-0.9.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 04:08:47.000000 coscine-0.9.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 04:08:47.000000 coscine-0.9.0/src/coscine/
--rw-rw-rw-   0 root         (0) root         (0)     2863 2023-03-09 03:41:36.000000 coscine-0.9.0/src/coscine/__about__.py
--rw-rw-rw-   0 root         (0) root         (0)     2231 2023-03-09 03:41:36.000000 coscine-0.9.0/src/coscine/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6267 2023-03-09 03:41:36.000000 coscine-0.9.0/src/coscine/cache.py
--rw-rw-rw-   0 root         (0) root         (0)    22139 2023-03-09 03:41:36.000000 coscine-0.9.0/src/coscine/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 04:08:47.000000 coscine-0.9.0/src/coscine/data/
--rw-rw-rw-   0 root         (0) root         (0)     1991 2023-03-09 03:41:36.000000 coscine-0.9.0/src/coscine/data/project.json
--rw-rw-rw-   0 root         (0) root         (0)     2029 2023-03-09 03:41:36.000000 coscine-0.9.0/src/coscine/data/resource.json
--rw-rw-rw-   0 root         (0) root         (0)     2276 2023-03-09 03:41:36.000000 coscine-0.9.0/src/coscine/defaults.py
--rw-rw-rw-   0 root         (0) root         (0)    27223 2023-03-09 03:59:26.000000 coscine-0.9.0/src/coscine/form.py
--rw-rw-rw-   0 root         (0) root         (0)     6910 2023-03-09 03:59:26.000000 coscine-0.9.0/src/coscine/graph.py
--rw-rw-rw-   0 root         (0) root         (0)    17140 2023-03-09 03:41:36.000000 coscine-0.9.0/src/coscine/object.py
--rw-rw-rw-   0 root         (0) root         (0)    20953 2023-03-09 03:56:44.000000 coscine-0.9.0/src/coscine/project.py
--rw-rw-rw-   0 root         (0) root         (0)    24963 2023-03-09 03:41:36.000000 coscine-0.9.0/src/coscine/resource.py
--rw-rw-rw-   0 root         (0) root         (0)     7402 2023-03-09 03:41:36.000000 coscine-0.9.0/src/coscine/s3.py
--rw-rw-rw-   0 root         (0) root         (0)    11884 2023-03-09 03:41:36.000000 coscine-0.9.0/src/coscine/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    14870 2023-03-09 03:41:36.000000 coscine-0.9.0/src/coscine/vocabulary.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 04:08:47.000000 coscine-0.9.0/src/coscine.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7001 2023-03-09 04:08:47.000000 coscine-0.9.0/src/coscine.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      556 2023-03-09 04:08:47.000000 coscine-0.9.0/src/coscine.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-09 04:08:47.000000 coscine-0.9.0/src/coscine.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       84 2023-03-09 04:08:47.000000 coscine-0.9.0/src/coscine.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-03-09 04:08:47.000000 coscine-0.9.0/src/coscine.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:21:26.000000 coscine-0.9.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1084 2023-03-09 03:41:37.000000 coscine-0.9.1/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)     7001 2023-04-11 13:21:26.000000 coscine-0.9.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5471 2023-03-09 03:41:37.000000 coscine-0.9.1/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-11 13:21:26.000000 coscine-0.9.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3905 2023-03-09 03:41:37.000000 coscine-0.9.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:21:26.000000 coscine-0.9.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:21:26.000000 coscine-0.9.1/src/coscine/
+-rw-rw-rw-   0 root         (0) root         (0)     2949 2023-04-11 13:11:24.000000 coscine-0.9.1/src/coscine/__about__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2231 2023-03-09 03:41:37.000000 coscine-0.9.1/src/coscine/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6267 2023-03-09 03:41:37.000000 coscine-0.9.1/src/coscine/cache.py
+-rw-rw-rw-   0 root         (0) root         (0)    24288 2023-04-11 13:11:24.000000 coscine-0.9.1/src/coscine/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:21:26.000000 coscine-0.9.1/src/coscine/data/
+-rw-rw-rw-   0 root         (0) root         (0)     1991 2023-03-09 03:41:37.000000 coscine-0.9.1/src/coscine/data/project.json
+-rw-rw-rw-   0 root         (0) root         (0)     2029 2023-03-09 03:41:37.000000 coscine-0.9.1/src/coscine/data/resource.json
+-rw-rw-rw-   0 root         (0) root         (0)     2276 2023-03-09 03:41:37.000000 coscine-0.9.1/src/coscine/defaults.py
+-rw-rw-rw-   0 root         (0) root         (0)    28275 2023-04-11 13:11:24.000000 coscine-0.9.1/src/coscine/form.py
+-rw-rw-rw-   0 root         (0) root         (0)     6910 2023-03-09 03:59:25.000000 coscine-0.9.1/src/coscine/graph.py
+-rw-rw-rw-   0 root         (0) root         (0)    19225 2023-04-11 13:18:30.000000 coscine-0.9.1/src/coscine/object.py
+-rw-rw-rw-   0 root         (0) root         (0)    21761 2023-04-11 13:11:24.000000 coscine-0.9.1/src/coscine/project.py
+-rw-rw-rw-   0 root         (0) root         (0)    26349 2023-04-11 13:18:30.000000 coscine-0.9.1/src/coscine/resource.py
+-rw-rw-rw-   0 root         (0) root         (0)     7402 2023-03-09 03:41:37.000000 coscine-0.9.1/src/coscine/s3.py
+-rw-rw-rw-   0 root         (0) root         (0)    11884 2023-03-09 03:41:37.000000 coscine-0.9.1/src/coscine/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    14870 2023-03-09 03:41:37.000000 coscine-0.9.1/src/coscine/vocabulary.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:21:26.000000 coscine-0.9.1/src/coscine.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7001 2023-04-11 13:21:26.000000 coscine-0.9.1/src/coscine.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      556 2023-04-11 13:21:26.000000 coscine-0.9.1/src/coscine.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 13:21:26.000000 coscine-0.9.1/src/coscine.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       84 2023-04-11 13:21:26.000000 coscine-0.9.1/src/coscine.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-11 13:21:26.000000 coscine-0.9.1/src/coscine.egg-info/top_level.txt
```

### Comparing `coscine-0.9.0/LICENSE.txt` & `coscine-0.9.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `coscine-0.9.0/PKG-INFO` & `coscine-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coscine
-Version: 0.9.0
+Version: 0.9.1
 Summary: The Coscine Python SDK provides a pythonic interface to the Coscine REST API.
 Home-page: https://git.rwth-aachen.de/coscine/community-features/coscine-python-sdk/
 Author: RWTH Aachen University
 Author-email: coscine@itc.rwth-aachen.de
 License: MIT License
 Project-URL: Issues, https://git.rwth-aachen.de/coscine/community-features/coscine-python-sdk/-/issues
 Project-URL: Documentation, https://coscine.pages.rwth-aachen.de/community-features/coscine-python-sdk/
```

### Comparing `coscine-0.9.0/README.md` & `coscine-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `coscine-0.9.0/setup.py` & `coscine-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `coscine-0.9.0/src/coscine/__about__.py` & `coscine-0.9.1/src/coscine/__about__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,86 +1,86 @@
-###############################################################################
-# Coscine Python SDK
-# Copyright (c) 2018-2023 RWTH Aachen University
-# Licensed under the terms of the MIT License
-###############################################################################
-# Coscine, short for Collaborative Scientific Integration Environment, is
-# a platform for research data management (RDM).
-# For more information on Coscine visit https://www.coscine.de/.
-#
-# Please note that this python module is open source software primarily
-# developed and maintained by the scientific community. It is not
-# an official service that RWTH Aachen provides support for.
-###############################################################################
-
-###############################################################################
-# File description
-###############################################################################
-
-"""
-This file contains package metadata primarily intended for setup.py but
-also accessed by various source files in src/.
-"""
-
-###############################################################################
-# Module globals / Constants
-###############################################################################
-
-# Package title/name as it would appear in PyPi
-__title__ = "coscine"
-
-# Current package version
-# Do not set version to 1.0.0 before Coscine end of pilot phase
-__version__ = "0.9.0"
-
-# Short package description
-__summary__ = (
-    "The Coscine Python SDK provides a pythonic interface to "
-    "the Coscine REST API."
-)
-
-# Package copyright owner
-__author__ = "RWTH Aachen University"
-
-# Coscine contact (Note: This is the official Coscine contact email!)
-# Only for copyright claims, licensing issues or sourcecode hosting!
-# Please do not direct bug reports or feature requests to that address!
-# They are not responsible for the development, they "just" represent Coscine!
-__contact__ = "coscine@itc.rwth-aachen.de"
-
-# Package license
-__license__ = "MIT License"
-
-# Package keywords/tags (must be given as a list!)
-__keywords__ = ["Coscine", "RWTH Aachen", "Research Data Management"]
-
-# Package dependencies (must be given as a list!)
-__dependencies__ = [
-    "rdflib",
-    "requests",
-    "requests-toolbelt",
-    "tqdm",
-    "colorama",
-    "prettytable",
-    "appdirs",
-    "python-dateutil"
-]
-
-# Python version required
-__pyver__ = ">=3.7"
-
-# Project url (official sourcecode hosting)
-__url__ = (
-    "https://git.rwth-aachen.de/coscine/community-features/"
-    "coscine-python-sdk/"
-)
-
-# Additional urls for e.g. bug reports and documentation
-__project_urls__ = {
-    "Issues": __url__ + "-/issues",
-    "Documentation": (
-        "https://coscine.pages.rwth-aachen.de/"
-        "community-features/coscine-python-sdk/"
-    )
-}
-
-###############################################################################
+###############################################################################
+# Coscine Python SDK
+# Copyright (c) 2018-2023 RWTH Aachen University
+# Licensed under the terms of the MIT License
+###############################################################################
+# Coscine, short for Collaborative Scientific Integration Environment, is
+# a platform for research data management (RDM).
+# For more information on Coscine visit https://www.coscine.de/.
+#
+# Please note that this python module is open source software primarily
+# developed and maintained by the scientific community. It is not
+# an official service that RWTH Aachen provides support for.
+###############################################################################
+
+###############################################################################
+# File description
+###############################################################################
+
+"""
+This file contains package metadata primarily intended for setup.py but
+also accessed by various source files in src/.
+"""
+
+###############################################################################
+# Module globals / Constants
+###############################################################################
+
+# Package title/name as it would appear in PyPi
+__title__ = "coscine"
+
+# Current package version
+# Do not set version to 1.0.0 before Coscine end of pilot phase
+__version__ = "0.9.1"
+
+# Short package description
+__summary__ = (
+    "The Coscine Python SDK provides a pythonic interface to "
+    "the Coscine REST API."
+)
+
+# Package copyright owner
+__author__ = "RWTH Aachen University"
+
+# Coscine contact (Note: This is the official Coscine contact email!)
+# Only for copyright claims, licensing issues or sourcecode hosting!
+# Please do not direct bug reports or feature requests to that address!
+# They are not responsible for the development, they "just" represent Coscine!
+__contact__ = "coscine@itc.rwth-aachen.de"
+
+# Package license
+__license__ = "MIT License"
+
+# Package keywords/tags (must be given as a list!)
+__keywords__ = ["Coscine", "RWTH Aachen", "Research Data Management"]
+
+# Package dependencies (must be given as a list!)
+__dependencies__ = [
+    "rdflib",
+    "requests",
+    "requests-toolbelt",
+    "tqdm",
+    "colorama",
+    "prettytable",
+    "appdirs",
+    "python-dateutil"
+]
+
+# Python version required
+__pyver__ = ">=3.7"
+
+# Project url (official sourcecode hosting)
+__url__ = (
+    "https://git.rwth-aachen.de/coscine/community-features/"
+    "coscine-python-sdk/"
+)
+
+# Additional urls for e.g. bug reports and documentation
+__project_urls__ = {
+    "Issues": __url__ + "-/issues",
+    "Documentation": (
+        "https://coscine.pages.rwth-aachen.de/"
+        "community-features/coscine-python-sdk/"
+    )
+}
+
+###############################################################################
```

### Comparing `coscine-0.9.0/src/coscine/__init__.py` & `coscine-0.9.1/src/coscine/__init__.py`

 * *Files identical despite different names*

### Comparing `coscine-0.9.0/src/coscine/cache.py` & `coscine-0.9.1/src/coscine/cache.py`

 * *Files identical despite different names*

### Comparing `coscine-0.9.0/src/coscine/client.py` & `coscine-0.9.1/src/coscine/client.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,673 +1,720 @@
-###############################################################################
-# Coscine Python SDK
-# Copyright (c) 2018-2023 RWTH Aachen University
-# Licensed under the terms of the MIT License
-###############################################################################
-# Coscine, short for Collaborative Scientific Integration Environment, is
-# a platform for research data management (RDM).
-# For more information on Coscine visit https://www.coscine.de/.
-#
-# Please note that this python module is open source software primarily
-# developed and maintained by the scientific community. It is not
-# an official service that RWTH Aachen provides support for.
-###############################################################################
-
-###############################################################################
-# File description
-###############################################################################
-
-"""
-This file contains the backbone of the Coscine Python SDK - the client class.
-The client class acts as the manager of the SDK and is mainly
-responsible for the communication and exchange of information
-with Coscine servers.
-"""
-
-###############################################################################
-# Dependencies
-###############################################################################
-
-from __future__ import annotations
-from typing import List, Optional, Union
-import urllib.parse
-import logging
-import platform
-import requests
-import colorama
-from coscine.__about__ import __version__
-from coscine.cache import Cache
-from coscine.defaults import BASE_URL, LANGUAGES
-from coscine.project import Project, ProjectForm
-from coscine.resource import ResourceForm
-from coscine.utils import in_cli_mode
-from coscine.vocabulary import VocabularyManager
-
-###############################################################################
-# Module globals / Constants
-###############################################################################
-
-# Coscine REST API Endpoints
-API_ENDPOINTS = (
-    "Blob", "Metadata", "Organization", "Project", "Resources",
-    "Tree", "User", "Search", "ActivatedFeatures", "Notices"
-)
-
-# Get a logger handle.
-logger = logging.getLogger(__name__)
-
-# A colorful pretty banner to show on startup when run in a cli.
-# Note: The noqa comment disables flake8 linter rule E101 for this variable.
-BANNER: str = rf"""{colorama.Fore.BLUE}
-                     _
-                    (_)
-   ___ ___  ___  ___ _ _ __   ___
-  / __/ _ \/ __|/ __| | '_ \ / _ \
- | (_| (_) \__ \ (__| | | | |  __/
-  \___\___/|___/\___|_|_| |_|\___|{colorama.Fore.WHITE}
-____________________________________
-
-    Coscine Python SDK {colorama.Fore.YELLOW}{__version__}{colorama.Fore.WHITE}
-____________________________________
-"""  # noqa: E101
-
-###############################################################################
-# Classes / Functions / Scripts
-###############################################################################
-
-
-class Settings:
-    """
-    Contains settings for configuring the Coscine Client class.
-    """
-
-    _language: str
-    read_only: bool
-    concurrent: bool
-    persistent_cache: bool
-    verbose: bool
-
-###############################################################################
-
-    @property
-    def language(self) -> str:
-        """Returns the language setting"""
-        return self._language
-
-###############################################################################
-
-    @language.setter
-    def language(self, lang: str) -> None:
-        lang = lang.lower()
-        if lang in LANGUAGES:
-            self._language = lang
-        else:
-            errormessage: str = (
-                f"Invalid value for argument 'lang' -> [{lang}]!\n"
-                f"Possible values are {str(LANGUAGES)}."
-            )
-            raise ValueError(errormessage)
-
-###############################################################################
-
-    def __init__(
-        self,
-        language: str = "en",
-        persistent_cache: bool = True,
-        concurrent: bool = True,
-        read_only: bool = False,
-        verbose: bool = True
-    ) -> None:
-        """
-        Parameters
-        ----------
-        language : str, "en" or "de", default: "en"
-            Language preset for input form fields and vocabularies.
-        persistent_cache : bool, default: True
-            Enable to store the cache in a file on deinitialization of
-            the client object. Will attempt to load the cache file
-            on initialization if enabled. Leads to a significant speed
-            boost when making static requests right after init, but may
-            also lead to invalid data when using outdated cache data, in case
-            the Coscine API changed recently. However this is mostly avoided
-            by performing frequent updates. Useful for applications with
-            a short runtime that get run often.
-        concurrent : bool, default: True
-            If enabled, a ThreadPool is used for bulk requests, speeding up
-            up- and downloads of multiple files tremendously.
-        read_only : bool, default: False
-            Do not perform PUT, POST, DELETE requests
-        verbose : bool, default: True
-            Print stuff to stdout if running from a command line
-        """
-        self.concurrent = concurrent
-        self.read_only = read_only
-        self.persistent_cache = persistent_cache
-        self.language = language
-        self.verbose = verbose
-
-###############################################################################
-###############################################################################
-###############################################################################
-
-
-class Client:
-    """
-    The client class handles the connection with the Coscine server.
-    It performs requests to the API and returns the response data.
-    All objects of the Python SDK use a handle to the client to
-    communicate with Coscine.
-    """
-
-    cache: Cache
-    session: requests.Session
-    settings: Settings
-    vocabularies: VocabularyManager
-    _id: int = 0  # unique identifier for each client instance
-
-###############################################################################
-
-    @property
-    def version(self) -> str:
-        """Returns the current Coscine Python SDK version"""
-        return __version__
-
-###############################################################################
-
-    def __init__(self, token: str, settings: Settings = Settings()) -> None:
-        """
-        Initializes an instance of the base class of the Coscine Python SDK.
-
-        Parameters
-        ----------
-        token : str
-            A Coscine API access token.
-        settings : Settings
-            Coscine Python SDK client settings.
-        """
-
-        if not isinstance(token, str):
-            raise TypeError("Invalid token type: Expected string!")
-
-        self.settings = settings
-        self.cache = Cache(self.settings.persistent_cache)
-        self.vocabularies = VocabularyManager(self)
-        self.session = requests.Session()
-        self.session.headers.update({
-            "Authorization": f"Bearer {token}",
-            "User-Agent": f"Coscine Python SDK {self.version}"
-        })
-        if in_cli_mode():
-            colorama.init(autoreset=True)
-            print(BANNER)
-        self._id += 1
-        logger.info(
-            "Initialized Coscine Python SDK version %s "
-            "Client instance (id=%d)", __version__, self._id
-        )
-        logger.debug(self.sysinfo())
-        maintenance = self._maintenance_string()
-        if maintenance:
-            logger.info(maintenance)
-
-###############################################################################
-
-    @staticmethod
-    def sysinfo() -> str:
-        """
-        Constructs system information for better bug reports.
-
-        Returns
-        -------
-        str
-            Multiline string containing system and python information.
-        """
-
-        return f"""
-            Platform: {platform.platform()}
-            Machine: {platform.machine()}
-            Processor: {platform.processor()}
-            Python compiler: {platform.python_compiler()}
-            Python branch: {platform.python_branch()}
-            Python implementation: {platform.python_implementation()}
-            Python revision: {platform.python_revision()}
-            Python version: {platform.python_version()}
-        """.replace("\t", " ")
-
-###############################################################################
-
-    @staticmethod
-    def uri(api: str, endpoint: str, *args) -> str:
-        """
-        Constructs a URL for performing a request to the Coscine API.
-
-        Parameters
-        ----------
-        api : str
-            The target Coscine API endpoint, e.g. Blob, Metadata, Tree, ...
-        endpoint : str
-            The subendpoint of `api`.
-        *args
-            Variable number of arguments of type string to append to the URL.
-            Arguments are automatically seperated by a slash '/' and
-            special characters are encoded.
-
-        Raises
-        ------
-        ValueError
-            If the api / endpoint is invalid.
-
-        Returns
-        -------
-        str
-            Encoded URL for communicating with the Coscine servers.
-        """
-
-        if api not in API_ENDPOINTS:
-            raise ValueError(
-                "Invalid value for argument 'api'! "
-                f"Possible values are {str(API_ENDPOINTS)}."
-            )
-
-        uri = BASE_URL % (api, endpoint)
-        for arg in args:
-            if arg is None:
-                continue
-            uri += "/" + urllib.parse.quote(arg, safe="")
-        return uri
-
-###############################################################################
-
-    def _maintenance_string(self) -> str:
-        """
-        Returns the Coscine maintenance notice as a human-readable string
-        """
-        message: str = ""
-        notice = self.get_maintenance()
-        if notice["type"] is not None:
-            message = (
-                f"{notice['type']}\n"
-                f"{notice['displayName']}\n"
-                f"{notice['body']}\n"
-            )
-        return message
-
-###############################################################################
-
-    def get_maintenance(self) -> dict:
-        """
-        Returns the maintenance status of the Coscine service
-        """
-        uri = self.uri("Notices", "Notice", "getMaintenance")
-        return self.get(uri).json()
-
-###############################################################################
-
-    def _request(self, method: str, uri: str, **kwargs) -> requests.Response:
-        """
-        Performs a HTTP request to the Coscine Servers.
-
-        Parameters
-        ----------
-        method : str
-            HTTP request method (GET, PUT, POST, DELETE).
-        uri : str
-            Coscine URL generated with Client.uri(...).
-        **kwargs
-            Additional keyword arguments forwarded to the requests library.
-
-        Raises
-        ------
-        ConnectionError
-            If the Coscine servers could not be reached.
-        PermissionError
-            If the Coscine API token is invalid.
-        RuntimeError
-            If the request resulted in an error.
-
-        Returns
-        -------
-        requests.Response
-            The response of the Coscine server as a requests.Response object.
-        """
-
-        # Debugging URL
-        params = kwargs["params"] if "params" in kwargs else None
-        full_url = requests.Request(method, uri, params=params).prepare().url
-        if full_url:
-            logger.debug("HTTP %s: %s", method, full_url)
-        else:
-            logger.debug("HTTP %s: %s", method, uri)
-
-        # Handling read_only setting
-        if self.settings.read_only and method != "GET":
-            logger.warning("READ_ONLY mode in effect for %s: %s", method, uri)
-            return requests.Response()
-
-        try:  # performing the request and handle any resulting errors
-            response = self.session.request(method, uri, **kwargs)
-            response.raise_for_status()
-            logger.debug("response: %s", str(response.content))
-            return response
-        except requests.exceptions.ConnectionError as exc:
-            raise ConnectionError("Failed to connect to Coscine!") from exc
-        except requests.exceptions.RequestException as exc:
-            if exc.response.status_code == 401:
-                raise PermissionError("Invalid Coscine API token!") from exc
-            raise RuntimeError(
-                "Unspecified error occurred when communicating "
-                "with the Coscine servers"
-            ) from exc
-
-###############################################################################
-
-    def get(self, uri: str, **kwargs) -> requests.Response:
-        """
-        Performs a GET request to the Coscine API.
-
-        Parameters
-        ----------
-        uri : str
-            Coscine URL generated with Client.uri(...).
-        **kwargs
-            Additional keyword arguments forwarded to the requests library.
-
-        Examples
-        --------
-        >>> uri = Client.uri("Project", "Project")
-        >>> projects = Client.get(uri).json()
-
-        Raises
-        ------
-        ConnectionError
-            If the Coscine servers could not be reached.
-        PermissionError
-            If the Coscine API token is invalid.
-        RuntimeError
-            If the request resulted in an error.
-
-        Returns
-        -------
-        requests.Response
-            The response of the Coscine server as a requests.Response object.
-        """
-
-        return self._request("GET", uri, **kwargs)
-
-###############################################################################
-
-    def put(self, uri: str, **kwargs) -> requests.Response:
-        """
-        Performs a PUT request to the Coscine API.
-
-        Parameters
-        ----------
-        uri : str
-            Coscine URL generated with Client.uri(...).
-        **kwargs
-            Additional keyword arguments forwarded to the requests library.
-
-        Examples
-        --------
-        >>> uri = Client.uri("Tree", "Tree", resource.id, filename)
-        >>> Client.put(uri, data = metadata)
-
-        Raises
-        ------
-        ConnectionError
-            If the Coscine servers could not be reached.
-        PermissionError
-            If the Coscine API token is invalid.
-        RuntimeError
-            If the request resulted in an error.
-
-        Returns
-        -------
-        requests.Response
-            The response of the Coscine server as a requests.Response object.
-        """
-
-        return self._request("PUT", uri, **kwargs)
-
-###############################################################################
-
-    def post(self, uri: str, **kwargs) -> requests.Response:
-        """
-        Performs a POST request to the Coscine API.
-
-        Parameters
-        ----------
-        uri : str
-            Coscine URL generated with Client.uri(...).
-        **kwargs
-            Additional arguments forwarded to the requests library.
-
-        Examples
-        --------
-        >>> data = member.data
-        >>> data["projectId"] = Client.id
-        >>> data["role"]["displayName"] = "Member"
-        >>> data["role"]["id"] = ProjectMember.ROLES["Member"]
-        >>> uri = Client.uri("Project", "ProjectRole")
-        >>> Client.post(uri, data=data)
-
-        Raises
-        ------
-        ConnectionError
-            If the Coscine servers could not be reached.
-        PermissionError
-            If the Coscine API token is invalid.
-        RuntimeError
-            If the request resulted in an error.
-
-        Returns
-        -------
-        requests.Response
-            The response of the Coscine server as a requests.Response object.
-        """
-
-        return self._request("POST", uri, **kwargs)
-
-###############################################################################
-
-    def delete(self, uri: str, **kwargs) -> requests.Response:
-        """
-        Performs a DELETE request to the Coscine API.
-
-        Parameters
-        ----------
-        uri : str
-            Coscine URL generated with Client.uri(...).
-        **kwargs
-            Additional keyword arguments forwarded to the requests library.
-
-        Examples
-        --------
-        >>> uri = Client.uri("Project", "Project", Client.id)
-        >>> Client.delete(uri)
-
-        Raises
-        ------
-        ConnectionError
-            If the Coscine servers could not be reached.
-        PermissionError
-            If the Coscine API token is invalid.
-        RuntimeError
-            If the request resulted in an error.
-
-        Returns
-        -------
-        requests.Response
-            The response of the Coscine server as a requests.Response object.
-        """
-
-        return self._request("DELETE", uri, **kwargs)
-
-###############################################################################
-
-    def static_request(self, uri: str) -> dict:
-        """
-        Performs a GET request for the given uri. If such a request
-        has been performed previously during the current session, the previous
-        response is returned. Otherwise a new request is made to Coscine
-        and that response is then stored inside the session cache.
-
-        Parameters
-        -----------
-        uri : str
-            Request URI
-
-        Returns
-        -------
-        dict
-        """
-
-        logger.debug("static_request(%s)", uri)
-        data = self.cache.get(uri)
-        if data is None:
-            data = self.get(uri).json()
-            self.cache.set(uri, data)
-        return data
-
-###############################################################################
-
-    def project_form(self, data: Optional[dict] = None) -> ProjectForm:
-        """
-        Returns an empty project form.
-
-        Parameters
-        ----------
-        data : dict, default: None
-            If data is specified, the form is initialized with that data
-            using the InputForm.fill() method.
-        """
-        form = ProjectForm(self)
-        if data:
-            form.fill(data)
-        return form
-
-###############################################################################
-
-    def resource_form(self, data: Optional[dict] = None) -> ResourceForm:
-        """
-        Returns an empty resource form.
-
-        Parameters
-        ----------
-        data : dict, default: None
-            If data is specified, the form is initialized with that data
-            using the InputForm.fill() method.
-        """
-        form = ResourceForm(self)
-        if data:
-            form.fill(data)
-        return form
-
-###############################################################################
-
-    def projects(self, toplevel: bool = True) -> List[Project]:
-        """
-        Retrieves a list of a all projects the creator of
-        the Coscine API token is currently a member of.
-
-        Parameters
-        ----------
-        toplevel : bool, default: True
-            Retrieve only toplevel projects (no subprojects).
-            Set to False if you want to retrieve all projects, regardless
-            of hierarchy.
-
-        Returns
-        -------
-        List[Project]
-            List of coscine.Project objects
-        """
-
-        endpoint = ("Project", "Project/-/topLevel")
-        uri = self.uri("Project", endpoint[toplevel])
-        projects = []
-        for project_data in self.get(uri).json():
-            projects.append(Project(self, project_data))
-        return projects
-
-###############################################################################
-
-    def project(
-        self,
-        display_name: str,
-        toplevel: bool = True
-    ) -> Union[Project, None]:
-        """
-        Returns a single project via its displayName
-
-        Parameters
-        ----------
-        display_name : str
-            Look for a project with the specified displayName
-        toplevel : bool, default: True
-            Retrieve only toplevel projects (no subprojects).
-            Set to False if you want to retrieve all projects, regardless
-            of hierarchy.
-
-        Returns
-        -------
-        Project or None
-            A single coscine project handle or None if no match found
-
-        Raises
-        ------
-        IndexError
-            In case more than 1 project matches the specified criteria.
-        """
-        filtered_project_list = list(filter(
-            lambda project: project.display_name == display_name,
-            self.projects(toplevel)
-        ))
-        if len(filtered_project_list) == 1:
-            return filtered_project_list[0]
-        if len(filtered_project_list) == 0:
-            return None
-        raise IndexError(
-            "Received more than 1 project matching the specified "
-            f"criteria (display_name = '{display_name}')!"
-        )
-
-###############################################################################
-
-    def create_project(self, form: Union[ProjectForm, dict]) -> Project:
-        """
-        Creates a project using the given ProjectForm.
-
-        Parameters
-        ----------
-        form : ProjectForm or dict
-            ProjectForm filled with project metadata or a dict with the
-            data generated from a form.
-
-        Returns
-        -------
-        Project
-            Project object for the new project.
-        """
-
-        if isinstance(form, ProjectForm):
-            form = form.generate()
-        uri = self.uri("Project", "Project")
-        return Project(self, self.post(uri, json=form).json())
-
-###############################################################################
-
-    def search(self, query: str) -> dict:
-        """
-        Performs a Coscine search query.
-
-        Returns
-        --------
-        dict
-            The search results as a dict
-        """
-
-        uri = self.uri("Search", f"Search?query={query}")
-        results = self.get(uri).json()
-        return results
-
-###############################################################################
+###############################################################################
+# Coscine Python SDK
+# Copyright (c) 2018-2023 RWTH Aachen University
+# Licensed under the terms of the MIT License
+###############################################################################
+# Coscine, short for Collaborative Scientific Integration Environment, is
+# a platform for research data management (RDM).
+# For more information on Coscine visit https://www.coscine.de/.
+#
+# Please note that this python module is open source software primarily
+# developed and maintained by the scientific community. It is not
+# an official service that RWTH Aachen provides support for.
+###############################################################################
+
+###############################################################################
+# File description
+###############################################################################
+
+"""
+This file contains the backbone of the Coscine Python SDK - the client class.
+The client class acts as the manager of the SDK and is mainly
+responsible for the communication and exchange of information
+with Coscine servers.
+"""
+
+###############################################################################
+# Dependencies
+###############################################################################
+
+from __future__ import annotations
+from typing import List, Optional, Union
+import urllib.parse
+import logging
+import platform
+import requests
+import colorama
+from coscine.__about__ import __version__
+from coscine.cache import Cache
+from coscine.defaults import BASE_URL, LANGUAGES
+from coscine.project import Project, ProjectForm
+from coscine.resource import ResourceForm
+from coscine.utils import in_cli_mode
+from coscine.vocabulary import VocabularyManager
+
+###############################################################################
+# Module globals / Constants
+###############################################################################
+
+# Coscine REST API Endpoints
+API_ENDPOINTS = (
+    "Blob", "Metadata", "Organization", "Project", "Resources",
+    "Tree", "User", "Search", "ActivatedFeatures", "Notices"
+)
+
+# Get a logger handle.
+logger = logging.getLogger(__name__)
+
+# A colorful pretty banner to show on startup when run in a cli.
+# Note: The noqa comment disables flake8 linter rule E101 for this variable.
+BANNER: str = rf"""{colorama.Fore.BLUE}
+                     _
+                    (_)
+   ___ ___  ___  ___ _ _ __   ___
+  / __/ _ \/ __|/ __| | '_ \ / _ \
+ | (_| (_) \__ \ (__| | | | |  __/
+  \___\___/|___/\___|_|_| |_|\___|{colorama.Fore.WHITE}
+____________________________________
+
+    Coscine Python SDK {colorama.Fore.YELLOW}{__version__}{colorama.Fore.WHITE}
+____________________________________
+"""  # noqa: E101
+
+###############################################################################
+# Classes / Functions / Scripts
+###############################################################################
+
+
+class Settings:
+    """
+    Contains settings for configuring the Coscine Client class.
+    """
+
+    _language: str
+    read_only: bool
+    concurrent: bool
+    persistent_cache: bool
+    verbose: bool
+
+###############################################################################
+
+    @property
+    def language(self) -> str:
+        """Returns the language setting"""
+        return self._language
+
+###############################################################################
+
+    @language.setter
+    def language(self, lang: str) -> None:
+        lang = lang.lower()
+        if lang in LANGUAGES:
+            self._language = lang
+        else:
+            errormessage: str = (
+                f"Invalid value for argument 'lang' -> [{lang}]!\n"
+                f"Possible values are {str(LANGUAGES)}."
+            )
+            raise ValueError(errormessage)
+
+###############################################################################
+
+    def __init__(
+        self,
+        language: str = "en",
+        persistent_cache: bool = True,
+        concurrent: bool = True,
+        read_only: bool = False,
+        verbose: bool = True
+    ) -> None:
+        """
+        Parameters
+        ----------
+        language : str, "en" or "de", default: "en"
+            Language preset for input form fields and vocabularies.
+        persistent_cache : bool, default: True
+            Enable to store the cache in a file on deinitialization of
+            the client object. Will attempt to load the cache file
+            on initialization if enabled. Leads to a significant speed
+            boost when making static requests right after init, but may
+            also lead to invalid data when using outdated cache data, in case
+            the Coscine API changed recently. However this is mostly avoided
+            by performing frequent updates. Useful for applications with
+            a short runtime that get run often.
+        concurrent : bool, default: True
+            If enabled, a ThreadPool is used for bulk requests, speeding up
+            up- and downloads of multiple files tremendously.
+        read_only : bool, default: False
+            Do not perform PUT, POST, DELETE requests
+        verbose : bool, default: True
+            Print stuff to stdout if running from a command line
+        """
+        self.concurrent = concurrent
+        self.read_only = read_only
+        self.persistent_cache = persistent_cache
+        self.language = language
+        self.verbose = verbose
+
+###############################################################################
+###############################################################################
+###############################################################################
+
+class User:
+    """
+    The Coscine user associated with the Coscine REST API Token.
+    """
+
+    _data: dict
+    _organization: str
+
+    def __init__(self, client: Client) -> None:
+        uri = client.uri("User", "User", "user")
+        self._data = client.get(uri).json()
+        uri = client.uri("Organization", "Organization", "-", "isMember")
+        self._organization = client.get(uri).json()["data"][0]["displayName"]
+
+    @property
+    def id(self) -> str:
+        return self._data["id"]
+
+    @property
+    def name(self) -> str:
+        return self._data["displayName"]
+
+    @property
+    def email(self) -> str:
+        return self._data["emailAddress"]
+
+    @property
+    def organization(self) -> str:
+        return self._organization
+
+###############################################################################
+###############################################################################
+###############################################################################
+
+class Client:
+    """
+    The client class handles the connection with the Coscine server.
+    It performs requests to the API and returns the response data.
+    All objects of the Python SDK use a handle to the client to
+    communicate with Coscine.
+    """
+
+    cache: Cache
+    session: requests.Session
+    settings: Settings
+    vocabularies: VocabularyManager
+    _id: int = 0  # unique identifier for each client instance
+
+###############################################################################
+
+    @property
+    def version(self) -> str:
+        """Returns the current Coscine Python SDK version"""
+        return __version__
+
+###############################################################################
+
+    def __init__(self, token: str, settings: Settings = Settings()) -> None:
+        """
+        Initializes an instance of the base class of the Coscine Python SDK.
+
+        Parameters
+        ----------
+        token : str
+            A Coscine API access token.
+        settings : Settings
+            Coscine Python SDK client settings.
+        """
+
+        if not isinstance(token, str):
+            raise TypeError("Invalid token type: Expected string!")
+
+        self.settings = settings
+        self.cache = Cache(self.settings.persistent_cache)
+        self.vocabularies = VocabularyManager(self)
+        self.session = requests.Session()
+        self.session.headers.update({
+            "Authorization": f"Bearer {token}",
+            "User-Agent": f"Coscine Python SDK {self.version}"
+        })
+        if in_cli_mode():
+            colorama.init(autoreset=True)
+            if self.settings.verbose:
+                print(BANNER)
+        self._id += 1
+        logger.info(
+            "Initialized Coscine Python SDK version %s "
+            "Client instance (id=%d)", __version__, self._id
+        )
+        logger.debug(self.sysinfo())
+        maintenance = self._maintenance_string()
+        if maintenance:
+            logger.info(maintenance)
+
+###############################################################################
+
+    @staticmethod
+    def sysinfo() -> str:
+        """
+        Constructs system information for better bug reports.
+
+        Returns
+        -------
+        str
+            Multiline string containing system and python information.
+        """
+
+        return f"""
+            Platform: {platform.platform()}
+            Machine: {platform.machine()}
+            Processor: {platform.processor()}
+            Python compiler: {platform.python_compiler()}
+            Python branch: {platform.python_branch()}
+            Python implementation: {platform.python_implementation()}
+            Python revision: {platform.python_revision()}
+            Python version: {platform.python_version()}
+        """.replace("\t", " ")
+
+###############################################################################
+
+    @staticmethod
+    def uri(api: str, endpoint: str, *args) -> str:
+        """
+        Constructs a URL for performing a request to the Coscine API.
+
+        Parameters
+        ----------
+        api : str
+            The target Coscine API endpoint, e.g. Blob, Metadata, Tree, ...
+        endpoint : str
+            The subendpoint of `api`.
+        *args
+            Variable number of arguments of type string to append to the URL.
+            Arguments are automatically seperated by a slash '/' and
+            special characters are encoded.
+
+        Raises
+        ------
+        ValueError
+            If the api / endpoint is invalid.
+
+        Returns
+        -------
+        str
+            Encoded URL for communicating with the Coscine servers.
+        """
+
+        if api not in API_ENDPOINTS:
+            raise ValueError(
+                "Invalid value for argument 'api'! "
+                f"Possible values are {str(API_ENDPOINTS)}."
+            )
+
+        uri = BASE_URL % (api, endpoint)
+        for arg in args:
+            if arg is None:
+                continue
+            uri += "/" + urllib.parse.quote(arg, safe="")
+        return uri
+
+###############################################################################
+
+    def _maintenance_string(self) -> str:
+        """
+        Returns the Coscine maintenance notice as a human-readable string
+        """
+        message: str = ""
+        notice = self.get_maintenance()
+        if notice["type"] is not None:
+            message = (
+                f"{notice['type']}\n"
+                f"{notice['displayName']}\n"
+                f"{notice['body']}\n"
+            )
+        return message
+
+###############################################################################
+
+    def get_maintenance(self) -> dict:
+        """
+        Returns the maintenance status of the Coscine service
+        """
+        uri = self.uri("Notices", "Notice", "getMaintenance")
+        return self.get(uri).json()
+
+###############################################################################
+
+    def _request(self, method: str, uri: str, **kwargs) -> requests.Response:
+        """
+        Performs a HTTP request to the Coscine Servers.
+
+        Parameters
+        ----------
+        method : str
+            HTTP request method (GET, PUT, POST, DELETE).
+        uri : str
+            Coscine URL generated with Client.uri(...).
+        **kwargs
+            Additional keyword arguments forwarded to the requests library.
+
+        Raises
+        ------
+        ConnectionError
+            If the Coscine servers could not be reached.
+        PermissionError
+            If the Coscine API token is invalid.
+        RuntimeError
+            If the request resulted in an error.
+
+        Returns
+        -------
+        requests.Response
+            The response of the Coscine server as a requests.Response object.
+        """
+
+        # Debugging URL
+        params = kwargs["params"] if "params" in kwargs else None
+        full_url = requests.Request(method, uri, params=params).prepare().url
+        if full_url:
+            logger.debug("HTTP %s: %s", method, full_url)
+        else:
+            logger.debug("HTTP %s: %s", method, uri)
+
+        # Handling read_only setting
+        if self.settings.read_only and method != "GET":
+            logger.warning("READ_ONLY mode in effect for %s: %s", method, uri)
+            return requests.Response()
+
+        try:  # performing the request and handle any resulting errors
+            response = self.session.request(method, uri, **kwargs)
+            response.raise_for_status()
+            logger.debug("response: %s", str(response.content))
+            return response
+        except requests.exceptions.ConnectionError as exc:
+            raise ConnectionError("Failed to connect to Coscine!") from exc
+        except requests.exceptions.RequestException as exc:
+            if exc.response.status_code == 401:
+                raise PermissionError("Invalid Coscine API token!") from exc
+            raise RuntimeError(
+                "Unspecified error occurred when communicating "
+                "with the Coscine servers"
+            ) from exc
+
+###############################################################################
+
+    def get(self, uri: str, **kwargs) -> requests.Response:
+        """
+        Performs a GET request to the Coscine API.
+
+        Parameters
+        ----------
+        uri : str
+            Coscine URL generated with Client.uri(...).
+        **kwargs
+            Additional keyword arguments forwarded to the requests library.
+
+        Examples
+        --------
+        >>> uri = Client.uri("Project", "Project")
+        >>> projects = Client.get(uri).json()
+
+        Raises
+        ------
+        ConnectionError
+            If the Coscine servers could not be reached.
+        PermissionError
+            If the Coscine API token is invalid.
+        RuntimeError
+            If the request resulted in an error.
+
+        Returns
+        -------
+        requests.Response
+            The response of the Coscine server as a requests.Response object.
+        """
+
+        return self._request("GET", uri, **kwargs)
+
+###############################################################################
+
+    def put(self, uri: str, **kwargs) -> requests.Response:
+        """
+        Performs a PUT request to the Coscine API.
+
+        Parameters
+        ----------
+        uri : str
+            Coscine URL generated with Client.uri(...).
+        **kwargs
+            Additional keyword arguments forwarded to the requests library.
+
+        Examples
+        --------
+        >>> uri = Client.uri("Tree", "Tree", resource.id, filename)
+        >>> Client.put(uri, data = metadata)
+
+        Raises
+        ------
+        ConnectionError
+            If the Coscine servers could not be reached.
+        PermissionError
+            If the Coscine API token is invalid.
+        RuntimeError
+            If the request resulted in an error.
+
+        Returns
+        -------
+        requests.Response
+            The response of the Coscine server as a requests.Response object.
+        """
+
+        return self._request("PUT", uri, **kwargs)
+
+###############################################################################
+
+    def post(self, uri: str, **kwargs) -> requests.Response:
+        """
+        Performs a POST request to the Coscine API.
+
+        Parameters
+        ----------
+        uri : str
+            Coscine URL generated with Client.uri(...).
+        **kwargs
+            Additional arguments forwarded to the requests library.
+
+        Examples
+        --------
+        >>> data = member.data
+        >>> data["projectId"] = Client.id
+        >>> data["role"]["displayName"] = "Member"
+        >>> data["role"]["id"] = ProjectMember.ROLES["Member"]
+        >>> uri = Client.uri("Project", "ProjectRole")
+        >>> Client.post(uri, data=data)
+
+        Raises
+        ------
+        ConnectionError
+            If the Coscine servers could not be reached.
+        PermissionError
+            If the Coscine API token is invalid.
+        RuntimeError
+            If the request resulted in an error.
+
+        Returns
+        -------
+        requests.Response
+            The response of the Coscine server as a requests.Response object.
+        """
+
+        return self._request("POST", uri, **kwargs)
+
+###############################################################################
+
+    def delete(self, uri: str, **kwargs) -> requests.Response:
+        """
+        Performs a DELETE request to the Coscine API.
+
+        Parameters
+        ----------
+        uri : str
+            Coscine URL generated with Client.uri(...).
+        **kwargs
+            Additional keyword arguments forwarded to the requests library.
+
+        Examples
+        --------
+        >>> uri = Client.uri("Project", "Project", Client.id)
+        >>> Client.delete(uri)
+
+        Raises
+        ------
+        ConnectionError
+            If the Coscine servers could not be reached.
+        PermissionError
+            If the Coscine API token is invalid.
+        RuntimeError
+            If the request resulted in an error.
+
+        Returns
+        -------
+        requests.Response
+            The response of the Coscine server as a requests.Response object.
+        """
+
+        return self._request("DELETE", uri, **kwargs)
+
+###############################################################################
+
+    def static_request(self, uri: str) -> dict:
+        """
+        Performs a GET request for the given uri. If such a request
+        has been performed previously during the current session, the previous
+        response is returned. Otherwise a new request is made to Coscine
+        and that response is then stored inside the session cache.
+
+        Parameters
+        -----------
+        uri : str
+            Request URI
+
+        Returns
+        -------
+        dict
+        """
+
+        logger.debug("static_request(%s)", uri)
+        data = self.cache.get(uri)
+        if data is None:
+            data = self.get(uri).json()
+            self.cache.set(uri, data)
+        return data
+
+###############################################################################
+
+    def user(self) -> User:
+        """
+        Returns the user associated with the Coscine API Token used by the
+        client.
+        """
+        return User(self)
+
+###############################################################################
+
+    def project_form(self, data: Optional[dict] = None) -> ProjectForm:
+        """
+        Returns an empty project form.
+
+        Parameters
+        ----------
+        data : dict, default: None
+            If data is specified, the form is initialized with that data
+            using the InputForm.fill() method.
+        """
+        form = ProjectForm(self)
+        if data:
+            form.fill(data)
+        return form
+
+###############################################################################
+
+    def resource_form(self, data: Optional[dict] = None) -> ResourceForm:
+        """
+        Returns an empty resource form.
+
+        Parameters
+        ----------
+        data : dict, default: None
+            If data is specified, the form is initialized with that data
+            using the InputForm.fill() method.
+        """
+        form = ResourceForm(self)
+        if data:
+            form.fill(data)
+        return form
+
+###############################################################################
+
+    def projects(self, toplevel: bool = True) -> List[Project]:
+        """
+        Retrieves a list of a all projects the creator of
+        the Coscine API token is currently a member of.
+
+        Parameters
+        ----------
+        toplevel : bool, default: True
+            Retrieve only toplevel projects (no subprojects).
+            Set to False if you want to retrieve all projects, regardless
+            of hierarchy.
+
+        Returns
+        -------
+        List[Project]
+            List of coscine.Project objects
+        """
+
+        endpoint = ("Project", "Project/-/topLevel")
+        uri = self.uri("Project", endpoint[toplevel])
+        projects = []
+        for project_data in self.get(uri).json():
+            projects.append(Project(self, project_data))
+        return projects
+
+###############################################################################
+
+    def project(
+        self,
+        display_name: str,
+        toplevel: bool = True
+    ) -> Project:
+        """
+        Returns a single project via its displayName
+
+        Parameters
+        ----------
+        display_name : str
+            Look for a project with the specified displayName
+        toplevel : bool, default: True
+            Retrieve only toplevel projects (no subprojects).
+            Set to False if you want to retrieve all projects, regardless
+            of hierarchy.
+
+        Returns
+        -------
+        Project
+            A single coscine project handle
+
+        Raises
+        ------
+        IndexError
+            In case more than 1 project matches the specified criteria.
+        FileNotFoundError
+            In case no project with the specified display_name was found.
+        """
+        filtered_project_list = list(filter(
+            lambda project: project.display_name == display_name,
+            self.projects(toplevel)
+        ))
+        if len(filtered_project_list) == 1:
+            return filtered_project_list[0]
+        if len(filtered_project_list) == 0:
+            raise FileNotFoundError(
+                f"Found no project with name '{display_name}'!"
+            )
+        raise IndexError(
+            "Received more than 1 project matching the specified "
+            f"criteria (display_name = '{display_name}')!"
+        )
+
+###############################################################################
+
+    def create_project(self, form: Union[ProjectForm, dict]) -> Project:
+        """
+        Creates a project using the given ProjectForm.
+
+        Parameters
+        ----------
+        form : ProjectForm or dict
+            ProjectForm filled with project metadata or a dict with the
+            data generated from a form.
+
+        Returns
+        -------
+        Project
+            Project object for the new project.
+        """
+
+        if isinstance(form, ProjectForm):
+            form = form.generate()
+        uri = self.uri("Project", "Project")
+        return Project(self, self.post(uri, json=form).json())
+
+###############################################################################
+
+    def search(self, query: str) -> dict:
+        """
+        Performs a Coscine search query.
+
+        Returns
+        --------
+        dict
+            The search results as a dict
+        """
+
+        uri = self.uri("Search", f"Search?query={query}")
+        results = self.get(uri).json()
+        return results
+
+###############################################################################
```

### Comparing `coscine-0.9.0/src/coscine/data/project.json` & `coscine-0.9.1/src/coscine/data/project.json`

 * *Files identical despite different names*

### Comparing `coscine-0.9.0/src/coscine/data/resource.json` & `coscine-0.9.1/src/coscine/data/resource.json`

 * *Files identical despite different names*

### Comparing `coscine-0.9.0/src/coscine/defaults.py` & `coscine-0.9.1/src/coscine/defaults.py`

 * *Files identical despite different names*

### Comparing `coscine-0.9.0/src/coscine/form.py` & `coscine-0.9.1/src/coscine/form.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,799 +1,804 @@
-###############################################################################
-# Coscine Python SDK
-# Copyright (c) 2018-2023 RWTH Aachen University
-# Licensed under the terms of the MIT License
-###############################################################################
-# Coscine, short for Collaborative Scientific Integration Environment, is
-# a platform for research data management (RDM).
-# For more information on Coscine visit https://www.coscine.de/.
-#
-# Please note that this python module is open source software primarily
-# developed and maintained by the scientific community. It is not
-# an official service that RWTH Aachen provides support for.
-###############################################################################
-
-###############################################################################
-# File description
-###############################################################################
-
-"""
-This file provides base class for all input forms defined by
-the Coscine Python SDK.
-"""
-
-###############################################################################
-# Dependencies
-###############################################################################
-
-from __future__ import annotations
-from typing import Any, TYPE_CHECKING, Union, Tuple, Iterator, List, Dict
-from datetime import datetime
-import urllib.parse
-from prettytable import PrettyTable
-if TYPE_CHECKING:
-    from coscine.client import Client
-    from coscine.vocabulary import Vocabulary
-
-###############################################################################
-# Module globals/constants
-###############################################################################
-
-XSD_TYPES: Dict[str, dict] = {
-    "integer": {
-        "type": int,
-        "values": [
-            "byte", "int", "integer", "long", "unsignedShort", "unsignedByte"
-            "negativeInteger", "nonNegativeInteger", "nonPositiveInteger",
-            "positiveInteger", "short", "unsignedLong", "unsignedInt",
-        ]
-    },
-    "decimal": {
-        "type": float,
-        "values": ["double", "float", "decimal"]
-    },
-    "boolean": {
-        "type": bool,
-        "values": ["boolean"]
-    },
-    "datetime": {
-        "type": datetime,
-        "values": [
-            "date", "dateTime", "duration", "gDay", "gMonth",
-            "gMonthDay", "gYear", "gYearMonth", "time"
-        ]
-    },
-    "string": {
-        "type": str,
-        "values": [
-            "ENTITIES", "ENTITY", "ID", "IDREF", "IDREFS", "language",
-            "Name", "NCName", "NMTOKEN", "NMTOKENS", "normalizedString",
-            "QName", "string", "token"
-        ]
-    }
-}
-
-###############################################################################
-# Classes / Functions / Scripts
-###############################################################################
-
-class FormField:
-    """
-    The FormField class defines a field such as "Display Name"
-    inside an InputForm with all of its properties.
-    """
-
-    client: Client
-    _data: Dict
-
-    def __init__(self, client: Client, data: Dict) -> None:
-        self.client = client
-        self._data = data
-
-    @property
-    def name(self) -> str:
-        """
-        The name of the field e.g. "Project Name"
-        """
-        return self._data["name"][self.client.settings.language]
-
-    @property
-    def path(self) -> str:
-        """
-        The unique Coscine internal name of the field e.g. "projectName"
-        """
-        return self._data["path"]
-
-    @property
-    def order(self) -> int:
-        """
-        The order of appearance of the field inside of the form
-        """
-        return int(self._data["order"])
-
-    @property
-    def vocabulary(self) -> str:
-        """
-        Name of the vocabulary instance for the field, may be None
-        """
-        return self._data["class"]
-
-    @property
-    def min_count(self) -> int:
-        """
-        Minimum amount of values required for a successful generate()
-        """
-        return int(self._data["minCount"])
-
-    @property
-    def max_count(self) -> int:
-        """
-        Maximum allowed amount of values
-        """
-        return int(self._data["maxCount"])
-
-    @property
-    def datatype(self) -> str:
-        """
-        Expected datatype of the field as a string identifier, e.g. "xsd:int"
-        """
-        return self._data["datatype"]
-
-    @property
-    def selection(self) -> List[str]:
-        """
-        Preset selection of values - no other value except for these values
-        can be specified. Think of it as a class defined in the profile.
-        """
-        if "in" in self._data and self._data["in"] is not None:
-            return self._data["in"]
-        return []
-
-###############################################################################
-###############################################################################
-###############################################################################
-
-class FormValue:
-    """
-    An InputForm specific representation of a value
-    """
-
-    _form: InputForm
-    _key: str
-    properties: FormField
-    # In case of form.properties(key).maxValues > 1 it is a list,
-    # otherwise a scalar object
-    _container: Union[List[Any], Any]
-
-###############################################################################
-
-    def __init__(
-        self,
-        form: InputForm,
-        key: str,
-        obj: Any = None,
-        raw: bool = False
-    ) -> None:
-        """
-        Specifying the associated InputForm and key may seem redundant from
-        the point of view of the InputForm, but ultimately it allows the form
-        value to access the vocabulary and the field properties.
-        """
-        self._form = form
-        self._key = key
-        self.properties = form.properties(key)
-        self.set_value(obj, raw)
-
-###############################################################################
-
-    def __bool__(self) -> bool:
-        if isinstance(self._container, list):
-            return self._container[0] is not None
-        return self._container is not None
-
-###############################################################################
-
-    def _set_list_value(self, values: List[Any], raw: bool = False) -> None:
-        if isinstance(values, (list, tuple)):
-            self._container = []
-            for entry in values:
-                self.append(entry, raw)
-        else:
-            # Let's be generous and do the conversion if scalar type to list
-            # of size 1 for the users ourselves
-            self._container = []
-            self.append(values, raw)
-
-###############################################################################
-
-    def _set_scalar_value(self, value: Any, raw: bool = False) -> None:
-        if isinstance(value, (list, tuple)):
-            # Be very generous and automatically convert lists
-            # of size 1 to an atomic value.
-            if len(value) > 1:
-                raise TypeError(
-                    "Did not expect list type exceeding "
-                    f"MaxValues property for key '{self._key}'."
-                )
-            value = value[0]
-        self._container = value if raw else self._objectify(value)
-
-###############################################################################
-
-    def set_value(self, value: Any, raw: bool = False) -> None:
-        """
-        Sets the FormValue equal to the specified value.
-
-        Parameters
-        ----------
-        value : Any
-            The value to set the FormField equal to. Could be
-            a list of values.
-        raw : bool
-            If set to True, the value is not interpreted for controlled
-            fields and its type is not checked. Use raw when dealing with
-            values in Coscines internal format.
-        """
-        if self.properties.max_count > 1:
-            self._set_list_value(value, raw)
-        else:
-            self._set_scalar_value(value, raw)
-
-###############################################################################
-
-    def append(self, value: Any, raw: bool = False) -> None:
-        """
-        Appends a value to a FormValue allowing multiple values.
-
-        Parameters
-        ----------
-        value : Any
-            The value to append to the FormField.
-        raw : bool
-            If set to True, the value is not interpreted for controlled
-            fields and its type is not checked. Use raw when dealing with
-            values in Coscines internal format.
-
-        Raises
-        ------
-        TypeError
-            In case of appending a value to a scalar FormField.
-        IndexError
-            When exceeding the maxValues setting for the FormField.
-        """
-        if not isinstance(self._container, list):
-            raise TypeError(
-                "Attempting to append a value to scalar "
-                f"FormField '{self._key}'. "
-                "See 'MaxCount' property in application profile."
-            )
-        if len(self._container) < self.properties.max_count:
-            if not raw:
-                value = self._objectify(value)
-            self._container.append(value)
-        else:
-            raise IndexError(f"Exceeding maxValues for field {self._key}.")
-
-###############################################################################
-
-    def type_format(self) -> str:
-        """
-        Returns the type format of the internal type.
-        See InputForm.type_format() as this is internally called.
-
-        Returns
-        -------
-        str
-            The type format as a string, e.g. "%s" for string types
-            or "%d" for integers. This function is handy when dealing with
-            datetime objects, as it returns the expected date format.
-        """
-        return self._form.type_format(self._key)
-
-###############################################################################
-
-    def _is_valid_type(self, key: str, value: Any) -> bool:
-        if self._form.is_controlled(self._key) and not isinstance(value, str):
-            raise TypeError(
-                "Values specified for controlled fields "
-                "must be of type string to make it possible to "
-                "look up their raw representation in the vocabulary: "
-                f"Expected 'str', got '{str(type(value))}'"
-            )
-        if self._form.datatype(key) is None:
-            return True
-        datatype = self._form.datatype(key)
-        return datatype is not None and isinstance(value, datatype)
-
-###############################################################################
-
-    def _objectify(self, value: Any) -> Any:
-        """
-        Checks if the type of the value matches the expecte type and
-        in case of controlled fields, converts the human-readable value to
-        the unique internal Coscine representation via
-        the associated vocabulary.
-        """
-        if value is None:
-            return None
-
-        if not self._is_valid_type(self._key, value):
-            raise TypeError(
-                f"Value of type {str(type(value))} specified "
-                f"for key {self._key} does not match expected "
-                f"type {self._form.datatype(self._key)}!"
-            )
-
-        if self._form.has_vocabulary(self._key):
-            if not self._form.vocabulary(self._key).contains(value):
-                suggestions = self._form.vocabulary(self._key).suggest(value)
-                raise ValueError(
-                    f"Invalid value '{value}' for vocabulary "
-                    f"controlled key '{self._key}'! "
-                    f"Perhaps you meant {suggestions}?"
-                )
-            return self._form.vocabulary(self._key).lookup_key(value)
-        if self._form.has_selection(self._key):
-            if value not in self._form.selection(self._key):
-                raise ValueError(
-                    f"Invalid value '{value}' for selection "
-                    f"controlled key '{self._key}'!"
-                )
-        return value
-
-###############################################################################
-
-    def _serialize_value(self, obj: Any, raw: bool = False) -> str:
-        """
-        Serializes a single value according to its type / format
-        -> This function converts a pythonic value to a string.
-        """
-        serialized_value: str = ""
-        if obj and self._form.has_vocabulary(self._key):
-            if raw:
-                serialized_value = obj
-            else:
-                serialized_value = str(
-                    self._form.vocabulary(self._key).lookup_value(obj)
-                )
-        elif isinstance(obj, datetime):
-            try:
-                serialized_value = obj.strftime(self.type_format())
-            except ValueError:
-                serialized_value = str(obj)  # Omit format if error
-        elif isinstance(obj, dict):
-            serialized_value = str(obj)
-        elif isinstance(obj, bool):
-            serialized_value = str(obj).lower()
-        elif obj is None:
-            serialized_value = ""
-        else:
-            serialized_value = str(obj)
-        return serialized_value
-
-###############################################################################
-
-    def _serialize_list_raw(self) -> List:
-        serialized_values = []
-        for value in self._container:
-            serialized_values.append(self._serialize_value(value, True))
-        return serialized_values
-
-###############################################################################
-
-    def _serialize_list(self) -> str:
-        serialized_values = []
-        for value in self._container:
-            serialized_values.append(self._serialize_value(value))
-        return "\n".join(serialized_values)
-
-###############################################################################
-
-    def __str__(self) -> str:
-        if self.properties.max_count > 1:
-            return self._serialize_list()
-        return self._serialize_value(self._container)
-
-###############################################################################
-
-    def raw(self) -> Any:
-        """
-        Returns the raw value of the FormValue.
-        """
-        if self.properties.max_count > 1:
-            return self._serialize_list_raw()
-        return self._serialize_value(self._container, True)
-
-###############################################################################
-###############################################################################
-###############################################################################
-
-class InputForm:
-    """
-    Coscine InputForm base class
-    """
-
-    client: Client
-    _fields: List[FormField]
-    _values: Dict[str, FormValue]
-    _vocabularies: Dict[str, Vocabulary]
-
-###############################################################################
-
-    def __init__(self, client: Client) -> None:
-        """
-        Parameters
-        ----------
-        client : Client
-            Coscine Python SDK Client handle
-        """
-        super().__init__()
-        self.client = client
-        self._fields = []
-        self._values = {}
-        self._vocabularies = {}
-
-###############################################################################
-
-    def __setitem__(self, key: str, value: Any) -> None:
-        self.set_value(key, value)
-
-###############################################################################
-
-    def __getitem__(self, key: str) -> FormValue:
-        return self.get_value(key)
-
-###############################################################################
-
-    def __delitem__(self, key: str) -> None:
-        del self._values[self.path(key)]
-
-###############################################################################
-
-    def __iter__(self) -> Iterator[str]:
-        return iter(self.keys())
-
-###############################################################################
-
-    def __len__(self) -> int:
-        return len(self._fields)
-
-###############################################################################
-
-    def __str__(self) -> str:
-        return self.as_str()
-
-###############################################################################
-
-    def clear(self) -> None:
-        """Removes all values of the InputForm"""
-        self._values.clear()
-
-###############################################################################
-
-    def path(self, key: str) -> str:
-        """
-        Returns the unique identifier for a multilanguage key.
-        Logical example:
-        path("Display Name") == path("Anzeigename") == "__XXX__"
-        ->> True
-        where "__XXX__" is of some fixed internal value.
-
-        Parameters
-        -----------
-        key : str
-            Multilanguage form key. Language depends on the
-            coscine.Client language setting.
-
-        Returns
-        -------
-        str
-            Unique identifier of a form field.
-        """
-        return self.properties(key).path
-
-###############################################################################
-
-    def properties(self, key: str) -> FormField:
-        """
-        Returns the form field properties corresponding to the given key.
-
-        Parameters
-        ----------
-        key : str
-            Form key
-
-        Returns
-        -------
-        FormField
-            Object containing the field properties for the given key
-        """
-        return self._fields[self.index_of(key)]
-
-###############################################################################
-
-    def index_of(self, key: str) -> int:
-        """
-        Returns the order/index of the given key.
-        """
-        for index, item in enumerate(self.keys()):
-            if item == key:
-                return index
-        raise KeyError(f"Key '{key}' not in InputForm!")
-
-###############################################################################
-
-    def name_of(self, path: str) -> str:
-        """
-        Returns the key name for the unique path depending on the client
-        language setting.
-        """
-        for field in self._fields:
-            if field.path == path:
-                return field.name
-        raise KeyError(f"Path '{path}' not in InputForm!")
-
-###############################################################################
-
-    def keys(self) -> List[str]:
-        """
-        Returns a list of keys in their respective order based on the
-        language setting of the client class instance used to initialize
-        the InputForm.
-        """
-        return [field.name for field in self._fields]
-
-###############################################################################
-
-    def values(self) -> List[FormValue]:
-        """
-        Returns a list of values in their respective order based on the
-        language setting of the client class instance used to initialize
-        the InputForm.
-        """
-        return [self.get_value(key) for key in self.keys()]
-
-###############################################################################
-
-    def items(self) -> List[Tuple[str, FormValue]]:
-        """
-        Returns a list of key, value pairs in their respective order based
-        on the 	language setting of the client class instance
-        used to initialize the InputForm.
-        """
-        return list(zip(self.keys(), self.values()))
-
-###############################################################################
-
-    @staticmethod
-    def _xsd_typeof(xsd_type: str) -> type:
-        if xsd_type.startswith("xsd:"):
-            xsd_type = xsd_type[4:]
-        for item in XSD_TYPES.values():
-            if xsd_type in item["values"]:
-                return item["type"]
-        return str
-
-###############################################################################
-
-###############################################################################
-
-    def datatype(self, key: str) -> type:
-        """
-        Returns the datatype for a given field (which may be None).
-        """
-        datatype = self.properties(key).datatype
-        if datatype and datatype.startswith("http:"):
-            datatype = f"xsd:{urllib.parse.urlparse(datatype)[-1]}"
-        if self.is_controlled(key):
-            return str
-        return self._xsd_typeof(datatype)
-
-###############################################################################
-
-    def type_format(self, key: str) -> str:
-        """
-        Returns the format for a datatype of a field.
-        This is especially useful for instances of type datetype.
-        """
-        datatype = self.datatype(key)
-        if datatype == str:
-            return "%s"
-        if datatype in (bool, int):
-            return "%d"
-        if datatype == float:
-            return "%f"
-        if datatype == datetime:
-            return "%Y-%m-%d"
-        return "Invalid Format"
-
-###############################################################################
-
-    def is_typed(self, key: str) -> bool:
-        """
-        Returns whether a value is expecting a certain datatype.
-        """
-        return self.datatype(key) is not None
-
-###############################################################################
-
-    def is_required(self, key: str) -> bool:
-        """
-        Determines whether a key is a required one.
-        """
-        return self.properties(key).min_count > 0
-
-###############################################################################
-
-    def has_vocabulary(self, key: str) -> bool:
-        """
-        Determines whether a key is controlled by a vocabulary.
-        """
-        return self.properties(key).vocabulary is not None
-
-###############################################################################
-
-    def has_selection(self, key: str) -> bool:
-        """
-        Determines whether a key is controlled by a selection.
-        """
-        return len(self.properties(key).selection) > 0
-
-###############################################################################
-
-    def is_controlled(self, key: str) -> bool:
-        """
-        Determines whether a key is controlled by a vocabulary or selection.
-        """
-        return self.has_vocabulary(key) or self.has_selection(key)
-
-###############################################################################
-
-    def vocabulary(self, key: str) -> Vocabulary:
-        """
-        Returns the vocabulary for the given controlled key. Make sure
-        the key is actually controlled to avoid an exception.
-
-        Raises
-        -------
-        KeyError
-            In case the specified key is not controlled by a vocabulary.
-        """
-        if self.has_vocabulary(key):
-            return self._vocabularies[self.path(key)]
-        raise KeyError(f"Key '{key}' is not controlled by a vocabulary!")
-
-###############################################################################
-
-    def selection(self, key: str) -> List[str]:
-        """
-        Returns the selection for the given controlled key. Make sure
-        the key is actually controlled to avoid an exception.
-
-        Raises
-        -------
-        KeyError
-            In case the specified key is not controlled by a selection.
-        """
-
-        if self.has_selection(key):
-            return self.properties(key).selection
-        raise KeyError(f"Key '{key}' is not controlled by a selection!")
-
-###############################################################################
-
-    def set_value(self, key: str, value: Any, raw: bool = False) -> None:
-        """
-        Sets the value for a given key.
-
-        Parameters
-        ----------
-        key : str
-            The key to associate the value with
-        value : Any
-            The typed value, either in raw format or human readable
-        raw : bool, default: False
-            Treat the value as a raw value (from Coscine) and do not apply
-            vocabulary search or type checking on it
-        """
-        self._values[self.path(key)] = FormValue(self, key, value, raw)
-
-###############################################################################
-
-    def get_value(self, key: str) -> FormValue:
-        """
-        Returns the FormValue for the specified key
-
-        Parameters
-        ----------
-        key : str
-            The key to get the value from.
-        """
-        if key not in self.keys():
-            raise KeyError(f"Key '{key}' not in InputForm!")
-        if self.path(key) in self._values:
-            return self._values[self.path(key)]
-        return FormValue(self, key)  # Yields an empty FormValue
-
-###############################################################################
-
-    def fill(self, data: Dict) -> None:
-        """
-        Fill in an InputForm from a dictionary
-
-        Parameters
-        ----------
-        data : dict
-            Python dictionary containing key value pairs in human-readable
-            form (not data from Coscine!).
-        """
-        for key, value in data.items():
-            self[key] = value
-
-###############################################################################
-
-    def parse(self, data: Dict) -> None:
-        """
-        Parses data from Coscine into an InputForm.
-
-        Parameters
-        ----------
-        data : dict
-            Python dictionary (output of json.loads) containing
-            the data from Coscine.
-        """
-
-###############################################################################
-
-    def generate(self) -> dict:
-        """
-        Generates Coscine formatted json-ld from an InputForm.
-        """
-        return {}
-
-###############################################################################
-
-    def as_str(self, format: str = "str") -> str:
-        """
-        Returns a string in the specified format
-
-        Parameters
-        -----------
-        format : str, default "str"
-            Format of the string, possible options are: str, csv, json, html
-
-        Returns
-        --------
-        str
-            A string with the form values in the specified format.
-        """
-
-        supported_formats = ["str", "csv", "json", "html"]
-        if format not in supported_formats:
-            raise ValueError(f"Unsupported format '{format}'!")
-        table = PrettyTable(
-            ("C", "Type", "Property", "Value"),
-            align="l"
-        )
-        rows = []
-        for key in self.keys():
-            value = str(self.get_value(key))
-            name: str = key
-            name = name + "*" if self.is_required(key) else name
-            controlled: str = ""
-            if self.is_controlled(key):
-                controlled = "V" if self.has_vocabulary(key) else "S"
-            datatype: str = str(self.datatype(key).__name__)
-            if self.properties(key).max_count > 1:
-                datatype = f"[{datatype}]"
-            rows.append((controlled, datatype, name, value))
-        table.max_width["Value"] = 50
-        table.add_rows(rows)
-        if format == "csv":
-            return table.get_csv_string()
-        if format == "json":
-            return table.get_json_string()
-        if format == "html":
-            return table.get_html_string()
-        return table.get_string()
-
-###############################################################################
+###############################################################################
+# Coscine Python SDK
+# Copyright (c) 2018-2023 RWTH Aachen University
+# Licensed under the terms of the MIT License
+###############################################################################
+# Coscine, short for Collaborative Scientific Integration Environment, is
+# a platform for research data management (RDM).
+# For more information on Coscine visit https://www.coscine.de/.
+#
+# Please note that this python module is open source software primarily
+# developed and maintained by the scientific community. It is not
+# an official service that RWTH Aachen provides support for.
+###############################################################################
+
+###############################################################################
+# File description
+###############################################################################
+
+"""
+This file provides base class for all input forms defined by
+the Coscine Python SDK.
+"""
+
+###############################################################################
+# Dependencies
+###############################################################################
+
+from __future__ import annotations
+from typing import Any, TYPE_CHECKING, Union, Tuple, Iterator, List, Dict
+from datetime import datetime
+import urllib.parse
+from prettytable import PrettyTable
+if TYPE_CHECKING:
+    from coscine.client import Client
+    from coscine.vocabulary import Vocabulary
+
+###############################################################################
+# Module globals/constants
+###############################################################################
+
+# TODO:
+# can we use rdflib namespace xsd for types?
+# -> https://rdflib.readthedocs.io/en/stable/rdf_terms.html
+# from rdflib.term import _castLexicalToPython
+# https://rdflib.readthedocs.io/en/stable/_modules/rdflib/term.html#_castLexicalToPython
+XSD_TYPES: Dict[str, dict] = {
+    "integer": {
+        "type": int,
+        "values": [
+            "byte", "int", "integer", "long", "unsignedShort", "unsignedByte"
+            "negativeInteger", "nonNegativeInteger", "nonPositiveInteger",
+            "positiveInteger", "short", "unsignedLong", "unsignedInt",
+        ]
+    },
+    "decimal": {
+        "type": float,
+        "values": ["double", "float", "decimal"]
+    },
+    "boolean": {
+        "type": bool,
+        "values": ["boolean"]
+    },
+    "datetime": {
+        "type": datetime,
+        "values": [
+            "date", "dateTime", "duration", "gDay", "gMonth",
+            "gMonthDay", "gYear", "gYearMonth", "time"
+        ]
+    },
+    "string": {
+        "type": str,
+        "values": [
+            "ENTITIES", "ENTITY", "ID", "IDREF", "IDREFS", "language",
+            "Name", "NCName", "NMTOKEN", "NMTOKENS", "normalizedString",
+            "QName", "string", "token"
+        ]
+    }
+}
+
+###############################################################################
+# Classes / Functions / Scripts
+###############################################################################
+
+class FormField:
+    """
+    The FormField class defines a field such as "Display Name"
+    inside an InputForm with all of its properties.
+    """
+
+    client: Client
+    _data: Dict
+
+    def __init__(self, client: Client, data: Dict) -> None:
+        self.client = client
+        self._data = data
+
+    @property
+    def name(self) -> str:
+        """
+        The name of the field e.g. "Project Name"
+        """
+        return self._data["name"][self.client.settings.language]
+
+    @property
+    def path(self) -> str:
+        """
+        The unique Coscine internal name of the field e.g. "projectName"
+        """
+        return self._data["path"]
+
+    @property
+    def order(self) -> int:
+        """
+        The order of appearance of the field inside of the form
+        """
+        return int(self._data["order"])
+
+    @property
+    def vocabulary(self) -> str:
+        """
+        Name of the vocabulary instance for the field, may be None
+        """
+        return self._data["class"]
+
+    @property
+    def min_count(self) -> int:
+        """
+        Minimum amount of values required for a successful generate()
+        """
+        return int(self._data["minCount"])
+
+    @property
+    def max_count(self) -> int:
+        """
+        Maximum allowed amount of values
+        """
+        return int(self._data["maxCount"])
+
+    @property
+    def datatype(self) -> str:
+        """
+        Expected datatype of the field as a string identifier, e.g. "xsd:int"
+        """
+        return self._data["datatype"]
+
+    @property
+    def selection(self) -> List[str]:
+        """
+        Preset selection of values - no other value except for these values
+        can be specified. Think of it as a class defined in the profile.
+        """
+        if "in" in self._data and self._data["in"] is not None:
+            return self._data["in"]
+        return []
+
+###############################################################################
+###############################################################################
+###############################################################################
+
+class FormValue:
+    """
+    An InputForm specific representation of a value
+    """
+
+    _form: InputForm
+    _key: str
+    properties: FormField
+    # In case of form.properties(key).maxValues > 1 it is a list,
+    # otherwise a scalar object
+    _container: Union[List[Any], Any]
+
+###############################################################################
+
+    def __init__(
+        self,
+        form: InputForm,
+        key: str,
+        obj: Any = None,
+        raw: bool = False
+    ) -> None:
+        """
+        Specifying the associated InputForm and key may seem redundant from
+        the point of view of the InputForm, but ultimately it allows the form
+        value to access the vocabulary and the field properties.
+        """
+        self._form = form
+        self._key = key
+        self.properties = form.properties(key)
+        self.set_value(obj, raw)
+
+###############################################################################
+
+    def __bool__(self) -> bool:
+        if isinstance(self._container, list):
+            return self._container[0] is not None
+        return self._container is not None
+
+###############################################################################
+
+    def _set_list_value(self, values: List[Any], raw: bool = False) -> None:
+        if isinstance(values, (list, tuple)):
+            self._container = []
+            for entry in values:
+                self.append(entry, raw)
+        else:
+            # Let's be generous and do the conversion if scalar type to list
+            # of size 1 for the users ourselves
+            self._container = []
+            self.append(values, raw)
+
+###############################################################################
+
+    def _set_scalar_value(self, value: Any, raw: bool = False) -> None:
+        if isinstance(value, (list, tuple)):
+            # Be very generous and automatically convert lists
+            # of size 1 to an atomic value.
+            if len(value) > 1:
+                raise TypeError(
+                    "Did not expect list type exceeding "
+                    f"MaxValues property for key '{self._key}'."
+                )
+            value = value[0]
+        self._container = value if raw else self._objectify(value)
+
+###############################################################################
+
+    def set_value(self, value: Any, raw: bool = False) -> None:
+        """
+        Sets the FormValue equal to the specified value.
+
+        Parameters
+        ----------
+        value : Any
+            The value to set the FormField equal to. Could be
+            a list of values.
+        raw : bool
+            If set to True, the value is not interpreted for controlled
+            fields and its type is not checked. Use raw when dealing with
+            values in Coscines internal format.
+        """
+        if self.properties.max_count > 1:
+            self._set_list_value(value, raw)
+        else:
+            self._set_scalar_value(value, raw)
+
+###############################################################################
+
+    def append(self, value: Any, raw: bool = False) -> None:
+        """
+        Appends a value to a FormValue allowing multiple values.
+
+        Parameters
+        ----------
+        value : Any
+            The value to append to the FormField.
+        raw : bool
+            If set to True, the value is not interpreted for controlled
+            fields and its type is not checked. Use raw when dealing with
+            values in Coscines internal format.
+
+        Raises
+        ------
+        TypeError
+            In case of appending a value to a scalar FormField.
+        IndexError
+            When exceeding the maxValues setting for the FormField.
+        """
+        if not isinstance(self._container, list):
+            raise TypeError(
+                "Attempting to append a value to scalar "
+                f"FormField '{self._key}'. "
+                "See 'MaxCount' property in application profile."
+            )
+        if len(self._container) < self.properties.max_count:
+            if not raw:
+                value = self._objectify(value)
+            self._container.append(value)
+        else:
+            raise IndexError(f"Exceeding maxValues for field {self._key}.")
+
+###############################################################################
+
+    def type_format(self) -> str:
+        """
+        Returns the type format of the internal type.
+        See InputForm.type_format() as this is internally called.
+
+        Returns
+        -------
+        str
+            The type format as a string, e.g. "%s" for string types
+            or "%d" for integers. This function is handy when dealing with
+            datetime objects, as it returns the expected date format.
+        """
+        return self._form.type_format(self._key)
+
+###############################################################################
+
+    def _is_valid_type(self, key: str, value: Any) -> bool:
+        if self._form.is_controlled(self._key) and not isinstance(value, str):
+            raise TypeError(
+                "Values specified for controlled fields "
+                "must be of type string to make it possible to "
+                "look up their raw representation in the vocabulary: "
+                f"Expected 'str', got '{str(type(value))}'"
+            )
+        if self._form.datatype(key) is None:
+            return True
+        datatype = self._form.datatype(key)
+        return datatype is not None and isinstance(value, datatype)
+
+###############################################################################
+
+    def _objectify(self, value: Any) -> Any:
+        """
+        Checks if the type of the value matches the expecte type and
+        in case of controlled fields, converts the human-readable value to
+        the unique internal Coscine representation via
+        the associated vocabulary.
+        """
+        if value is None:
+            return None
+
+        if not self._is_valid_type(self._key, value):
+            raise TypeError(
+                f"Value of type {str(type(value))} specified "
+                f"for key {self._key} does not match expected "
+                f"type {self._form.datatype(self._key)}!"
+            )
+
+        if self._form.has_vocabulary(self._key):
+            if not self._form.vocabulary(self._key).contains(value):
+                suggestions = self._form.vocabulary(self._key).suggest(value)
+                raise ValueError(
+                    f"Invalid value '{value}' for vocabulary "
+                    f"controlled key '{self._key}'! "
+                    f"Perhaps you meant {suggestions}?"
+                )
+            return self._form.vocabulary(self._key).lookup_key(value)
+        if self._form.has_selection(self._key):
+            if value not in self._form.selection(self._key):
+                raise ValueError(
+                    f"Invalid value '{value}' for selection "
+                    f"controlled key '{self._key}'!"
+                )
+        return value
+
+###############################################################################
+
+    def _serialize_value(self, obj: Any, raw: bool = False) -> str:
+        """
+        Serializes a single value according to its type / format
+        -> This function converts a pythonic value to a string.
+        """
+        serialized_value: str = ""
+        if obj and self._form.has_vocabulary(self._key):
+            if raw:
+                serialized_value = obj
+            else:
+                serialized_value = str(
+                    self._form.vocabulary(self._key).lookup_value(obj)
+                )
+        elif isinstance(obj, datetime):
+            try:
+                serialized_value = obj.strftime(self.type_format())
+            except ValueError:
+                serialized_value = str(obj)  # Omit format if error
+        elif isinstance(obj, dict):
+            serialized_value = str(obj)
+        elif isinstance(obj, bool):
+            serialized_value = str(obj).lower()
+        elif obj is None:
+            serialized_value = ""
+        else:
+            serialized_value = str(obj)
+        return serialized_value
+
+###############################################################################
+
+    def _serialize_list_raw(self) -> List:
+        serialized_values = []
+        for value in self._container:
+            serialized_values.append(self._serialize_value(value, True))
+        return serialized_values
+
+###############################################################################
+
+    def _serialize_list(self) -> str:
+        serialized_values = []
+        for value in self._container:
+            serialized_values.append(self._serialize_value(value))
+        return ",".join(serialized_values)
+
+###############################################################################
+
+    def __str__(self) -> str:
+        if self.properties.max_count > 1:
+            return self._serialize_list()
+        return self._serialize_value(self._container)
+
+###############################################################################
+
+    def raw(self) -> Any:
+        """
+        Returns the raw value of the FormValue.
+        """
+        if self.properties.max_count > 1:
+            return self._serialize_list_raw()
+        return self._serialize_value(self._container, True)
+
+###############################################################################
+###############################################################################
+###############################################################################
+
+class InputForm:
+    """
+    Coscine InputForm base class
+    """
+
+    client: Client
+    _fields: List[FormField]
+    _values: Dict[str, FormValue]
+    _vocabularies: Dict[str, Vocabulary]
+
+###############################################################################
+
+    def __init__(self, client: Client) -> None:
+        """
+        Parameters
+        ----------
+        client : Client
+            Coscine Python SDK Client handle
+        """
+        super().__init__()
+        self.client = client
+        self._fields = []
+        self._values = {}
+        self._vocabularies = {}
+
+###############################################################################
+
+    def __setitem__(self, key: str, value: Any) -> None:
+        self.set_value(key, value)
+
+###############################################################################
+
+    def __getitem__(self, key: str) -> FormValue:
+        return self.get_value(key)
+
+###############################################################################
+
+    def __delitem__(self, key: str) -> None:
+        del self._values[self.path(key)]
+
+###############################################################################
+
+    def __iter__(self) -> Iterator[str]:
+        return iter(self.keys())
+
+###############################################################################
+
+    def __len__(self) -> int:
+        return len(self._fields)
+
+###############################################################################
+
+    def __str__(self) -> str:
+        return self.as_str()
+
+###############################################################################
+
+    def clear(self) -> None:
+        """Removes all values of the InputForm"""
+        self._values.clear()
+
+###############################################################################
+
+    def path(self, key: str) -> str:
+        """
+        Returns the unique identifier for a multilanguage key.
+        Logical example:
+        path("Display Name") == path("Anzeigename") == "__XXX__"
+        ->> True
+        where "__XXX__" is of some fixed internal value.
+
+        Parameters
+        -----------
+        key : str
+            Multilanguage form key. Language depends on the
+            coscine.Client language setting.
+
+        Returns
+        -------
+        str
+            Unique identifier of a form field.
+        """
+        return self.properties(key).path
+
+###############################################################################
+
+    def properties(self, key: str) -> FormField:
+        """
+        Returns the form field properties corresponding to the given key.
+
+        Parameters
+        ----------
+        key : str
+            Form key
+
+        Returns
+        -------
+        FormField
+            Object containing the field properties for the given key
+        """
+        return self._fields[self.index_of(key)]
+
+###############################################################################
+
+    def index_of(self, key: str) -> int:
+        """
+        Returns the order/index of the given key.
+        """
+        for index, item in enumerate(self.keys()):
+            if item == key:
+                return index
+        raise KeyError(f"Key '{key}' not in InputForm!")
+
+###############################################################################
+
+    def name_of(self, path: str) -> str:
+        """
+        Returns the key name for the unique path depending on the client
+        language setting.
+        """
+        for field in self._fields:
+            if field.path == path:
+                return field.name
+        raise KeyError(f"Path '{path}' not in InputForm!")
+
+###############################################################################
+
+    def keys(self) -> List[str]:
+        """
+        Returns a list of keys in their respective order based on the
+        language setting of the client class instance used to initialize
+        the InputForm.
+        """
+        return [field.name for field in self._fields]
+
+###############################################################################
+
+    def values(self) -> List[FormValue]:
+        """
+        Returns a list of values in their respective order based on the
+        language setting of the client class instance used to initialize
+        the InputForm.
+        """
+        return [self.get_value(key) for key in self.keys()]
+
+###############################################################################
+
+    def items(self) -> List[Tuple[str, FormValue]]:
+        """
+        Returns a list of key, value pairs in their respective order based
+        on the 	language setting of the client class instance
+        used to initialize the InputForm.
+        """
+        return list(zip(self.keys(), self.values()))
+
+###############################################################################
+
+    @staticmethod
+    def _xsd_typeof(xsd_type: str) -> type:
+        if xsd_type.startswith("xsd:"):
+            xsd_type = xsd_type[4:]
+        for item in XSD_TYPES.values():
+            if xsd_type in item["values"]:
+                return item["type"]
+        return str
+
+###############################################################################
+
+###############################################################################
+
+    def datatype(self, key: str) -> type:
+        """
+        Returns the datatype for a given field (which may be None).
+        """
+        datatype = self.properties(key).datatype
+        if datatype and datatype.startswith("http:"):
+            datatype = f"xsd:{urllib.parse.urlparse(datatype)[-1]}"
+        if self.is_controlled(key):
+            return str
+        return self._xsd_typeof(datatype)
+
+###############################################################################
+
+    def type_format(self, key: str) -> str:
+        """
+        Returns the format for a datatype of a field.
+        This is especially useful for instances of type datetype.
+        """
+        datatype = self.datatype(key)
+        if datatype == str:
+            return "%s"
+        if datatype in (bool, int):
+            return "%d"
+        if datatype == float:
+            return "%f"
+        if datatype == datetime:
+            return "%Y-%m-%d"
+        return "Invalid Format"
+
+###############################################################################
+
+    def is_typed(self, key: str) -> bool:
+        """
+        Returns whether a value is expecting a certain datatype.
+        """
+        return self.datatype(key) is not None
+
+###############################################################################
+
+    def is_required(self, key: str) -> bool:
+        """
+        Determines whether a key is a required one.
+        """
+        return self.properties(key).min_count > 0
+
+###############################################################################
+
+    def has_vocabulary(self, key: str) -> bool:
+        """
+        Determines whether a key is controlled by a vocabulary.
+        """
+        return self.properties(key).vocabulary is not None
+
+###############################################################################
+
+    def has_selection(self, key: str) -> bool:
+        """
+        Determines whether a key is controlled by a selection.
+        """
+        return len(self.properties(key).selection) > 0
+
+###############################################################################
+
+    def is_controlled(self, key: str) -> bool:
+        """
+        Determines whether a key is controlled by a vocabulary or selection.
+        """
+        return self.has_vocabulary(key) or self.has_selection(key)
+
+###############################################################################
+
+    def vocabulary(self, key: str) -> Vocabulary:
+        """
+        Returns the vocabulary for the given controlled key. Make sure
+        the key is actually controlled to avoid an exception.
+
+        Raises
+        -------
+        KeyError
+            In case the specified key is not controlled by a vocabulary.
+        """
+        if self.has_vocabulary(key):
+            return self._vocabularies[self.path(key)]
+        raise KeyError(f"Key '{key}' is not controlled by a vocabulary!")
+
+###############################################################################
+
+    def selection(self, key: str) -> List[str]:
+        """
+        Returns the selection for the given controlled key. Make sure
+        the key is actually controlled to avoid an exception.
+
+        Raises
+        -------
+        KeyError
+            In case the specified key is not controlled by a selection.
+        """
+
+        if self.has_selection(key):
+            return self.properties(key).selection
+        raise KeyError(f"Key '{key}' is not controlled by a selection!")
+
+###############################################################################
+
+    def set_value(self, key: str, value: Any, raw: bool = False) -> None:
+        """
+        Sets the value for a given key.
+
+        Parameters
+        ----------
+        key : str
+            The key to associate the value with
+        value : Any
+            The typed value, either in raw format or human readable
+        raw : bool, default: False
+            Treat the value as a raw value (from Coscine) and do not apply
+            vocabulary search or type checking on it
+        """
+        self._values[self.path(key)] = FormValue(self, key, value, raw)
+
+###############################################################################
+
+    def get_value(self, key: str) -> FormValue:
+        """
+        Returns the FormValue for the specified key
+
+        Parameters
+        ----------
+        key : str
+            The key to get the value from.
+        """
+        if key not in self.keys():
+            raise KeyError(f"Key '{key}' not in InputForm!")
+        if self.path(key) in self._values:
+            return self._values[self.path(key)]
+        return FormValue(self, key)  # Yields an empty FormValue
+
+###############################################################################
+
+    def fill(self, data: Dict) -> None:
+        """
+        Fill in an InputForm from a dictionary
+
+        Parameters
+        ----------
+        data : dict
+            Python dictionary containing key value pairs in human-readable
+            form (not data from Coscine!).
+        """
+        for key, value in data.items():
+            self[key] = value
+
+###############################################################################
+
+    def parse(self, data: Dict) -> None:
+        """
+        Parses data from Coscine into an InputForm.
+
+        Parameters
+        ----------
+        data : dict
+            Python dictionary (output of json.loads) containing
+            the data from Coscine.
+        """
+
+###############################################################################
+
+    def generate(self) -> dict:
+        """
+        Generates Coscine formatted json-ld from an InputForm.
+        """
+        return {}
+
+###############################################################################
+
+    def as_str(self, format: str = "str") -> str:
+        """
+        Returns a string in the specified format
+
+        Parameters
+        -----------
+        format : str, default "str"
+            Format of the string, possible options are: str, csv, json, html
+
+        Returns
+        --------
+        str
+            A string with the form values in the specified format.
+        """
+
+        supported_formats = ["str", "csv", "json", "html"]
+        if format not in supported_formats:
+            raise ValueError(f"Unsupported format '{format}'!")
+        table = PrettyTable(
+            ("C", "Type", "Property", "Value"),
+            align="l"
+        )
+        rows = []
+        for key in self.keys():
+            value = str(self.get_value(key))
+            name: str = key
+            name = name + "*" if self.is_required(key) else name
+            controlled: str = ""
+            if self.is_controlled(key):
+                controlled = "V" if self.has_vocabulary(key) else "S"
+            datatype: str = str(self.datatype(key).__name__)
+            if self.properties(key).max_count > 1:
+                datatype = f"[{datatype}]"
+            rows.append((controlled, datatype, name, value))
+        table.max_width["Value"] = 50
+        table.add_rows(rows)
+        if format == "csv":
+            return table.get_csv_string()
+        if format == "json":
+            return table.get_json_string()
+        if format == "html":
+            return table.get_html_string()
+        return table.get_string()
+
+###############################################################################
```

### Comparing `coscine-0.9.0/src/coscine/graph.py` & `coscine-0.9.1/src/coscine/graph.py`

 * *Files identical despite different names*

### Comparing `coscine-0.9.0/src/coscine/object.py` & `coscine-0.9.1/src/coscine/object.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,506 +1,551 @@
-###############################################################################
-# Coscine Python SDK
-# Copyright (c) 2018-2023 RWTH Aachen University
-# Licensed under the terms of the MIT License
-###############################################################################
-# Coscine, short for Collaborative Scientific Integration Environment, is
-# a platform for research data management (RDM).
-# For more information on Coscine visit https://www.coscine.de/.
-#
-# Please note that this python module is open source software primarily
-# developed and maintained by the scientific community. It is not
-# an official service that RWTH Aachen provides support for.
-###############################################################################
-
-###############################################################################
-# File description
-###############################################################################
-
-"""
-Implements classes and routines for manipulating Metadata and interacting
-with files and file-like data in Coscine.
-"""
-
-###############################################################################
-# Dependencies
-###############################################################################
-
-from __future__ import annotations
-from datetime import datetime
-from typing import List, Optional, TYPE_CHECKING, Callable, Union
-import os
-import posixpath
-import logging
-import dateutil.parser
-from prettytable.prettytable import PrettyTable
-from coscine.graph import ApplicationProfile
-from coscine.form import InputForm, FormField
-from coscine.utils import HumanBytes, ProgressBar, parallelizable
-if TYPE_CHECKING:
-    from coscine.client import Client
-    from coscine.resource import Resource
-
-###############################################################################
-# Module globals / Constants
-###############################################################################
-
-logger = logging.getLogger(__name__)
-
-###############################################################################
-# Classes / Functions / Scripts
-###############################################################################
-
-class MetadataForm(InputForm):
-    """
-    The MetadataForm supports parsing coscine.Object metadata, generating
-    metadata and manipulating it in the same way one would manipulate
-    a python dict.
-    """
-
-    profile: ApplicationProfile
-
-###############################################################################
-
-    def __init__(self, client: Client, graph: ApplicationProfile) -> None:
-        """
-        Initializes an instance of type MetadataForm.
-
-        Parameters
-        ----------
-        client : Client
-            Coscine Python SDK client handle
-        graph : ApplicationProfile
-            Coscine application profile rdf graph
-        """
-
-        super().__init__(client)
-        self.profile = graph
-        self._fields = [
-            FormField(client, item) for item in self.profile.items()
-        ]
-        # Query vocabularies for controlled fields
-        for field in self._fields:
-            if field.vocabulary:
-                instance = client.vocabularies.instance(field.vocabulary)
-                self._vocabularies[field.path] = instance
-
-###############################################################################
-
-    def generate(self) -> dict:
-        """
-        Generates and validates metadata for sending to Coscine.
-        """
-
-        metadata = {}
-        metadata[ApplicationProfile.RDFTYPE] = [{
-            "type": "uri",
-            "value": self.profile.target()
-        }]
-
-        # Collect missing required fields
-        missing = []
-
-        # Set metadata
-        for key, values in self.items():
-            if not values:
-                if self.is_required(key):
-                    missing.append(key)
-                continue
-
-            properties = self.properties(key)
-            metadata[properties.path] = []
-            raw_value = values.raw()
-            if not isinstance(raw_value, list):
-                raw_value = [raw_value]
-            for value in raw_value:
-                entry = {
-                    "value": value,
-                    "datatype": (
-                        properties.datatype if properties.datatype
-                        else properties.vocabulary
-                    ),
-                    "type": "uri" if properties.vocabulary else "literal"
-                }
-                if not entry["datatype"]:
-                    del entry["datatype"]
-                metadata[properties.path].append(entry)
-
-        # Check for missing required fields
-        if len(missing) > 0:
-            raise ValueError(missing)
-
-        return metadata
-
-###############################################################################
-
-    def parse(self, data: Union[dict, None]) -> None:
-        if data is None:
-            return
-        for path, values in data.items():
-            if path == ApplicationProfile.RDFTYPE:
-                continue
-            try:
-                key = self.name_of(path)
-                self.set_value(key, [v["value"] for v in values], True)
-            except KeyError:
-                continue
-
-###############################################################################
-###############################################################################
-###############################################################################
-
-class FileObject:
-    """
-    Objects in Coscine represent file-like data. We could have called it
-    'File', but in case of linked data we are not actually dealing with files
-    themselves, but with links to files.Thus we require a more general
-    datatype.
-    """
-
-    client: Client
-    resource: Resource
-    data: dict
-    _cached_metadata: Optional[dict]  # None in case of no metadata
-    _metadata_cache_is_invalid: bool
-
-    @property
-    def has_metadata(self) -> bool:
-        """
-        Evaluates whether the FileObject has metadata attached to it
-        """
-        return bool(self._cached_metadata)
-
-    @property
-    def name(self) -> str:
-        """
-        FileObject name
-        """
-        return self.data["Name"]
-
-    @property
-    def size(self) -> int:
-        """
-        FileObject size in bytes
-        """
-        return int(self.data["Size"])
-
-    @property
-    def type(self) -> str:
-        """
-        FileObject type, e.g. 'file' or 'folder'
-        """
-        return self.data["Kind"]
-
-    @property
-    def modified(self) -> datetime:
-        """
-        Last time the FileObject was modified
-        """
-        if not self.data["Modified"]:
-            return datetime(1900, 1, 1)
-        return dateutil.parser.parse(self.data["Modified"])
-
-    @property
-    def created(self) -> datetime:
-        """
-        Time the FileObject was created
-        """
-        if not self.data["Created"]:
-            return datetime(1900, 1, 1)
-        return dateutil.parser.parse(self.data["Created"])
-
-    @property
-    def provider(self) -> str:
-        """
-        Resource type
-        """
-        return self.data["Provider"]
-
-    @property
-    def filetype(self) -> str:
-        """
-        FileObject file type, e.g. '.png'
-        """
-        return os.path.splitext(self.data["Name"])[1]
-
-    @property
-    def path(self) -> str:
-        """
-        FileObject path including folders (in case of S3 resources)
-        """
-        return self.data["Path"]
-
-    @property
-    def is_folder(self) -> bool:
-        """
-        Evaluates to true if the FileObject resembles a folder (only S3)
-        """
-        return bool(self.data["IsFolder"])
-
-    CHUNK_SIZE: int = 4096
-
-###############################################################################
-
-    def __init__(
-        self,
-        resource: Resource, data: dict,
-        metadata: Optional[dict] = None
-    ) -> None:
-        """
-        Initializes the Coscine FileObject.
-
-        Parameters
-        ----------
-        resource : Resource
-            Coscine resource handle.
-        data : dict
-            data of the file-like object.
-        """
-
-        # Configuration
-        self.client = resource.client
-        self.resource = resource
-        self.data = data
-        self._cached_metadata = metadata
-        self._metadata_cache_is_invalid = False
-
-###############################################################################
-
-    def __str__(self) -> str:
-        table = PrettyTable(("Property", "Value"))
-        rows = [
-            ("Name", self.name),
-            ("Size", HumanBytes.format(self.size)),
-            ("Type", self.type),
-            ("Path", self.path),
-            ("Folder", self.is_folder)
-        ]
-        table.max_width["Value"] = 50
-        table.add_rows(rows)
-        return table.get_string(title=f"Object {self.name}")
-
-###############################################################################
-
-    def metadata(self, force_update: bool = False) -> Union[dict, None]:
-        """
-        Retrieves the metadata of the file-like object.
-
-        Parameters
-        ----------
-        force_update : bool, default: False
-            Normally, metadata is cached and that cache is only updated
-            when an action is performed via the Coscine Python SDK, that
-            would invalidate that cache (e.g. update()).
-            By setting force_update to True, metadata is always fetched
-            from Coscine, ignoring the cache. Keep in mind that fetching
-            the metadata from every file in a resource will result in a
-            seperate request for each file, while with caching it only
-            fetches all metadata once.
-
-        Returns
-        -------
-        dict
-            Metadata as a python dictionary.
-        None
-            If no metadata has been set for the file-like object.
-        """
-
-        if not (force_update or self._metadata_cache_is_invalid):
-            if self._cached_metadata:
-                for key in self._cached_metadata:
-                    return self._cached_metadata[key]
-            return None
-        uri = self.client.uri("Tree", "Tree", self.resource.id)
-        args = {"path": self.path}
-        data = self.client.get(uri, params=args).json()
-        metadata = data["data"]["metadataStorage"]
-        if not metadata:
-            return None
-        metadata = metadata[0]
-        for key in metadata:
-            self._cached_metadata = metadata
-            self._metadata_cache_is_invalid = False
-            return metadata[key]
-        return None
-
-###############################################################################
-
-    @parallelizable
-    def update(self, metadata: Union[MetadataForm, dict]) -> None:
-        """
-        Updates the metadata of the file-like object.
-
-        Parameters
-        ----------
-        metadata : MetadataForm or dict
-            MetadataForm or JSON-LD formatted metadata dict
-
-        Raises
-        ------
-        TypeError
-            If argument `metadata` has an unexpected type.
-        """
-
-        if isinstance(metadata, MetadataForm):
-            metadata = metadata.generate()
-        elif not isinstance(metadata, dict):
-            raise TypeError("Expected MetadataForm or dict.")
-        logger.info("Updating metadata of FileObject '%s'...", self.path)
-        uri = self.client.uri("Tree", "Tree", self.resource.id)
-        self.client.put(uri, params={"path": self.path}, json=metadata)
-        self._metadata_cache_is_invalid = True  # Invalidate cached metadata
-
-###############################################################################
-
-    @parallelizable
-    def content(self) -> bytes:
-        """
-        Retrieves the content/data of the object. In case of linked data
-        this would be the link, not the actual file itself. It is impossible
-        to get the contents of linked data objects with this python module.
-        In case of rds or rds-s3 data this would return the file contents.
-        Be aware that for very large files this will consume a considerable
-        amount of RAM!
-
-        Returns
-        -------
-        bytes
-            A raw byte-array containing the Coscine file-object's data.
-        """
-
-        uri = self.client.uri("Blob", "Blob", self.resource.id)
-        return self.client.get(uri, params={"path": self.path}).content
-
-###############################################################################
-
-    @parallelizable
-    def download(
-        self,
-        path: str = "./",
-        callback: Optional[Callable[[int], None]] = None,
-        preserve_path: Optional[bool] = False
-    ) -> None:
-        """
-        Downloads the file-like object to the local harddrive.
-
-        Parameters
-        ----------
-        path : str, default: "./"
-            The path to the download location on the harddrive.
-        callback : function(chunksize: int)
-            A callback function to be called during downloading chunks.
-        preserve_path : bool, default: False
-            Preserve the folder structure, i.e. if the file object is located
-            in a subfolder, create said subfolder if it does not exist yet
-            on the local harddrive and put the file in there.
-        """
-
-        logger.info("Downloading FileObject '%s'...", self.path)
-        if self.is_folder:
-            if preserve_path:
-                path = posixpath.join(path, self.path)
-                os.makedirs(path, exist_ok=True)
-            else:
-                raise TypeError(
-                    "FileObject is a folder! "
-                    "Set 'preserve_path=True' to download folders."
-                )
-        else:
-            if "Action" in self.data:
-                uri = self.data["Action"]["Download"]["Url"]
-                response = self.client.get(uri, stream=True)
-            else:
-                uri = self.client.uri("Blob", "Blob", self.resource.id)
-                args = {"path": self.path}
-                response = self.client.get(uri, params=args, stream=True)
-            if preserve_path:
-                path = posixpath.join(path, self.path)
-            else:
-                path = os.path.join(path, self.name)
-            with open(path, 'wb') as file:
-                progress_bar = ProgressBar(
-                    self.client.settings.verbose,
-                    self.size, self.name, callback
-                )
-                for chunk in response.iter_content(chunk_size=self.CHUNK_SIZE):
-                    file.write(chunk)
-                    progress_bar.update(len(chunk))
-
-###############################################################################
-
-    @parallelizable
-    def delete(self) -> None:
-        """
-        Deletes the file-like object on the Coscine server.
-        """
-
-        logger.info("Deleting FileObject '%s'...", self.path)
-        uri = self.client.uri("Blob", "Blob", self.resource.id)
-        self.client.delete(uri, params={"path": self.path})
-
-###############################################################################
-
-    def objects(self, path: str = "") -> List[FileObject]:
-        """
-        Returns a list of FileObjects resembling the contents of
-        the current object in case the current object is a folder.
-        Irrelevant for anything other than S3 resources.
-
-        Parameters
-        -----------
-        path : str, default: None
-            Path to a directory. Irrelevant for anything other than S3.
-
-        Returns
-        -------
-        List[FileObject]
-            A list of file objects.
-
-        Raises
-        -------
-        TypeError
-            In case the current FileObject is not a folder or not part of an
-            S3 resource.
-        """
-        if self.is_folder:
-            fullpath = posixpath.join(self.path, path)
-            return self.resource.objects(fullpath)
-        raise TypeError(f"FileObject '{self.path}' is not a directory!")
-
-###############################################################################
-
-    def object(self, path: str) -> Optional[FileObject]:
-        """
-        Returns a FileObject resembling a file inside of
-        the current object in case the current object is a folder.
-        Irrelevant for anything other than S3 resources.
-
-        Parameters
-        -----------
-        path : str
-            Path to the file or folder.
-
-        Raises
-        -------
-        TypeError
-            In case the current FileObject is not a folder or not part of an
-            S3 resource.
-        """
-        if self.is_folder:
-            fullpath = posixpath.join(self.path, path)
-            return self.resource.object(fullpath)
-        raise TypeError(f"FileObject '{self.path}' is not a directory!")
-
-###############################################################################
-
-    def form(self) -> MetadataForm:
-        """
-        Returns a MetadataForm to interact with the metadata of the FileObject.
-        """
-
-        graph = self.resource.application_profile()
-        form = MetadataForm(self.client, graph)
-        form.parse(self.metadata())
-        return form
-
-###############################################################################
+###############################################################################
+# Coscine Python SDK
+# Copyright (c) 2018-2023 RWTH Aachen University
+# Licensed under the terms of the MIT License
+###############################################################################
+# Coscine, short for Collaborative Scientific Integration Environment, is
+# a platform for research data management (RDM).
+# For more information on Coscine visit https://www.coscine.de/.
+#
+# Please note that this python module is open source software primarily
+# developed and maintained by the scientific community. It is not
+# an official service that RWTH Aachen provides support for.
+###############################################################################
+
+###############################################################################
+# File description
+###############################################################################
+
+"""
+Implements classes and routines for manipulating Metadata and interacting
+with files and file-like data in Coscine.
+"""
+
+###############################################################################
+# Dependencies
+###############################################################################
+
+from __future__ import annotations
+from datetime import datetime
+from typing import List, Optional, TYPE_CHECKING, Callable, Union
+import os
+import posixpath
+import logging
+import dateutil.parser
+from prettytable.prettytable import PrettyTable
+from coscine.graph import ApplicationProfile
+from coscine.form import InputForm, FormField
+from coscine.utils import HumanBytes, ProgressBar, parallelizable
+if TYPE_CHECKING:
+    from coscine.client import Client
+    from coscine.resource import Resource
+
+###############################################################################
+# Module globals / Constants
+###############################################################################
+
+logger = logging.getLogger(__name__)
+
+###############################################################################
+# Classes / Functions / Scripts
+###############################################################################
+
+class MetadataForm(InputForm):
+    """
+    The MetadataForm supports parsing coscine.Object metadata, generating
+    metadata and manipulating it in the same way one would manipulate
+    a python dict.
+    """
+
+    profile: ApplicationProfile
+
+###############################################################################
+
+    def __init__(self, client: Client, graph: ApplicationProfile) -> None:
+        """
+        Initializes an instance of type MetadataForm.
+
+        Parameters
+        ----------
+        client : Client
+            Coscine Python SDK client handle
+        graph : ApplicationProfile
+            Coscine application profile rdf graph
+        """
+
+        super().__init__(client)
+        self.profile = graph
+        self._fields = [
+            FormField(client, item) for item in self.profile.items()
+        ]
+        # Query vocabularies for controlled fields
+        for field in self._fields:
+            if field.vocabulary:
+                instance = client.vocabularies.instance(field.vocabulary)
+                self._vocabularies[field.path] = instance
+
+###############################################################################
+
+    def generate(self) -> dict:
+        """
+        Generates and validates metadata for sending to Coscine.
+        """
+
+        metadata = {}
+        metadata[ApplicationProfile.RDFTYPE] = [{
+            "type": "uri",
+            "value": self.profile.target()
+        }]
+
+        # Collect missing required fields
+        missing = []
+
+        # Set metadata
+        for key, values in self.items():
+            if not values:
+                if self.is_required(key):
+                    missing.append(key)
+                continue
+
+            properties = self.properties(key)
+            metadata[properties.path] = []
+            raw_value = values.raw()
+            if not isinstance(raw_value, list):
+                raw_value = [raw_value]
+            for value in raw_value:
+                entry = {
+                    "value": value,
+                    "datatype": (
+                        properties.datatype if properties.datatype
+                        else properties.vocabulary
+                    ),
+                    "type": "uri" if properties.vocabulary else "literal"
+                }
+                if not entry["datatype"]:
+                    del entry["datatype"]
+                metadata[properties.path].append(entry)
+
+        # Check for missing required fields
+        if len(missing) > 0:
+            raise ValueError(missing)
+
+        return metadata
+
+###############################################################################
+
+    def parse(self, data: Union[dict, None]) -> None:
+        if data is None:
+            return
+        for path, values in data.items():
+            if path == ApplicationProfile.RDFTYPE:
+                continue
+            try:
+                key = self.name_of(path)
+                self.set_value(key, [v["value"] for v in values], True)
+            except KeyError:
+                continue
+
+###############################################################################
+###############################################################################
+###############################################################################
+
+class FileActions:
+    """
+    Provides FileObject Action URLs that provide direct access to a FileObject
+    without requiring authentication/credentials. Once generated,
+    the URLs are only valid for a limited time.
+    """
+
+    _data: dict
+
+    def __init__(self, data: dict) -> None:
+        self._data = data
+
+    @property
+    def download(self) -> str:
+        """
+        Returns the direct download URL for an object of type file.
+        The URL is valid for 24 hours and requires no authentication.
+        """
+        if "Download" in self._data:
+            return self._data["Download"]["Url"]
+        return ""
+
+    @property
+    def delete(self) -> str:
+        """
+        Returns the direct download URL for an object of type file.
+        The URL is valid for 24 hours and requires no authentication.
+        """
+        return self._data["Delete"]["Url"] if "Delete" in self._data else ""
+
+    @property
+    def update(self) -> str:
+        """
+        Returns the direct download URL for an object of type file.
+        The URL is valid for 24 hours and requires no authentication.
+        """
+        return self._data["Update"]["Url"] if "Update" in self._data else ""
+
+###############################################################################
+###############################################################################
+###############################################################################
+
+class FileObject:
+    """
+    Objects in Coscine represent file-like data. We could have called it
+    'File', but in case of linked data we are not actually dealing with files
+    themselves, but with links to files.Thus we require a more general
+    datatype.
+    """
+
+    client: Client
+    resource: Resource
+    data: dict
+    actions: FileActions
+    _cached_metadata: Optional[dict]  # None in case of no metadata
+    _metadata_cache_is_invalid: bool
+
+    @property
+    def has_metadata(self) -> bool:
+        """
+        Evaluates whether the FileObject has metadata attached to it
+        """
+        return bool(self._cached_metadata)
+
+    @property
+    def name(self) -> str:
+        """
+        FileObject name
+        """
+        return self.data["Name"]
+
+    @property
+    def size(self) -> int:
+        """
+        FileObject size in bytes
+        """
+        return int(self.data["Size"])
+
+    @property
+    def type(self) -> str:
+        """
+        FileObject type, e.g. 'file' or 'folder'
+        """
+        return self.data["Kind"]
+
+    @property
+    def modified(self) -> datetime:
+        """
+        Last time the FileObject was modified
+        """
+        if not self.data["Modified"]:
+            return datetime(1900, 1, 1)
+        return dateutil.parser.parse(self.data["Modified"])
+
+    @property
+    def created(self) -> datetime:
+        """
+        Time the FileObject was created
+        """
+        if not self.data["Created"]:
+            return datetime(1900, 1, 1)
+        return dateutil.parser.parse(self.data["Created"])
+
+    @property
+    def provider(self) -> str:
+        """
+        Resource type
+        """
+        return self.data["Provider"]
+
+    @property
+    def filetype(self) -> str:
+        """
+        FileObject file type, e.g. '.png'
+        """
+        return os.path.splitext(self.data["Name"])[1]
+
+    @property
+    def path(self) -> str:
+        """
+        FileObject path including folders (in case of S3 resources)
+        """
+        return self.data["Path"]
+
+    @property
+    def is_folder(self) -> bool:
+        """
+        Evaluates to true if the FileObject resembles a folder (only S3)
+        """
+        return bool(self.data["IsFolder"])
+
+    CHUNK_SIZE: int = 4096
+
+###############################################################################
+
+    def __init__(
+        self,
+        resource: Resource, data: dict,
+        metadata: Optional[dict] = None
+    ) -> None:
+        """
+        Initializes the Coscine FileObject.
+
+        Parameters
+        ----------
+        resource : Resource
+            Coscine resource handle.
+        data : dict
+            data of the file-like object.
+        """
+
+        # Configuration
+        self.client = resource.client
+        self.resource = resource
+        self.data = data
+        self.actions = FileActions(data["Action"])
+        self._cached_metadata = metadata
+        self._metadata_cache_is_invalid = False
+
+###############################################################################
+
+    def __str__(self) -> str:
+        table = PrettyTable(("Property", "Value"))
+        rows = [
+            ("Name", self.name),
+            ("Size", HumanBytes.format(self.size)),
+            ("Type", self.type),
+            ("Path", self.path),
+            ("Folder", self.is_folder)
+        ]
+        table.max_width["Value"] = 50
+        table.add_rows(rows)
+        return table.get_string(title=f"Object {self.name}")
+
+###############################################################################
+
+    def metadata(self, force_update: bool = False) -> Union[dict, None]:
+        """
+        Retrieves the metadata of the file-like object.
+
+        Parameters
+        ----------
+        force_update : bool, default: False
+            Normally, metadata is cached and that cache is only updated
+            when an action is performed via the Coscine Python SDK, that
+            would invalidate that cache (e.g. update()).
+            By setting force_update to True, metadata is always fetched
+            from Coscine, ignoring the cache. Keep in mind that fetching
+            the metadata from every file in a resource will result in a
+            seperate request for each file, while with caching it only
+            fetches all metadata once.
+
+        Returns
+        -------
+        dict
+            Metadata as a python dictionary.
+        None
+            If no metadata has been set for the file-like object.
+        """
+
+        if not (force_update or self._metadata_cache_is_invalid):
+            if self._cached_metadata:
+                for key in self._cached_metadata:
+                    return self._cached_metadata[key]
+            else:
+                return None
+        uri = self.client.uri("Tree", "Tree", self.resource.id)
+        args = {"path": self.path}
+        data = self.client.get(uri, params=args).json()
+        metadata = data["data"]["metadataStorage"]
+        if not metadata:
+            return None
+        metadata = metadata[0]
+        for key in metadata:
+            self._cached_metadata = metadata
+            self._metadata_cache_is_invalid = False
+            return metadata[key]
+        return None
+
+###############################################################################
+
+    @parallelizable
+    def update(self, metadata: Union[MetadataForm, dict]) -> None:
+        """
+        Updates the metadata of the file-like object.
+
+        Parameters
+        ----------
+        metadata : MetadataForm or dict
+            MetadataForm or JSON-LD formatted metadata dict
+
+        Raises
+        ------
+        TypeError
+            If argument `metadata` has an unexpected type.
+        """
+
+        if isinstance(metadata, MetadataForm):
+            metadata = metadata.generate()
+        elif not isinstance(metadata, dict):
+            raise TypeError("Expected MetadataForm or dict.")
+        logger.info("Updating metadata of FileObject '%s'...", self.path)
+        uri = self.client.uri("Tree", "Tree", self.resource.id)
+        self.client.put(uri, params={"path": self.path}, json=metadata)
+        self._metadata_cache_is_invalid = True  # Invalidate cached metadata
+
+###############################################################################
+
+    @parallelizable
+    def content(self) -> bytes:
+        """
+        Retrieves the content/data of the object. In case of linked data
+        this would be the link, not the actual file itself. It is impossible
+        to get the contents of linked data objects with this python module.
+        In case of rds or rds-s3 data this would return the file contents.
+        Be aware that for very large files this will consume a considerable
+        amount of RAM!
+
+        Returns
+        -------
+        bytes
+            A raw byte-array containing the Coscine file-object's data.
+        """
+
+        uri = self.client.uri("Blob", "Blob", self.resource.id)
+        return self.client.get(uri, params={"path": self.path}).content
+
+###############################################################################
+
+    @parallelizable
+    def download(
+        self,
+        path: str = "./",
+        callback: Optional[Callable[[int], None]] = None,
+        preserve_path: Optional[bool] = False
+    ) -> None:
+        """
+        Downloads the file-like object to the local harddrive.
+
+        Parameters
+        ----------
+        path : str, default: "./"
+            The path to the download location on the harddrive.
+        callback : function(chunksize: int)
+            A callback function to be called during downloading chunks.
+        preserve_path : bool, default: False
+            Preserve the folder structure, i.e. if the file object is located
+            in a subfolder, create said subfolder if it does not exist yet
+            on the local harddrive and put the file in there.
+        """
+
+        logger.info("Downloading FileObject '%s'...", self.path)
+        if self.is_folder:
+            if preserve_path:
+                path = posixpath.join(path, self.path)
+                os.makedirs(path, exist_ok=True)
+            else:
+                raise TypeError(
+                    "FileObject is a folder! "
+                    "Set 'preserve_path=True' to download folders."
+                )
+        else:
+            if "Action" in self.data:
+                uri = self.data["Action"]["Download"]["Url"]
+                response = self.client.get(uri, stream=True)
+            else:
+                uri = self.client.uri("Blob", "Blob", self.resource.id)
+                args = {"path": self.path}
+                response = self.client.get(uri, params=args, stream=True)
+            if preserve_path:
+                path = posixpath.join(path, self.path)
+            else:
+                path = os.path.join(path, self.name)
+            with open(path, 'wb') as file:
+                progress_bar = ProgressBar(
+                    self.client.settings.verbose,
+                    self.size, self.name, callback
+                )
+                for chunk in response.iter_content(chunk_size=self.CHUNK_SIZE):
+                    file.write(chunk)
+                    progress_bar.update(len(chunk))
+
+###############################################################################
+
+    @parallelizable
+    def delete(self) -> None:
+        """
+        Deletes the file-like object on the Coscine server.
+        """
+
+        logger.info("Deleting FileObject '%s'...", self.path)
+        uri = self.client.uri("Blob", "Blob", self.resource.id)
+        self.client.delete(uri, params={"path": self.path})
+
+###############################################################################
+
+    def objects(self, path: str = "") -> List[FileObject]:
+        """
+        Returns a list of FileObjects resembling the contents of
+        the current object in case the current object is a folder.
+        Irrelevant for anything other than S3 resources.
+
+        Parameters
+        -----------
+        path : str, default: None
+            Path to a directory. Irrelevant for anything other than S3.
+
+        Returns
+        -------
+        List[FileObject]
+            A list of file objects.
+
+        Raises
+        -------
+        TypeError
+            In case the current FileObject is not a folder or not part of an
+            S3 resource.
+        """
+        if self.is_folder:
+            fullpath = posixpath.join(self.path, path)
+            return self.resource.objects(fullpath)
+        raise TypeError(f"FileObject '{self.path}' is not a directory!")
+
+###############################################################################
+
+    def object(self, path: str) -> Optional[FileObject]:
+        """
+        Returns a FileObject resembling a file inside of
+        the current object in case the current object is a folder.
+        Irrelevant for anything other than S3 resources.
+
+        Parameters
+        -----------
+        path : str
+            Path to the file or folder.
+
+        Raises
+        -------
+        TypeError
+            In case the current FileObject is not a folder or not part of an
+            S3 resource.
+        """
+        if self.is_folder:
+            fullpath = posixpath.join(self.path, path)
+            return self.resource.object(fullpath)
+        raise TypeError(f"FileObject '{self.path}' is not a directory!")
+
+###############################################################################
+
+    def form(self) -> MetadataForm:
+        """
+        Returns a MetadataForm to interact with the metadata of the FileObject.
+        """
+
+        graph = self.resource.application_profile()
+        form = MetadataForm(self.client, graph)
+        form.parse(self.metadata())
+        return form
+
+###############################################################################
```

### Comparing `coscine-0.9.0/src/coscine/project.py` & `coscine-0.9.1/src/coscine/project.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,659 +1,661 @@
-###############################################################################
-# Coscine Python SDK
-# Copyright (c) 2018-2023 RWTH Aachen University
-# Licensed under the terms of the MIT License
-###############################################################################
-# Coscine, short for Collaborative Scientific Integration Environment, is
-# a platform for research data management (RDM).
-# For more information on Coscine visit https://www.coscine.de/.
-#
-# Please note that this python module is open source software primarily
-# developed and maintained by the scientific community. It is not
-# an official service that RWTH Aachen provides support for.
-###############################################################################
-
-###############################################################################
-# File description
-###############################################################################
-
-"""
-This file defines the project object for the representation of
-Coscine projects. It provides a simple interface to interact with Coscine
-projects from python.
-"""
-
-###############################################################################
-# Dependencies
-###############################################################################
-
-from __future__ import annotations
-from typing import Optional, TYPE_CHECKING, Union, List
-import json
-import os
-from datetime import datetime
-import logging
-import dateutil.parser
-from prettytable.prettytable import PrettyTable
-from coscine.resource import Resource, ResourceForm
-from coscine.form import InputForm
-from coscine.utils import parallelizable
-if TYPE_CHECKING:
-    from coscine.client import Client
-
-###############################################################################
-# Module globals / Constants
-###############################################################################
-
-logger = logging.getLogger(__name__)
-
-###############################################################################
-# Classes / Functions / Scripts
-###############################################################################
-
-class ProjectForm(InputForm):
-    """
-    An InputForm for Coscine project metadata. Use this form
-    to generate or edit project metadata such as the project name
-    and start date.
-    """
-
-###############################################################################
-
-    def __init__(self, client: Client) -> None:
-        """
-        Generates a new instance of type ProjectForm.
-
-        Parameters
-        ----------
-        client : Client
-            Coscine Python SDK Client handle
-        """
-        super().__init__(client)
-        self._fields = client.vocabularies.builtin("project")
-        vocabularies = {
-            "disciplines": client.vocabularies.disciplines(True),
-            "visibility": client.vocabularies.visibility(True)
-        }
-        for item in self._fields:
-            if item.vocabulary:
-                self._vocabularies[item.path] = vocabularies[item.path]
-
-###############################################################################
-
-    @staticmethod
-    def _parse_organizations(data: List):
-        return [value["url"] for value in data]
-
-###############################################################################
-
-    def parse(self, data: dict) -> None:
-        for path, value in data.items():
-            if path in ["id", "slug", "parentId"]:  # ignored paths
-                continue
-            if path == "organizations":
-                value = self._parse_organizations(value)
-            try:
-                key = self.name_of(path)
-                self.set_value(key, value, True)
-            except KeyError:
-                continue
-
-###############################################################################
-
-    def generate(self) -> dict:
-        metadata = {}
-        missing = []
-
-        for key, value in self.items():
-            if not value:
-                if self.is_required(key):
-                    missing.append(key)
-                continue
-            properties = self.properties(key)
-            metadata[properties.path] = value.raw()
-
-            # The organizations field is normally controlled, but we omit
-            # actively controlling it, because doing so is too complicated.
-            # Because we handle things differently here, some special care
-            # is needed when preparing it for Coscine:
-            if properties.path == "organizations":
-                metadata[properties.path] = [{
-                    "displayName": url, "url": url
-                } for url in value.raw()]
-        if missing:
-            raise ValueError(missing)
-        return metadata
-
-###############################################################################
-# Class definition
-###############################################################################
-
-class Project:
-    """
-    Python representation of a Coscine Project
-    """
-
-    client: Client
-    data: dict
-    parent: Optional[Project]
-
-###############################################################################
-
-    def __init__(
-        self,
-        client: Client,
-        data: dict,
-        parent: Optional[Project] = None
-    ) -> None:
-        """
-        Initializes a Coscine project object.
-
-        Parameters
-        ----------
-        client : Client
-            Coscine client handle
-        data : dict
-            Project data received from Coscine.
-        parent : Project, default: None
-            Optional parent project.
-        """
-
-        self.client = client
-        self.data = data
-        self.parent = parent
-
-###############################################################################
-
-    @property
-    def id(self) -> str:
-        """
-        Project ID
-        """
-        return self.data["id"]
-
-    @property
-    def name(self) -> str:
-        """
-        Project Name
-        """
-        return self.data["projectName"]
-
-    @property
-    def display_name(self) -> str:
-        """
-        Project Display Name
-        """
-        return self.data["displayName"]
-
-    @property
-    def description(self) -> str:
-        """
-        Project Description
-        """
-        return self.data["description"]
-
-    @property
-    def principle_investigators(self) -> str:
-        """
-        Project PIs
-        """
-        return self.data["principleInvestigators"]
-
-    @property
-    def start_date(self) -> datetime:
-        """
-        Project Start Date as datetime object
-        """
-        return dateutil.parser.parse(self.data["startDate"])
-
-    @property
-    def end_date(self) -> datetime:
-        """
-        Project End Date as datetime object
-        """
-        return dateutil.parser.parse(self.data["endDate"])
-
-    @property
-    def disciplines(self) -> List[str]:
-        """
-        Project Disciplines
-        """
-        lang = {
-            "en": "displayNameEn",
-            "de": "displayNameDe"
-        }[self.client.settings.language]
-        return [k[lang] for k in self.data["disciplines"]]
-
-    @property
-    def organizations(self) -> List[str]:
-        """
-        Project Associated Organizations
-        """
-        return [k["displayName"] for k in self.data["organizations"]]
-
-    @property
-    def visibility(self) -> str:
-        """
-        Project Visibility in Coscine
-        """
-        return self.data["visibility"]["displayName"]
-
-###############################################################################
-
-    def __str__(self) -> str:
-        table = PrettyTable(("Property", "Value"))
-        rows = [
-            ("ID", self.id),
-            ("Name", self.name),
-            ("Display Name", self.display_name),
-            ("Description", self.description),
-            ("Principle Investigators", self.principle_investigators),
-            ("Disciplines", "\n".join(self.disciplines)),
-            ("Organizations", "\n".join(self.organizations)),
-            ("Start Date", self.start_date),
-            ("End Date", self.end_date),
-            ("Visibility", self.visibility)
-        ]
-        table.max_width["Value"] = 50
-        table.add_rows(rows)
-        return table.get_string(title=f"Project {self.display_name}")
-
-###############################################################################
-
-    def subprojects(self) -> List[Project]:
-        """
-        Retrieves a list of a all projects the creator of the Coscine API token
-        is currently a member of.
-
-        Returns
-        -------
-        list
-            List of coscine.Project objects
-        """
-
-        uri = self.client.uri("Project", "SubProject", self.id)
-        projects = []
-        for data in self.client.get(uri).json():
-            projects.append(Project(self.client, data, self))
-        return projects
-
-###############################################################################
-
-    def subproject(self, display_name: str) -> Optional[Project]:
-        """
-        Returns a single subproject via its displayName
-
-        Parameters
-        ----------
-        display_name : str
-            Look for a project with the specified displayName
-
-        Returns
-        -------
-        Project
-            A single coscine project handle or None if no match found
-
-        Raises
-        ------
-        IndexError
-        """
-
-        filtered_project_list = list(filter(
-            lambda project: project.display_name == display_name,
-            self.subprojects()
-        ))
-        if len(filtered_project_list) == 1:
-            return filtered_project_list[0]
-        if len(filtered_project_list) == 0:
-            return None
-        raise IndexError("Too many projects matching the specified criteria!")
-
-###############################################################################
-
-    def create_subproject(self, form: ProjectForm) -> Project:
-        """
-        Creates a subproject inside of the current project
-        """
-        metadata = form.generate()
-        metadata["ParentId"] = self.id
-        return self.client.create_project(metadata)
-
-###############################################################################
-
-    def delete(self) -> None:
-        """
-        Deletes the project on the Coscine servers.
-        """
-
-        uri = self.client.uri("Project", "Project", self.id)
-        self.client.delete(uri)
-
-###############################################################################
-
-    def resources(self) -> List[Resource]:
-        """
-        Retrieves a list of Resources of the current project.
-
-        Returns
-        -------
-        list[Resource]
-            list of resources matching the supplied filter.
-        """
-
-        uri = self.client.uri("Project", "Project", self.id, "resources")
-        resources = []
-        for data in self.client.get(uri).json():
-            resources.append(Resource(self, data))
-        return resources
-
-###############################################################################
-
-    def resource(self, display_name: str) -> Optional[Resource]:
-        """
-        Retrieves a certain resource of the current project
-        identified by its displayName.
-
-        Parameters
-        ----------
-        display_name : str
-            The display name of the resource.
-
-        Returns
-        --------
-        Resource or None
-
-        Raises
-        -------
-        IndexError
-        """
-
-        resources = list(filter(
-            lambda resource: resource.display_name == display_name,
-            self.resources()
-        ))
-        if len(resources) == 1:
-            return resources[0]
-        if len(resources) == 0:
-            return None
-        raise IndexError("Too many resources matching the specified criteria!")
-
-###############################################################################
-
-    def download(self, path: str = "./", metadata: bool = False) -> None:
-        """
-        Downloads the project to the location referenced by 'path'.
-
-        Parameters
-        ----------
-        path : str
-            Download location on the harddrive
-            Default: current directory './'
-        metadata : bool, default: False
-            If enabled, project metadata is downloaded and put in
-            a hidden file '.metadata.json'.
-        """
-
-        logger.info("Downloading project '%s' (%s)...", self.name, self.id)
-        path = os.path.join(path, self.display_name)
-        if not os.path.isdir(path):
-            os.mkdir(path)
-        for resource in self.resources():
-            resource.download(path=path, metadata=metadata)
-        if metadata:
-            data = json.dumps(self.data, indent=4)
-            metadata_path: str = os.path.join(path, ".metadata.json")
-            with open(metadata_path, "w", encoding="utf-8") as file:
-                file.write(data)
-
-###############################################################################
-
-    def members(self) -> List[ProjectMember]:
-        """
-        Retrieves a list of all members of the current project
-
-        Returns
-        --------
-        list[ProjectMember]
-            List of project members as ProjectMember objects.
-        """
-
-        uri = self.client.uri("Project", "ProjectRole", self.id)
-        data = self.client.get(uri).json()
-        members = [ProjectMember(self, m) for m in data]
-        return members
-
-###############################################################################
-
-    @parallelizable
-    def invite(self, email: str, role: str = "Member") -> None:
-        """
-        Invites a person to a project via their email address
-
-        Parameters
-        ----------
-        email : str
-            The email address to send the invite to
-        role : str, "Member", "Guest" or "Owner", default: "Member"
-            The role for the new project member
-        """
-
-        if role not in ProjectMember.ROLES:
-            raise ValueError(f"Invalid role {role}.")
-
-        logger.info("Inviting %s as %s to project %s.", email, role, self.name)
-        uri = self.client.uri("Project", "Project", "invitation")
-        data = {
-            "projectId": self.data["id"],
-            "role": ProjectMember.ROLES[role],
-            "email": email
-        }
-
-        try:
-            self.client.post(uri, json=data)
-        except RuntimeError:
-            logger.warning("User %s has pending invites.", email)
-
-###############################################################################
-
-    @parallelizable
-    def add_member(self, member: ProjectMember, role: str = "Member"):
-        """
-        Adds a project member of another project to the current project.
-
-        Parameters
-        ----------
-        member : ProjectMember
-            Member of another Coscine project
-        role : str, "Member", "Guest" or "Owner", default: "Member"
-
-        Raises
-        ------
-        ValueError
-            In case the specified role is unsupported
-        """
-
-        if role not in ProjectMember.ROLES:
-            raise ValueError(f"Invalid role for member '{member.name}'!")
-        data = member.data
-        data["projectId"] = self.id
-        data["role"]["displayName"] = role
-        data["role"]["id"] = ProjectMember.ROLES[role]
-        uri = self.client.uri("Project", "ProjectRole")
-        self.client.post(uri, json=data)
-        logger.info(
-            "Added '%s' as a project member with "
-            "role '%s' to project '%s'.",
-            member.name, role, self.name
-        )
-
-###############################################################################
-
-    def form(self) -> ProjectForm:
-        """
-        Returns the project metadata form of the project. That form can
-        then be used to edit the project metadata.
-
-        Examples
-        ---------
-        >>> metadata = Project.form()
-        >>> metadata["Display Name"] = "Different display name"
-        >>> Project.update(metadata)
-        """
-
-        form = ProjectForm(self.client)
-        form.parse(self.data)
-        return form
-
-###############################################################################
-
-    def update(self, form: Union[ProjectForm, dict]) -> Project:
-        """
-        Updates a project using the given ProjectForm
-
-        Parameters
-        ----------
-        form : ProjectForm or dict
-            ProjectForm containing updated data or dict generated from a form.
-        """
-
-        if isinstance(form, ProjectForm):
-            form = form.generate()
-        uri = self.client.uri("Project", "Project", self.id)
-        response = self.client.post(uri, json=form)
-        logger.info(
-            "Updated project metadata for '%s' (%s).",
-            self.name, self.id
-        )
-        updated_project_handle = self
-        if response.ok:
-            # Update project properties
-            # The response unfortunately does not return
-            # the new project data - bummer!
-            updated_project_handle = list(filter(
-                lambda p: p.id == self.id,
-                self.client.projects(False)
-            ))[0]
-        return updated_project_handle
-
-###############################################################################
-
-    @parallelizable
-    def create_resource(self, form: Union[ResourceForm, dict]) -> Resource:
-        """
-        Creates a resource within the current project using the supplied
-        resource form.
-
-        Parameters
-        ----------
-        resourceForm : ResourceForm
-            Form to generate the resource with.
-        metadataPreset : MetadataPresetForm
-            optional application profile configuration.
-            Currently not supported.
-        """
-        if isinstance(form, ResourceForm):
-            form = form.generate()
-        uri = self.client.uri("Resources", "Resource", "project", self.id)
-        logger.info("Creating resource in project '%s'.", self.name)
-        return Resource(self, self.client.post(uri, json=form).json())
-
-###############################################################################
-###############################################################################
-
-class ProjectMember:
-    """
-    Python representation of a Coscine project member.
-    """
-
-    ROLES = {
-        "Owner": "be294c5e-4e42-49b3-bec4-4b15f49df9a5",
-        "Member": "508b6d4e-c6ac-4aa5-8a8d-caa31dd39527",
-        "Guest": "9184a442-4419-4e30-9fe6-0cfe32c9a81f"
-    }
-
-    data: dict
-    client: Client
-    project: Project
-
-###############################################################################
-
-    @property
-    def name(self) -> str:
-        """Name of the Project Member"""
-        return self.data["user"]["displayName"]
-
-    @property
-    def email(self) -> str:
-        """E-Mail address of the Project Member"""
-        return self.data["user"]["emailAddress"]
-
-    @property
-    def id(self) -> str:
-        """Project Member ID"""
-        return self.data["user"]["id"]
-
-    @property
-    def role(self) -> str:
-        """Role of the Project Member within the Project"""
-        return self.data["role"]["displayName"]
-
-###############################################################################
-
-    def __init__(self, project: Project, data: dict) -> None:
-        """
-        Initializes a project member for a given project.
-
-        Parameters
-        ----------
-        project : Project
-            Coscine Python SDK project handle.
-        data: dict
-            User data as dict, retrieved via
-            client.uri("Project", "ProjectRole", self.id).
-        """
-
-        self.project = project
-        self.client = self.project.client
-        self.data = data
-
-###############################################################################
-
-    @parallelizable
-    def set_role(self, role: str) -> None:
-        """
-        Sets the role of a project member
-
-        Parameters
-        ----------
-        role : str
-            The new role of the member ('Owner', 'Guest' or 'Member').
-        """
-
-        if role not in ProjectMember.ROLES:
-            raise ValueError(f"Invalid role {role}.")
-
-        uri = self.client.uri("Project", "ProjectRole")
-        self.data["role"]["id"] = ProjectMember.ROLES[role]
-        self.data["role"]["displayName"] = role
-        logger.info("Setting role of '%s' to '%s'...", self.name, role)
-        self.client.post(uri, json=self.data)
-
-###############################################################################
-
-    @parallelizable
-    def remove(self) -> None:
-        """
-        Removes a project member from their associated project.
-        """
-
-        uri = self.client.uri(
-            "Project", "ProjectRole", "project", self.project.id, "user",
-            self.id, "role", self.data["role"]["id"]
-        )
-        logger.info(
-            "Removing member '%s' from project '%s'...",
-            self.name, self.project.name
-        )
-        self.client.delete(uri)
-
-###############################################################################
+###############################################################################
+# Coscine Python SDK
+# Copyright (c) 2018-2023 RWTH Aachen University
+# Licensed under the terms of the MIT License
+###############################################################################
+# Coscine, short for Collaborative Scientific Integration Environment, is
+# a platform for research data management (RDM).
+# For more information on Coscine visit https://www.coscine.de/.
+#
+# Please note that this python module is open source software primarily
+# developed and maintained by the scientific community. It is not
+# an official service that RWTH Aachen provides support for.
+###############################################################################
+
+###############################################################################
+# File description
+###############################################################################
+
+"""
+This file defines the project object for the representation of
+Coscine projects. It provides a simple interface to interact with Coscine
+projects from python.
+"""
+
+###############################################################################
+# Dependencies
+###############################################################################
+
+from __future__ import annotations
+from typing import Optional, TYPE_CHECKING, Union, List
+import json
+import os
+from datetime import datetime
+import logging
+import dateutil.parser
+from prettytable.prettytable import PrettyTable
+from coscine.resource import Resource, ResourceForm
+from coscine.form import InputForm
+from coscine.utils import parallelizable
+if TYPE_CHECKING:
+    from coscine.client import Client
+
+###############################################################################
+# Module globals / Constants
+###############################################################################
+
+logger = logging.getLogger(__name__)
+
+###############################################################################
+# Classes / Functions / Scripts
+###############################################################################
+
+class ProjectForm(InputForm):
+    """
+    An InputForm for Coscine project metadata. Use this form
+    to generate or edit project metadata such as the project name
+    and start date.
+    """
+
+###############################################################################
+
+    def __init__(self, client: Client) -> None:
+        """
+        Generates a new instance of type ProjectForm.
+
+        Parameters
+        ----------
+        client : Client
+            Coscine Python SDK Client handle
+        """
+        super().__init__(client)
+        self._fields = client.vocabularies.builtin("project")
+        vocabularies = {
+            "disciplines": client.vocabularies.disciplines(True),
+            "visibility": client.vocabularies.visibility(True)
+        }
+        for item in self._fields:
+            if item.vocabulary:
+                self._vocabularies[item.path] = vocabularies[item.path]
+
+###############################################################################
+
+    @staticmethod
+    def _parse_organizations(data: List):
+        return [value["url"] for value in data]
+
+###############################################################################
+
+    def parse(self, data: dict) -> None:
+        for path, value in data.items():
+            if path in ["id", "slug", "parentId"]:  # ignored paths
+                continue
+            if path == "organizations":
+                value = self._parse_organizations(value)
+            try:
+                key = self.name_of(path)
+                self.set_value(key, value, True)
+            except KeyError:
+                continue
+
+###############################################################################
+
+    def generate(self) -> dict:
+        metadata = {}
+        missing = []
+
+        for key, value in self.items():
+            if not value:
+                if self.is_required(key):
+                    missing.append(key)
+                continue
+            properties = self.properties(key)
+            metadata[properties.path] = value.raw()
+
+            # The organizations field is normally controlled, but we omit
+            # actively controlling it, because doing so is too complicated.
+            # Because we handle things differently here, some special care
+            # is needed when preparing it for Coscine:
+            if properties.path == "organizations":
+                metadata[properties.path] = [{
+                    "displayName": url, "url": url
+                } for url in value.raw()]
+        if missing:
+            raise ValueError(missing)
+        return metadata
+
+###############################################################################
+# Class definition
+###############################################################################
+
+class Project:
+    """
+    Python representation of a Coscine Project
+    """
+
+    client: Client
+    data: dict
+    parent: Optional[Project]
+
+###############################################################################
+
+    def __init__(
+        self,
+        client: Client,
+        data: dict,
+        parent: Optional[Project] = None
+    ) -> None:
+        """
+        Initializes a Coscine project object.
+
+        Parameters
+        ----------
+        client : Client
+            Coscine client handle
+        data : dict
+            Project data received from Coscine.
+        parent : Project, default: None
+            Optional parent project.
+        """
+
+        self.client = client
+        self.data = data
+        self.parent = parent
+
+###############################################################################
+
+    @property
+    def id(self) -> str:
+        """
+        Project ID
+        """
+        return self.data["id"]
+
+    @property
+    def name(self) -> str:
+        """
+        Project Name
+        """
+        return self.data["projectName"]
+
+    @property
+    def display_name(self) -> str:
+        """
+        Project Display Name
+        """
+        return self.data["displayName"]
+
+    @property
+    def description(self) -> str:
+        """
+        Project Description
+        """
+        return self.data["description"]
+
+    @property
+    def principle_investigators(self) -> str:
+        """
+        Project PIs
+        """
+        return self.data["principleInvestigators"]
+
+    @property
+    def start_date(self) -> datetime:
+        """
+        Project Start Date as datetime object
+        """
+        return dateutil.parser.parse(self.data["startDate"])
+
+    @property
+    def end_date(self) -> datetime:
+        """
+        Project End Date as datetime object
+        """
+        return dateutil.parser.parse(self.data["endDate"])
+
+    @property
+    def disciplines(self) -> List[str]:
+        """
+        Project Disciplines
+        """
+        lang = {
+            "en": "displayNameEn",
+            "de": "displayNameDe"
+        }[self.client.settings.language]
+        return [k[lang] for k in self.data["disciplines"]]
+
+    @property
+    def organizations(self) -> List[str]:
+        """
+        Project Associated Organizations
+        """
+        return [k["displayName"] for k in self.data["organizations"]]
+
+    @property
+    def visibility(self) -> str:
+        """
+        Project Visibility in Coscine
+        """
+        return self.data["visibility"]["displayName"]
+
+###############################################################################
+
+    def __str__(self) -> str:
+        table = PrettyTable(("Property", "Value"))
+        rows = [
+            ("ID", self.id),
+            ("Name", self.name),
+            ("Display Name", self.display_name),
+            ("Description", self.description),
+            ("Principle Investigators", self.principle_investigators),
+            ("Disciplines", "\n".join(self.disciplines)),
+            ("Organizations", "\n".join(self.organizations)),
+            ("Start Date", self.start_date),
+            ("End Date", self.end_date),
+            ("Visibility", self.visibility)
+        ]
+        table.max_width["Value"] = 50
+        table.add_rows(rows)
+        return table.get_string(title=f"Project {self.display_name}")
+
+###############################################################################
+
+    def subprojects(self) -> List[Project]:
+        """
+        Retrieves a list of a all projects the creator of the Coscine API token
+        is currently a member of.
+
+        Returns
+        -------
+        list
+            List of coscine.Project objects
+        """
+
+        uri = self.client.uri("Project", "SubProject", self.id)
+        projects = []
+        for data in self.client.get(uri).json():
+            projects.append(Project(self.client, data, self))
+        return projects
+
+###############################################################################
+
+    def subproject(self, display_name: str) -> Optional[Project]:
+        """
+        Returns a single subproject via its displayName
+
+        Parameters
+        ----------
+        display_name : str
+            Look for a project with the specified displayName
+
+        Returns
+        -------
+        Project
+            A single coscine project handle or None if no match found
+
+        Raises
+        ------
+        IndexError
+        """
+
+        filtered_project_list = list(filter(
+            lambda project: project.display_name == display_name,
+            self.subprojects()
+        ))
+        if len(filtered_project_list) == 1:
+            return filtered_project_list[0]
+        if len(filtered_project_list) == 0:
+            return None
+        raise IndexError("Too many projects matching the specified criteria!")
+
+###############################################################################
+
+    def create_subproject(self, form: ProjectForm) -> Project:
+        """
+        Creates a subproject inside of the current project
+        """
+        metadata = form.generate()
+        metadata["ParentId"] = self.id
+        return self.client.create_project(metadata)
+
+###############################################################################
+
+    def delete(self) -> None:
+        """
+        Deletes the project on the Coscine servers.
+        """
+
+        uri = self.client.uri("Project", "Project", self.id)
+        self.client.delete(uri)
+
+###############################################################################
+
+    def resources(self) -> List[Resource]:
+        """
+        Retrieves a list of Resources of the current project.
+
+        Returns
+        -------
+        list[Resource]
+            list of resources matching the supplied filter.
+        """
+
+        uri = self.client.uri("Project", "Project", self.id, "resources")
+        resources = []
+        for data in self.client.get(uri).json():
+            resources.append(Resource(self, data))
+        return resources
+
+###############################################################################
+
+    def resource(self, display_name: str) -> Resource:
+        """
+        Retrieves a certain resource of the current project
+        identified by its displayName.
+
+        Parameters
+        ----------
+        display_name : str
+            The display name of the resource.
+
+        Returns
+        --------
+        A single Coscine Resource handle
+
+        Raises
+        -------
+        IndexError
+        FileNotFoundError
+            In case no resource with the specified display_name was found.
+        """
+
+        resources = list(filter(
+            lambda resource: resource.display_name == display_name,
+            self.resources()
+        ))
+        if len(resources) == 1:
+            return resources[0]
+        if len(resources) == 0:
+            raise FileNotFoundError("Could not find resource!")
+        raise IndexError("Too many resources matching the specified criteria!")
+
+###############################################################################
+
+    def download(self, path: str = "./", metadata: bool = False) -> None:
+        """
+        Downloads the project to the location referenced by 'path'.
+
+        Parameters
+        ----------
+        path : str
+            Download location on the harddrive
+            Default: current directory './'
+        metadata : bool, default: False
+            If enabled, project metadata is downloaded and put in
+            a hidden file '.metadata.json'.
+        """
+
+        logger.info("Downloading project '%s' (%s)...", self.name, self.id)
+        path = os.path.join(path, self.display_name)
+        if not os.path.isdir(path):
+            os.mkdir(path)
+        for resource in self.resources():
+            resource.download(path=path, metadata=metadata)
+        if metadata:
+            data = json.dumps(self.data, indent=4)
+            metadata_path: str = os.path.join(path, ".metadata.json")
+            with open(metadata_path, "w", encoding="utf-8") as file:
+                file.write(data)
+
+###############################################################################
+
+    def members(self) -> List[ProjectMember]:
+        """
+        Retrieves a list of all members of the current project
+
+        Returns
+        --------
+        list[ProjectMember]
+            List of project members as ProjectMember objects.
+        """
+
+        uri = self.client.uri("Project", "ProjectRole", self.id)
+        data = self.client.get(uri).json()
+        members = [ProjectMember(self, m) for m in data]
+        return members
+
+###############################################################################
+
+    @parallelizable
+    def invite(self, email: str, role: str = "Member") -> None:
+        """
+        Invites a person to a project via their email address
+
+        Parameters
+        ----------
+        email : str
+            The email address to send the invite to
+        role : str, "Member", "Guest" or "Owner", default: "Member"
+            The role for the new project member
+        """
+
+        if role not in ProjectMember.ROLES:
+            raise ValueError(f"Invalid role {role}.")
+
+        logger.info("Inviting %s as %s to project %s.", email, role, self.name)
+        uri = self.client.uri("Project", "Project", "invitation")
+        data = {
+            "projectId": self.data["id"],
+            "role": ProjectMember.ROLES[role],
+            "email": email
+        }
+
+        try:
+            self.client.post(uri, json=data)
+        except RuntimeError:
+            logger.warning("User %s has pending invites.", email)
+
+###############################################################################
+
+    @parallelizable
+    def add_member(self, member: ProjectMember, role: str = "Member"):
+        """
+        Adds a project member of another project to the current project.
+
+        Parameters
+        ----------
+        member : ProjectMember
+            Member of another Coscine project
+        role : str, "Member", "Guest" or "Owner", default: "Member"
+
+        Raises
+        ------
+        ValueError
+            In case the specified role is unsupported
+        """
+
+        if role not in ProjectMember.ROLES:
+            raise ValueError(f"Invalid role for member '{member.name}'!")
+        data = member.data
+        data["projectId"] = self.id
+        data["role"]["displayName"] = role
+        data["role"]["id"] = ProjectMember.ROLES[role]
+        uri = self.client.uri("Project", "ProjectRole")
+        self.client.post(uri, json=data)
+        logger.info(
+            "Added '%s' as a project member with "
+            "role '%s' to project '%s'.",
+            member.name, role, self.name
+        )
+
+###############################################################################
+
+    def form(self) -> ProjectForm:
+        """
+        Returns the project metadata form of the project. That form can
+        then be used to edit the project metadata.
+
+        Examples
+        ---------
+        >>> metadata = Project.form()
+        >>> metadata["Display Name"] = "Different display name"
+        >>> Project.update(metadata)
+        """
+
+        form = ProjectForm(self.client)
+        form.parse(self.data)
+        return form
+
+###############################################################################
+
+    def update(self, form: Union[ProjectForm, dict]) -> Project:
+        """
+        Updates a project using the given ProjectForm
+
+        Parameters
+        ----------
+        form : ProjectForm or dict
+            ProjectForm containing updated data or dict generated from a form.
+        """
+
+        if isinstance(form, ProjectForm):
+            form = form.generate()
+        uri = self.client.uri("Project", "Project", self.id)
+        response = self.client.post(uri, json=form)
+        logger.info(
+            "Updated project metadata for '%s' (%s).",
+            self.name, self.id
+        )
+        updated_project_handle = self
+        if response.ok:
+            # Update project properties
+            # The response unfortunately does not return
+            # the new project data - bummer!
+            updated_project_handle = list(filter(
+                lambda p: p.id == self.id,
+                self.client.projects(False)
+            ))[0]
+        return updated_project_handle
+
+###############################################################################
+
+    @parallelizable
+    def create_resource(self, form: Union[ResourceForm, dict]) -> Resource:
+        """
+        Creates a resource within the current project using the supplied
+        resource form.
+
+        Parameters
+        ----------
+        resourceForm : ResourceForm
+            Form to generate the resource with.
+        metadataPreset : MetadataPresetForm
+            optional application profile configuration.
+            Currently not supported.
+        """
+        if isinstance(form, ResourceForm):
+            form = form.generate()
+        uri = self.client.uri("Resources", "Resource", "project", self.id)
+        logger.info("Creating resource in project '%s'.", self.name)
+        return Resource(self, self.client.post(uri, json=form).json())
+
+###############################################################################
+###############################################################################
+
+class ProjectMember:
+    """
+    Python representation of a Coscine project member.
+    """
+
+    ROLES = {
+        "Owner": "be294c5e-4e42-49b3-bec4-4b15f49df9a5",
+        "Member": "508b6d4e-c6ac-4aa5-8a8d-caa31dd39527",
+        "Guest": "9184a442-4419-4e30-9fe6-0cfe32c9a81f"
+    }
+
+    data: dict
+    client: Client
+    project: Project
+
+###############################################################################
+
+    @property
+    def name(self) -> str:
+        """Name of the Project Member"""
+        return self.data["user"]["displayName"]
+
+    @property
+    def email(self) -> str:
+        """E-Mail address of the Project Member"""
+        return self.data["user"]["emailAddress"]
+
+    @property
+    def id(self) -> str:
+        """Project Member ID"""
+        return self.data["user"]["id"]
+
+    @property
+    def role(self) -> str:
+        """Role of the Project Member within the Project"""
+        return self.data["role"]["displayName"]
+
+###############################################################################
+
+    def __init__(self, project: Project, data: dict) -> None:
+        """
+        Initializes a project member for a given project.
+
+        Parameters
+        ----------
+        project : Project
+            Coscine Python SDK project handle.
+        data: dict
+            User data as dict, retrieved via
+            client.uri("Project", "ProjectRole", self.id).
+        """
+
+        self.project = project
+        self.client = self.project.client
+        self.data = data
+
+###############################################################################
+
+    @parallelizable
+    def set_role(self, role: str) -> None:
+        """
+        Sets the role of a project member
+
+        Parameters
+        ----------
+        role : str
+            The new role of the member ('Owner', 'Guest' or 'Member').
+        """
+
+        if role not in ProjectMember.ROLES:
+            raise ValueError(f"Invalid role {role}.")
+
+        uri = self.client.uri("Project", "ProjectRole")
+        self.data["role"]["id"] = ProjectMember.ROLES[role]
+        self.data["role"]["displayName"] = role
+        logger.info("Setting role of '%s' to '%s'...", self.name, role)
+        self.client.post(uri, json=self.data)
+
+###############################################################################
+
+    @parallelizable
+    def remove(self) -> None:
+        """
+        Removes a project member from their associated project.
+        """
+
+        uri = self.client.uri(
+            "Project", "ProjectRole", "project", self.project.id, "user",
+            self.id, "role", self.data["role"]["id"]
+        )
+        logger.info(
+            "Removing member '%s' from project '%s'...",
+            self.name, self.project.name
+        )
+        self.client.delete(uri)
+
+###############################################################################
```

### Comparing `coscine-0.9.0/src/coscine/resource.py` & `coscine-0.9.1/src/coscine/resource.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,738 +1,752 @@
-###############################################################################
-# Coscine Python SDK
-# Copyright (c) 2018-2023 RWTH Aachen University
-# Licensed under the terms of the MIT License
-###############################################################################
-# Coscine, short for Collaborative Scientific Integration Environment, is
-# a platform for research data management (RDM).
-# For more information on Coscine visit https://www.coscine.de/.
-#
-# Please note that this python module is open source software primarily
-# developed and maintained by the scientific community. It is not
-# an official service that RWTH Aachen provides support for.
-###############################################################################
-
-###############################################################################
-# File description
-###############################################################################
-
-"""
-This file defines the resource object for the representation of
-Coscine resources. It provides an easy interface to interact with Coscine
-resources from python.
-"""
-
-###############################################################################
-# Dependencies
-###############################################################################
-
-from __future__ import annotations
-import json
-import os
-import posixpath
-import logging
-from typing import Callable, TYPE_CHECKING, Union, List, Optional
-import urllib.parse
-import csv
-from requests_toolbelt import MultipartEncoder, MultipartEncoderMonitor
-from prettytable.prettytable import PrettyTable
-import rdflib
-try:
-    import pandas
-except ImportError:
-    pandas = None
-from coscine.object import FileObject, MetadataForm
-from coscine.form import InputForm
-from coscine.graph import ApplicationProfile
-from coscine.utils import ProgressBar, parallelizable, concurrent
-from coscine.s3 import S3
-if TYPE_CHECKING:
-    from coscine.client import Client
-    from coscine.project import Project
-
-###############################################################################
-# Module globals / Constants
-###############################################################################
-
-logger = logging.getLogger(__name__)
-
-###############################################################################
-# Classes / Functions / Scripts
-###############################################################################
-
-class ResourceForm(InputForm):
-    """
-    An InputForm for Coscine Resource metadata.
-    """
-
-###############################################################################
-
-    def __init__(self, client: Client) -> None:
-        """
-        Parameters
-        -----------
-        client : Client
-            Coscine Python SDK Client instance
-        """
-        super().__init__(client)
-        self._fields = client.vocabularies.builtin("resource")
-        vocabularies = {
-            "type": client.vocabularies.resource_types(True),
-            "applicationProfile":
-                client.vocabularies.application_profiles(True),
-            "license": client.vocabularies.licenses(True),
-            "visibility": client.vocabularies.visibility(True),
-            "disciplines": client.vocabularies.disciplines(True)
-        }
-        for item in self._fields:
-            if item.vocabulary:
-                self._vocabularies[item.path] = vocabularies[item.path]
-
-###############################################################################
-
-    def parse(self, data: dict) -> None:
-        ignore = ["id", "pid", "fixedValues", "creator", "archived"]
-        for path, value in data.items():
-            if path not in ignore:
-                try:
-                    key = self.name_of(path)
-                    self.set_value(key, value, True)
-                except KeyError:
-                    continue
-
-###############################################################################
-
-    def generate(self) -> dict:
-        metadata = {}
-
-        # Collect missing required fields
-        missing: List[str] = []
-
-        # Set metadata
-        for key, value in self.items():
-            if value is None:
-                if self.is_required(key):
-                    missing.append(key)
-                continue
-
-            properties = self.properties(key)
-            metadata[properties.path] = value.raw()
-            # The resourceTypeOption requires a dict with additional
-            # 'Size' field in it.
-            if properties.path == "resourceTypeOption":
-                metadata[properties.path] = {
-                    "Size": value.raw()
-                }
-
-        # Check for missing required fields
-        if len(missing) > 0:
-            if not (
-                len(missing) == 1
-                and missing[0] == "resourceTypeOption"
-                and metadata["type"] == "linked"
-            ):
-                raise ValueError(missing)
-
-        return metadata
-
-###############################################################################
-###############################################################################
-###############################################################################
-
-class Resource:
-    """
-    Python representation of a Coscine Resource type.
-    """
-
-    client: Client
-    project: Project
-    data: dict
-    s3: Optional[S3]
-
-###############################################################################
-
-    def __init__(self, project: Project, data: dict) -> None:
-        """
-        Initializes a Coscine resource object.
-
-        Parameters
-        ----------
-        project : Project
-            Coscine project handle
-        data : dict
-            Resource data received from Coscine.
-        """
-
-        self.project = project
-        self.client = self.project.client
-        self.data = data
-        self.s3 = S3(data, self.client.settings.verbose)
-
-###############################################################################
-
-    @property
-    def id(self) -> str:
-        """Resource ID"""
-        return self.data["id"]
-
-    @property
-    def pid(self) -> str:
-        """Resource Persistent Identifier"""
-        return self.data["pid"]
-
-    @property
-    def name(self) -> str:
-        """Resource Name"""
-        return self.data["resourceName"]
-
-    @property
-    def display_name(self) -> str:
-        """Resource Display Name"""
-        return self.data["displayName"]
-
-    @property
-    def description(self) -> str:
-        """Resource Description"""
-        return self.data["description"]
-
-    @property
-    def license(self) -> str:
-        """Resource License Name"""
-        return (
-            self.data["license"]["displayName"] if self.data["license"] else ""
-        )
-
-    @property
-    def type(self) -> str:
-        """Resource Type e.g. rdss3rwth"""
-        return self.data["type"]["displayName"]
-
-    @property
-    def disciplines(self) -> List[str]:
-        """Associated Disciplines"""
-        lang = {
-            "en": "displayNameEn",
-            "de": "displayNameDe"
-        }[self.client.settings.language]
-        return [k[lang] for k in self.data["disciplines"]]
-
-    @property
-    def profile(self) -> str:
-        """Name of the Application Profile used in the Resource"""
-        return self.data["applicationProfile"]
-
-    @property
-    def archived(self) -> bool:
-        """Status indicator, indicating whether the resource is archived"""
-        return bool(self.data["archived"])
-
-    @property
-    def creator(self) -> str:
-        """Resource Creator"""
-        return self.data["creator"]
-
-###############################################################################
-
-    def __str__(self) -> str:
-        table = PrettyTable(["Property", "Value"])
-        rows = [
-            ("ID", self.id),
-            ("Resource Name", self.name),
-            ("Display Name", self.display_name),
-            ("Description", self.description),
-            ("PID", self.pid),
-            ("Type", self.type),
-            ("Disciplines", "\n".join(self.disciplines)),
-            ("License", self.license),
-            ("Application Profile", self.profile),
-            ("Archived", self.archived),
-            ("Creator", self.creator),
-            ("Project", self.project.display_name),
-            ("Project ID", self.project.id)
-        ]
-        table.max_width["Value"] = 50
-        table.add_rows(rows)
-        return table.get_string(title=f"Resource {self.display_name}")
-
-###############################################################################
-
-    @parallelizable
-    def delete(self) -> None:
-        """
-        Deletes the Coscine resource and all objects contained within it on
-        the Coscine servers.
-        """
-
-        logger.info("Deleting resource '%s' (%s)...", self.name, self.id)
-        uri = self.client.uri("Resources", "Resource", self.id)
-        self.client.delete(uri)
-
-###############################################################################
-
-    def application_profile(self) -> ApplicationProfile:
-        """
-        Returns the application profile of the resource.
-        """
-
-        return self.client.vocabularies.application_profile(self.profile)
-
-###############################################################################
-
-    def download_metadata(self, path: str = "./", format: str = "csv") -> None:
-        """
-        Downloads the metadata of the file objects stored within the resource
-        in the specified format.
-
-        Parameters
-        ----------
-        format : str, default: "csv"
-            The file format to store the data in. Available formats are:
-            "json", "csv"
-
-        Raises
-        -------
-        ValueError
-            In case of an unexpected format.
-        """
-
-        if format == "csv":
-            with open(
-                os.path.join(path, ".file-metadata.csv"),
-                "w", encoding="utf-8", newline=""
-            ) as file_handle:
-                csvwriter = csv.writer(file_handle)
-                csvwriter.writerow(["File"] + self.metadata_form().keys())
-                for obj in self.contents():
-                    values = [obj.path] + [
-                        str(value) for value in obj.form().values()
-                    ]
-                    csvwriter.writerow(values)
-        elif format == "json":
-            metadata = []
-            keys = ["File"] + self.metadata_form().keys()
-            for obj in self.contents():
-                values = [obj.path] + [
-                    str(value) for value in obj.form().values()
-                ]
-                entry = {
-                    keys[i]: values[i] for i in range(len(keys))
-                }
-                metadata.append(entry)
-            with open(
-                os.path.join(path, ".file-metadata.json"),
-                "w", encoding="utf-8"
-            ) as file_handle:
-                json.dump(metadata, file_handle)
-        else:
-            raise ValueError("Unexpected metadata format!")
-
-###############################################################################
-
-    def download(self, path: str = "./", metadata: bool = False) -> None:
-        """
-        Downloads the resource and all of its contents to the local harddrive.
-
-        Parameters
-        ----------
-        path : str, default: "./"
-            Path to the local storage location.
-        metadata : bool, default: False
-            If enabled, resource metadata is downloaded and put in
-            the file '.resource-metadata.json'.
-        """
-
-        logger.info("Downloading resource '%s' (%s)...", self.name, self.id)
-        path = os.path.join(path, self.name)
-        if not os.path.isdir(path):
-            os.mkdir(path)
-        if self.client.settings.concurrent:
-            with concurrent():
-                for obj in self.contents():
-                    obj.download(path, preserve_path=True)
-        else:
-            for obj in self.contents():
-                obj.download(path, preserve_path=True)
-        if metadata:
-            self.download_metadata(path)
-            data = json.dumps(self.data, indent=4)
-            metadata_path: str = os.path.join(path, ".resource-metadata.json")
-            with open(metadata_path, "w", encoding="utf-8") as file:
-                file.write(data)
-
-###############################################################################
-
-    def exists(self, path: str) -> bool:
-        """
-        Returns whether the file referenced by key is contained
-        in the resource.
-
-        Parameters
-        -----------
-        path : str
-            The key/path to the file object
-
-        Returns
-        -------
-        bool
-            True if file object exists, False if not
-        """
-        return self.object(path) is not None
-
-###############################################################################
-
-    def contents(self) -> List[FileObject]:
-        """
-        Returns a list of ALL Objects stored within the resource
-        by recursively traversing directories
-
-        Returns
-        -------
-        List[FileObject]
-            List of Coscine file-like objects.
-        """
-
-        more_folders: bool = True
-        contents = []
-        directories = []
-        files = self.objects()
-        while more_folders:
-            more_folders = False
-            for obj in files:
-                if obj.is_folder:
-                    files.remove(obj)
-                    directories.append(obj)
-                    files.extend(obj.objects())
-                    more_folders = True
-        contents.extend(directories)
-        contents.extend(files)
-        return contents
-
-###############################################################################
-
-    def objects(self, path: Optional[str] = None) -> List[FileObject]:
-        """
-        Returns a list of Objects stored within the resource.
-
-        Parameters
-        ------------
-        path : str, default: None
-            Path to a directory. Irrelevant for anything other than S3.
-
-        Examples
-        ---------
-        >>> Resource.objects(path="Folder/Subfolder")
-        Returns all objects inside 'Folder/Subfolder' (s3 resources only)
-
-        Returns
-        -------
-        List[FileObject]
-            List of Coscine file-like objects.
-        """
-
-        objects = []
-        uri = self.client.uri("Tree", "Tree", self.id)
-        dirpath = posixpath.dirname(path) if path else None
-        args = {"path": path} if dirpath and dirpath != "/" else None
-        data = self.client.get(uri, params=args).json()
-        file_storage: List[dict] = data["data"]["fileStorage"]
-        metadata_storage: List[dict] = data["data"]["metadataStorage"]
-        for data in file_storage:
-            path = urllib.parse.quote("/" + data["Path"], safe="")
-            metadata: dict = {}
-            for meta in metadata_storage:
-                if list(meta.keys())[0].endswith(f"@path={path}"):
-                    metadata = meta
-                    break
-            objects.append(FileObject(self, data, metadata))
-        return objects
-
-###############################################################################
-
-    def object(self, path: str) -> Union[FileObject, None]:
-        """
-        Returns an Object stored within the resource
-
-        Parameters
-        ------------
-        path : str, default: None
-            Path to a directory. Irrelevant for anything other than S3.
-
-        Examples
-        ---------
-        >>> Resource.object(path="Folder/Subfolder/Filename.jpg")
-        Returns the file inside 'Folder/Subfolder' (s3 resources only)
-
-        Returns
-        -------
-        FileObject
-            Python representation of the file-object as an Object instance
-        None
-            In case nothing was found.
-
-        Raises
-        ------
-        IndexError
-            In case more than 1 FileObject was found at the path.
-        """
-
-        dirpath = posixpath.join(posixpath.dirname(path), "")
-        dirpath = dirpath if dirpath != "/" else ""
-        filename = posixpath.basename(path)
-        if not filename:
-            filename = posixpath.dirname(dirpath)
-            dirpath = ""
-        filtered_list = list(filter(lambda fo: fo.name == filename,
-                                    self.objects(path=dirpath)))
-        if len(filtered_list) == 1:
-            return filtered_list[0]
-        if len(filtered_list) == 0:
-            return None
-        raise IndexError("Too many files matching the specified criteria!")
-
-###############################################################################
-
-    def upload(
-        self,
-        key: str,
-        file,
-        metadata: Union[MetadataForm, dict],
-        callback: Optional[Callable[[int], None]] = None
-    ) -> None:
-        """
-        Uploads a file-like object to a resource on the Coscine server
-
-        Parameters
-        ----------
-        key : str
-            filename of the file-like object.
-        file : object with read() attribute
-            Either open file handle or local file location path.
-        metadata : MetadataForm or dict
-            File metadata matching the resource application profile.
-        callback : Callable[[int], None], default: None
-            Optional callback called during chunk uploads
-            indicating the progress.
-
-        Raises
-        ------
-        TypeError
-            In case the file object specified cannot be used.
-        """
-
-        logger.info(
-            "Uploading FileObject '%s' to resource '%s' (%s)...",
-            key, self.name, self.id
-        )
-        if hasattr(file, "read"):
-            self._upload_file_metadata(key, metadata)
-            self._upload_file_data(key, file, callback)
-        elif isinstance(file, str):
-            with open(file, "rb") as file_handle:
-                self._upload_file_metadata(key, metadata)
-                self._upload_file_data(key, file_handle, callback)
-        else:
-            raise TypeError("Argument `file` has unexpected type!")
-
-###############################################################################
-
-    def _upload_file_metadata(self, key: str, metadata) -> None:
-        if isinstance(metadata, MetadataForm):
-            metadata = metadata.generate()
-        uri = self.client.uri("Tree", "Tree", self.id)
-        params = {"path": key}
-        self.client.put(uri, json=metadata, params=params)
-
-###############################################################################
-
-    def _upload_file_data(
-        self,
-        key: str,
-        file_handle,
-        callback: Optional[Callable[[int], None]] = None
-    ) -> None:
-        uri = self.client.uri("Blob", "Blob", self.id)
-        fields = {"files": (key, file_handle, "application/octect-stream")}
-        encoder = MultipartEncoder(fields=fields)
-        progress_bar = ProgressBar(
-            self.client.settings.verbose, encoder.len, key, callback
-        )
-        monitor = MultipartEncoderMonitor(
-            encoder,
-            callback=lambda monitor:
-                progress_bar.update(monitor.bytes_read - progress_bar.count)
-        )
-        headers = {"Content-Type": monitor.content_type}
-        params = {"path": key}
-        self.client.put(uri, data=monitor, headers=headers, params=params)
-
-###############################################################################
-
-    @parallelizable
-    def set_archived(self, flag: bool) -> None:
-        """
-        Set the archived flag of the resource to put it in read-only mode.
-        Only the resource creator or project owner can do this.
-
-        Parameters
-        ----------
-        flag : bool
-            Enable with True, Disable with False.
-        """
-
-        uri = self.client.uri(
-            "Resources", "Resource", self.id,
-            f"setReadonly?status={str(flag).lower()}"
-        )
-        logger.info(
-            "Setting resource '%s' read only flag = %d",
-            self.name, flag
-        )
-        self.client.post(uri)
-        self.data["archived"] = flag
-
-###############################################################################
-
-    def form(self) -> ResourceForm:
-        """
-        Returns a ResourceForm filled with the metadata of
-        the current resource.
-
-        Returns
-        -------
-        ResourceForm
-        """
-
-        form = self.client.resource_form()
-        form.parse(self.data)
-        return form
-
-###############################################################################
-
-    def update(self, form: Union[ResourceForm, dict]) -> Resource:
-        """
-        Updates the metadata of the resource using the supplied ResourceForm.
-
-        Parameters
-        ----------
-        form : ResourceForm or dict
-            ResourceForm filled with updated values
-            or generated form data dict.
-
-        Returns
-        -------
-        Resource
-            A new resource object with updated resource metadata
-        """
-
-        if isinstance(form, ResourceForm):
-            form = form.generate()
-        elif not isinstance(form, dict):
-            raise TypeError("Resource metadata form has unexpected type.")
-
-        logger.info("Updating resource metadata of resource '%s'.", self.name)
-        uri = self.client.uri("Resources", "Resource", self.id)
-        response = self.client.post(uri, json=form)
-        updated_resource_handle = self
-        if response.ok:
-            # Update resource properties:
-            # The response unfortunately does not return the new resource data
-            updated_resource_handle = list(
-                filter(lambda r: r.id == self.id, self.project.resources())
-            )[0]
-        return updated_resource_handle
-
-###############################################################################
-
-    def metadata_form(self, data: Optional[dict] = None) -> MetadataForm:
-        """
-        Creates a MetadataForm for this resource
-
-        Parameters
-        ----------
-        data : dict, default: None
-            If data is specified, the form is initialized with that data
-            using the InputForm.fill() method.
-        """
-
-        form = MetadataForm(self.client, self.application_profile())
-        if data:
-            form.fill(data)
-        return form
-
-###############################################################################
-
-    def dataframe(self):
-        """
-        Creates a pandas dataframe from resource metadata.
-        Requires an installation of the pandas package.
-
-        Returns
-        -------
-        pandas.DataFrame
-        """
-
-        if not pandas:
-            raise ModuleNotFoundError("Method requires package 'pandas'!")
-        form = self.metadata_form()
-        headers = ["Path"] + form.keys()
-        values = [
-            [obj.path] + obj.form().values() for obj in self.objects()
-        ]
-        return pandas.DataFrame(values, columns=headers)
-
-###############################################################################
-
-    def graph(self) -> Optional[rdflib.Graph]:
-        """
-        Create an rdflib graph from the resource contents.
-        The rdflib graph can be queried with SPARQL, merged with the graphs
-        from other resources and serialized into various formats such
-        as xml or dot (for rendering it as a graph).
-
-        Parameters
-        ----------
-        literal : bool, default: False
-            If enabled, the literal values as seen in the MetadataForm
-            are used for the triples in the graph (the human
-            readable values instead of the URIs).
-
-        Returns
-        --------
-        rdflib.Graph
-        """
-
-        #######################################################################
-
-        def add_to_graph(graph: rdflib.Graph, file: FileObject):
-            """Adds the FileObject to the rdflib graph"""
-            metadata = file.metadata()
-            if metadata:
-                file_reference = rdflib.URIRef(
-                    file.name,
-                    "https://purl.org/coscine/file/"
-                )
-                for key, values in metadata.items():
-                    for value in values:
-                        graph.add((
-                            file_reference,
-                            rdflib.URIRef(key),
-                            rdflib.Literal(value["value"])
-                        ))
-
-        #######################################################################
-
-        file_objects = self.objects()
-        logger.info("Constructing graph for resource %s...", self.display_name)
-        pbar = ProgressBar(
-            self.client.settings.verbose,
-            len(file_objects),
-            f"Creating rdf graph for '{self.display_name}'"
-        )
-        graph = rdflib.Graph()
-        for file in file_objects:
-            pbar.update(1)
-            if file.has_metadata:
-                add_to_graph(graph, file)
-        return graph
-
-###############################################################################
+###############################################################################
+# Coscine Python SDK
+# Copyright (c) 2018-2023 RWTH Aachen University
+# Licensed under the terms of the MIT License
+###############################################################################
+# Coscine, short for Collaborative Scientific Integration Environment, is
+# a platform for research data management (RDM).
+# For more information on Coscine visit https://www.coscine.de/.
+#
+# Please note that this python module is open source software primarily
+# developed and maintained by the scientific community. It is not
+# an official service that RWTH Aachen provides support for.
+###############################################################################
+
+###############################################################################
+# File description
+###############################################################################
+
+"""
+This file defines the resource object for the representation of
+Coscine resources. It provides an easy interface to interact with Coscine
+resources from python.
+"""
+
+###############################################################################
+# Dependencies
+###############################################################################
+
+from __future__ import annotations
+import json
+import os
+import posixpath
+import logging
+from typing import Callable, TYPE_CHECKING, Union, List, Optional
+import csv
+from requests_toolbelt import MultipartEncoder, MultipartEncoderMonitor
+from prettytable.prettytable import PrettyTable
+from urllib.parse import quote
+import rdflib
+try:
+    import pandas
+except ImportError:
+    pandas = None
+from coscine.object import FileObject, MetadataForm
+from coscine.form import InputForm
+from coscine.graph import ApplicationProfile
+from coscine.utils import ProgressBar, parallelizable, concurrent
+from coscine.s3 import S3
+if TYPE_CHECKING:
+    from coscine.client import Client
+    from coscine.project import Project
+
+###############################################################################
+# Module globals / Constants
+###############################################################################
+
+logger = logging.getLogger(__name__)
+
+###############################################################################
+# Classes / Functions / Scripts
+###############################################################################
+
+class ResourceForm(InputForm):
+    """
+    An InputForm for Coscine Resource metadata.
+    """
+
+###############################################################################
+
+    def __init__(self, client: Client) -> None:
+        """
+        Parameters
+        -----------
+        client : Client
+            Coscine Python SDK Client instance
+        """
+        super().__init__(client)
+        self._fields = client.vocabularies.builtin("resource")
+        vocabularies = {
+            "type": client.vocabularies.resource_types(True),
+            "applicationProfile":
+                client.vocabularies.application_profiles(True),
+            "license": client.vocabularies.licenses(True),
+            "visibility": client.vocabularies.visibility(True),
+            "disciplines": client.vocabularies.disciplines(True)
+        }
+        for item in self._fields:
+            if item.vocabulary:
+                self._vocabularies[item.path] = vocabularies[item.path]
+
+###############################################################################
+
+    def parse(self, data: dict) -> None:
+        ignore = ["id", "pid", "fixedValues", "creator", "archived"]
+        for path, value in data.items():
+            if path not in ignore:
+                try:
+                    key = self.name_of(path)
+                    self.set_value(key, value, True)
+                except KeyError:
+                    continue
+
+###############################################################################
+
+    def generate(self) -> dict:
+        metadata = {}
+
+        # Collect missing required fields
+        missing: List[str] = []
+
+        # Set metadata
+        for key, value in self.items():
+            if value is None:
+                if self.is_required(key):
+                    missing.append(key)
+                continue
+
+            properties = self.properties(key)
+            metadata[properties.path] = value.raw()
+            # The resourceTypeOption requires a dict with additional
+            # 'Size' field in it.
+            if properties.path == "resourceTypeOption":
+                metadata[properties.path] = {
+                    "Size": value.raw()
+                }
+
+        # Check for missing required fields
+        if len(missing) > 0:
+            if not (
+                len(missing) == 1
+                and missing[0] == "resourceTypeOption"
+                and metadata["type"] == "linked"
+            ):
+                raise ValueError(missing)
+
+        return metadata
+
+###############################################################################
+###############################################################################
+###############################################################################
+
+class Resource:
+    """
+    Python representation of a Coscine Resource type.
+    """
+
+    client: Client
+    project: Project
+    data: dict
+    s3: Optional[S3]
+
+###############################################################################
+
+    def __init__(self, project: Project, data: dict) -> None:
+        """
+        Initializes a Coscine resource object.
+
+        Parameters
+        ----------
+        project : Project
+            Coscine project handle
+        data : dict
+            Resource data received from Coscine.
+        """
+
+        self.project = project
+        self.client = self.project.client
+        self.data = data
+        self.s3 = S3(data, self.client.settings.verbose)
+
+###############################################################################
+
+    @property
+    def id(self) -> str:
+        """Resource ID"""
+        return self.data["id"]
+
+    @property
+    def pid(self) -> str:
+        """Resource Persistent Identifier"""
+        return self.data["pid"]
+
+    @property
+    def access_url(self) -> str:
+        """Resource Access URL via PID"""
+        return f"http://hdl.handle.net/{self.pid}"
+
+    @property
+    def name(self) -> str:
+        """Resource Name"""
+        return self.data["resourceName"]
+
+    @property
+    def display_name(self) -> str:
+        """Resource Display Name"""
+        return self.data["displayName"]
+
+    @property
+    def description(self) -> str:
+        """Resource Description"""
+        return self.data["description"]
+
+    @property
+    def license(self) -> str:
+        """Resource License Name"""
+        return (
+            self.data["license"]["displayName"] if self.data["license"] else ""
+        )
+
+    @property
+    def type(self) -> str:
+        """Resource Type e.g. rdss3rwth"""
+        return self.data["type"]["displayName"]
+
+    @property
+    def disciplines(self) -> List[str]:
+        """Associated Disciplines"""
+        lang = {
+            "en": "displayNameEn",
+            "de": "displayNameDe"
+        }[self.client.settings.language]
+        return [k[lang] for k in self.data["disciplines"]]
+
+    @property
+    def profile(self) -> str:
+        """Name of the Application Profile used in the Resource"""
+        return self.data["applicationProfile"]
+
+    @property
+    def archived(self) -> bool:
+        """Status indicator, indicating whether the resource is archived"""
+        return bool(self.data["archived"])
+
+    @property
+    def creator(self) -> str:
+        """Resource Creator"""
+        return self.data["creator"]
+
+###############################################################################
+
+    def __str__(self) -> str:
+        table = PrettyTable(["Property", "Value"])
+        rows = [
+            ("ID", self.id),
+            ("Resource Name", self.name),
+            ("Display Name", self.display_name),
+            ("Description", self.description),
+            ("PID", self.pid),
+            ("Type", self.type),
+            ("Disciplines", "\n".join(self.disciplines)),
+            ("License", self.license),
+            ("Application Profile", self.profile),
+            ("Archived", self.archived),
+            ("Creator", self.creator),
+            ("Project", self.project.display_name),
+            ("Project ID", self.project.id)
+        ]
+        table.max_width["Value"] = 50
+        table.add_rows(rows)
+        return table.get_string(title=f"Resource {self.display_name}")
+
+###############################################################################
+
+    @parallelizable
+    def delete(self) -> None:
+        """
+        Deletes the Coscine resource and all objects contained within it on
+        the Coscine servers.
+        """
+
+        logger.info("Deleting resource '%s' (%s)...", self.name, self.id)
+        uri = self.client.uri("Resources", "Resource", self.id)
+        self.client.delete(uri)
+
+###############################################################################
+
+    def application_profile(self) -> ApplicationProfile:
+        """
+        Returns the application profile of the resource.
+        """
+
+        return self.client.vocabularies.application_profile(self.profile)
+
+###############################################################################
+
+    def download_metadata(self, path: str = "./", format: str = "csv") -> None:
+        """
+        Downloads the metadata of the file objects stored within the resource
+        in the specified format.
+
+        Parameters
+        ----------
+        format : str, default: "csv"
+            The file format to store the data in. Available formats are:
+            "json", "csv"
+
+        Raises
+        -------
+        ValueError
+            In case of an unexpected format.
+        """
+
+        if format == "csv":
+            with open(
+                os.path.join(path, ".file-metadata.csv"),
+                "w", encoding="utf-8", newline=""
+            ) as file_handle:
+                csvwriter = csv.writer(file_handle)
+                csvwriter.writerow(["File"] + self.metadata_form().keys())
+                for obj in self.contents():
+                    values = [obj.path] + [
+                        str(value) for value in obj.form().values()
+                    ]
+                    csvwriter.writerow(values)
+        elif format == "json":
+            metadata = []
+            keys = ["File"] + self.metadata_form().keys()
+            for obj in self.contents():
+                values = [obj.path] + [
+                    str(value) for value in obj.form().values()
+                ]
+                entry = {
+                    keys[i]: values[i] for i in range(len(keys))
+                }
+                metadata.append(entry)
+            with open(
+                os.path.join(path, ".file-metadata.json"),
+                "w", encoding="utf-8"
+            ) as file_handle:
+                json.dump(metadata, file_handle)
+        else:
+            raise ValueError("Unexpected metadata format!")
+
+###############################################################################
+
+    def download(self, path: str = "./", metadata: bool = False) -> None:
+        """
+        Downloads the resource and all of its contents to the local harddrive.
+
+        Parameters
+        ----------
+        path : str, default: "./"
+            Path to the local storage location.
+        metadata : bool, default: False
+            If enabled, resource metadata is downloaded and put in
+            the file '.resource-metadata.json'.
+        """
+
+        logger.info("Downloading resource '%s' (%s)...", self.name, self.id)
+        path = os.path.join(path, self.name)
+        if not os.path.isdir(path):
+            os.mkdir(path)
+        if self.client.settings.concurrent:
+            with concurrent():
+                for obj in self.contents():
+                    obj.download(path, preserve_path=True)
+        else:
+            for obj in self.contents():
+                obj.download(path, preserve_path=True)
+        if metadata:
+            self.download_metadata(path)
+            data = json.dumps(self.data, indent=4)
+            metadata_path: str = os.path.join(path, ".resource-metadata.json")
+            with open(metadata_path, "w", encoding="utf-8") as file:
+                file.write(data)
+
+###############################################################################
+
+    def exists(self, path: str) -> bool:
+        """
+        Returns whether the file referenced by key is contained
+        in the resource.
+
+        Parameters
+        -----------
+        path : str
+            The key/path to the file object
+
+        Returns
+        -------
+        bool
+            True if file object exists, False if not
+        """
+        return self.object(path) is not None
+
+###############################################################################
+
+    def contents(self) -> List[FileObject]:
+        """
+        Returns a list of ALL Objects stored within the resource
+        by recursively traversing directories
+
+        Returns
+        -------
+        List[FileObject]
+            List of Coscine file-like objects.
+        """
+
+        more_folders: bool = True
+        contents = []
+        directories = []
+        files = self.objects()
+        while more_folders:
+            more_folders = False
+            for obj in files:
+                if obj.is_folder:
+                    files.remove(obj)
+                    directories.append(obj)
+                    files.extend(obj.objects())
+                    more_folders = True
+        contents.extend(directories)
+        contents.extend(files)
+        return contents
+
+###############################################################################
+
+    def objects(self, path: Optional[str] = None) -> List[FileObject]:
+        """
+        Returns a list of Objects stored within the resource.
+
+        Parameters
+        ------------
+        path : str, default: None
+            Path to a directory. Irrelevant for anything other than S3.
+
+        Examples
+        ---------
+        >>> Resource.objects(path="Folder/Subfolder")
+        Returns all objects inside 'Folder/Subfolder' (s3 resources only)
+
+        Returns
+        -------
+        List[FileObject]
+            List of Coscine file-like objects.
+        """
+
+        objects = []
+        uri = self.client.uri("Tree", "Tree", self.id)
+        dirpath = posixpath.dirname(path) if path else None
+        args = {"path": path} if dirpath and dirpath != "/" else None
+        data = self.client.get(uri, params=args).json()
+        file_storage: List[dict] = data["data"]["fileStorage"]
+        metadata_storage: List[dict] = data["data"]["metadataStorage"]
+        for data in file_storage:
+            metadata: dict = {}
+            for meta in metadata_storage:
+                key: str = list(meta.keys())[0]
+                if f"{self.id}/{quote(data['Path'])}" in key:
+                    metadata = meta
+                    break
+            objects.append(FileObject(self, data, metadata))
+        return objects
+
+###############################################################################
+
+    def object(self, path: str) -> Union[FileObject, None]:
+        """
+        Returns an Object stored within the resource
+
+        Parameters
+        ------------
+        path : str, default: None
+            Path to a directory. Irrelevant for anything other than S3.
+
+        Examples
+        ---------
+        >>> Resource.object(path="Folder/Subfolder/Filename.jpg")
+        Returns the file inside 'Folder/Subfolder' (s3 resources only)
+
+        Returns
+        -------
+        FileObject
+            Python representation of the file-object as an Object instance
+        None
+            In case nothing was found.
+
+        Raises
+        ------
+        IndexError
+            In case more than 1 FileObject was found at the path.
+        """
+
+        dirpath = posixpath.join(posixpath.dirname(path), "")
+        dirpath = dirpath if dirpath != "/" else ""
+        filename = posixpath.basename(path)
+        if not filename:
+            filename = posixpath.dirname(dirpath)
+            dirpath = ""
+        filtered_list = list(filter(lambda fo: fo.name == filename,
+                                    self.objects(path=dirpath)))
+        if len(filtered_list) == 1:
+            return filtered_list[0]
+        if len(filtered_list) == 0:
+            return None
+        raise IndexError("Too many files matching the specified criteria!")
+
+###############################################################################
+
+    def upload(
+        self,
+        key: str,
+        file,
+        metadata: Union[MetadataForm, dict],
+        callback: Optional[Callable[[int], None]] = None
+    ) -> None:
+        """
+        Uploads a file-like object to a resource on the Coscine server
+
+        Parameters
+        ----------
+        key : str
+            filename of the file-like object.
+        file : object with read() attribute
+            Either open file handle or local file location path.
+        metadata : MetadataForm or dict
+            File metadata matching the resource application profile.
+        callback : Callable[[int], None], default: None
+            Optional callback called during chunk uploads
+            indicating the progress.
+
+        Raises
+        ------
+        TypeError
+            In case the file object specified cannot be used.
+        """
+
+        logger.info(
+            "Uploading FileObject '%s' to resource '%s' (%s)...",
+            key, self.name, self.id
+        )
+        if hasattr(file, "read"):
+            self._upload_file_metadata(key, metadata)
+            self._upload_file_data(key, file, callback)
+        elif isinstance(file, str):
+            with open(file, "rb") as file_handle:
+                self._upload_file_metadata(key, metadata)
+                self._upload_file_data(key, file_handle, callback)
+        else:
+            raise TypeError("Argument `file` has unexpected type!")
+
+###############################################################################
+
+    def _upload_file_metadata(self, key: str, metadata) -> None:
+        if isinstance(metadata, MetadataForm):
+            metadata = metadata.generate()
+        uri = self.client.uri("Tree", "Tree", self.id)
+        params = {"path": key}
+        self.client.put(uri, json=metadata, params=params)
+
+###############################################################################
+
+    def _upload_file_data(
+        self,
+        key: str,
+        file_handle,
+        callback: Optional[Callable[[int], None]] = None
+    ) -> None:
+        uri = self.client.uri("Blob", "Blob", self.id)
+        fields = {"files": (key, file_handle, "application/octect-stream")}
+        encoder = MultipartEncoder(fields=fields)
+        progress_bar = ProgressBar(
+            self.client.settings.verbose, encoder.len, key, callback
+        )
+        monitor = MultipartEncoderMonitor(
+            encoder,
+            callback=lambda monitor:
+                progress_bar.update(monitor.bytes_read - progress_bar.count)
+        )
+        headers = {"Content-Type": monitor.content_type}
+        params = {"path": key}
+        self.client.put(uri, data=monitor, headers=headers, params=params)
+
+###############################################################################
+
+    @parallelizable
+    def set_archived(self, flag: bool) -> None:
+        """
+        Set the archived flag of the resource to put it in read-only mode.
+        Only the resource creator or project owner can do this.
+
+        Parameters
+        ----------
+        flag : bool
+            Enable with True, Disable with False.
+        """
+
+        uri = self.client.uri(
+            "Resources", "Resource", self.id,
+            f"setReadonly?status={str(flag).lower()}"
+        )
+        logger.info(
+            "Setting resource '%s' read only flag = %d",
+            self.name, flag
+        )
+        self.client.post(uri)
+        self.data["archived"] = flag
+
+###############################################################################
+
+    def form(self) -> ResourceForm:
+        """
+        Returns a ResourceForm filled with the metadata of
+        the current resource.
+
+        Returns
+        -------
+        ResourceForm
+        """
+
+        form = self.client.resource_form()
+        form.parse(self.data)
+        return form
+
+###############################################################################
+
+    def update(self, form: Union[ResourceForm, dict]) -> Resource:
+        """
+        Updates the metadata of the resource using the supplied ResourceForm.
+
+        Parameters
+        ----------
+        form : ResourceForm or dict
+            ResourceForm filled with updated values
+            or generated form data dict.
+
+        Returns
+        -------
+        Resource
+            A new resource object with updated resource metadata
+        """
+
+        if isinstance(form, ResourceForm):
+            form = form.generate()
+        elif not isinstance(form, dict):
+            raise TypeError("Resource metadata form has unexpected type.")
+
+        logger.info("Updating resource metadata of resource '%s'.", self.name)
+        uri = self.client.uri("Resources", "Resource", self.id)
+        response = self.client.post(uri, json=form)
+        updated_resource_handle = self
+        if response.ok:
+            # Update resource properties:
+            # The response unfortunately does not return the new resource data
+            updated_resource_handle = list(
+                filter(lambda r: r.id == self.id, self.project.resources())
+            )[0]
+        return updated_resource_handle
+
+###############################################################################
+
+    def metadata_form(self, data: Optional[dict] = None) -> MetadataForm:
+        """
+        Creates a MetadataForm for this resource
+
+        Parameters
+        ----------
+        data : dict, default: None
+            If data is specified, the form is initialized with that data
+            using the InputForm.fill() method.
+        """
+
+        form = MetadataForm(self.client, self.application_profile())
+        if data:
+            form.fill(data)
+        return form
+
+###############################################################################
+# TODO: Add options to create file index, metadata index, file+metadata index
+# TODO: Speed up by not creating individual forms for each file object
+    def dataframe(self):
+        """
+        Creates a pandas dataframe from resource metadata.
+        Requires an installation of the pandas package.
+
+        Returns
+        -------
+        pandas.DataFrame
+        """
+
+        if not pandas:
+            raise ModuleNotFoundError("Method requires package 'pandas'!")
+        form = self.metadata_form()
+        headers = ["Path"] + form.keys()
+        values = [
+            [obj.path] + [
+                str(val) for val in obj.form().values()
+            ] for obj in self.contents()
+        ]
+        return pandas.DataFrame(values, columns=headers)
+
+###############################################################################
+
+    def graph(self) -> Optional[rdflib.Graph]:
+        """
+        Create an rdflib graph from the resource contents.
+        The rdflib graph can be queried with SPARQL, merged with the graphs
+        from other resources and serialized into various formats such
+        as xml or dot (for rendering it as a graph).
+
+        Parameters
+        ----------
+        literal : bool, default: False
+            If enabled, the literal values as seen in the MetadataForm
+            are used for the triples in the graph (the human
+            readable values instead of the URIs).
+
+        Returns
+        --------
+        rdflib.Graph
+        """
+
+        #######################################################################
+
+        def add_to_graph(graph: rdflib.Graph, file: FileObject):
+            """Adds the FileObject to the rdflib graph"""
+            metadata = file.metadata()
+            if metadata:
+                file_reference = rdflib.URIRef(
+                    file.path,
+                    "https://purl.org/coscine/file/"
+                )
+                for key, values in metadata.items():
+                    for value in values:
+                        valtype: str = value["type"]
+                        valuestr: str = value["value"]
+                        if valtype == "uri":
+                            rdf_object = rdflib.URIRef(valuestr)
+                        else:
+                            rdflib.Literal(valuestr)
+                        graph.add((
+                            file_reference,
+                            rdflib.URIRef(key),
+                            rdf_object
+                        ))
+
+        #######################################################################
+
+        file_objects = self.objects()
+        logger.info("Constructing graph for resource %s...", self.display_name)
+        pbar = ProgressBar(
+            self.client.settings.verbose,
+            len(file_objects),
+            f"Creating rdf graph for '{self.display_name}'"
+        )
+        graph = rdflib.Graph(bind_namespaces="rdflib")
+        for file in file_objects:
+            pbar.update(1)
+            if file.has_metadata:
+                add_to_graph(graph, file)
+        return graph
+
+###############################################################################
```

### Comparing `coscine-0.9.0/src/coscine/s3.py` & `coscine-0.9.1/src/coscine/s3.py`

 * *Files identical despite different names*

### Comparing `coscine-0.9.0/src/coscine/utils.py` & `coscine-0.9.1/src/coscine/utils.py`

 * *Files identical despite different names*

### Comparing `coscine-0.9.0/src/coscine/vocabulary.py` & `coscine-0.9.1/src/coscine/vocabulary.py`

 * *Files identical despite different names*

### Comparing `coscine-0.9.0/src/coscine.egg-info/PKG-INFO` & `coscine-0.9.1/src/coscine.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coscine
-Version: 0.9.0
+Version: 0.9.1
 Summary: The Coscine Python SDK provides a pythonic interface to the Coscine REST API.
 Home-page: https://git.rwth-aachen.de/coscine/community-features/coscine-python-sdk/
 Author: RWTH Aachen University
 Author-email: coscine@itc.rwth-aachen.de
 License: MIT License
 Project-URL: Issues, https://git.rwth-aachen.de/coscine/community-features/coscine-python-sdk/-/issues
 Project-URL: Documentation, https://coscine.pages.rwth-aachen.de/community-features/coscine-python-sdk/
```

### Comparing `coscine-0.9.0/src/coscine.egg-info/SOURCES.txt` & `coscine-0.9.1/src/coscine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

