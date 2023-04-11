# Comparing `tmp/checkontap-0.1a1.tar.gz` & `tmp/checkontap-0.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "checkontap-0.1a1.tar", last modified: Thu Mar 23 15:59:45 2023, max compression
+gzip compressed data, was "checkontap-0.1a2.tar", last modified: Tue Apr 11 08:45:43 2023, max compression
```

## Comparing `checkontap-0.1a1.tar` & `checkontap-0.1a2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      223 2023-03-23 09:02:45.881436 checkontap-0.1a1/README.md
--rw-r--r--   0        0        0      926 2023-03-22 16:30:38.341339 checkontap-0.1a1/checkontap/__init__.py
--rw-r--r--   0        0        0     3431 2023-03-23 14:53:12.575066 checkontap-0.1a1/checkontap/cli.py
--rw-r--r--   0        0        0      756 2023-03-22 16:09:15.025609 checkontap-0.1a1/checkontap/ontapcmd/__init__.py
--rw-r--r--   0        0        0     2239 2023-03-23 10:23:29.838743 checkontap-0.1a1/checkontap/ontapcmd/about.py
--rw-r--r--   0        0        0     6879 2023-03-23 10:24:04.245021 checkontap-0.1a1/checkontap/ontapcmd/aggregateusage.py
--rw-r--r--   0        0        0     2906 2023-03-23 10:24:18.101957 checkontap-0.1a1/checkontap/ontapcmd/clusterhealth.py
--rw-r--r--   0        0        0     7706 2023-03-23 10:34:24.107947 checkontap-0.1a1/checkontap/ontapcmd/diskhealth.py
--rw-r--r--   0        0        0     4521 2023-03-23 10:34:56.095206 checkontap-0.1a1/checkontap/ontapcmd/hardwarehealth.py
--rw-r--r--   0        0        0     3848 2023-03-23 15:56:05.462390 checkontap-0.1a1/checkontap/ontapcmd/interfacehealth.py
--rw-r--r--   0        0        0     4935 2023-03-23 10:31:05.034364 checkontap-0.1a1/checkontap/ontapcmd/lunusage.py
--rw-r--r--   0        0        0     5091 2023-03-23 10:31:27.440904 checkontap-0.1a1/checkontap/ontapcmd/volumehealth.py
--rw-r--r--   0        0        0     6563 2023-03-23 10:31:43.327447 checkontap-0.1a1/checkontap/ontapcmd/volumeusage.py
--rw-r--r--   0        0        0      757 2023-03-22 16:09:25.201105 checkontap-0.1a1/checkontap/tools/__init__.py
--rw-r--r--   0        0        0     8774 2023-03-15 10:17:40.434320 checkontap-0.1a1/checkontap/tools/cli.py
--rw-r--r--   0        0        0     2986 2023-03-23 10:28:55.299455 checkontap-0.1a1/checkontap/tools/helper.py
--rw-r--r--   0        0        0      857 2023-03-23 15:59:16.664884 checkontap-0.1a1/pyproject.toml
--rw-r--r--   0        0        0      893 1970-01-01 00:00:00.000000 checkontap-0.1a1/PKG-INFO
+-rw-r--r--   0        0        0      223 2023-03-23 09:02:45.881436 checkontap-0.1a2/README.md
+-rw-r--r--   0        0        0      926 2023-03-22 16:30:38.341339 checkontap-0.1a2/checkontap/__init__.py
+-rw-r--r--   0        0        0     3431 2023-03-23 14:53:12.575066 checkontap-0.1a2/checkontap/cli.py
+-rw-r--r--   0        0        0      756 2023-03-22 16:09:15.025609 checkontap-0.1a2/checkontap/ontapcmd/__init__.py
+-rw-r--r--   0        0        0     2239 2023-03-23 10:23:29.838743 checkontap-0.1a2/checkontap/ontapcmd/about.py
+-rw-r--r--   0        0        0     6957 2023-04-11 08:29:43.568792 checkontap-0.1a2/checkontap/ontapcmd/aggregateusage.py
+-rw-r--r--   0        0        0     2906 2023-03-23 10:24:18.101957 checkontap-0.1a2/checkontap/ontapcmd/clusterhealth.py
+-rw-r--r--   0        0        0     7706 2023-03-23 10:34:24.107947 checkontap-0.1a2/checkontap/ontapcmd/diskhealth.py
+-rw-r--r--   0        0        0     4521 2023-03-23 10:34:56.095206 checkontap-0.1a2/checkontap/ontapcmd/hardwarehealth.py
+-rw-r--r--   0        0        0     3848 2023-03-23 15:56:05.462390 checkontap-0.1a2/checkontap/ontapcmd/interfacehealth.py
+-rw-r--r--   0        0        0     5006 2023-04-11 08:31:25.465579 checkontap-0.1a2/checkontap/ontapcmd/lunusage.py
+-rw-r--r--   0        0        0     5091 2023-03-23 10:31:27.440904 checkontap-0.1a2/checkontap/ontapcmd/volumehealth.py
+-rw-r--r--   0        0        0     6634 2023-04-11 08:32:37.797398 checkontap-0.1a2/checkontap/ontapcmd/volumeusage.py
+-rw-r--r--   0        0        0      757 2023-03-22 16:09:25.201105 checkontap-0.1a2/checkontap/tools/__init__.py
+-rw-r--r--   0        0        0     8774 2023-03-15 10:17:40.434320 checkontap-0.1a2/checkontap/tools/cli.py
+-rw-r--r--   0        0        0     2986 2023-03-23 10:28:55.299455 checkontap-0.1a2/checkontap/tools/helper.py
+-rw-r--r--   0        0        0      857 2023-04-11 08:40:22.079330 checkontap-0.1a2/pyproject.toml
+-rw-r--r--   0        0        0      893 1970-01-01 00:00:00.000000 checkontap-0.1a2/PKG-INFO
```

### Comparing `checkontap-0.1a1/checkontap/__init__.py` & `checkontap-0.1a2/checkontap/__init__.py`

 * *Files identical despite different names*

### Comparing `checkontap-0.1a1/checkontap/cli.py` & `checkontap-0.1a2/checkontap/cli.py`

 * *Files identical despite different names*

### Comparing `checkontap-0.1a1/checkontap/ontapcmd/__init__.py` & `checkontap-0.1a2/checkontap/ontapcmd/__init__.py`

 * *Files identical despite different names*

### Comparing `checkontap-0.1a1/checkontap/ontapcmd/about.py` & `checkontap-0.1a2/checkontap/ontapcmd/about.py`

 * *Files identical despite different names*

### Comparing `checkontap-0.1a1/checkontap/ontapcmd/aggregateusage.py` & `checkontap-0.1a2/checkontap/ontapcmd/aggregateusage.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,14 +98,15 @@
         logger.debug(f"found {aggr_count} Aggregates")
         if aggr_count == 0:
             check.exit(Status.UNKNOWN, "no aggregates found")
 
         for aggr in Aggregate.get_collection():
             aggr.get(fields="space,uuid")
             if (args.exclude or args.include) and item_filter(args,aggr.name):
