# Comparing `tmp/umzz-0.0.0.tar.gz` & `tmp/umzz-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "umzz-0.0.0.tar", last modified: Mon Apr 10 22:53:36 2023, max compression
+gzip compressed data, was "umzz-0.0.1.tar", last modified: Fri Apr  7 04:48:51 2023, max compression
```

## Comparing `umzz-0.0.0.tar` & `umzz-0.0.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-04-10 22:53:36.130574 umzz-0.0.0/
--rw-r--r--   0 a         (1000) a         (1000)    35149 2023-04-09 22:02:13.000000 umzz-0.0.0/LICENSE
--rw-r--r--   0 a         (1000) a         (1000)     6908 2023-04-10 22:53:36.130574 umzz-0.0.0/PKG-INFO
--rw-r--r--   0 a         (1000) a         (1000)     6346 2023-04-10 22:53:14.000000 umzz-0.0.0/README.md
-drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-04-10 22:53:36.130574 umzz-0.0.0/bin/
--rw-r--r--   0 a         (1000) a         (1000)       57 2023-04-09 22:02:13.000000 umzz-0.0.0/bin/umzz
--rw-r--r--   0 a         (1000) a         (1000)       38 2023-04-10 22:53:36.130574 umzz-0.0.0/setup.cfg
--rw-r--r--   0 a         (1000) a         (1000)     1102 2023-04-10 22:53:14.000000 umzz-0.0.0/setup.py
-drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-04-10 22:53:36.130574 umzz-0.0.0/umzz/
--rw-r--r--   0 a         (1000) a         (1000)        1 2023-04-09 22:02:13.000000 umzz-0.0.0/umzz/__init__.py
--rw-r--r--   0 a         (1000) a         (1000)     2331 2023-04-09 22:02:13.000000 umzz-0.0.0/umzz/argue.py
--rw-r--r--   0 a         (1000) a         (1000)      779 2023-04-10 22:53:14.000000 umzz-0.0.0/umzz/chunky.py
--rw-r--r--   0 a         (1000) a         (1000)      801 2023-04-10 22:53:14.000000 umzz-0.0.0/umzz/cli.py
--rw-r--r--   0 a         (1000) a         (1000)     1190 2023-04-10 22:53:14.000000 umzz-0.0.0/umzz/sliding.py
--rw-r--r--   0 a         (1000) a         (1000)     1262 2023-04-09 22:02:13.000000 umzz-0.0.0/umzz/timer.py
--rw-r--r--   0 a         (1000) a         (1000)     4286 2023-04-10 22:53:14.000000 umzz-0.0.0/umzz/umzz.py
--rw-r--r--   0 a         (1000) a         (1000)       37 2023-04-10 22:53:14.000000 umzz-0.0.0/umzz/version.py
--rw-r--r--   0 a         (1000) a         (1000)    11630 2023-04-10 22:53:14.000000 umzz-0.0.0/umzz/x9mp.py
-drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-04-10 22:53:36.130574 umzz-0.0.0/umzz.egg-info/
--rw-r--r--   0 a         (1000) a         (1000)     6908 2023-04-10 22:53:36.000000 umzz-0.0.0/umzz.egg-info/PKG-INFO
--rw-r--r--   0 a         (1000) a         (1000)      304 2023-04-10 22:53:36.000000 umzz-0.0.0/umzz.egg-info/SOURCES.txt
--rw-r--r--   0 a         (1000) a         (1000)        1 2023-04-10 22:53:36.000000 umzz-0.0.0/umzz.egg-info/dependency_links.txt
--rw-r--r--   0 a         (1000) a         (1000)       78 2023-04-10 22:53:36.000000 umzz-0.0.0/umzz.egg-info/requires.txt
--rw-r--r--   0 a         (1000) a         (1000)        5 2023-04-10 22:53:36.000000 umzz-0.0.0/umzz.egg-info/top_level.txt
+drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-04-07 04:48:51.703455 umzz-0.0.1/
+-rw-r--r--   0 a         (1000) a         (1000)    35149 2023-04-03 22:01:50.000000 umzz-0.0.1/LICENSE
+-rw-r--r--   0 a         (1000) a         (1000)      734 2023-04-07 04:48:51.703455 umzz-0.0.1/PKG-INFO
+-rw-r--r--   0 a         (1000) a         (1000)      171 2023-04-03 22:01:50.000000 umzz-0.0.1/README.md
+drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-04-07 04:48:51.699455 umzz-0.0.1/bin/
+-rwxr-xr-x   0 a         (1000) a         (1000)       57 2023-04-06 22:25:11.000000 umzz-0.0.1/bin/umzz
+-rw-r--r--   0 a         (1000) a         (1000)       38 2023-04-07 04:48:51.703455 umzz-0.0.1/setup.cfg
+-rw-r--r--   0 a         (1000) a         (1000)     1104 2023-04-07 04:47:26.000000 umzz-0.0.1/setup.py
+drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-04-07 04:48:51.703455 umzz-0.0.1/umzz/
+-rw-r--r--   0 a         (1000) a         (1000)        1 2023-04-03 22:01:50.000000 umzz-0.0.1/umzz/__init__.py
+-rw-r--r--   0 a         (1000) a         (1000)     2331 2023-04-06 22:24:06.000000 umzz-0.0.1/umzz/argue.py
+-rw-r--r--   0 a         (1000) a         (1000)      732 2023-04-03 22:01:50.000000 umzz-0.0.1/umzz/chunky.py
+-rw-r--r--   0 a         (1000) a         (1000)      803 2023-04-07 04:44:53.000000 umzz-0.0.1/umzz/cli.py
+-rw-r--r--   0 a         (1000) a         (1000)     1147 2023-04-03 22:01:50.000000 umzz-0.0.1/umzz/sliding.py
+-rw-r--r--   0 a         (1000) a         (1000)     1263 2023-04-06 22:24:06.000000 umzz-0.0.1/umzz/timer.py
+-rw-r--r--   0 a         (1000) a         (1000)     3141 2023-04-07 04:44:53.000000 umzz-0.0.1/umzz/umzz.py
+-rw-r--r--   0 a         (1000) a         (1000)       39 2023-04-07 04:46:56.000000 umzz-0.0.1/umzz/version.py
+-rw-r--r--   0 a         (1000) a         (1000)    10730 2023-04-07 04:44:53.000000 umzz-0.0.1/umzz/x9mp.py
+drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-04-07 04:48:51.703455 umzz-0.0.1/umzz.egg-info/
+-rw-r--r--   0 a         (1000) a         (1000)      734 2023-04-07 04:48:51.000000 umzz-0.0.1/umzz.egg-info/PKG-INFO
+-rw-r--r--   0 a         (1000) a         (1000)      304 2023-04-07 04:48:51.000000 umzz-0.0.1/umzz.egg-info/SOURCES.txt
+-rw-r--r--   0 a         (1000) a         (1000)        1 2023-04-07 04:48:51.000000 umzz-0.0.1/umzz.egg-info/dependency_links.txt
+-rw-r--r--   0 a         (1000) a         (1000)       78 2023-04-07 04:48:51.000000 umzz-0.0.1/umzz.egg-info/requires.txt
+-rw-r--r--   0 a         (1000) a         (1000)        5 2023-04-07 04:48:51.000000 umzz-0.0.1/umzz.egg-info/top_level.txt
```

### Comparing `umzz-0.0.0/LICENSE` & `umzz-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `umzz-0.0.0/setup.py` & `umzz-0.0.1/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 #!/usr/bin/env python3
 
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     readme = fh.read()
 
-with open("umzz/version.py","r", encoding="utf-8") as latest:
-    version = latest.read().split('"')[1]
+with open("umzz/version.py", "r", encoding="utf-8") as latest:
+    version = latest.read().split("'")[1]
 
 
 setuptools.setup(
     name="umzz",
     version=version,
     author="Adrian",
     author_email="spam@iodisco.com",
-    description="SCTE-35 Injection for Adaptive Bitrate HLS",
+    description="SCTE-35  Injection for Adaptive Bitrate HLS",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/futzu/umzz",
     install_requires=[
         "new_reader >= 0.1.7",
         "iframes >= 0.0.5",
         "x9k3 >= 0.1.89",
-        "m3ufu >=0.0.67",
+        "m3ufu >=0.0.65",
         "threefive >= 2.3.81",
     ],
     scripts=["bin/umzz"],
     packages=setuptools.find_packages(),
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

### Comparing `umzz-0.0.0/umzz/argue.py` & `umzz-0.0.1/umzz/argue.py`

 * *Files identical despite different names*

### Comparing `umzz-0.0.0/umzz/chunky.py` & `umzz-0.0.1/umzz/chunky.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,28 +8,27 @@
     Class to hold hls segment tags
     for a segment.
     """
 
     def __init__(self, name, num):
         self.tags = {}
         self.name = name
-        self.file = self.name.rsplit('/',1)[1]
         self.num = num
 
     def get(self):
         """
         get returns the Chunk data formated.
         """
         this = []
         for kay, vee in self.tags.items():
             if vee is None:
                 this.append(kay)
             else:
                 this.append(f"{kay}:{vee}")
-        this.append(self.file)
+        this.append(self.name)
         this.append("")
         this = "\n".join(this)
         return this
 
     def add_tag(self, quay, val):
         """
         add_tag appends key and value for a hls tag
