# Comparing `tmp/storpool.spopenstack-3.1.0.tar.gz` & `tmp/storpool.spopenstack-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "storpool.spopenstack-3.1.0.tar", last modified: Mon Sep 27 23:17:32 2021, max compression
+gzip compressed data, was "storpool.spopenstack-3.2.0.tar", last modified: Tue Apr 11 08:31:13 2023, max compression
```

## Comparing `storpool.spopenstack-3.1.0.tar` & `storpool.spopenstack-3.2.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2021-09-27 23:17:32.567123 storpool.spopenstack-3.1.0/
--rw-r--r--   0 roam      (1000) roam      (1000)      340 2021-09-27 23:17:32.567123 storpool.spopenstack-3.1.0/PKG-INFO
--rw-r--r--   0 roam      (1000) roam      (1000)     4000 2021-09-27 23:14:22.000000 storpool.spopenstack-3.1.0/README.rst
--rw-r--r--   0 roam      (1000) roam      (1000)       67 2021-09-27 23:17:32.567123 storpool.spopenstack-3.1.0/setup.cfg
--rw-r--r--   0 roam      (1000) roam      (1000)     1178 2021-09-27 23:14:22.000000 storpool.spopenstack-3.1.0/setup.py
-drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2021-09-27 23:17:32.567123 storpool.spopenstack-3.1.0/storpool/
--rw-r--r--   0 roam      (1000) roam      (1000)      672 2019-08-26 12:49:44.000000 storpool.spopenstack-3.1.0/storpool/__init__.py
-drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2021-09-27 23:17:32.567123 storpool.spopenstack-3.1.0/storpool/spopenstack/
--rw-r--r--   0 roam      (1000) roam      (1000)      663 2019-08-26 12:49:44.000000 storpool.spopenstack-3.1.0/storpool/spopenstack/__init__.py
--rw-r--r--   0 roam      (1000) roam      (1000)     9303 2021-09-27 23:07:17.000000 storpool.spopenstack-3.1.0/storpool/spopenstack/spattachdb.py
--rw-r--r--   0 roam      (1000) roam      (1000)     6037 2021-09-27 23:14:22.000000 storpool.spopenstack-3.1.0/storpool/spopenstack/splocked.py
-drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2021-09-27 23:17:32.567123 storpool.spopenstack-3.1.0/storpool.spopenstack.egg-info/
--rw-r--r--   0 roam      (1000) roam      (1000)      340 2021-09-27 23:17:32.000000 storpool.spopenstack-3.1.0/storpool.spopenstack.egg-info/PKG-INFO
--rw-r--r--   0 roam      (1000) roam      (1000)      462 2021-09-27 23:17:32.000000 storpool.spopenstack-3.1.0/storpool.spopenstack.egg-info/SOURCES.txt
--rw-r--r--   0 roam      (1000) roam      (1000)        1 2021-09-27 23:17:32.000000 storpool.spopenstack-3.1.0/storpool.spopenstack.egg-info/dependency_links.txt
--rw-r--r--   0 roam      (1000) roam      (1000)        9 2021-09-27 23:17:32.000000 storpool.spopenstack-3.1.0/storpool.spopenstack.egg-info/namespace_packages.txt
--rw-r--r--   0 roam      (1000) roam      (1000)       16 2021-09-27 23:17:32.000000 storpool.spopenstack-3.1.0/storpool.spopenstack.egg-info/requires.txt
--rw-r--r--   0 roam      (1000) roam      (1000)        9 2021-09-27 23:17:32.000000 storpool.spopenstack-3.1.0/storpool.spopenstack.egg-info/top_level.txt
--rw-r--r--   0 roam      (1000) roam      (1000)        1 2021-09-27 23:17:32.000000 storpool.spopenstack-3.1.0/storpool.spopenstack.egg-info/zip-safe
+drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2023-04-11 08:31:13.050701 storpool.spopenstack-3.2.0/
+-rw-r--r--   0 roam      (1000) roam      (1000)      312 2023-04-11 08:31:13.050701 storpool.spopenstack-3.2.0/PKG-INFO
+-rw-r--r--   0 roam      (1000) roam      (1000)     5036 2023-04-11 08:26:17.000000 storpool.spopenstack-3.2.0/README.rst
+-rw-r--r--   0 roam      (1000) roam      (1000)      234 2023-04-11 08:26:17.000000 storpool.spopenstack-3.2.0/pyproject.toml
+-rw-r--r--   0 roam      (1000) roam      (1000)       67 2023-04-11 08:31:13.050701 storpool.spopenstack-3.2.0/setup.cfg
+-rw-r--r--   0 roam      (1000) roam      (1000)     1185 2023-04-11 08:26:17.000000 storpool.spopenstack-3.2.0/setup.py
+drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2023-04-11 08:31:13.050701 storpool.spopenstack-3.2.0/storpool/
+-rw-r--r--   0 roam      (1000) roam      (1000)      672 2019-08-26 12:49:44.000000 storpool.spopenstack-3.2.0/storpool/__init__.py
+drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2023-04-11 08:31:13.050701 storpool.spopenstack-3.2.0/storpool/spopenstack/
+-rw-r--r--   0 roam      (1000) roam      (1000)      663 2019-08-26 12:49:44.000000 storpool.spopenstack-3.2.0/storpool/spopenstack/__init__.py
+-rw-r--r--   0 roam      (1000) roam      (1000)     9642 2023-04-11 08:26:17.000000 storpool.spopenstack-3.2.0/storpool/spopenstack/spattachdb.py
+-rw-r--r--   0 roam      (1000) roam      (1000)     6117 2023-04-11 08:26:17.000000 storpool.spopenstack-3.2.0/storpool/spopenstack/splocked.py
+drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2023-04-11 08:31:13.050701 storpool.spopenstack-3.2.0/storpool.spopenstack.egg-info/
+-rw-r--r--   0 roam      (1000) roam      (1000)      312 2023-04-11 08:31:13.000000 storpool.spopenstack-3.2.0/storpool.spopenstack.egg-info/PKG-INFO
+-rw-r--r--   0 roam      (1000) roam      (1000)      477 2023-04-11 08:31:13.000000 storpool.spopenstack-3.2.0/storpool.spopenstack.egg-info/SOURCES.txt
+-rw-r--r--   0 roam      (1000) roam      (1000)        1 2023-04-11 08:31:13.000000 storpool.spopenstack-3.2.0/storpool.spopenstack.egg-info/dependency_links.txt
+-rw-r--r--   0 roam      (1000) roam      (1000)        9 2023-04-11 08:31:13.000000 storpool.spopenstack-3.2.0/storpool.spopenstack.egg-info/namespace_packages.txt
+-rw-r--r--   0 roam      (1000) roam      (1000)       19 2023-04-11 08:31:13.000000 storpool.spopenstack-3.2.0/storpool.spopenstack.egg-info/requires.txt
+-rw-r--r--   0 roam      (1000) roam      (1000)        9 2023-04-11 08:31:13.000000 storpool.spopenstack-3.2.0/storpool.spopenstack.egg-info/top_level.txt
+-rw-r--r--   0 roam      (1000) roam      (1000)        1 2023-04-11 08:30:58.000000 storpool.spopenstack-3.2.0/storpool.spopenstack.egg-info/zip-safe
```

### Comparing `storpool.spopenstack-3.1.0/README.rst` & `storpool.spopenstack-3.2.0/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -13,14 +13,36 @@
 while the StorPool client allows a hypervisor node to access the storage pool
 and act as a compute node.  In OpenStack terms the StorPool solution allows
 each hypervisor node to be both a storage and a compute node simultaneously.
 
 Version history
 ===============
 
