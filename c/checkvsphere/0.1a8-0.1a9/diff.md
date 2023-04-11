# Comparing `tmp/checkvsphere-0.1a8.tar.gz` & `tmp/checkvsphere-0.1a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "checkvsphere-0.1a8.tar", last modified: Tue Mar 14 16:26:33 2023, max compression
+gzip compressed data, was "checkvsphere-0.1a9.tar", last modified: Wed Mar 15 09:39:49 2023, max compression
```

## Comparing `checkvsphere-0.1a8.tar` & `checkvsphere-0.1a9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      264 2023-01-25 12:30:10.233192 checkvsphere-0.1a8/README.md
--rw-r--r--   0        0        0      174 2023-01-17 10:42:21.404433 checkvsphere-0.1a8/checkvsphere/__init__.py
--rw-r--r--   0        0        0     3829 2023-03-13 09:01:04.949489 checkvsphere-0.1a8/checkvsphere/cli.py
--rw-r--r--   0        0        0      760 2023-03-13 09:01:04.949489 checkvsphere-0.1a8/checkvsphere/tools/__init__.py
--rw-r--r--   0        0        0    16298 2022-12-02 09:15:25.388293 checkvsphere-0.1a8/checkvsphere/tools/cli.py
--rw-r--r--   0        0        0     5839 2023-03-13 09:01:04.949489 checkvsphere-0.1a8/checkvsphere/tools/helper.py
--rw-r--r--   0        0        0     5200 2022-07-18 09:51:10.222733 checkvsphere-0.1a8/checkvsphere/tools/pchelper.py
--rw-r--r--   0        0        0     2183 2022-11-11 09:56:50.829790 checkvsphere-0.1a8/checkvsphere/tools/service_instance.py
--rw-r--r--   0        0        0     4153 2022-08-01 15:28:58.196194 checkvsphere-0.1a8/checkvsphere/tools/serviceutil.py
--rw-r--r--   0        0        0      760 2023-03-13 09:01:04.949489 checkvsphere-0.1a8/checkvsphere/vcmd/__init__.py
--rw-r--r--   0        0        0     1961 2023-03-14 15:32:57.011973 checkvsphere-0.1a8/checkvsphere/vcmd/about.py
--rw-r--r--   0        0        0     6717 2023-03-14 15:32:57.011973 checkvsphere-0.1a8/checkvsphere/vcmd/datastores.py
--rw-r--r--   0        0        0     3434 2023-03-14 12:20:28.528461 checkvsphere-0.1a8/checkvsphere/vcmd/hosthealth.py
--rw-r--r--   0        0        0     4553 2023-03-14 15:32:57.011973 checkvsphere-0.1a8/checkvsphere/vcmd/hostnic.py
--rw-r--r--   0        0        0     9815 2023-03-14 15:32:57.011973 checkvsphere-0.1a8/checkvsphere/vcmd/hostruntime.py
--rw-r--r--   0        0        0     4311 2023-03-14 16:23:36.452783 checkvsphere-0.1a8/checkvsphere/vcmd/hostservice.py
--rw-r--r--   0        0        0     7817 2023-03-14 15:59:19.819094 checkvsphere-0.1a8/checkvsphere/vcmd/hoststorage.py
--rw-r--r--   0        0        0     2071 2023-03-14 15:32:57.011973 checkvsphere-0.1a8/checkvsphere/vcmd/listmetrics.py
--rw-r--r--   0        0        0     3440 2023-03-14 15:32:45.464185 checkvsphere-0.1a8/checkvsphere/vcmd/media.py
--rw-r--r--   0        0        0     8238 2023-03-13 09:01:04.949489 checkvsphere-0.1a8/checkvsphere/vcmd/perf.py
--rw-r--r--   0        0        0     5050 2023-03-14 15:32:57.011973 checkvsphere-0.1a8/checkvsphere/vcmd/snapshots.py
--rw-r--r--   0        0        0      939 2023-03-14 16:24:45.243530 checkvsphere-0.1a8/pyproject.toml
--rw-r--r--   0        0        0     1000 1970-01-01 00:00:00.000000 checkvsphere-0.1a8/PKG-INFO
+-rw-r--r--   0        0        0      264 2023-01-25 12:30:10.233192 checkvsphere-0.1a9/README.md
+-rw-r--r--   0        0        0      174 2023-01-17 10:42:21.404433 checkvsphere-0.1a9/checkvsphere/__init__.py
+-rw-r--r--   0        0        0     3829 2023-03-13 09:01:04.949489 checkvsphere-0.1a9/checkvsphere/cli.py
+-rw-r--r--   0        0        0      760 2023-03-13 09:01:04.949489 checkvsphere-0.1a9/checkvsphere/tools/__init__.py
+-rw-r--r--   0        0        0    16298 2022-12-02 09:15:25.388293 checkvsphere-0.1a9/checkvsphere/tools/cli.py
+-rw-r--r--   0        0        0     5839 2023-03-13 09:01:04.949489 checkvsphere-0.1a9/checkvsphere/tools/helper.py
+-rw-r--r--   0        0        0     5200 2022-07-18 09:51:10.222733 checkvsphere-0.1a9/checkvsphere/tools/pchelper.py
+-rw-r--r--   0        0        0     2183 2022-11-11 09:56:50.829790 checkvsphere-0.1a9/checkvsphere/tools/service_instance.py
+-rw-r--r--   0        0        0     4153 2022-08-01 15:28:58.196194 checkvsphere-0.1a9/checkvsphere/tools/serviceutil.py
+-rw-r--r--   0        0        0      760 2023-03-13 09:01:04.949489 checkvsphere-0.1a9/checkvsphere/vcmd/__init__.py
+-rw-r--r--   0        0        0     1961 2023-03-14 15:32:57.011973 checkvsphere-0.1a9/checkvsphere/vcmd/about.py
+-rw-r--r--   0        0        0     6717 2023-03-14 15:32:57.011973 checkvsphere-0.1a9/checkvsphere/vcmd/datastores.py
+-rw-r--r--   0        0        0     3434 2023-03-14 12:20:28.528461 checkvsphere-0.1a9/checkvsphere/vcmd/hosthealth.py
+-rw-r--r--   0        0        0     4553 2023-03-14 15:32:57.011973 checkvsphere-0.1a9/checkvsphere/vcmd/hostnic.py
+-rw-r--r--   0        0        0     9815 2023-03-14 15:32:57.011973 checkvsphere-0.1a9/checkvsphere/vcmd/hostruntime.py
+-rw-r--r--   0        0        0     4311 2023-03-14 16:23:36.452783 checkvsphere-0.1a9/checkvsphere/vcmd/hostservice.py
+-rw-r--r--   0        0        0     7833 2023-03-15 09:27:51.677211 checkvsphere-0.1a9/checkvsphere/vcmd/hoststorage.py
+-rw-r--r--   0        0        0     2071 2023-03-14 15:32:57.011973 checkvsphere-0.1a9/checkvsphere/vcmd/listmetrics.py
+-rw-r--r--   0        0        0     3440 2023-03-14 15:32:45.464185 checkvsphere-0.1a9/checkvsphere/vcmd/media.py
+-rw-r--r--   0        0        0     8238 2023-03-13 09:01:04.949489 checkvsphere-0.1a9/checkvsphere/vcmd/perf.py
+-rw-r--r--   0        0        0     5050 2023-03-14 15:32:57.011973 checkvsphere-0.1a9/checkvsphere/vcmd/snapshots.py
+-rw-r--r--   0        0        0      939 2023-03-15 09:39:39.196408 checkvsphere-0.1a9/pyproject.toml
+-rw-r--r--   0        0        0     1000 1970-01-01 00:00:00.000000 checkvsphere-0.1a9/PKG-INFO
```

### Comparing `checkvsphere-0.1a8/checkvsphere/cli.py` & `checkvsphere-0.1a9/checkvsphere/cli.py`

 * *Files identical despite different names*

### Comparing `checkvsphere-0.1a8/checkvsphere/tools/__init__.py` & `checkvsphere-0.1a9/checkvsphere/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `checkvsphere-0.1a8/checkvsphere/tools/cli.py` & `checkvsphere-0.1a9/checkvsphere/tools/cli.py`

 * *Files identical despite different names*