```

### Comparing `umzz-0.0.0/umzz/cli.py` & `umzz-0.0.1/umzz/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 from .version import version
 
 
 def cli():
     """
     cli provides one function call
     for running shari with command line args
-    Two lines of code gives you a full umzz command line tool.
+    Two lines of code gives you a full shari command line tool.
 
-     from umzz import cli
+     from shari import cli
      cli()
 
     """
     args = argue()
     if args.version:
         print(f"umzz {version}")
         sys.exit()
```

### Comparing `umzz-0.0.0/umzz/sliding.py` & `umzz-0.0.1/umzz/sliding.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 
     def pop_pane(self):
         """
         pop_pane removes the first item in self.panes
         """
         if len(self.panes) >= self.size:
             if self.delete:
-                print(vars(self.panes[0]))
                 popped = self.panes[0].name
                 print(f"deleting {popped}")
                 os.unlink(popped)
             self.panes = self.panes[1:]
 
     def push_pane(self, a_pane):
         """
```

### Comparing `umzz-0.0.0/umzz/timer.py` & `umzz-0.0.1/umzz/timer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 """
 timer.py
 """
 
 import time
 
 
-
-
 class Timer:
     """
     Timer class instances are used for
     segment duration, and live throttling.
     """
 
     def __init__(self):
@@ -49,10 +47,10 @@
         """
         throttle is called to slow segment creation
         to simulate live streaming.
         """
         self.stop(end)
         diff = round(seg_time - self.lap_time, 2)
         if diff > 0:
-            print(f"throttling {diff}")#,file=sys.stderr, end='\r')
+            print(f"throttling {diff}")  # ,file=sys.stderr, end='\r')
             time.sleep(diff)
         self.start(begin)
```

### Comparing `umzz-0.0.0/umzz/x9mp.py` & `umzz-0.0.1/umzz/x9mp.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 from iframes import IFramer
 from new_reader import reader
 from threefive import Cue
 from x9k3 import X9K3, SCTE35
 from .chunky import Chunk
 from .sliding import SlidingWindow
 from .timer import Timer
-from .version import version
 
 
 class X9MP(X9K3):
     """
     X9MP IS X9K3 modified to use multiprocessing
     for Adaptive Bit Rate.
     """
@@ -89,36 +88,14 @@
             kay = tag
             vee = None
             if ":" in tag:
                 kay, vee = tag.split(":", 1)
             chunk.add_tag(kay, vee)
             # print(kay, vee)
 
-    def _header(self):
-        """
-        header generates the m3u8 header lines
-        """
-        m3u = "#EXTM3U"
-        m3u_version = "#EXT-X-VERSION:3"
-        target = f"#EXT-X-TARGETDURATION:{int(self.args.time+1)}"
-        seq = f"#EXT-X-MEDIA-SEQUENCE:{self.media_seq}"
-        dseq = f"#EXT-X-DISCONTINUITY-SEQUENCE:{self.discontinuity_sequence}"
-        umzzv = f"#EXT-X-UMZZ-VERSION:{version}"
-        bumper = ""
-        return "\n".join(
-            [
-                m3u,
-                m3u_version,
-                target,
-                seq,
-                dseq,
-                umzzv,
-                bumper,
-            ]
-        )
     def _chk_pdt_flag(self, chunk):
         if self.args.program_date_time:
             iso8601 = f"{datetime.datetime.utcnow().isoformat()}Z"
             chunk.add_tag("#Iframe", f"{self.started}")
             chunk.add_tag("#EXT-X-PROGRAM-DATE-TIME", f"{iso8601}")
 
     def _chk_live(self, seg_time):
@@ -139,15 +116,15 @@
 
     def _write_segment(self):
         seg_file = f"seg{self.segnum}.ts"
         seg_name = self.mk_uri(self.args.output_dir, seg_file)
         seg_time = round(self.next_start - self.started, 6)
         with open(seg_name, "wb") as seg:
             seg.write(self.active_segment.getbuffer())
-        chunk = Chunk(seg_name, self.segnum)
+        chunk = Chunk(seg_file, self.segnum)
         self._mk_chunk_tags(chunk, seg_time)
         self.window.push_pane(chunk)
         self._write_m3u8()
         self._print_segment_details(seg_name, seg_time)
         self._start_next_start()
         if self.scte35.break_timer is not None:
             self.scte35.break_timer += seg_time
@@ -301,15 +278,14 @@
         else:
             self.decode()
 
     def decode_m3u8(self, manifest=None):
         """
         decode_m3u8 is called when the input file is a m3u8 playlist.
         """
-      #  if not  manifest.startswith('http') or not manifest.startswith('/'): 
         based = manifest.rsplit("/", 1)
         if len(based) > 1:
             base_uri = f"{based[0]}/"
         else:
             base_uri = ""
         last_segnum = -1
         reload = 25
@@ -325,16 +301,13 @@
                     if self.segnum == last_segnum:
                         reload -= 1
                     else:
                         reload = 25
                     last_segnum = self.segnum
                     if not line.startswith("#"):
                         if len(line):
-                            if base_uri not in line:
-                                media = base_uri + line
-                            else:
-                                media = line
+                            media = base_uri + line
                             if media not in self.media_list:
                                 self.media_list.append(media)
                                 self.media_list = self.media_list[-200:]
                                 self._tsdata = reader(media)
                                 self.decode()
```