+3.2.0
+-----
+
+- Do not require `SP_OURID` to be defined in the StorPool configuration
+  so that we can support iSCSI-only deployments
+- Add the optional `override_config` dictionary to the AttachDB constructor
+  to skip reading the StorPool configuration files altogether. This should
+  simplify isolated deployments and allow the StorPool OpenStack helper
+  tools to be configured with settings read from the OpenStack config
+  files only
+- Depend on `storpool >= 7.2.0` for `override_config` support in
+  the `SPConfig` configuration class
+- Depend on `storpool < 8`, since incompatible changes are planned in
+  the StorPool API bindings library itself
+- Minor refactoring so that stricter type checking can be enabled
+- Build and testing infrastructure changes:
+    - clamp the versions of some Python build tools and required libraries;
+      add both lower and upper version constraints
+    - put Tox environment commands on separate lines
+    - move the configuration of some static checker tools to
+      the pyproject.toml file
+
 3.1.0
 -----
 
 - Reraise unexpected StorPool API errors instead of ignoring them
 - Handle the StorPool API returning a "busy" error code instead of
   the "invalidParam" one previously
 - Fix attempting to lock a file for the second time after the first one
```

### Comparing `storpool.spopenstack-3.1.0/setup.py` & `storpool.spopenstack-3.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,19 +17,19 @@
 #
 
 import setuptools  # type: ignore
 
 
 setuptools.setup(
     name="storpool.spopenstack",
-    version="3.1.0",
+    version="3.2.0",
     packages=("storpool", "storpool.spopenstack"),
     namespace_packages=("storpool",),
     python_requires=">= 2.7",
-    install_requires=("storpool>=4.0.0",),
+    install_requires=("storpool >= 7.2.0, < 8",),
     author="Peter Pentchev",
     author_email="openstack-dev@storpool.com",
     description="OpenStack helpers for the StorPool API",
     license="Apache 2.0 License",
     keywords="storpool StorPool openstack OpenStack",
     url="http://www.storpool.com/",
     zip_safe=True,
```

### Comparing `storpool.spopenstack-3.1.0/storpool/__init__.py` & `storpool.spopenstack-3.2.0/storpool/__init__.py`

 * *Files identical despite different names*

### Comparing `storpool.spopenstack-3.1.0/storpool/spopenstack/__init__.py` & `storpool.spopenstack-3.2.0/storpool/spopenstack/__init__.py`

 * *Files identical despite different names*

### Comparing `storpool.spopenstack-3.1.0/storpool/spopenstack/spattachdb.py` & `storpool.spopenstack-3.2.0/storpool/spopenstack/spattachdb.py`

 * *Files 7% similar despite different names*

```diff
@@ -48,28 +48,40 @@
 from . import splocked
 
 
 LOCKFILE = "/var/spool/openstack-storpool/openstack-attach.json"
 
 
 class AttachDB(splocked.SPLockedJSONDB):
-    def __init__(self, log, fname=LOCKFILE):
-        # type: (AttachDB, logging.Logger, str) -> None
+    def __init__(
+        self,  # type: AttachDB
+        log,  # type: logging.Logger
+        fname=LOCKFILE,  # type: str
+        override_config=None,  # type: Optional[Dict[str, str]]
+    ):  # type: (...) -> None
         super(AttachDB, self).__init__(fname)
         self._api = None  # type: Optional[spapi.Api]
         self._config = None  # type: Optional[spconfig.SPConfig]
         self._ourId = None  # type: Optional[int]
+        self._override_config = override_config
         self._volume_prefix = None  # type: Optional[str]
         self.LOG = log
 
     def config(self):
         # type: (AttachDB) -> spconfig.SPConfig
         if self._config is None:
-            self._config = spconfig.SPConfig()
-            self._ourId = int(self._config["SP_OURID"])
+            self._config = spconfig.SPConfig(
+                override_config=self._override_config
+            )
+
+            try:
+                self._ourId = int(self._config["SP_OURID"])
+            except KeyError:
+                self._ourId = -1
+
         return self._config
 
     def api(self):
         # type: (AttachDB) -> spapi.Api
         if self._api is None:
             self._api = spapi.Api.fromConfig(self.config())
         return self._api
@@ -110,15 +122,15 @@
             for att in self.api().attachmentsList()
             if att.volume.startswith(pfx)
         ]
         return (self.get(), attached)
 
     def sync(self, req_id, detached):
         # type: (AttachDB, str, Optional[str]) -> None