+                aggr_count -= 1
                 continue
             for plex in Plex.get_collection(aggr.uuid):
                 plex.get(fields="raid_groups")
                 logging.debug(f"Plex {plex.name}\n{plex.__dict__}") 
                 for rg in plex.raid_groups:
                     if rg.reconstruct.active:
                         check.add_message(Status.CRITICAL, f"RaidGroup {rg.name} on Plex {plex.name} is reconstructing")
@@ -147,15 +148,15 @@
                 unitPerf['threshold'] = check.threshold
                 check.add_perfdata(**unitPerf)
                 check.add_perfdata(**pctPerf)
                 check.add_message(
                     check.threshold.get_status(aggr.space.block_storage.used),
                     f"{aggr.name} (Usage {aggr.space.block_storage.used}/{aggr.space.block_storage.size}B {pctUsage}%)"
                 )
-        (code, message) = check.check_messages(separator='\n  ')
+        (code, message) = check.check_messages(separator='\n  ',allok=f"all {aggr_count} aggregates are fine")
         check.exit(code=code,message=message)
 
     except NetAppRestError as error:
         check.exit(Status.UNKNOWN, "Error => {}".format(error.http_err_response.http_response.text))
     
 if __name__ == "__main__":
     run()
```

### Comparing `checkontap-0.1a1/checkontap/ontapcmd/clusterhealth.py` & `checkontap-0.1a2/checkontap/ontapcmd/clusterhealth.py`

 * *Files identical despite different names*

### Comparing `checkontap-0.1a1/checkontap/ontapcmd/diskhealth.py` & `checkontap-0.1a2/checkontap/ontapcmd/diskhealth.py`

 * *Files identical despite different names*

### Comparing `checkontap-0.1a1/checkontap/ontapcmd/hardwarehealth.py` & `checkontap-0.1a2/checkontap/ontapcmd/hardwarehealth.py`

 * *Files identical despite different names*

### Comparing `checkontap-0.1a1/checkontap/ontapcmd/interfacehealth.py` & `checkontap-0.1a2/checkontap/ontapcmd/interfacehealth.py`

 * *Files identical despite different names*

### Comparing `checkontap-0.1a1/checkontap/ontapcmd/lunusage.py` & `checkontap-0.1a2/checkontap/ontapcmd/lunusage.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,14 +57,15 @@
         luns_count = Lun.count_collection()
         if luns_count == 0:
             check.exit(Status.UNKNOWN, "no luns found")
         for lun in Lun.get_collection():
             lun.get(fields="space")
             logger.debug(f"lun info for {lun.name}\n{lun.__dict__}")
             if (args.exclude or args.include) and item_filter(args,lun.name):
