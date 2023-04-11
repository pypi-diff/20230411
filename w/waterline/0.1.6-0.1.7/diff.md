# Comparing `tmp/waterline-0.1.6-py3-none-any.whl.zip` & `tmp/waterline-0.1.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 6216406 bytes, number of entries: 66
+Zip file size: 6216442 bytes, number of entries: 66
 -rw-rw-r--  2.0 unx      223 b- defN 23-Apr-09 20:46 waterline/__init__.py
 -rw-rw-r--  2.0 unx     1805 b- defN 23-Apr-07 00:51 waterline/jobs.py
 -rw-rw-r--  2.0 unx     2609 b- defN 23-Apr-10 05:15 waterline/pipeline.py
--rw-rw-r--  2.0 unx     1096 b- defN 23-Apr-10 15:28 waterline/run.py
--rw-rw-r--  2.0 unx     3382 b- defN 23-Apr-07 20:58 waterline/suite.py
+-rw-rw-r--  2.0 unx     1156 b- defN 23-Apr-11 21:24 waterline/run.py
+-rw-rw-r--  2.0 unx     3407 b- defN 23-Apr-11 21:22 waterline/suite.py
 -rw-rw-r--  2.0 unx     7123 b- defN 23-Apr-06 17:01 waterline/suites.py
 -rw-rw-r--  2.0 unx      641 b- defN 23-Apr-10 05:20 waterline/utils.py
 -rw-rw-r--  2.0 unx     6323 b- defN 23-Apr-10 04:50 waterline/workspace.py
 -rw-rw-r--  2.0 unx      135 b- defN 23-Apr-07 15:59 waterline/suites/__init__.py
 -rw-rw-r--  2.0 unx     1593 b- defN 23-Apr-10 04:52 waterline/suites/gap.py
 -rw-rw-r--  2.0 unx     9004 b- defN 23-Apr-10 19:44 waterline/suites/mibench.py
 -rw-rw-r--  2.0 unx     2546 b- defN 23-Apr-09 19:39 waterline/suites/nas.py
@@ -56,13 +56,13 @@
 -rwxrwxr-x  2.0 unx     2024 b- defN 23-Apr-09 20:58 waterline/suites/SPEC2017/scripts/collect_output.sh
 -rwxrwxr-x  2.0 unx      426 b- defN 23-Apr-09 20:58 waterline/suites/SPEC2017/scripts/compile.sh
 -rwxrwxr-x  2.0 unx      582 b- defN 23-Apr-09 20:58 waterline/suites/SPEC2017/scripts/install.sh
 -rwxrwxr-x  2.0 unx     1410 b- defN 23-Apr-09 20:58 waterline/suites/SPEC2017/scripts/optimization.sh
 -rwxrwxr-x  2.0 unx     2626 b- defN 23-Apr-09 20:58 waterline/suites/SPEC2017/scripts/run.sh
 -rwxrwxr-x  2.0 unx     2757 b- defN 23-Apr-09 20:58 waterline/suites/SPEC2017/scripts/setup.sh
 -rwxrwxr-x  2.0 unx      267 b- defN 23-Apr-09 20:58 waterline/suites/SPEC2017/scripts/uninstall.sh
--rw-rw-r--  2.0 unx     1057 b- defN 23-Apr-11 21:13 waterline-0.1.6.dist-info/LICENSE
--rw-rw-r--  2.0 unx      246 b- defN 23-Apr-11 21:13 waterline-0.1.6.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-11 21:13 waterline-0.1.6.dist-info/WHEEL
--rw-rw-r--  2.0 unx       10 b- defN 23-Apr-11 21:13 waterline-0.1.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     6388 b- defN 23-Apr-11 21:13 waterline-0.1.6.dist-info/RECORD
-66 files, 22293702 bytes uncompressed, 6205946 bytes compressed:  72.2%
+-rw-rw-r--  2.0 unx     1057 b- defN 23-Apr-11 21:24 waterline-0.1.7.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      246 b- defN 23-Apr-11 21:24 waterline-0.1.7.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-11 21:24 waterline-0.1.7.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       10 b- defN 23-Apr-11 21:24 waterline-0.1.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     6388 b- defN 23-Apr-11 21:24 waterline-0.1.7.dist-info/RECORD
+66 files, 22293787 bytes uncompressed, 6205982 bytes compressed:  72.2%
```

## zipnote {}

```diff
@@ -177,23 +177,23 @@
 
 Filename: waterline/suites/SPEC2017/scripts/setup.sh
 Comment: 
 
 Filename: waterline/suites/SPEC2017/scripts/uninstall.sh
 Comment: 
 