-        assert self._ourId is not None
+        assert self._ourId is not None and self._ourId != -1
 
         with self:
             (attach_req_d, apiatt) = self._get_attachments_data()
 
             attach = attach_req_d.get(req_id, None)
             if attach is None:
                 if detached is not None:
```

### Comparing `storpool.spopenstack-3.1.0/storpool/spopenstack/splocked.py` & `storpool.spopenstack-3.2.0/storpool/spopenstack/splocked.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #
 # -
-# Copyright (c) 2014, 2015, 2019 - 2021  StorPool.
+# Copyright (c) 2014, 2015, 2019 - 2022  StorPool.
 # All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -148,27 +148,29 @@
 
         self._count -= 1
         rlock.release()
 
     def jsload(self):
         # type: (SPLockedFile) -> Any
         with self:
+            assert self._fd is not None
             os.lseek(self._fd, 0, os.SEEK_SET)
             contents = b""
             while True:
                 chunk = os.read(self._fd, 8192)
                 if not chunk:
                     break
                 contents += chunk
 
             return json.loads(contents)
 
     def jsdump(self, obj):
         # type: (SPLockedFile, Any) -> None
         with self:
+            assert self._fd is not None
             contents = json.dumps(obj).encode("UTF-8")
 
             os.lseek(self._fd, 0, os.SEEK_SET)
             os.ftruncate(self._fd, 0)
             while contents:
                 written = os.write(self._fd, contents)
                 contents = contents[written:]
```

