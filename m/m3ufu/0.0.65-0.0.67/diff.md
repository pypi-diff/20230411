# Comparing `tmp/m3ufu-0.0.65.tar.gz` & `tmp/m3ufu-0.0.67.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m3ufu-0.0.65.tar", last modified: Mon Apr  3 22:15:05 2023, max compression
+gzip compressed data, was "m3ufu-0.0.67.tar", last modified: Mon Apr 10 22:45:50 2023, max compression
```

## Comparing `m3ufu-0.0.65.tar` & `m3ufu-0.0.67.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-04-03 22:15:05.219297 m3ufu-0.0.65/
--rw-r--r--   0 a         (1000) a         (1000)    10183 2023-04-03 22:15:05.219297 m3ufu-0.0.65/PKG-INFO
--rw-r--r--   0 a         (1000) a         (1000)     9649 2023-04-03 22:14:37.000000 m3ufu-0.0.65/README.md
-drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-04-03 22:15:05.219297 m3ufu-0.0.65/bin/
--rw-r--r--   0 a         (1000) a         (1000)       54 2023-04-03 22:14:37.000000 m3ufu-0.0.65/bin/m3ufu
-drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-04-03 22:15:05.219297 m3ufu-0.0.65/m3ufu.egg-info/
--rw-r--r--   0 a         (1000) a         (1000)    10183 2023-04-03 22:15:05.000000 m3ufu-0.0.65/m3ufu.egg-info/PKG-INFO
--rw-r--r--   0 a         (1000) a         (1000)      181 2023-04-03 22:15:05.000000 m3ufu-0.0.65/m3ufu.egg-info/SOURCES.txt
--rw-r--r--   0 a         (1000) a         (1000)        1 2023-04-03 22:15:05.000000 m3ufu-0.0.65/m3ufu.egg-info/dependency_links.txt
--rw-r--r--   0 a         (1000) a         (1000)       42 2023-04-03 22:15:05.000000 m3ufu-0.0.65/m3ufu.egg-info/requires.txt
--rw-r--r--   0 a         (1000) a         (1000)        6 2023-04-03 22:15:05.000000 m3ufu-0.0.65/m3ufu.egg-info/top_level.txt
--rw-r--r--   0 a         (1000) a         (1000)    17518 2023-04-03 22:14:37.000000 m3ufu-0.0.65/m3ufu.py
--rw-r--r--   0 a         (1000) a         (1000)       38 2023-04-03 22:15:05.219297 m3ufu-0.0.65/setup.cfg
--rw-r--r--   0 a         (1000) a         (1000)      956 2023-04-03 22:14:37.000000 m3ufu-0.0.65/setup.py
+drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-04-10 22:45:50.315814 m3ufu-0.0.67/
+-rw-r--r--   0 a         (1000) a         (1000)    10183 2023-04-10 22:45:50.315814 m3ufu-0.0.67/PKG-INFO
+-rw-r--r--   0 a         (1000) a         (1000)     9649 2023-04-03 22:14:37.000000 m3ufu-0.0.67/README.md
+drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-04-10 22:45:50.315814 m3ufu-0.0.67/bin/
+-rw-r--r--   0 a         (1000) a         (1000)       54 2023-04-03 22:14:37.000000 m3ufu-0.0.67/bin/m3ufu
+drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-04-10 22:45:50.315814 m3ufu-0.0.67/m3ufu.egg-info/
+-rw-r--r--   0 a         (1000) a         (1000)    10183 2023-04-10 22:45:50.000000 m3ufu-0.0.67/m3ufu.egg-info/PKG-INFO
+-rw-r--r--   0 a         (1000) a         (1000)      181 2023-04-10 22:45:50.000000 m3ufu-0.0.67/m3ufu.egg-info/SOURCES.txt
+-rw-r--r--   0 a         (1000) a         (1000)        1 2023-04-10 22:45:50.000000 m3ufu-0.0.67/m3ufu.egg-info/dependency_links.txt
+-rw-r--r--   0 a         (1000) a         (1000)       42 2023-04-10 22:45:50.000000 m3ufu-0.0.67/m3ufu.egg-info/requires.txt
+-rw-r--r--   0 a         (1000) a         (1000)        6 2023-04-10 22:45:50.000000 m3ufu-0.0.67/m3ufu.egg-info/top_level.txt
+-rw-r--r--   0 a         (1000) a         (1000)    17744 2023-04-10 22:45:39.000000 m3ufu-0.0.67/m3ufu.py
+-rw-r--r--   0 a         (1000) a         (1000)       38 2023-04-10 22:45:50.315814 m3ufu-0.0.67/setup.cfg
+-rw-r--r--   0 a         (1000) a         (1000)      956 2023-04-03 22:14:37.000000 m3ufu-0.0.67/setup.py
```

### Comparing `m3ufu-0.0.65/PKG-INFO` & `m3ufu-0.0.67/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m3ufu
-Version: 0.0.65
+Version: 0.0.67
 Summary: M3U8 Parser with SCTE-35 Support
 Home-page: https://github.com/futzu/m3u8fu
 Author: Adrian
 Author-email: spam@iodisco.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `m3ufu-0.0.65/README.md` & `m3ufu-0.0.67/README.md`

 * *Files identical despite different names*