### Comparing `checkvsphere-0.1a8/checkvsphere/tools/helper.py` & `checkvsphere-0.1a9/checkvsphere/tools/helper.py`

 * *Files identical despite different names*

### Comparing `checkvsphere-0.1a8/checkvsphere/tools/pchelper.py` & `checkvsphere-0.1a9/checkvsphere/tools/pchelper.py`

 * *Files identical despite different names*

### Comparing `checkvsphere-0.1a8/checkvsphere/tools/service_instance.py` & `checkvsphere-0.1a9/checkvsphere/tools/service_instance.py`

 * *Files identical despite different names*

### Comparing `checkvsphere-0.1a8/checkvsphere/tools/serviceutil.py` & `checkvsphere-0.1a9/checkvsphere/tools/serviceutil.py`

 * *Files identical despite different names*

### Comparing `checkvsphere-0.1a8/checkvsphere/vcmd/__init__.py` & `checkvsphere-0.1a9/checkvsphere/vcmd/__init__.py`

 * *Files identical despite different names*

### Comparing `checkvsphere-0.1a8/checkvsphere/vcmd/about.py` & `checkvsphere-0.1a9/checkvsphere/vcmd/about.py`

 * *Files identical despite different names*

### Comparing `checkvsphere-0.1a8/checkvsphere/vcmd/datastores.py` & `checkvsphere-0.1a9/checkvsphere/vcmd/datastores.py`

 * *Files identical despite different names*

