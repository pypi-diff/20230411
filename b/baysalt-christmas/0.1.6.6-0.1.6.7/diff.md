# Comparing `tmp/baysalt_christmas-0.1.6.6.tar.gz` & `tmp/baysalt_christmas-0.1.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baysalt_christmas-0.1.6.6.tar", last modified: Fri Mar 31 22:02:12 2023, max compression
+gzip compressed data, was "baysalt_christmas-0.1.6.7.tar", last modified: Tue Apr 11 06:12:35 2023, max compression
```

## Comparing `baysalt_christmas-0.1.6.6.tar` & `baysalt_christmas-0.1.6.7.tar`

### file list

```diff
@@ -1,29 +1,32 @@
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-03-31 22:02:12.755124 baysalt_christmas-0.1.6.6/
--rw-r--r--   0 christmas   (501) staff       (20)    10244 2023-03-25 19:21:48.000000 baysalt_christmas-0.1.6.6/.DS_Store
--rw-r--r--   0 christmas   (501) staff       (20)      117 2023-03-25 19:22:27.000000 baysalt_christmas-0.1.6.6/MANIFEST.in
--rw-r--r--   0 christmas   (501) staff       (20)     4095 2023-03-31 22:02:12.754988 baysalt_christmas-0.1.6.6/PKG-INFO
--rw-r--r--   0 christmas   (501) staff       (20)     3732 2023-03-29 03:30:38.000000 baysalt_christmas-0.1.6.6/README.md
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-03-31 22:02:12.751556 baysalt_christmas-0.1.6.6/baysalt_christmas.egg-info/
--rw-r--r--   0 christmas   (501) staff       (20)     4095 2023-03-31 22:02:12.000000 baysalt_christmas-0.1.6.6/baysalt_christmas.egg-info/PKG-INFO
--rw-r--r--   0 christmas   (501) staff       (20)      584 2023-03-31 22:02:12.000000 baysalt_christmas-0.1.6.6/baysalt_christmas.egg-info/SOURCES.txt
--rw-r--r--   0 christmas   (501) staff       (20)        1 2023-03-31 22:02:12.000000 baysalt_christmas-0.1.6.6/baysalt_christmas.egg-info/dependency_links.txt
--rw-r--r--   0 christmas   (501) staff       (20)       21 2023-03-31 22:02:12.000000 baysalt_christmas-0.1.6.6/baysalt_christmas.egg-info/requires.txt
--rw-r--r--   0 christmas   (501) staff       (20)       10 2023-03-31 22:02:12.000000 baysalt_christmas-0.1.6.6/baysalt_christmas.egg-info/top_level.txt
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-03-31 22:02:12.752795 baysalt_christmas-0.1.6.6/christmas/
--rw-r--r--   0 christmas   (501) staff       (20)     1895 2023-03-25 02:55:02.000000 baysalt_christmas-0.1.6.6/christmas/S_DateTime.py
--rw-r--r--   0 christmas   (501) staff       (20)      346 2023-03-25 02:55:55.000000 baysalt_christmas-0.1.6.6/christmas/__init__.py
--rw-r--r--   0 christmas   (501) staff       (20)     3991 2023-03-31 22:01:41.000000 baysalt_christmas-0.1.6.6/christmas/commonCode.py
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-03-31 22:02:12.754361 baysalt_christmas-0.1.6.6/christmas/mncPy/
--rw-r--r--   0 christmas   (501) staff       (20)     1203 2023-03-03 04:53:20.000000 baysalt_christmas-0.1.6.6/christmas/mncPy/.gitignore
--rw-r--r--   0 christmas   (501) staff       (20)    35149 2023-03-03 04:53:20.000000 baysalt_christmas-0.1.6.6/christmas/mncPy/LICENSE
--rw-r--r--   0 christmas   (501) staff       (20)      239 2023-03-03 08:53:41.000000 baysalt_christmas-0.1.6.6/christmas/mncPy/__init__.py
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-03-31 22:02:12.754672 baysalt_christmas-0.1.6.6/christmas/mncPy/__pycache__/
--rw-r--r--   0 christmas   (501) staff       (20)      228 2023-03-26 18:28:05.000000 baysalt_christmas-0.1.6.6/christmas/mncPy/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 christmas   (501) staff       (20)    12920 2023-03-09 13:49:40.000000 baysalt_christmas-0.1.6.6/christmas/mncPy/common.py
--rw-r--r--   0 christmas   (501) staff       (20)     4347 2023-03-09 14:00:22.000000 baysalt_christmas-0.1.6.6/christmas/mncPy/compress.py
--rw-r--r--   0 christmas   (501) staff       (20)     3554 2023-03-29 02:58:20.000000 baysalt_christmas-0.1.6.6/christmas/processBar.py
--rw-r--r--   0 christmas   (501) staff       (20)     3473 2023-03-27 04:47:12.000000 baysalt_christmas-0.1.6.6/christmas/read_conf.py
--rw-r--r--   0 christmas   (501) staff       (20)     1506 2022-12-07 09:44:40.000000 baysalt_christmas-0.1.6.6/christmas/server_info.py
--rw-r--r--   0 christmas   (501) staff       (20)      456 2023-03-25 18:44:30.000000 baysalt_christmas-0.1.6.6/run_twine.py
--rw-r--r--   0 christmas   (501) staff       (20)       38 2023-03-31 22:02:12.755177 baysalt_christmas-0.1.6.6/setup.cfg
--rw-r--r--   0 christmas   (501) staff       (20)      796 2023-03-31 22:02:03.000000 baysalt_christmas-0.1.6.6/setup.py
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-04-11 06:12:35.336669 baysalt_christmas-0.1.6.7/
+-rw-r--r--   0 christmas   (501) staff       (20)    10244 2023-04-09 17:00:21.000000 baysalt_christmas-0.1.6.7/.DS_Store
+-rw-r--r--   0 christmas   (501) staff       (20)      117 2023-03-25 19:22:27.000000 baysalt_christmas-0.1.6.7/MANIFEST.in
+-rw-r--r--   0 christmas   (501) staff       (20)     4095 2023-04-11 06:12:35.336542 baysalt_christmas-0.1.6.7/PKG-INFO
+-rw-r--r--   0 christmas   (501) staff       (20)     3732 2023-03-29 03:30:38.000000 baysalt_christmas-0.1.6.7/README.md
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-04-11 06:12:35.331130 baysalt_christmas-0.1.6.7/baysalt_christmas.egg-info/
+-rw-r--r--   0 christmas   (501) staff       (20)     4095 2023-04-11 06:12:35.000000 baysalt_christmas-0.1.6.7/baysalt_christmas.egg-info/PKG-INFO
+-rw-r--r--   0 christmas   (501) staff       (20)      707 2023-04-11 06:12:35.000000 baysalt_christmas-0.1.6.7/baysalt_christmas.egg-info/SOURCES.txt
+-rw-r--r--   0 christmas   (501) staff       (20)        1 2023-04-11 06:12:35.000000 baysalt_christmas-0.1.6.7/baysalt_christmas.egg-info/dependency_links.txt
+-rw-r--r--   0 christmas   (501) staff       (20)       21 2023-04-11 06:12:35.000000 baysalt_christmas-0.1.6.7/baysalt_christmas.egg-info/requires.txt
+-rw-r--r--   0 christmas   (501) staff       (20)       10 2023-04-11 06:12:35.000000 baysalt_christmas-0.1.6.7/baysalt_christmas.egg-info/top_level.txt
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-04-11 06:12:35.332861 baysalt_christmas-0.1.6.7/christmas/
+-rw-r--r--   0 christmas   (501) staff       (20)     1895 2023-03-25 02:55:02.000000 baysalt_christmas-0.1.6.7/christmas/S_DateTime.py
+-rw-r--r--   0 christmas   (501) staff       (20)      412 2023-04-11 06:11:25.000000 baysalt_christmas-0.1.6.7/christmas/__init__.py
+-rw-r--r--   0 christmas   (501) staff       (20)     4154 2023-04-11 05:36:23.000000 baysalt_christmas-0.1.6.7/christmas/commonCode.py
+-rw-r--r--   0 christmas   (501) staff       (20)     1619 2023-04-11 06:11:05.000000 baysalt_christmas-0.1.6.7/christmas/cprintf.py
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-04-11 06:12:35.334315 baysalt_christmas-0.1.6.7/christmas/mncPy/
+-rw-r--r--   0 christmas   (501) staff       (20)     1203 2023-03-03 04:53:20.000000 baysalt_christmas-0.1.6.7/christmas/mncPy/.gitignore
+-rw-r--r--   0 christmas   (501) staff       (20)    35149 2023-03-03 04:53:20.000000 baysalt_christmas-0.1.6.7/christmas/mncPy/LICENSE
+-rw-r--r--   0 christmas   (501) staff       (20)      239 2023-03-03 08:53:41.000000 baysalt_christmas-0.1.6.7/christmas/mncPy/__init__.py
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-04-11 06:12:35.336192 baysalt_christmas-0.1.6.7/christmas/mncPy/__pycache__/
+-rw-r--r--   0 christmas   (501) staff       (20)      228 2023-03-26 18:28:05.000000 baysalt_christmas-0.1.6.7/christmas/mncPy/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 christmas   (501) staff       (20)     8964 2023-04-08 09:55:17.000000 baysalt_christmas-0.1.6.7/christmas/mncPy/__pycache__/common.cpython-39.pyc
+-rw-r--r--   0 christmas   (501) staff       (20)     3411 2023-04-08 09:55:17.000000 baysalt_christmas-0.1.6.7/christmas/mncPy/__pycache__/compress.cpython-39.pyc
+-rw-r--r--   0 christmas   (501) staff       (20)    12920 2023-03-09 13:49:40.000000 baysalt_christmas-0.1.6.7/christmas/mncPy/common.py
+-rw-r--r--   0 christmas   (501) staff       (20)     4347 2023-03-09 14:00:22.000000 baysalt_christmas-0.1.6.7/christmas/mncPy/compress.py
+-rw-r--r--   0 christmas   (501) staff       (20)     3554 2023-03-29 02:58:20.000000 baysalt_christmas-0.1.6.7/christmas/processBar.py
+-rw-r--r--   0 christmas   (501) staff       (20)     3473 2023-03-27 04:47:12.000000 baysalt_christmas-0.1.6.7/christmas/read_conf.py
+-rw-r--r--   0 christmas   (501) staff       (20)     1506 2022-12-07 09:44:40.000000 baysalt_christmas-0.1.6.7/christmas/server_info.py
+-rw-r--r--   0 christmas   (501) staff       (20)      456 2023-03-25 18:44:30.000000 baysalt_christmas-0.1.6.7/run_twine.py
+-rw-r--r--   0 christmas   (501) staff       (20)       38 2023-04-11 06:12:35.336717 baysalt_christmas-0.1.6.7/setup.cfg
+-rw-r--r--   0 christmas   (501) staff       (20)      796 2023-04-11 06:12:28.000000 baysalt_christmas-0.1.6.7/setup.py
```

### Comparing `baysalt_christmas-0.1.6.6/.DS_Store` & `baysalt_christmas-0.1.6.7/.DS_Store`

 * *Files 11% similar despite different names*

```diff
@@ -266,37 +266,37 @@
 00001090: c441 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
 000010a0: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
 000010b0: 636f 6d70 0000 0000 0000 0000 0000 001a  comp............
 000010c0: 0062 0061 0079 0073 0061 006c 0074 005f  .b.a.y.s.a.l.t._
 000010d0: 0063 0068 0072 0069 0073 0074 006d 0061  .c.h.r.i.s.t.m.a
 000010e0: 0073 002e 0065 0067 0067 002d 0069 006e  .s...e.g.g.-.i.n
 000010f0: 0066 006f 6c67 3153 636f 6d70 0000 0000  .f.olg1Scomp....