+                luns_count -= 1
                 continue
 
             pctUsage = to_percent(lun.space.size,lun.space.used)
             unitPerf = {'label': f'{lun.name}_space',
                     'value': lun.space.used,
                     'uom': 'B',
                     'min': 0,
@@ -104,15 +105,15 @@
                 pctPerf['warning'] = to_percent(lun.space.size,args.warning)
                 pctPerf['critical'] = to_percent(lun.space.size,args.critical)
                 check.add_perfdata(**pctPerf)
                 check.add_message(
                     check.threshold.get_status(lun.space.used),
                     f"{lun.name} (Usage {lun.space.used}/{lun.space.size}B {pctUsage}%)"
                 )
-        (code, message) = check.check_messages(separator='\n  ')
+        (code, message) = check.check_messages(separator='\n  ', allok=f"all {luns_count} luns are ok")
         check.exit(code=code,message=message)
 
     except NetAppRestError as error:
         check.exit(Status.UNKNOWN, "Error => {}".format(error.http_err_response.http_response.text))
     
 if __name__ == "__main__":
     run()
```

### Comparing `checkontap-0.1a1/checkontap/ontapcmd/volumehealth.py` & `checkontap-0.1a2/checkontap/ontapcmd/volumehealth.py`

 * *Files identical despite different names*

### Comparing `checkontap-0.1a1/checkontap/ontapcmd/volumeusage.py` & `checkontap-0.1a2/checkontap/ontapcmd/volumeusage.py`

 * *Files 6% similar despite different names*

```diff
@@ -97,14 +97,15 @@
             check.exit(Status.UNKNOWN, "no vols found")
         
         for vol in Volume.get_collection():
             vol.get()
             if not hasattr(vol,'space'):
                 continue
             if (args.exclude or args.include) and item_filter(args,vol.name):
+                volumes_count -= 1
                 continue
             logger.debug(f"VOLUME {vol.name}\n{vol}")
             vols.append(vol) 
 
     except NetAppRestError as error:
         check.exit(Status.UNKNOWN, "Error => {}".format(error.http_err_response.http_response.text))
 
@@ -151,12 +152,12 @@
             unitPerf['threshold'] = check.threshold
             check.add_perfdata(**unitPerf)
             check.add_perfdata(**pctPerf)
             check.add_message(
                 check.threshold.get_status(vol.space.used),
                 f"{vol.name} (Usage {vol.space.used}/{vol.space.size}B {pctUsage}%)"
             )
-    (code, message) = check.check_messages(separator='\n  ')
+    (code, message) = check.check_messages(separator='\n  ',allok=f"all {volumes_count} are ok")
     check.exit(code=code,message=message)
 
 if __name__ == "__main__":
     run()
```

### Comparing `checkontap-0.1a1/checkontap/tools/__init__.py` & `checkontap-0.1a2/checkontap/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `checkontap-0.1a1/checkontap/tools/cli.py` & `checkontap-0.1a2/checkontap/tools/cli.py`

 * *Files identical despite different names*

### Comparing `checkontap-0.1a1/checkontap/tools/helper.py` & `checkontap-0.1a2/checkontap/tools/helper.py`

 * *Files identical despite different names*

### Comparing `checkontap-0.1a1/pyproject.toml` & `checkontap-0.1a2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 build-backend = "flit_core.buildapi"
 requires = ["flit_core >=3.2,<4"]
 
 [project]
 name = "checkontap"
 readme = "README.md"
 description = "check_ontap monitoring plugin"
-version = "0.1a1"
+version = "0.1a2"
 requires-python = ">= 3.6"
 authors = [
     { name = "Matthias Gallinger", email = "matthias.gallinger@consol.de" }
 ]
 dependencies = [
     "netapp-ontap >= 9.11.1.0",
-    "monplugin >= 0.4",
+    "monplugin >= 0.5",
 ]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Topic :: System :: Monitoring",
     "License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)",
 ]
```

### Comparing `checkontap-0.1a1/PKG-INFO` & `checkontap-0.1a2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: checkontap
-Version: 0.1a1
+Version: 0.1a2
 Summary: check_ontap monitoring plugin
 Author-email: Matthias Gallinger <matthias.gallinger@consol.de>
 Requires-Python: >= 3.6
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: System :: Monitoring
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Requires-Dist: netapp-ontap >= 9.11.1.0
-Requires-Dist: monplugin >= 0.4
+Requires-Dist: monplugin >= 0.5
 Project-URL: homepage, https://github.com/consol/check_ontap
 Project-URL: issues, https://github.com/consol/check_ontap/issues
 Project-URL: repository, https://github.com/consol/check_ontap.git
 
 # check_ontap
 
 Plugin for Naemon / Nagios like monitoring systems.
```

