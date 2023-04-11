# Comparing `tmp/jdmtool-0.0.1.tar.gz` & `tmp/jdmtool-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jdmtool-0.0.1.tar", last modified: Wed Mar 29 21:04:17 2023, max compression
+gzip compressed data, was "jdmtool-0.0.2.tar", last modified: Tue Apr 11 02:19:48 2023, max compression
```

## Comparing `jdmtool-0.0.1.tar` & `jdmtool-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-03-29 21:04:17.919769 jdmtool-0.0.1/
--rw-r--r--   0 dima      (1000) dima      (1000)    11357 2023-03-28 17:09:03.000000 jdmtool-0.0.1/LICENSE
--rw-r--r--   0 dima      (1000) dima      (1000)     6580 2023-03-29 21:04:17.918769 jdmtool-0.0.1/PKG-INFO
--rw-r--r--   0 dima      (1000) dima      (1000)     6020 2023-03-29 21:02:54.000000 jdmtool-0.0.1/README.md
--rw-r--r--   0 dima      (1000) dima      (1000)      788 2023-03-29 20:59:35.000000 jdmtool-0.0.1/pyproject.toml
--rw-r--r--   0 dima      (1000) dima      (1000)       38 2023-03-29 21:04:17.919769 jdmtool-0.0.1/setup.cfg
-drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-03-29 21:04:17.914769 jdmtool-0.0.1/src/
-drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-03-29 21:04:17.916769 jdmtool-0.0.1/src/jdmtool/
--rw-r--r--   0 dima      (1000) dima      (1000)        0 2023-03-28 16:55:30.000000 jdmtool-0.0.1/src/jdmtool/__init__.py
--rw-r--r--   0 dima      (1000) dima      (1000)     3700 2023-03-29 07:08:50.000000 jdmtool-0.0.1/src/jdmtool/device.py
--rw-r--r--   0 dima      (1000) dima      (1000)     4701 2023-03-29 20:35:15.000000 jdmtool-0.0.1/src/jdmtool/downloader.py
--rwxr-xr-x   0 dima      (1000) dima      (1000)    13651 2023-03-29 20:46:11.000000 jdmtool-0.0.1/src/jdmtool/main.py
-drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-03-29 21:04:17.918769 jdmtool-0.0.1/src/jdmtool.egg-info/
--rw-r--r--   0 dima      (1000) dima      (1000)     6580 2023-03-29 21:04:17.000000 jdmtool-0.0.1/src/jdmtool.egg-info/PKG-INFO
--rw-r--r--   0 dima      (1000) dima      (1000)      336 2023-03-29 21:04:17.000000 jdmtool-0.0.1/src/jdmtool.egg-info/SOURCES.txt
--rw-r--r--   0 dima      (1000) dima      (1000)        1 2023-03-29 21:04:17.000000 jdmtool-0.0.1/src/jdmtool.egg-info/dependency_links.txt
--rw-r--r--   0 dima      (1000) dima      (1000)       46 2023-03-29 21:04:17.000000 jdmtool-0.0.1/src/jdmtool.egg-info/entry_points.txt
--rw-r--r--   0 dima      (1000) dima      (1000)       64 2023-03-29 21:04:17.000000 jdmtool-0.0.1/src/jdmtool.egg-info/requires.txt
--rw-r--r--   0 dima      (1000) dima      (1000)        8 2023-03-29 21:04:17.000000 jdmtool-0.0.1/src/jdmtool.egg-info/top_level.txt
+drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-04-11 02:19:48.779738 jdmtool-0.0.2/
+-rw-r--r--   0 dima      (1000) dima      (1000)    11357 2023-03-28 17:09:03.000000 jdmtool-0.0.2/LICENSE
+-rw-r--r--   0 dima      (1000) dima      (1000)     6769 2023-04-11 02:19:48.779738 jdmtool-0.0.2/PKG-INFO
+-rw-r--r--   0 dima      (1000) dima      (1000)     6209 2023-04-11 02:13:35.000000 jdmtool-0.0.2/README.md
+-rw-r--r--   0 dima      (1000) dima      (1000)      788 2023-04-11 02:19:07.000000 jdmtool-0.0.2/pyproject.toml
+-rw-r--r--   0 dima      (1000) dima      (1000)       38 2023-04-11 02:19:48.779738 jdmtool-0.0.2/setup.cfg
+drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-04-11 02:19:48.774738 jdmtool-0.0.2/src/
+drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-04-11 02:19:48.777738 jdmtool-0.0.2/src/jdmtool/
+-rw-r--r--   0 dima      (1000) dima      (1000)        0 2023-03-28 16:55:30.000000 jdmtool-0.0.2/src/jdmtool/__init__.py
+-rw-r--r--   0 dima      (1000) dima      (1000)     3700 2023-04-09 01:59:45.000000 jdmtool-0.0.2/src/jdmtool/device.py
+-rw-r--r--   0 dima      (1000) dima      (1000)     4769 2023-04-11 02:12:56.000000 jdmtool-0.0.2/src/jdmtool/downloader.py
+-rwxr-xr-x   0 dima      (1000) dima      (1000)    13749 2023-04-11 02:12:56.000000 jdmtool-0.0.2/src/jdmtool/main.py
+drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-04-11 02:19:48.779738 jdmtool-0.0.2/src/jdmtool.egg-info/
+-rw-r--r--   0 dima      (1000) dima      (1000)     6769 2023-04-11 02:19:48.000000 jdmtool-0.0.2/src/jdmtool.egg-info/PKG-INFO
+-rw-r--r--   0 dima      (1000) dima      (1000)      336 2023-04-11 02:19:48.000000 jdmtool-0.0.2/src/jdmtool.egg-info/SOURCES.txt
+-rw-r--r--   0 dima      (1000) dima      (1000)        1 2023-04-11 02:19:48.000000 jdmtool-0.0.2/src/jdmtool.egg-info/dependency_links.txt
+-rw-r--r--   0 dima      (1000) dima      (1000)       46 2023-04-11 02:19:48.000000 jdmtool-0.0.2/src/jdmtool.egg-info/entry_points.txt
+-rw-r--r--   0 dima      (1000) dima      (1000)       64 2023-04-11 02:19:48.000000 jdmtool-0.0.2/src/jdmtool.egg-info/requires.txt
+-rw-r--r--   0 dima      (1000) dima      (1000)        8 2023-04-11 02:19:48.000000 jdmtool-0.0.2/src/jdmtool.egg-info/top_level.txt
```

### Comparing `jdmtool-0.0.1/LICENSE` & `jdmtool-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jdmtool-0.0.1/PKG-INFO` & `jdmtool-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jdmtool
-Version: 0.0.1
+Version: 0.0.2
 Summary: Tool for downloading Jeppesen databases and programming Garmin aviation data cards
 Author-email: Dima Ryazanov <dima@gmail.com>
 Project-URL: Homepage, https://github.com/dimaryaz/jdmtool
 Project-URL: Bug Tracker, https://github.com/dimaryaz/jdmtool/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -59,16 +59,17 @@
 Success
 ```
 
 ### View available downloads
 
 ```
 $ jdmtool list