-00001100: 0000 0422 0000 001a 0062 0061 0079 0073  ...".....b.a.y.s
+00001100: 0000 1267 0000 001a 0062 0061 0079 0073  ...g.....b.a.y.s
 00001110: 0061 006c 0074 005f 0063 0068 0072 0069  .a.l.t._.c.h.r.i
 00001120: 0073 0074 006d 0061 0073 002e 0065 0067  .s.t.m.a.s...e.g
 00001130: 0067 002d 0069 006e 0066 006f 6d6f 4444  .g.-.i.n.f.omoDD
-00001140: 626c 6f62 0000 0008 2502 913d bae7 c441  blob....%..=...A
+00001140: 626c 6f62 0000 0008 234e 55f2 c7eb c441  blob....#NU....A
 00001150: 0000 001a 0062 0061 0079 0073 0061 006c  .....b.a.y.s.a.l
 00001160: 0074 005f 0063 0068 0072 0069 0073 0074  .t._.c.h.r.i.s.t
 00001170: 006d 0061 0073 002e 0065 0067 0067 002d  .m.a.s...e.g.g.-
 00001180: 0069 006e 0066 006f 6d6f 6444 626c 6f62  .i.n.f.omodDblob
-00001190: 0000 0008 04af e0b3 80dd c441 0000 001a  ...........A....
+00001190: 0000 0008 234e 55f2 c7eb c441 0000 001a  ....#NU....A....
 000011a0: 0062 0061 0079 0073 0061 006c 0074 005f  .b.a.y.s.a.l.t._
 000011b0: 0063 0068 0072 0069 0073 0074 006d 0061  .c.h.r.i.s.t.m.a
 000011c0: 0073 002e 0065 0067 0067 002d 0069 006e  .s...e.g.g.-.i.n
 000011d0: 0066 006f 7068 3153 636f 6d70 0000 0000  .f.oph1Scomp....
 000011e0: 0000 5000 0000 0005 0062 0075 0069 006c  ..P......b.u.i.l