### Comparing `checkvsphere-0.1a8/checkvsphere/vcmd/hosthealth.py` & `checkvsphere-0.1a9/checkvsphere/vcmd/hosthealth.py`

 * *Files identical despite different names*

### Comparing `checkvsphere-0.1a8/checkvsphere/vcmd/hostnic.py` & `checkvsphere-0.1a9/checkvsphere/vcmd/hostnic.py`

 * *Files identical despite different names*

### Comparing `checkvsphere-0.1a8/checkvsphere/vcmd/hostruntime.py` & `checkvsphere-0.1a9/checkvsphere/vcmd/hostruntime.py`

 * *Files identical despite different names*

### Comparing `checkvsphere-0.1a8/checkvsphere/vcmd/hostservice.py` & `checkvsphere-0.1a9/checkvsphere/vcmd/hostservice.py`

 * *Files identical despite different names*

### Comparing `checkvsphere-0.1a8/checkvsphere/vcmd/hoststorage.py` & `checkvsphere-0.1a9/checkvsphere/vcmd/hoststorage.py`

 * *Files 1% similar despite different names*

```diff
@@ -183,15 +183,15 @@
             'offline': Status.CRITICAL,
         }.get(dev.status, Status.UNKNOWN)
         count.setdefault(dev.status, 0)
         count[dev.status]+=1
         check.add_message(status, f"{dev.model} {dev.device} ({dev.status})")
 
     short = f"Adapters {len(adapters)}; " + "; ".join([f"{x}: {count[x]}" for x in sorted(count.keys())])
-    (code, message) = check.check_messages(separator_all="\n")#, allok=okmessage)
+    (code, message) = check.check_messages(separator="\n", separator_all="\n")#, allok=okmessage)
     check.exit(
         code=code,
         message=f"{short}\n{message}"
     )
 
 def storage_info(si: vim.ServiceInstance, host):
     ObjectSpec = vmodl.query.PropertyCollector.ObjectSpec
```

### Comparing `checkvsphere-0.1a8/checkvsphere/vcmd/listmetrics.py` & `checkvsphere-0.1a9/checkvsphere/vcmd/listmetrics.py`

 * *Files identical despite different names*

### Comparing `checkvsphere-0.1a8/checkvsphere/vcmd/media.py` & `checkvsphere-0.1a9/checkvsphere/vcmd/media.py`

 * *Files identical despite different names*

### Comparing `checkvsphere-0.1a8/checkvsphere/vcmd/perf.py` & `checkvsphere-0.1a9/checkvsphere/vcmd/perf.py`

 * *Files identical despite different names*

### Comparing `checkvsphere-0.1a8/checkvsphere/vcmd/snapshots.py` & `checkvsphere-0.1a9/checkvsphere/vcmd/snapshots.py`

 * *Files identical despite different names*

### Comparing `checkvsphere-0.1a8/pyproject.toml` & `checkvsphere-0.1a9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 build-backend = "flit_core.buildapi"
 requires = ["flit_core >=3.2,<4"]
 
 [project]
 name = "checkvsphere"
 readme = "README.md"
 description = "check_vsphere monitoring plugin"
-version = "0.1a8"
+version = "0.1a9"
 requires-python = ">= 3.6"
 authors = [
     { name = "Danijel Tasov", email = "danijel.tasov@consol.de" }
 ]
 dependencies = [
     "pyvmomi >= 8.0.0.1, < 9",
     "monplugin >= 0.4",
```

### Comparing `checkvsphere-0.1a8/PKG-INFO` & `checkvsphere-0.1a9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: checkvsphere
-Version: 0.1a8
+Version: 0.1a9
 Summary: check_vsphere monitoring plugin
 Author-email: Danijel Tasov <danijel.tasov@consol.de>
 Requires-Python: >= 3.6
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: System :: Monitoring
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