-ID  Name                                                                    Cycle  Start Date  End Date    Downloaded
- 0  NavData Coverage Garmin GNS 400/500 Series WAAS Americas                 2303  2023-03-23  2023-04-20            
+ID  Name                                                                    Version   Start Date  End Date    Downloaded
+ 0  NavData Coverage Garmin GNS 400/500 Series WAAS Americas                2303      2023-03-23  2023-04-20  Y         
+ 1  NavData Coverage Garmin GNS 400/500 Series WAAS Americas                2304      2023-04-20  2023-05-18            
 ```
 
 ### View detailed info
 
 ```
 $ jdmtool info 0
 Aircraft Manufacturer:        LOCKHEED
@@ -89,14 +90,16 @@
 Next Version:                 2304
 Next Version Available Date:  2023-04-10 06:00:00
 Next Version Start Date:      2023-04-20 06:00:00
 
 File Name:                    dgrw72_2303_eceb0273.bin
 File Size:                    8443904
 File CRC32:                   eceb0273
+Serial Number:                
+System ID:                    
 ```
 
 ### Download the database
 
 ```
 $ jdmtool download 0
 Downloading: 100%|█████████████████████████████████████████████████| 8.44M/8.44M [00:03<00:00, 2.15MB/s]
```

### Comparing `jdmtool-0.0.1/README.md` & `jdmtool-0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -45,16 +45,17 @@
 Success
 ```
 
 ### View available downloads
 
 ```
 $ jdmtool list