-000011f0: 0064 6c67 3153 636f 6d70 0000 0000 0000  .dlg1Scomp......
-00001200: 78c6 0000 0005 0062 0075 0069 006c 0064  x......b.u.i.l.d
-00001210: 6d6f 4444 626c 6f62 0000 0008 0126 ad3d  moDDblob.....&.=
-00001220: bae7 c441 0000 0005 0062 0075 0069 006c  ...A.....b.u.i.l
-00001230: 0064 6d6f 6444 626c 6f62 0000 0008 0126  .dmodDblob.....&
-00001240: ad3d bae7 c441 0000 0005 0062 0075 0069  .=...A.....b.u.i
+000011f0: 0064 6c67 3153 636f 6d70 0000 0000 0001  .dlg1Scomp......
+00001200: 0cf3 0000 0005 0062 0075 0069 006c 0064  .......b.u.i.l.d
+00001210: 6d6f 4444 626c 6f62 0000 0008 eca3 73f2  moDDblob......s.
+00001220: c7eb c441 0000 0005 0062 0075 0069 006c  ...A.....b.u.i.l
+00001230: 0064 6d6f 6444 626c 6f62 0000 0008 eca3  .dmodDblob......
+00001240: 73f2 c7eb c441 0000 0005 0062 0075 0069  s....A.....b.u.i
 00001250: 006c 0064 7068 3153 636f 6d70 0000 0000  .l.dph1Scomp....