### Comparing `m3ufu-0.0.65/m3ufu.egg-info/PKG-INFO` & `m3ufu-0.0.67/m3ufu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m3ufu
-Version: 0.0.65
+Version: 0.0.67
 Summary: M3U8 Parser with SCTE-35 Support
 Home-page: https://github.com/futzu/m3u8fu
 Author: Adrian
 Author-email: spam@iodisco.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `m3ufu-0.0.65/m3ufu.py` & `m3ufu-0.0.67/m3ufu.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 Used to set version in setup.py
 and as an easy way to check which
 version you have installed.
 """
 
 MAJOR = "0"
 MINOR = "0"
-MAINTAINENCE = "65"
+MAINTAINENCE = "67"
 
 
 def version():
     """
     version prints the m3ufu version as a string
     """
     return f"{MAJOR}.{MINOR}.{MAINTAINENCE}"
@@ -498,19 +498,20 @@
         if isinstance(line, bytes):
             line = line.decode(errors="ignore")
             line = line.replace("\n", "").replace("\r", "")
         return line
 
     def _is_master(self, line):
         playlist = False
-        if "STREAM-INF" in line:
-            self.master = True
-            self.reload = False
-            if "URI" in line:
-                playlist = line.split('URI="')[1].split('"')[0]
+        for this in ["STREAM-INF", "EXT-X-MEDIA"]:
+            if this in line:
+                self.master = True
+                self.reload = False
+                if "URI" in line:
+                    playlist = line.split('URI="')[1].split('"')[0]
         return playlist
 
     def _set_times(self, segment):
         if not self._start:
             self._start = segment.start
         if not self._start:
             self._start = 0.0
@@ -535,19 +536,21 @@
                 os.unlink(segment.tmp)
                 del segment.tmp
 
             self.segments.append(segment)
             self._set_times(segment)
 
     def _do_media(self, line):
-        media = line
-        media = self.base_uri + media
         playlist = self._is_master(line)
         if playlist:
             media = playlist
+        else:
+            media = line
+            if self.base_uri not in line:
+               media = self.base_uri + media
         self._add_media(media)
         self.chunk = []
 
     def _parse_header(self, line):
         splitline = line.split(":", 1)
         if splitline[0] in HEADER_TAGS:
             val = ""
@@ -568,15 +571,19 @@
             return False
         line = self._clean_line(line)
         if "ENDLIST" in line:
             self.reload = False
         if not self._parse_header(line):
             self._is_master(line)
             self.chunk.append(line)
-            if not line.startswith("#") or line.startswith("#EXT-X-I-FRAME-STREAM-INF"):
+            if (
+                not line.startswith("#")
+                or line.startswith("#EXT-X-I-FRAME-STREAM-INF")
+                or line.startswith("EXT-X-MEDIA")
+            ):
                 if len(line):
                     self._do_media(line)
         return True
 
     def decode(self):
         if self.desegment and os.path.exists(self.outfile):
             os.unlink(self.outfile)
@@ -589,25 +596,23 @@
             if len(based) > 1:
                 self.base_uri = f"{based[0]}/"
         while self.reload:
             with reader(self.m3u8) as self.manifest:
                 while self.manifest:
                     if not self._parse_line():
                         break
-
                 jason = {
                     "headers": self.headers,
                 }
                 print(json.dumps(jason, indent=2))
                 if "#EXT-X-TARGETDURATION" in self.headers:
                     time.sleep(self.headers["#EXT-X-TARGETDURATION"])
 
 
 def cli():
     fu = M3uFu()
     fu._parse_args()
-
     fu.decode()
 
 
 if __name__ == "__main__":
     cli()
```

### Comparing `m3ufu-0.0.65/setup.py` & `m3ufu-0.0.67/setup.py`

 * *Files identical despite different names*