-ID  Name                                                                    Cycle  Start Date  End Date    Downloaded
- 0  NavData Coverage Garmin GNS 400/500 Series WAAS Americas                 2303  2023-03-23  2023-04-20            
+ID  Name                                                                    Version   Start Date  End Date    Downloaded
+ 0  NavData Coverage Garmin GNS 400/500 Series WAAS Americas                2303      2023-03-23  2023-04-20  Y         
+ 1  NavData Coverage Garmin GNS 400/500 Series WAAS Americas                2304      2023-04-20  2023-05-18            
 ```
 
 ### View detailed info
 
 ```
 $ jdmtool info 0
 Aircraft Manufacturer:        LOCKHEED
@@ -75,14 +76,16 @@
 Next Version:                 2304
 Next Version Available Date:  2023-04-10 06:00:00
 Next Version Start Date:      2023-04-20 06:00:00
 
 File Name:                    dgrw72_2303_eceb0273.bin
 File Size:                    8443904
 File CRC32:                   eceb0273
+Serial Number:                
+System ID:                    
 ```
 
 ### Download the database
 
 ```
 $ jdmtool download 0
 Downloading: 100%|█████████████████████████████████████████████████| 8.44M/8.44M [00:03<00:00, 2.15MB/s]
```

### Comparing `jdmtool-0.0.1/pyproject.toml` & `jdmtool-0.0.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jdmtool"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Dima Ryazanov", email="dima@gmail.com" },
 ]
 description = "Tool for downloading Jeppesen databases and programming Garmin aviation data cards"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `jdmtool-0.0.1/src/jdmtool/device.py` & `jdmtool-0.0.2/src/jdmtool/device.py`

 * *Files identical despite different names*

### Comparing `jdmtool-0.0.1/src/jdmtool/downloader.py` & `jdmtool-0.0.2/src/jdmtool/downloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,16 +113,14 @@
         service: ET.Element,
         progress_cb: T.Callable[[int], None],
     ) -> None:
         filename = service.findtext('./filename')
         assert '/' not in filename, filename
         assert '\\' not in filename, filename
 