-Filename: waterline-0.1.6.dist-info/LICENSE
+Filename: waterline-0.1.7.dist-info/LICENSE
 Comment: 
 
-Filename: waterline-0.1.6.dist-info/METADATA
+Filename: waterline-0.1.7.dist-info/METADATA
 Comment: 
 
-Filename: waterline-0.1.6.dist-info/WHEEL
+Filename: waterline-0.1.7.dist-info/WHEEL
 Comment: 
 
-Filename: waterline-0.1.6.dist-info/top_level.txt
+Filename: waterline-0.1.7.dist-info/top_level.txt
 Comment: 
 
-Filename: waterline-0.1.6.dist-info/RECORD
+Filename: waterline-0.1.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## waterline/run.py

```diff
@@ -1,13 +1,13 @@
 from dataclasses import dataclass
 from pathlib import Path
 import subprocess
 import time
 import waterline.utils
-
+import os
 
 class RunConfiguration:
     def __init__(self, name, args=[], env={}, cwd=None):
         self.name = name
         self.args = args
         self.env = env
         self.cwd = None
@@ -21,20 +21,22 @@
 class Runner:
     name = "time"
 
     def run(self, workspace, config: RunConfiguration, binary: Path):
         """Run the benchmark, and return the metric. By default, it returns the execution time"""
         assert binary.exists()
 
-        with waterline.utils.cd(config.cwd):
+
+        cwd = os.getcwd() if config.cwd is None else config.cwd
+        with waterline.utils.cd(cwd):
             start = time.time()
             proc = subprocess.Popen(
                 [binary, *config.args],
                 stdout=subprocess.DEVNULL,
                 # stderr=subprocess.DEVNULL,
                 env=config.env,
-                cwd=config.cwd,
+                cwd=cwd,
             )
             res = proc.wait()
             print(res)
             end = time.time()
         return end - start
```

## waterline/suite.py

```diff
@@ -103,14 +103,14 @@
 
     def link_bitcode(self, bitcode: Path, destination: Path):
         """
         Compile a bitcode file to an object file, then link the object file to the destination
         using `self.link()`
         """
         object = bitcode.parent / (bitcode.stem + ".o")
-        self.shell("llc", "-O3", bitcode, "--filetype=obj", "-o", object)
+        self.shell("llc", "-relocation-model=pic", "-O3", bitcode, "--filetype=obj", "-o", object)
 
         self.link(object, destination)
         pass
 
     def shell(self, *args):
         self.suite.workspace.shell(*args)
```

## Comparing `waterline-0.1.6.dist-info/LICENSE` & `waterline-0.1.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `waterline-0.1.6.dist-info/RECORD` & `waterline-0.1.7.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 waterline/__init__.py,sha256=4UwrTIE53TLXgBtiS8bm9QI3FH75W1AZM4e9XcpCRfo,223
 waterline/jobs.py,sha256=0yYmMT-BK_TzrGRzBbZBmLIjwxxHddCSPHVKn8ZUjXU,1805
 waterline/pipeline.py,sha256=A-9hqHRtpKrIGo2iEFfv9Cw0CdNF6NqihuAXhHNM-RU,2609