-00001260: 0000 d000 0000 0009 0063 0068 0072 0069  .........c.h.r.i
+00001260: 0001 8000 0000 0009 0063 0068 0072 0069  .........c.h.r.i
 00001270: 0073 0074 006d 0061 0073 6277 7370 626c  .s.t.m.a.sbwspbl
 00001280: 6f62 0000 00b9 6270 6c69 7374 3030 d601  ob....bplist00..
 00001290: 0203 0405 0607 0807 080b 085d 5368 6f77  ...........]Show
 000012a0: 5374 6174 7573 4261 725b 5368 6f77 546f  StatusBar[ShowTo
 000012b0: 6f6c 6261 725b 5368 6f77 5461 6256 6965  olbar[ShowTabVie
 000012c0: 775f 1014 436f 6e74 6169 6e65 7253 686f  w_..ContainerSho
 000012d0: 7753 6964 6562 6172 5c57 696e 646f 7742  wSidebar\WindowB
@@ -306,15 +306,15 @@
 00001310: 7d09 0815 232f 3b52 5f6b 6c6d 6e6f 8b00  }...#/;R_klmno..
 00001320: 0000 0000 0001 0100 0000 0000 0000 0d00  ................
 00001330: 0000 0000 0000 0000 0000 0000 0000 8c00  ................
 00001340: 0000 0900 6300 6800 7200 6900 7300 7400  ....c.h.r.i.s.t.
 00001350: 6d00 6100 7364 7363 6c62 6f6f 6c00 0000  m.a.sdsclbool...
 00001360: 0009 0063 0068 0072 0069 0073 0074 006d  ...c.h.r.i.s.t.m
 00001370: 0061 0073 6c67 3153 636f 6d70 0000 0000  .a.slg1Scomp....
-00001380: 0001 2b17 0000 0009 0063 0068 0072 0069  ..+......c.h.r.i
+00001380: 0001 7f69 0000 0009 0063 0068 0072 0069  ...i.....c.h.r.i
 00001390: 0073 0074 006d 0061 0073 6c73 7643 626c  .s.t.m.a.slsvCbl
 000013a0: 6f62 0000 0316 6270 6c69 7374 3030 d801  ob....bplist00..
 000013b0: 0203 0405 0607 0809 0a0b 1956 5758 0a5f  ...........VWX._
 000013c0: 1012 7669 6577 4f70 7469 6f6e 7356 6572  ..viewOptionsVer
 000013d0: 7369 6f6e 5f10 0f73 686f 7749 636f 6e50  sion_..showIconP
 000013e0: 7265 7669 6577 5763 6f6c 756d 6e73 5f10  reviewWcolumns_.
 000013f0: 1163 616c 6375 6c61 7465 416c 6c53 697a  .calculateAllSiz
@@ -400,30 +400,30 @@
 000018f0: 5701 5901 5a01 6301 6501 6601 6801 6901  W.Y.Z.c.e.f.h.i.
 00001900: 7201 7401 7501 7601 7f01 8101 8201 8401  r.t.u.v.........
 00001910: 8501 8e01 9001 9101 9401 9501 9e01 a001  ................
 00001920: a101 a201 a301 ac01 b101 ba00 0000 0000  ................
 00001930: 0002 0100 0000 0000 0000 4900 0000 0000  ..........I.....
 00001940: 0000 0000 0000 0000 0001 bb00 0000 0900  ................
 00001950: 6300 6800 7200 6900 7300 7400 6d00 6100  c.h.r.i.s.t.m.a.
-00001960: 736d 6f44 4462 6c6f 6200 0000 0861 3a27  smoDDblob....a:'
-00001970: adb9 e7c4 4100 0000 0900 6300 6800 7200  ....A.....c.h.r.
+00001960: 736d 6f44 4462 6c6f 6200 0000 08f2 d1da  smoDDblob.......
+00001970: e2c7 ebc4 4100 0000 0900 6300 6800 7200  ....A.....c.h.r.
 00001980: 6900 7300 7400 6d00 6100 736d 6f64 4462  i.s.t.m.a.smodDb
-00001990: 6c6f 6200 0000 0861 3a27 adb9 e7c4 4100  lob....a:'....A.
+00001990: 6c6f 6200 0000 08f2 d1da e2c7 ebc4 4100  lob...........A.
 000019a0: 0000 0900 6300 6800 7200 6900 7300 7400  ....c.h.r.i.s.t.
 000019b0: 6d00 6100 7370 6831 5363 6f6d 7000 0000  m.a.sph1Scomp...
-000019c0: 0000 01d0 0000 0000 0900 6300 6800 7200  ..........c.h.r.
+000019c0: 0000 0240 0000 0000 0900 6300 6800 7200  ...@......c.h.r.
 000019d0: 6900 7300 7400 6d00 6100 7376 5372 6e6c  i.s.t.m.a.svSrnl
 000019e0: 6f6e 6700 0000 0100 0000 0400 6400 6900  ong.........d.i.
 000019f0: 7300 746c 6731 5363 6f6d 7000 0000 0000  s.tlg1Scomp.....
-00001a00: 0060 7b00 0000 0400 6400 6900 7300 746d  .`{.....d.i.s.tm
-00001a10: 6f44 4462 6c6f 6200 0000 08fa c2b0 3dba  oDDblob.......=.
-00001a20: e7c4 4100 0000 0400 6400 6900 7300 746d  ..A.....d.i.s.tm
-00001a30: 6f64 4462 6c6f 6200 0000 08fa c2b0 3dba  odDblob.......=.
-00001a40: e7c4 4100 0000 0400 6400 6900 7300 7470  ..A.....d.i.s.tp
-00001a50: 6831 5363 6f6d 7000 0000 0000 0070 0000  h1Scomp......p..
+00001a00: 00de 7100 0000 0400 6400 6900 7300 746d  ..q.....d.i.s.tm
+00001a10: 6f44 4462 6c6f 6200 0000 0846 6378 f2c7  oDDblob....Fcx..
+00001a20: ebc4 4100 0000 0400 6400 6900 7300 746d  ..A.....d.i.s.tm
+00001a30: 6f64 4462 6c6f 6200 0000 0846 6378 f2c7  odDblob....Fcx..
+00001a40: ebc4 4100 0000 0400 6400 6900 7300 7470  ..A.....d.i.s.tp
+00001a50: 6831 5363 6f6d 7000 0000 0000 00f0 0000  h1Scomp.........
 00001a60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001a70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001a80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001a90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001aa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001ab0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001ac0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `baysalt_christmas-0.1.6.6/PKG-INFO` & `baysalt_christmas-0.1.6.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baysalt_christmas
-Version: 0.1.6.6
+Version: 0.1.6.7
 Summary: Some simple tools for Christmas
 Author: Christmas
 Author-email: 273519355@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `baysalt_christmas-0.1.6.6/README.md` & `baysalt_christmas-0.1.6.7/README.md`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.6.6/baysalt_christmas.egg-info/PKG-INFO` & `baysalt_christmas-0.1.6.7/baysalt_christmas.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baysalt-christmas
-Version: 0.1.6.6
+Version: 0.1.6.7
 Summary: Some simple tools for Christmas
 Author: Christmas
 Author-email: 273519355@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `baysalt_christmas-0.1.6.6/baysalt_christmas.egg-info/SOURCES.txt` & `baysalt_christmas-0.1.6.7/baysalt_christmas.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -7,16 +7,19 @@
 baysalt_christmas.egg-info/SOURCES.txt
 baysalt_christmas.egg-info/dependency_links.txt
 baysalt_christmas.egg-info/requires.txt
 baysalt_christmas.egg-info/top_level.txt
 christmas/S_DateTime.py
 christmas/__init__.py
 christmas/commonCode.py
+christmas/cprintf.py
 christmas/processBar.py
 christmas/read_conf.py
 christmas/server_info.py
 christmas/mncPy/.gitignore
 christmas/mncPy/LICENSE
 christmas/mncPy/__init__.py
 christmas/mncPy/common.py
 christmas/mncPy/compress.py
-christmas/mncPy/__pycache__/__init__.cpython-39.pyc
+christmas/mncPy/__pycache__/__init__.cpython-39.pyc
+christmas/mncPy/__pycache__/common.cpython-39.pyc
+christmas/mncPy/__pycache__/compress.cpython-39.pyc
```

### Comparing `baysalt_christmas-0.1.6.6/christmas/S_DateTime.py` & `baysalt_christmas-0.1.6.7/christmas/S_DateTime.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.6.6/christmas/commonCode.py` & `baysalt_christmas-0.1.6.7/christmas/commonCode.py`

 * *Files 3% similar despite different names*

```diff
@@ -89,14 +89,24 @@
     :param path: 文件夹路径
     :return:
     """
     if not os.path.exists(path):
         os.makedirs(path)
 
 
+def makedirs(path):
+    """
+    创建文件夹
+    :param path: 文件夹路径
+    :return:
+    """
+    if not os.path.exists(path):
+        os.makedirs(path)
+
+
 class FtpUploadTracker:
     sizeWritten = 0
     totalSize = 0
     lastShownPercent = 0
 
     def __init__(self, totalSize, sizeWritten):
         self.totalSize = totalSize
```

### Comparing `baysalt_christmas-0.1.6.6/christmas/mncPy/.gitignore` & `baysalt_christmas-0.1.6.7/christmas/mncPy/.gitignore`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.6.6/christmas/mncPy/LICENSE` & `baysalt_christmas-0.1.6.7/christmas/mncPy/LICENSE`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.6.6/christmas/mncPy/common.py` & `baysalt_christmas-0.1.6.7/christmas/mncPy/common.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.6.6/christmas/mncPy/compress.py` & `baysalt_christmas-0.1.6.7/christmas/mncPy/compress.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.6.6/christmas/processBar.py` & `baysalt_christmas-0.1.6.7/christmas/processBar.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.6.6/christmas/read_conf.py` & `baysalt_christmas-0.1.6.7/christmas/read_conf.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.6.6/christmas/server_info.py` & `baysalt_christmas-0.1.6.7/christmas/server_info.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.6.6/setup.py` & `baysalt_christmas-0.1.6.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="baysalt_christmas",
-    version="0.1.6.6",
+    version="0.1.6.7",
     author="Christmas",
     author_email="273519355@qq.com",
     description="Some simple tools for Christmas",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     include_package_data=True,
```