-        expected_crc = int(service.findtext('./file_crc'), 16)
-
         auth = self.get_auth()
 
         with self.session.get(
             f'{self.JSUM_URL}/DownloadJDMService',
             stream=True,
             params={
                 'jdam_version': self.JDAM_VERSION,
@@ -143,12 +141,15 @@
             crc = 0
             with open(download_path, 'wb') as fd:
                 for chunk in resp.iter_content(0x1000):
                     fd.write(chunk)
                     crc = binascii.crc32(chunk, crc)
                     progress_cb(len(chunk))
 
+        expected_crc_str = service.findtext('./file_crc')
+        if expected_crc_str:
+            expected_crc = int(expected_crc_str, 16)
             if crc != expected_crc:
                 raise DownloaderException(f"Invalid checksum: expected {expected_crc:08x}, got {crc:08x}")
 
-            download_path.rename(final_path)
-            return final_path
+        download_path.rename(final_path)
+        return final_path
```

### Comparing `jdmtool-0.0.1/src/jdmtool/main.py` & `jdmtool-0.0.2/src/jdmtool/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,16 @@
     ("Next Version", "./next_display_version"),
     ("Next Version Available Date", "./next_version_avail_date"),
     ("Next Version Start Date", "./next_version_start_date"),
     (None, None),
     ("File Name", "./filename"),
     ("File Size", "./file_size"),
     ("File CRC32", "./file_crc"),
+    ("Serial Number", "./serial_number"),
+    ("System ID", "./avionics_id"),
 ]
 
 
 def with_usb(f):
     @wraps(f)
     def wrapper(*args, **kwargs):
         with usb1.USBContext() as usbcontext:
@@ -93,42 +95,42 @@
 
 def cmd_list() -> None:
     downloader = Downloader()
     services = downloader.get_services()
 
     downloads_dir = downloader.get_downloads_dir()
 
-    row_format = "{:>2}  {:<70}  {:>5}  {:<10}  {:<10}  {:<10}"
+    row_format = "{:>2}  {:<70}  {:<8}  {:<10}  {:<10}  {:<10}"
 
-    print(row_format.format("ID", "Name", "Cycle", "Start Date", "End Date", "Downloaded"))
+    print(row_format.format("ID", "Name", "Version", "Start Date", "End Date", "Downloaded"))
     for idx, service in enumerate(services):
         name: str = service.findtext('./short_desc')
-        cycle: str = service.findtext('./version')
+        version: str = service.findtext('./display_version')
         start_date: str = service.findtext('./version_start_date').split()[0]
         end_date: str = service.findtext('./version_end_date').split()[0]
         filename: str = service.findtext('./filename')
 
         downloaded = (downloads_dir / filename).exists()
 
-        print(row_format.format(idx, name, cycle, start_date, end_date, 'Y' if downloaded else ''))
+        print(row_format.format(idx, name, version, start_date, end_date, 'Y' if downloaded else ''))
 
 def cmd_info(id) -> None:
     downloader = Downloader()
 
     services = downloader.get_services()
     if id < 0 or id >= len(services):
         raise DownloaderException("Invalid download ID")
 
     service = services[id]
 
     for desc, path in DETAILED_INFO_MAP:
         if desc is None:
             print()
         else:
-            value = service.findtext(path)
+            value = service.findtext(path) or ''
             print(f'{desc+":":<30}{value}')
 
 def cmd_download(id) -> None:
     downloader = Downloader()
 
     services = downloader.get_services()
     if id < 0 or id >= len(services):
```

### Comparing `jdmtool-0.0.1/src/jdmtool.egg-info/PKG-INFO` & `jdmtool-0.0.2/src/jdmtool.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jdmtool
-Version: 0.0.1
+Version: 0.0.2
 Summary: Tool for downloading Jeppesen databases and programming Garmin aviation data cards
 Author-email: Dima Ryazanov <dima@gmail.com>
 Project-URL: Homepage, https://github.com/dimaryaz/jdmtool
 Project-URL: Bug Tracker, https://github.com/dimaryaz/jdmtool/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -59,16 +59,17 @@
 Success
 ```
 
 ### View available downloads
 
 ```
 $ jdmtool list
-ID  Name                                                                    Cycle  Start Date  End Date    Downloaded
- 0  NavData Coverage Garmin GNS 400/500 Series WAAS Americas                 2303  2023-03-23  2023-04-20            
+ID  Name                                                                    Version   Start Date  End Date    Downloaded
+ 0  NavData Coverage Garmin GNS 400/500 Series WAAS Americas                2303      2023-03-23  2023-04-20  Y         
+ 1  NavData Coverage Garmin GNS 400/500 Series WAAS Americas                2304      2023-04-20  2023-05-18            
 ```
 
 ### View detailed info
 
 ```
 $ jdmtool info 0
 Aircraft Manufacturer:        LOCKHEED
@@ -89,14 +90,16 @@
 Next Version:                 2304
 Next Version Available Date:  2023-04-10 06:00:00
 Next Version Start Date:      2023-04-20 06:00:00
 
 File Name:                    dgrw72_2303_eceb0273.bin
 File Size:                    8443904
 File CRC32:                   eceb0273
+Serial Number:                
+System ID:                    
 ```
 
 ### Download the database
 
 ```
 $ jdmtool download 0
 Downloading: 100%|█████████████████████████████████████████████████| 8.44M/8.44M [00:03<00:00, 2.15MB/s]
```