-waterline/run.py,sha256=1Wjh5cd9DqHqF_megqYjYbeoMjwS3w0XpIMV8_vMv70,1096
-waterline/suite.py,sha256=HAfny2WJoxOUTcfcHI3MwN_PXiFL5MCOED39RjpA5C8,3382
+waterline/run.py,sha256=5Y8UMl46LKxson_A99hUzgq6JdpGgCRCJlrzkATx6NA,1156
+waterline/suite.py,sha256=S5EO-iOVzjXnOzyMi5DAEvvR3-N15DwHeH4114ZrdyM,3407
 waterline/suites.py,sha256=cBJ3KU1Mzzq5LkuCisuvCwcnU9xjPontHEFYYxCtsz0,7123
 waterline/utils.py,sha256=G7a0Bqt8ibml4o7airQ5vL6fkdtFWpnZ8-AocHlk7mA,641
 waterline/workspace.py,sha256=KRIwQEqpmCcHxJgcPWZ_bYKm_1HpMFH7igGUxMJg1UA,6323
 waterline/suites/__init__.py,sha256=ETK4N7n6M9dzDASROaNAthTPdUl97qw2lbW_q5sIgrQ,135
 waterline/suites/gap.py,sha256=XbLPn0mMb0JxzH1yVT3J98Y-cCJa_06wu55ABmL1_nY,1593
 waterline/suites/mibench.py,sha256=zX0u-rcmYbtEww2n01ElUEICqn-bl-hiWd_M8w0ac7I,9004
 waterline/suites/nas.py,sha256=WLqeP3CPqUFhZt5ECEpjDGYJA61MOSK2-cn7Vx1suzU,2546
@@ -55,12 +55,12 @@
 waterline/suites/SPEC2017/scripts/collect_output.sh,sha256=ggAiKroVgHC5rq26J3eVa0fW4FFaeiLsG6BUfWZ2weY,2024
 waterline/suites/SPEC2017/scripts/compile.sh,sha256=9VpgIqHmLgfKjjibS0i4xFkNh6dgEgrWqKyyK-MiceI,426
 waterline/suites/SPEC2017/scripts/install.sh,sha256=3fQeOYVldVYHHfh6WgQLJeKot3J0ijMUQ7nz8YUE1Vw,582
 waterline/suites/SPEC2017/scripts/optimization.sh,sha256=6qHL1B3J-M5M80RJp2E7W9FB_jmNS6grcRYKOgOo5jk,1410
 waterline/suites/SPEC2017/scripts/run.sh,sha256=zWKgeZ_pteRG3Quks7e8KKbkQbz38CWHBBWTVUzOR68,2626
 waterline/suites/SPEC2017/scripts/setup.sh,sha256=FnVDLvabQm6CVwxl0y0rA5g6V5j5VXLm2ZZVIO2xZI8,2757
 waterline/suites/SPEC2017/scripts/uninstall.sh,sha256=0szAcj1MraRZ0QjGdL6aLq8QkxKdFm9qoTAaKdhOeUY,267
-waterline-0.1.6.dist-info/LICENSE,sha256=UveJQplGBXBAOAqKBm_4SQ2XE2VBHPRJDIuVa9829uc,1057
-waterline-0.1.6.dist-info/METADATA,sha256=upsltlAyPFUcI0Lfd1898wONgsqkt_fsqUCgdccphxY,246
-waterline-0.1.6.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-waterline-0.1.6.dist-info/top_level.txt,sha256=ptFfPeDDWWfu4ZroUwKjceRrASyf4j3zXvL1UxLuLTk,10
-waterline-0.1.6.dist-info/RECORD,,
+waterline-0.1.7.dist-info/LICENSE,sha256=UveJQplGBXBAOAqKBm_4SQ2XE2VBHPRJDIuVa9829uc,1057
+waterline-0.1.7.dist-info/METADATA,sha256=14ZR-NsgpFiNGeCCLTIDAHnqEDx1p4wQNcb3_4p1wZQ,246
+waterline-0.1.7.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+waterline-0.1.7.dist-info/top_level.txt,sha256=ptFfPeDDWWfu4ZroUwKjceRrASyf4j3zXvL1UxLuLTk,10
+waterline-0.1.7.dist-info/RECORD,,
```

