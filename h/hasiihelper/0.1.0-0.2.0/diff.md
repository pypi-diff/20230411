# Comparing `tmp/hasiihelper-0.1.0.tar.gz` & `tmp/hasiihelper-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hasiihelper-0.1.0.tar", last modified: Sun Mar 26 19:00:21 2023, max compression
+gzip compressed data, was "hasiihelper-0.2.0.tar", last modified: Tue Apr 11 20:37:40 2023, max compression
```

## Comparing `hasiihelper-0.1.0.tar` & `hasiihelper-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-03-26 19:00:21.210011 hasiihelper-0.1.0/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    34523 2023-03-26 16:04:54.000000 hasiihelper-0.1.0/LICENSE
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1662 2023-03-26 19:00:21.209886 hasiihelper-0.1.0/PKG-INFO
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1295 2023-03-26 18:57:07.000000 hasiihelper-0.1.0/README.md
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-03-26 19:00:21.209159 hasiihelper-0.1.0/hasiihelper/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      705 2022-04-25 21:01:57.000000 hasiihelper-0.1.0/hasiihelper/Dimensions.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      694 2021-03-31 01:16:10.000000 hasiihelper-0.1.0/hasiihelper/Position.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5601 2023-03-08 18:43:42.000000 hasiihelper-0.1.0/hasiihelper/SemanticVersion.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1832 2022-11-20 03:20:07.000000 hasiihelper-0.1.0/hasiihelper/Singleton.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2362 2023-03-26 18:03:07.000000 hasiihelper-0.1.0/hasiihelper/UnitTestBase.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-02-08 21:59:24.000000 hasiihelper-0.1.0/hasiihelper/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 hasiihelper-0.1.0/hasiihelper/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-03-26 19:00:21.209735 hasiihelper-0.1.0/hasiihelper.egg-info/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1662 2023-03-26 19:00:21.000000 hasiihelper-0.1.0/hasiihelper.egg-info/PKG-INFO
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      379 2023-03-26 19:00:21.000000 hasiihelper-0.1.0/hasiihelper.egg-info/SOURCES.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2023-03-26 19:00:21.000000 hasiihelper-0.1.0/hasiihelper.egg-info/dependency_links.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       19 2023-03-26 19:00:21.000000 hasiihelper-0.1.0/hasiihelper.egg-info/requires.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       12 2023-03-26 19:00:21.000000 hasiihelper-0.1.0/hasiihelper.egg-info/top_level.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2023-03-26 19:00:21.210041 hasiihelper-0.1.0/setup.cfg
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      806 2023-03-26 16:04:40.000000 hasiihelper-0.1.0/setup.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-11 20:37:40.266367 hasiihelper-0.2.0/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    34523 2023-03-26 16:04:54.000000 hasiihelper-0.2.0/LICENSE
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2030 2023-04-11 20:37:40.266243 hasiihelper-0.2.0/PKG-INFO
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1663 2023-04-11 01:32:43.000000 hasiihelper-0.2.0/README.md
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-11 20:37:40.265457 hasiihelper-0.2.0/hasiihelper/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      705 2022-04-25 21:01:57.000000 hasiihelper-0.2.0/hasiihelper/Dimensions.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      694 2021-03-31 01:16:10.000000 hasiihelper-0.2.0/hasiihelper/Position.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1123 2023-04-04 01:18:09.000000 hasiihelper-0.2.0/hasiihelper/ResourceManager.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5601 2023-03-08 18:43:42.000000 hasiihelper-0.2.0/hasiihelper/SemanticVersion.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1832 2022-11-20 03:20:07.000000 hasiihelper-0.2.0/hasiihelper/Singleton.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2369 2023-04-10 20:04:39.000000 hasiihelper-0.2.0/hasiihelper/UnitTestBase.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-02-08 21:59:24.000000 hasiihelper-0.2.0/hasiihelper/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 hasiihelper-0.2.0/hasiihelper/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-11 20:37:40.266083 hasiihelper-0.2.0/hasiihelper.egg-info/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2030 2023-04-11 20:37:40.000000 hasiihelper-0.2.0/hasiihelper.egg-info/PKG-INFO
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      410 2023-04-11 20:37:40.000000 hasiihelper-0.2.0/hasiihelper.egg-info/SOURCES.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2023-04-11 20:37:40.000000 hasiihelper-0.2.0/hasiihelper.egg-info/dependency_links.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       19 2023-04-11 20:37:40.000000 hasiihelper-0.2.0/hasiihelper.egg-info/requires.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       12 2023-04-11 20:37:40.000000 hasiihelper-0.2.0/hasiihelper.egg-info/top_level.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2023-04-11 20:37:40.266401 hasiihelper-0.2.0/setup.cfg
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      806 2023-04-10 18:38:31.000000 hasiihelper-0.2.0/setup.py
```

### Comparing `hasiihelper-0.1.0/LICENSE` & `hasiihelper-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hasiihelper-0.1.0/PKG-INFO` & `hasiihelper-0.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6861 7369  : 2.1.Name: hasi
 00000020: 6968 656c 7065 720a 5665 7273 696f 6e3a  ihelper.Version:
-00000030: 2030 2e31 2e30 0a53 756d 6d61 7279 3a20   0.1.0.Summary: 
+00000030: 2030 2e32 2e30 0a53 756d 6d61 7279 3a20   0.2.0.Summary: 
 00000040: 4875 6d62 6572 746f 6073 2048 656c 7065  Humberto`s Helpe
 00000050: 7220 436c 6173 7365 730a 486f 6d65 2d70  r Classes.Home-p
 00000060: 6167 653a 2068 7474 7073 3a2f 2f67 6974  age: https://git
 00000070: 6875 622e 636f 6d2f 6861 7369 6932 3031  hub.com/hasii201
 00000080: 312f 6861 7369 6968 656c 7065 720a 4175  1/hasiihelper.Au
 00000090: 7468 6f72 3a20 4875 6d62 6572 746f 2041  thor: Humberto A
 000000a0: 2e20 5361 6e63 6865 7a20 4949 0a41 7574  . Sanchez II.Aut
@@ -48,57 +48,80 @@
 000002f0: 6f73 7420 636f 6d6d 6f6e 2061 7274 6966  ost common artif
 00000300: 6163 7473 2066 6f72 2076 6172 696f 7573  acts for various
 00000310: 2070 726f 6a65 6374 7320 4920 616d 2064   projects I am d
 00000320: 6576 656c 6f70 696e 672e 2020 5468 6973  eveloping.  This
 00000330: 2069 7320 7061 636b 6167 6520 646f 6573   is package does
 00000340: 206e 6f74 2069 6e63 6c75 6465 2061 6e79   not include any
 00000350: 2077 7850 7974 686f 6e20 6465 7065 6e64   wxPython depend
-00000360: 656e 6379 0a0a 0a21 5b48 756d 6265 7274  ency...![Humbert
-00000370: 6f27 7320 4d6f 6469 6669 6564 204c 6f67  o's Modified Log
-00000380: 6f5d 282e 2f64 6576 656c 6f70 6572 2f53  o](./developer/S
-00000390: 696c 6c79 4769 7448 7562 2e70 6e67 290a  illyGitHub.png).
-000003a0: 0a49 2061 6d20 636f 6e63 6572 6e65 6420  .I am concerned 
-000003b0: 6162 6f75 7420 4769 7448 7562 2773 2043  about GitHub's C
-000003c0: 6f70 696c 6f74 2070 726f 6a65 6374 0a0a  opilot project..
-000003d0: 0a0a 4920 7572 6765 2079 6f75 2074 6f20  ..I urge you to 
-000003e0: 7265 6164 2061 626f 7574 2074 6865 0a5b  read about the.[
-000003f0: 4769 7665 2075 7020 4769 7448 7562 5d28  Give up GitHub](
-00000400: 6874 7470 733a 2f2f 4769 7665 5570 4769  https://GiveUpGi
-00000410: 7448 7562 2e6f 7267 2920 6361 6d70 6169  tHub.org) campai
-00000420: 676e 2066 726f 6d0a 5b74 6865 2053 6f66  gn from.[the Sof
-00000430: 7477 6172 6520 4672 6565 646f 6d20 436f  tware Freedom Co
-00000440: 6e73 6572 7661 6e63 795d 2868 7474 7073  nservancy](https
-00000450: 3a2f 2f73 6663 6f6e 7365 7276 616e 6379  ://sfconservancy
-00000460: 2e6f 7267 292e 0a0a 5768 696c 6520 4920  .org)...While I 
-00000470: 646f 206e 6f74 2061 6476 6f63 6174 6520  do not advocate 
-00000480: 666f 7220 616c 6c20 7468 6520 6973 7375  for all the issu
-00000490: 6573 206c 6973 7465 6420 7468 6572 6520  es listed there 
-000004a0: 4920 646f 206e 6f74 206c 696b 6520 7468  I do not like th
-000004b0: 6174 0a61 2063 6f6d 7061 6e79 206c 696b  at.a company lik
-000004c0: 6520 4d69 6372 6f73 6f66 7420 6d61 7920  e Microsoft may 
-000004d0: 7072 6f66 6974 2066 726f 6d20 6f70 656e  profit from open
-000004e0: 2073 6f75 7263 6520 7072 6f6a 6563 7473   source projects
-000004f0: 2e0a 0a49 2063 6f6e 7469 6e75 6520 746f  ...I continue to
-00000500: 2075 7365 2047 6974 4875 6220 6265 6361   use GitHub beca
-00000510: 7573 6520 6974 206f 6666 6572 7320 7468  use it offers th
-00000520: 6520 7365 7276 6963 6573 2049 206e 6565  e services I nee
-00000530: 6420 666f 7220 6672 6565 2e20 2042 7574  d for free.  But
-00000540: 2c20 4920 636f 6e74 696e 7565 0a74 6f20  , I continue.to 
-00000550: 6d6f 6e69 746f 7220 7468 6569 7220 7465  monitor their te
-00000560: 726d 7320 6f66 2073 6572 7669 6365 2e0a  rms of service..
-00000570: 0a41 6e79 2075 7365 206f 6620 7468 6973  .Any use of this
-00000580: 2070 726f 6a65 6374 2773 2063 6f64 6520   project's code 
-00000590: 6279 2047 6974 4875 6220 436f 7069 6c6f  by GitHub Copilo
-000005a0: 742c 2070 6173 7420 6f72 2070 7265 7365  t, past or prese
-000005b0: 6e74 2c20 6973 2064 6f6e 650a 7769 7468  nt, is done.with
-000005c0: 6f75 7420 6d79 2070 6572 6d69 7373 696f  out my permissio
-000005d0: 6e2e 2020 4920 646f 206e 6f74 2063 6f6e  n.  I do not con
-000005e0: 7365 6e74 2074 6f20 4769 7448 7562 2773  sent to GitHub's
-000005f0: 2075 7365 206f 6620 7468 6973 2070 726f   use of this pro
-00000600: 6a65 6374 2773 0a63 6f64 6520 696e 2043  ject's.code in C
-00000610: 6f70 696c 6f74 2e0a 0a41 2072 6570 6f73  opilot...A repos
-00000620: 6974 6f72 7920 6f77 6e65 7220 6d61 7920  itory owner may 
-00000630: 6f70 7420 6f75 7420 6f66 2043 6f70 696c  opt out of Copil
-00000640: 6f74 2062 7920 6368 616e 6769 6e67 2053  ot by changing S
-00000650: 6574 7469 6e67 7320 2d2d 3e20 4769 7448  ettings --> GitH
-00000660: 7562 2043 6f70 696c 6f74 2e0a 0a49 2068  ub Copilot...I h
-00000670: 6176 6520 646f 6e65 2073 6f2e 0a0a       ave done so...
+00000360: 656e 6379 0a0a 5f5f 5f0a 0a57 7269 7474  ency..___..Writt
+00000370: 656e 2062 7920 3c61 2068 7265 663d 226d  en by <a href="m
+00000380: 6169 6c74 6f3a 656d 6169 6c40 6875 6d62  ailto:email@humb
+00000390: 6572 746f 2e61 2e73 616e 6368 657a 2e69  erto.a.sanchez.i
+000003a0: 6940 676d 6169 6c2e 636f 6d3f 7375 626a  i@gmail.com?subj
+000003b0: 6563 743d 4865 6c6c 6f20 4875 6d62 6572  ect=Hello Humber
+000003c0: 746f 223e 4875 6d62 6572 746f 2041 2e20  to">Humberto A. 
+000003d0: 5361 6e63 6865 7a20 4949 3c2f 613e 2020  Sanchez II</a>  
+000003e0: 2843 2920 3230 3233 0a0a 2323 204e 6f74  (C) 2023..## Not
+000003f0: 650a 466f 7220 616c 6c20 6b69 6e64 206f  e.For all kind o
+00000400: 6620 7072 6f62 6c65 6d73 2c20 7265 7175  f problems, requ
+00000410: 6573 7473 2c20 656e 6861 6e63 656d 656e  ests, enhancemen
+00000420: 7473 2c20 6275 6720 7265 706f 7274 732c  ts, bug reports,
+00000430: 2065 7463 2e2c 0a70 6c65 6173 6520 6472   etc.,.please dr
+00000440: 6f70 206d 6520 616e 2065 2d6d 6169 6c2e  op me an e-mail.
+00000450: 0a0a 2323 2044 6576 656c 6f70 6572 204e  ..## Developer N
+00000460: 6f74 6573 0a54 6869 7320 7072 6f6a 6563  otes.This projec
+00000470: 7420 7573 6573 205b 6275 696c 646c 6163  t uses [buildlac
+00000480: 6b65 795d 2868 7474 7073 3a2f 2f67 6974  key](https://git
+00000490: 6875 622e 636f 6d2f 6861 7369 6932 3031  hub.com/hasii201
+000004a0: 312f 6275 696c 646c 6163 6b65 7929 2066  1/buildlackey) f
+000004b0: 6f72 2064 6179 2074 6f20 6461 7920 6465  or day to day de
+000004c0: 7665 6c6f 706d 656e 7420 6275 696c 6473  velopment builds
+000004d0: 0a0a 2d2d 2d0a 0a21 5b48 756d 6265 7274  ..---..![Humbert
+000004e0: 6f27 7320 4d6f 6469 6669 6564 204c 6f67  o's Modified Log
+000004f0: 6f5d 282e 2f64 6576 656c 6f70 6572 2f53  o](./developer/S
+00000500: 696c 6c79 4769 7448 7562 2e70 6e67 290a  illyGitHub.png).
+00000510: 0a49 2061 6d20 636f 6e63 6572 6e65 6420  .I am concerned 
+00000520: 6162 6f75 7420 4769 7448 7562 2773 2043  about GitHub's C
+00000530: 6f70 696c 6f74 2070 726f 6a65 6374 0a0a  opilot project..
+00000540: 0a0a 4920 7572 6765 2079 6f75 2074 6f20  ..I urge you to 
+00000550: 7265 6164 2061 626f 7574 2074 6865 0a5b  read about the.[
+00000560: 4769 7665 2075 7020 4769 7448 7562 5d28  Give up GitHub](
+00000570: 6874 7470 733a 2f2f 4769 7665 5570 4769  https://GiveUpGi
+00000580: 7448 7562 2e6f 7267 2920 6361 6d70 6169  tHub.org) campai
+00000590: 676e 2066 726f 6d0a 5b74 6865 2053 6f66  gn from.[the Sof
+000005a0: 7477 6172 6520 4672 6565 646f 6d20 436f  tware Freedom Co
+000005b0: 6e73 6572 7661 6e63 795d 2868 7474 7073  nservancy](https
+000005c0: 3a2f 2f73 6663 6f6e 7365 7276 616e 6379  ://sfconservancy
+000005d0: 2e6f 7267 292e 0a0a 5768 696c 6520 4920  .org)...While I 
+000005e0: 646f 206e 6f74 2061 6476 6f63 6174 6520  do not advocate 
+000005f0: 666f 7220 616c 6c20 7468 6520 6973 7375  for all the issu
+00000600: 6573 206c 6973 7465 6420 7468 6572 6520  es listed there 
+00000610: 4920 646f 206e 6f74 206c 696b 6520 7468  I do not like th
+00000620: 6174 0a61 2063 6f6d 7061 6e79 206c 696b  at.a company lik
+00000630: 6520 4d69 6372 6f73 6f66 7420 6d61 7920  e Microsoft may 
+00000640: 7072 6f66 6974 2066 726f 6d20 6f70 656e  profit from open
+00000650: 2073 6f75 7263 6520 7072 6f6a 6563 7473   source projects
+00000660: 2e0a 0a49 2063 6f6e 7469 6e75 6520 746f  ...I continue to
+00000670: 2075 7365 2047 6974 4875 6220 6265 6361   use GitHub beca
+00000680: 7573 6520 6974 206f 6666 6572 7320 7468  use it offers th
+00000690: 6520 7365 7276 6963 6573 2049 206e 6565  e services I nee
+000006a0: 6420 666f 7220 6672 6565 2e20 2042 7574  d for free.  But
+000006b0: 2c20 4920 636f 6e74 696e 7565 0a74 6f20  , I continue.to 
+000006c0: 6d6f 6e69 746f 7220 7468 6569 7220 7465  monitor their te
+000006d0: 726d 7320 6f66 2073 6572 7669 6365 2e0a  rms of service..
+000006e0: 0a41 6e79 2075 7365 206f 6620 7468 6973  .Any use of this
+000006f0: 2070 726f 6a65 6374 2773 2063 6f64 6520   project's code 
+00000700: 6279 2047 6974 4875 6220 436f 7069 6c6f  by GitHub Copilo
+00000710: 742c 2070 6173 7420 6f72 2070 7265 7365  t, past or prese
+00000720: 6e74 2c20 6973 2064 6f6e 650a 7769 7468  nt, is done.with
+00000730: 6f75 7420 6d79 2070 6572 6d69 7373 696f  out my permissio
+00000740: 6e2e 2020 4920 646f 206e 6f74 2063 6f6e  n.  I do not con
+00000750: 7365 6e74 2074 6f20 4769 7448 7562 2773  sent to GitHub's
+00000760: 2075 7365 206f 6620 7468 6973 2070 726f   use of this pro
+00000770: 6a65 6374 2773 0a63 6f64 6520 696e 2043  ject's.code in C
+00000780: 6f70 696c 6f74 2e0a 0a41 2072 6570 6f73  opilot...A repos
+00000790: 6974 6f72 7920 6f77 6e65 7220 6d61 7920  itory owner may 
+000007a0: 6f70 7420 6f75 7420 6f66 2043 6f70 696c  opt out of Copil
+000007b0: 6f74 2062 7920 6368 616e 6769 6e67 2053  ot by changing S
+000007c0: 6574 7469 6e67 7320 2d2d 3e20 4769 7448  ettings --> GitH
+000007d0: 7562 2043 6f70 696c 6f74 2e0a 0a49 2068  ub Copilot...I h
+000007e0: 6176 6520 646f 6e65 2073 6f2e 0a0a       ave done so...
```

### Comparing `hasiihelper-0.1.0/README.md` & `hasiihelper-0.2.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -25,57 +25,80 @@
 00000180: 486f 7374 2063 6f6d 6d6f 6e20 6172 7469  Host common arti
 00000190: 6661 6374 7320 666f 7220 7661 7269 6f75  facts for variou
 000001a0: 7320 7072 6f6a 6563 7473 2049 2061 6d20  s projects I am 
 000001b0: 6465 7665 6c6f 7069 6e67 2e20 2054 6869  developing.  Thi
 000001c0: 7320 6973 2070 6163 6b61 6765 2064 6f65  s is package doe
 000001d0: 7320 6e6f 7420 696e 636c 7564 6520 616e  s not include an
 000001e0: 7920 7778 5079 7468 6f6e 2064 6570 656e  y wxPython depen
-000001f0: 6465 6e63 790a 0a0a 215b 4875 6d62 6572  dency...![Humber
-00000200: 746f 2773 204d 6f64 6966 6965 6420 4c6f  to's Modified Lo
-00000210: 676f 5d28 2e2f 6465 7665 6c6f 7065 722f  go](./developer/
-00000220: 5369 6c6c 7947 6974 4875 622e 706e 6729  SillyGitHub.png)
-00000230: 0a0a 4920 616d 2063 6f6e 6365 726e 6564  ..I am concerned
-00000240: 2061 626f 7574 2047 6974 4875 6227 7320   about GitHub's 
-00000250: 436f 7069 6c6f 7420 7072 6f6a 6563 740a  Copilot project.
-00000260: 0a0a 0a49 2075 7267 6520 796f 7520 746f  ...I urge you to
-00000270: 2072 6561 6420 6162 6f75 7420 7468 650a   read about the.
-00000280: 5b47 6976 6520 7570 2047 6974 4875 625d  [Give up GitHub]
-00000290: 2868 7474 7073 3a2f 2f47 6976 6555 7047  (https://GiveUpG
-000002a0: 6974 4875 622e 6f72 6729 2063 616d 7061  itHub.org) campa
-000002b0: 6967 6e20 6672 6f6d 0a5b 7468 6520 536f  ign from.[the So
-000002c0: 6674 7761 7265 2046 7265 6564 6f6d 2043  ftware Freedom C
-000002d0: 6f6e 7365 7276 616e 6379 5d28 6874 7470  onservancy](http
-000002e0: 733a 2f2f 7366 636f 6e73 6572 7661 6e63  s://sfconservanc
-000002f0: 792e 6f72 6729 2e0a 0a57 6869 6c65 2049  y.org)...While I
-00000300: 2064 6f20 6e6f 7420 6164 766f 6361 7465   do not advocate
-00000310: 2066 6f72 2061 6c6c 2074 6865 2069 7373   for all the iss
-00000320: 7565 7320 6c69 7374 6564 2074 6865 7265  ues listed there
-00000330: 2049 2064 6f20 6e6f 7420 6c69 6b65 2074   I do not like t
-00000340: 6861 740a 6120 636f 6d70 616e 7920 6c69  hat.a company li
-00000350: 6b65 204d 6963 726f 736f 6674 206d 6179  ke Microsoft may
-00000360: 2070 726f 6669 7420 6672 6f6d 206f 7065   profit from ope
-00000370: 6e20 736f 7572 6365 2070 726f 6a65 6374  n source project
-00000380: 732e 0a0a 4920 636f 6e74 696e 7565 2074  s...I continue t
-00000390: 6f20 7573 6520 4769 7448 7562 2062 6563  o use GitHub bec
-000003a0: 6175 7365 2069 7420 6f66 6665 7273 2074  ause it offers t
-000003b0: 6865 2073 6572 7669 6365 7320 4920 6e65  he services I ne
-000003c0: 6564 2066 6f72 2066 7265 652e 2020 4275  ed for free.  Bu
-000003d0: 742c 2049 2063 6f6e 7469 6e75 650a 746f  t, I continue.to
-000003e0: 206d 6f6e 6974 6f72 2074 6865 6972 2074   monitor their t
-000003f0: 6572 6d73 206f 6620 7365 7276 6963 652e  erms of service.
-00000400: 0a0a 416e 7920 7573 6520 6f66 2074 6869  ..Any use of thi
-00000410: 7320 7072 6f6a 6563 7427 7320 636f 6465  s project's code
-00000420: 2062 7920 4769 7448 7562 2043 6f70 696c   by GitHub Copil
-00000430: 6f74 2c20 7061 7374 206f 7220 7072 6573  ot, past or pres
-00000440: 656e 742c 2069 7320 646f 6e65 0a77 6974  ent, is done.wit
-00000450: 686f 7574 206d 7920 7065 726d 6973 7369  hout my permissi
-00000460: 6f6e 2e20 2049 2064 6f20 6e6f 7420 636f  on.  I do not co
-00000470: 6e73 656e 7420 746f 2047 6974 4875 6227  nsent to GitHub'
-00000480: 7320 7573 6520 6f66 2074 6869 7320 7072  s use of this pr
-00000490: 6f6a 6563 7427 730a 636f 6465 2069 6e20  oject's.code in 
-000004a0: 436f 7069 6c6f 742e 0a0a 4120 7265 706f  Copilot...A repo
-000004b0: 7369 746f 7279 206f 776e 6572 206d 6179  sitory owner may
-000004c0: 206f 7074 206f 7574 206f 6620 436f 7069   opt out of Copi
-000004d0: 6c6f 7420 6279 2063 6861 6e67 696e 6720  lot by changing 
-000004e0: 5365 7474 696e 6773 202d 2d3e 2047 6974  Settings --> Git
-000004f0: 4875 6220 436f 7069 6c6f 742e 0a0a 4920  Hub Copilot...I 
-00000500: 6861 7665 2064 6f6e 6520 736f 2e0a 0a    have done so...
+000001f0: 6465 6e63 790a 0a5f 5f5f 0a0a 5772 6974  dency..___..Writ
+00000200: 7465 6e20 6279 203c 6120 6872 6566 3d22  ten by <a href="
+00000210: 6d61 696c 746f 3a65 6d61 696c 4068 756d  mailto:email@hum
+00000220: 6265 7274 6f2e 612e 7361 6e63 6865 7a2e  berto.a.sanchez.
+00000230: 6969 4067 6d61 696c 2e63 6f6d 3f73 7562  ii@gmail.com?sub
+00000240: 6a65 6374 3d48 656c 6c6f 2048 756d 6265  ject=Hello Humbe
+00000250: 7274 6f22 3e48 756d 6265 7274 6f20 412e  rto">Humberto A.
+00000260: 2053 616e 6368 657a 2049 493c 2f61 3e20   Sanchez II</a> 
+00000270: 2028 4329 2032 3032 330a 0a23 2320 4e6f   (C) 2023..## No
+00000280: 7465 0a46 6f72 2061 6c6c 206b 696e 6420  te.For all kind 
+00000290: 6f66 2070 726f 626c 656d 732c 2072 6571  of problems, req
+000002a0: 7565 7374 732c 2065 6e68 616e 6365 6d65  uests, enhanceme
+000002b0: 6e74 732c 2062 7567 2072 6570 6f72 7473  nts, bug reports
+000002c0: 2c20 6574 632e 2c0a 706c 6561 7365 2064  , etc.,.please d
+000002d0: 726f 7020 6d65 2061 6e20 652d 6d61 696c  rop me an e-mail
+000002e0: 2e0a 0a23 2320 4465 7665 6c6f 7065 7220  ...## Developer 
+000002f0: 4e6f 7465 730a 5468 6973 2070 726f 6a65  Notes.This proje
+00000300: 6374 2075 7365 7320 5b62 7569 6c64 6c61  ct uses [buildla
+00000310: 636b 6579 5d28 6874 7470 733a 2f2f 6769  ckey](https://gi
+00000320: 7468 7562 2e63 6f6d 2f68 6173 6969 3230  thub.com/hasii20
+00000330: 3131 2f62 7569 6c64 6c61 636b 6579 2920  11/buildlackey) 
+00000340: 666f 7220 6461 7920 746f 2064 6179 2064  for day to day d
+00000350: 6576 656c 6f70 6d65 6e74 2062 7569 6c64  evelopment build
+00000360: 730a 0a2d 2d2d 0a0a 215b 4875 6d62 6572  s..---..![Humber
+00000370: 746f 2773 204d 6f64 6966 6965 6420 4c6f  to's Modified Lo
+00000380: 676f 5d28 2e2f 6465 7665 6c6f 7065 722f  go](./developer/
+00000390: 5369 6c6c 7947 6974 4875 622e 706e 6729  SillyGitHub.png)
+000003a0: 0a0a 4920 616d 2063 6f6e 6365 726e 6564  ..I am concerned
+000003b0: 2061 626f 7574 2047 6974 4875 6227 7320   about GitHub's 
+000003c0: 436f 7069 6c6f 7420 7072 6f6a 6563 740a  Copilot project.
+000003d0: 0a0a 0a49 2075 7267 6520 796f 7520 746f  ...I urge you to
+000003e0: 2072 6561 6420 6162 6f75 7420 7468 650a   read about the.
+000003f0: 5b47 6976 6520 7570 2047 6974 4875 625d  [Give up GitHub]
+00000400: 2868 7474 7073 3a2f 2f47 6976 6555 7047  (https://GiveUpG
+00000410: 6974 4875 622e 6f72 6729 2063 616d 7061  itHub.org) campa
+00000420: 6967 6e20 6672 6f6d 0a5b 7468 6520 536f  ign from.[the So
+00000430: 6674 7761 7265 2046 7265 6564 6f6d 2043  ftware Freedom C
+00000440: 6f6e 7365 7276 616e 6379 5d28 6874 7470  onservancy](http
+00000450: 733a 2f2f 7366 636f 6e73 6572 7661 6e63  s://sfconservanc
+00000460: 792e 6f72 6729 2e0a 0a57 6869 6c65 2049  y.org)...While I
+00000470: 2064 6f20 6e6f 7420 6164 766f 6361 7465   do not advocate
+00000480: 2066 6f72 2061 6c6c 2074 6865 2069 7373   for all the iss
+00000490: 7565 7320 6c69 7374 6564 2074 6865 7265  ues listed there
+000004a0: 2049 2064 6f20 6e6f 7420 6c69 6b65 2074   I do not like t
+000004b0: 6861 740a 6120 636f 6d70 616e 7920 6c69  hat.a company li
+000004c0: 6b65 204d 6963 726f 736f 6674 206d 6179  ke Microsoft may
+000004d0: 2070 726f 6669 7420 6672 6f6d 206f 7065   profit from ope
+000004e0: 6e20 736f 7572 6365 2070 726f 6a65 6374  n source project
+000004f0: 732e 0a0a 4920 636f 6e74 696e 7565 2074  s...I continue t
+00000500: 6f20 7573 6520 4769 7448 7562 2062 6563  o use GitHub bec
+00000510: 6175 7365 2069 7420 6f66 6665 7273 2074  ause it offers t
+00000520: 6865 2073 6572 7669 6365 7320 4920 6e65  he services I ne
+00000530: 6564 2066 6f72 2066 7265 652e 2020 4275  ed for free.  Bu
+00000540: 742c 2049 2063 6f6e 7469 6e75 650a 746f  t, I continue.to
+00000550: 206d 6f6e 6974 6f72 2074 6865 6972 2074   monitor their t
+00000560: 6572 6d73 206f 6620 7365 7276 6963 652e  erms of service.
+00000570: 0a0a 416e 7920 7573 6520 6f66 2074 6869  ..Any use of thi
+00000580: 7320 7072 6f6a 6563 7427 7320 636f 6465  s project's code
+00000590: 2062 7920 4769 7448 7562 2043 6f70 696c   by GitHub Copil
+000005a0: 6f74 2c20 7061 7374 206f 7220 7072 6573  ot, past or pres
+000005b0: 656e 742c 2069 7320 646f 6e65 0a77 6974  ent, is done.wit
+000005c0: 686f 7574 206d 7920 7065 726d 6973 7369  hout my permissi
+000005d0: 6f6e 2e20 2049 2064 6f20 6e6f 7420 636f  on.  I do not co
+000005e0: 6e73 656e 7420 746f 2047 6974 4875 6227  nsent to GitHub'
+000005f0: 7320 7573 6520 6f66 2074 6869 7320 7072  s use of this pr
+00000600: 6f6a 6563 7427 730a 636f 6465 2069 6e20  oject's.code in 
+00000610: 436f 7069 6c6f 742e 0a0a 4120 7265 706f  Copilot...A repo
+00000620: 7369 746f 7279 206f 776e 6572 206d 6179  sitory owner may
+00000630: 206f 7074 206f 7574 206f 6620 436f 7069   opt out of Copi
+00000640: 6c6f 7420 6279 2063 6861 6e67 696e 6720  lot by changing 
+00000650: 5365 7474 696e 6773 202d 2d3e 2047 6974  Settings --> Git
+00000660: 4875 6220 436f 7069 6c6f 742e 0a0a 4920  Hub Copilot...I 
+00000670: 6861 7665 2064 6f6e 6520 736f 2e0a 0a    have done so...
```

### Comparing `hasiihelper-0.1.0/hasiihelper/Dimensions.py` & `hasiihelper-0.2.0/hasiihelper/Dimensions.py`

 * *Files identical despite different names*

### Comparing `hasiihelper-0.1.0/hasiihelper/Position.py` & `hasiihelper-0.2.0/hasiihelper/Position.py`

 * *Files identical despite different names*

### Comparing `hasiihelper-0.1.0/hasiihelper/SemanticVersion.py` & `hasiihelper-0.2.0/hasiihelper/SemanticVersion.py`

 * *Files identical despite different names*

### Comparing `hasiihelper-0.1.0/hasiihelper/Singleton.py` & `hasiihelper-0.2.0/hasiihelper/Singleton.py`

 * *Files identical despite different names*

### Comparing `hasiihelper-0.1.0/hasiihelper/UnitTestBase.py` & `hasiihelper-0.2.0/hasiihelper/UnitTestBase.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from importlib.abc import Traversable
 
 from importlib.resources import files
 
 from unittest import TestCase
 
-JSON_LOGGING_CONFIG_FILENAME: str = "testLoggingConfig.json"
+JSON_LOGGING_CONFIG_FILENAME: str = "testLoggingConfiguration.json"
 TEST_DIRECTORY:               str = 'tests'
 
 
 class UnitTestBase(TestCase):
     """
     This is a copy of the one in the export package
```

### Comparing `hasiihelper-0.1.0/hasiihelper.egg-info/PKG-INFO` & `hasiihelper-0.2.0/hasiihelper.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6861 7369  : 2.1.Name: hasi
 00000020: 6968 656c 7065 720a 5665 7273 696f 6e3a  ihelper.Version:
-00000030: 2030 2e31 2e30 0a53 756d 6d61 7279 3a20   0.1.0.Summary: 
+00000030: 2030 2e32 2e30 0a53 756d 6d61 7279 3a20   0.2.0.Summary: 
 00000040: 4875 6d62 6572 746f 6073 2048 656c 7065  Humberto`s Helpe
 00000050: 7220 436c 6173 7365 730a 486f 6d65 2d70  r Classes.Home-p
 00000060: 6167 653a 2068 7474 7073 3a2f 2f67 6974  age: https://git
 00000070: 6875 622e 636f 6d2f 6861 7369 6932 3031  hub.com/hasii201
 00000080: 312f 6861 7369 6968 656c 7065 720a 4175  1/hasiihelper.Au
 00000090: 7468 6f72 3a20 4875 6d62 6572 746f 2041  thor: Humberto A
 000000a0: 2e20 5361 6e63 6865 7a20 4949 0a41 7574  . Sanchez II.Aut
@@ -48,57 +48,80 @@
 000002f0: 6f73 7420 636f 6d6d 6f6e 2061 7274 6966  ost common artif
 00000300: 6163 7473 2066 6f72 2076 6172 696f 7573  acts for various
 00000310: 2070 726f 6a65 6374 7320 4920 616d 2064   projects I am d
 00000320: 6576 656c 6f70 696e 672e 2020 5468 6973  eveloping.  This
 00000330: 2069 7320 7061 636b 6167 6520 646f 6573   is package does
 00000340: 206e 6f74 2069 6e63 6c75 6465 2061 6e79   not include any
 00000350: 2077 7850 7974 686f 6e20 6465 7065 6e64   wxPython depend
-00000360: 656e 6379 0a0a 0a21 5b48 756d 6265 7274  ency...![Humbert
-00000370: 6f27 7320 4d6f 6469 6669 6564 204c 6f67  o's Modified Log
-00000380: 6f5d 282e 2f64 6576 656c 6f70 6572 2f53  o](./developer/S
-00000390: 696c 6c79 4769 7448 7562 2e70 6e67 290a  illyGitHub.png).
-000003a0: 0a49 2061 6d20 636f 6e63 6572 6e65 6420  .I am concerned 
-000003b0: 6162 6f75 7420 4769 7448 7562 2773 2043  about GitHub's C
-000003c0: 6f70 696c 6f74 2070 726f 6a65 6374 0a0a  opilot project..
-000003d0: 0a0a 4920 7572 6765 2079 6f75 2074 6f20  ..I urge you to 
-000003e0: 7265 6164 2061 626f 7574 2074 6865 0a5b  read about the.[
-000003f0: 4769 7665 2075 7020 4769 7448 7562 5d28  Give up GitHub](
-00000400: 6874 7470 733a 2f2f 4769 7665 5570 4769  https://GiveUpGi
-00000410: 7448 7562 2e6f 7267 2920 6361 6d70 6169  tHub.org) campai
-00000420: 676e 2066 726f 6d0a 5b74 6865 2053 6f66  gn from.[the Sof
-00000430: 7477 6172 6520 4672 6565 646f 6d20 436f  tware Freedom Co
-00000440: 6e73 6572 7661 6e63 795d 2868 7474 7073  nservancy](https
-00000450: 3a2f 2f73 6663 6f6e 7365 7276 616e 6379  ://sfconservancy
-00000460: 2e6f 7267 292e 0a0a 5768 696c 6520 4920  .org)...While I 
-00000470: 646f 206e 6f74 2061 6476 6f63 6174 6520  do not advocate 
-00000480: 666f 7220 616c 6c20 7468 6520 6973 7375  for all the issu
-00000490: 6573 206c 6973 7465 6420 7468 6572 6520  es listed there 
-000004a0: 4920 646f 206e 6f74 206c 696b 6520 7468  I do not like th
-000004b0: 6174 0a61 2063 6f6d 7061 6e79 206c 696b  at.a company lik
-000004c0: 6520 4d69 6372 6f73 6f66 7420 6d61 7920  e Microsoft may 
-000004d0: 7072 6f66 6974 2066 726f 6d20 6f70 656e  profit from open
-000004e0: 2073 6f75 7263 6520 7072 6f6a 6563 7473   source projects
-000004f0: 2e0a 0a49 2063 6f6e 7469 6e75 6520 746f  ...I continue to
-00000500: 2075 7365 2047 6974 4875 6220 6265 6361   use GitHub beca
-00000510: 7573 6520 6974 206f 6666 6572 7320 7468  use it offers th
-00000520: 6520 7365 7276 6963 6573 2049 206e 6565  e services I nee
-00000530: 6420 666f 7220 6672 6565 2e20 2042 7574  d for free.  But
-00000540: 2c20 4920 636f 6e74 696e 7565 0a74 6f20  , I continue.to 
-00000550: 6d6f 6e69 746f 7220 7468 6569 7220 7465  monitor their te
-00000560: 726d 7320 6f66 2073 6572 7669 6365 2e0a  rms of service..
-00000570: 0a41 6e79 2075 7365 206f 6620 7468 6973  .Any use of this
-00000580: 2070 726f 6a65 6374 2773 2063 6f64 6520   project's code 
-00000590: 6279 2047 6974 4875 6220 436f 7069 6c6f  by GitHub Copilo
-000005a0: 742c 2070 6173 7420 6f72 2070 7265 7365  t, past or prese
-000005b0: 6e74 2c20 6973 2064 6f6e 650a 7769 7468  nt, is done.with
-000005c0: 6f75 7420 6d79 2070 6572 6d69 7373 696f  out my permissio
-000005d0: 6e2e 2020 4920 646f 206e 6f74 2063 6f6e  n.  I do not con
-000005e0: 7365 6e74 2074 6f20 4769 7448 7562 2773  sent to GitHub's
-000005f0: 2075 7365 206f 6620 7468 6973 2070 726f   use of this pro
-00000600: 6a65 6374 2773 0a63 6f64 6520 696e 2043  ject's.code in C
-00000610: 6f70 696c 6f74 2e0a 0a41 2072 6570 6f73  opilot...A repos
-00000620: 6974 6f72 7920 6f77 6e65 7220 6d61 7920  itory owner may 
-00000630: 6f70 7420 6f75 7420 6f66 2043 6f70 696c  opt out of Copil
-00000640: 6f74 2062 7920 6368 616e 6769 6e67 2053  ot by changing S
-00000650: 6574 7469 6e67 7320 2d2d 3e20 4769 7448  ettings --> GitH
-00000660: 7562 2043 6f70 696c 6f74 2e0a 0a49 2068  ub Copilot...I h
-00000670: 6176 6520 646f 6e65 2073 6f2e 0a0a       ave done so...
+00000360: 656e 6379 0a0a 5f5f 5f0a 0a57 7269 7474  ency..___..Writt
+00000370: 656e 2062 7920 3c61 2068 7265 663d 226d  en by <a href="m
+00000380: 6169 6c74 6f3a 656d 6169 6c40 6875 6d62  ailto:email@humb
+00000390: 6572 746f 2e61 2e73 616e 6368 657a 2e69  erto.a.sanchez.i
+000003a0: 6940 676d 6169 6c2e 636f 6d3f 7375 626a  i@gmail.com?subj
+000003b0: 6563 743d 4865 6c6c 6f20 4875 6d62 6572  ect=Hello Humber
+000003c0: 746f 223e 4875 6d62 6572 746f 2041 2e20  to">Humberto A. 
+000003d0: 5361 6e63 6865 7a20 4949 3c2f 613e 2020  Sanchez II</a>  
+000003e0: 2843 2920 3230 3233 0a0a 2323 204e 6f74  (C) 2023..## Not
+000003f0: 650a 466f 7220 616c 6c20 6b69 6e64 206f  e.For all kind o
+00000400: 6620 7072 6f62 6c65 6d73 2c20 7265 7175  f problems, requ
+00000410: 6573 7473 2c20 656e 6861 6e63 656d 656e  ests, enhancemen
+00000420: 7473 2c20 6275 6720 7265 706f 7274 732c  ts, bug reports,
+00000430: 2065 7463 2e2c 0a70 6c65 6173 6520 6472   etc.,.please dr
+00000440: 6f70 206d 6520 616e 2065 2d6d 6169 6c2e  op me an e-mail.
+00000450: 0a0a 2323 2044 6576 656c 6f70 6572 204e  ..## Developer N
+00000460: 6f74 6573 0a54 6869 7320 7072 6f6a 6563  otes.This projec
+00000470: 7420 7573 6573 205b 6275 696c 646c 6163  t uses [buildlac
+00000480: 6b65 795d 2868 7474 7073 3a2f 2f67 6974  key](https://git
+00000490: 6875 622e 636f 6d2f 6861 7369 6932 3031  hub.com/hasii201
+000004a0: 312f 6275 696c 646c 6163 6b65 7929 2066  1/buildlackey) f
+000004b0: 6f72 2064 6179 2074 6f20 6461 7920 6465  or day to day de
+000004c0: 7665 6c6f 706d 656e 7420 6275 696c 6473  velopment builds
+000004d0: 0a0a 2d2d 2d0a 0a21 5b48 756d 6265 7274  ..---..![Humbert
+000004e0: 6f27 7320 4d6f 6469 6669 6564 204c 6f67  o's Modified Log
+000004f0: 6f5d 282e 2f64 6576 656c 6f70 6572 2f53  o](./developer/S
+00000500: 696c 6c79 4769 7448 7562 2e70 6e67 290a  illyGitHub.png).
+00000510: 0a49 2061 6d20 636f 6e63 6572 6e65 6420  .I am concerned 
+00000520: 6162 6f75 7420 4769 7448 7562 2773 2043  about GitHub's C
+00000530: 6f70 696c 6f74 2070 726f 6a65 6374 0a0a  opilot project..
+00000540: 0a0a 4920 7572 6765 2079 6f75 2074 6f20  ..I urge you to 
+00000550: 7265 6164 2061 626f 7574 2074 6865 0a5b  read about the.[
+00000560: 4769 7665 2075 7020 4769 7448 7562 5d28  Give up GitHub](
+00000570: 6874 7470 733a 2f2f 4769 7665 5570 4769  https://GiveUpGi
+00000580: 7448 7562 2e6f 7267 2920 6361 6d70 6169  tHub.org) campai
+00000590: 676e 2066 726f 6d0a 5b74 6865 2053 6f66  gn from.[the Sof
+000005a0: 7477 6172 6520 4672 6565 646f 6d20 436f  tware Freedom Co
+000005b0: 6e73 6572 7661 6e63 795d 2868 7474 7073  nservancy](https
+000005c0: 3a2f 2f73 6663 6f6e 7365 7276 616e 6379  ://sfconservancy
+000005d0: 2e6f 7267 292e 0a0a 5768 696c 6520 4920  .org)...While I 
+000005e0: 646f 206e 6f74 2061 6476 6f63 6174 6520  do not advocate 
+000005f0: 666f 7220 616c 6c20 7468 6520 6973 7375  for all the issu
+00000600: 6573 206c 6973 7465 6420 7468 6572 6520  es listed there 
+00000610: 4920 646f 206e 6f74 206c 696b 6520 7468  I do not like th
+00000620: 6174 0a61 2063 6f6d 7061 6e79 206c 696b  at.a company lik
+00000630: 6520 4d69 6372 6f73 6f66 7420 6d61 7920  e Microsoft may 
+00000640: 7072 6f66 6974 2066 726f 6d20 6f70 656e  profit from open
+00000650: 2073 6f75 7263 6520 7072 6f6a 6563 7473   source projects
+00000660: 2e0a 0a49 2063 6f6e 7469 6e75 6520 746f  ...I continue to
+00000670: 2075 7365 2047 6974 4875 6220 6265 6361   use GitHub beca
+00000680: 7573 6520 6974 206f 6666 6572 7320 7468  use it offers th
+00000690: 6520 7365 7276 6963 6573 2049 206e 6565  e services I nee
+000006a0: 6420 666f 7220 6672 6565 2e20 2042 7574  d for free.  But
+000006b0: 2c20 4920 636f 6e74 696e 7565 0a74 6f20  , I continue.to 
+000006c0: 6d6f 6e69 746f 7220 7468 6569 7220 7465  monitor their te
+000006d0: 726d 7320 6f66 2073 6572 7669 6365 2e0a  rms of service..
+000006e0: 0a41 6e79 2075 7365 206f 6620 7468 6973  .Any use of this
+000006f0: 2070 726f 6a65 6374 2773 2063 6f64 6520   project's code 
+00000700: 6279 2047 6974 4875 6220 436f 7069 6c6f  by GitHub Copilo
+00000710: 742c 2070 6173 7420 6f72 2070 7265 7365  t, past or prese
+00000720: 6e74 2c20 6973 2064 6f6e 650a 7769 7468  nt, is done.with
+00000730: 6f75 7420 6d79 2070 6572 6d69 7373 696f  out my permissio
+00000740: 6e2e 2020 4920 646f 206e 6f74 2063 6f6e  n.  I do not con
+00000750: 7365 6e74 2074 6f20 4769 7448 7562 2773  sent to GitHub's
+00000760: 2075 7365 206f 6620 7468 6973 2070 726f   use of this pro
+00000770: 6a65 6374 2773 0a63 6f64 6520 696e 2043  ject's.code in C
+00000780: 6f70 696c 6f74 2e0a 0a41 2072 6570 6f73  opilot...A repos
+00000790: 6974 6f72 7920 6f77 6e65 7220 6d61 7920  itory owner may 
+000007a0: 6f70 7420 6f75 7420 6f66 2043 6f70 696c  opt out of Copil
+000007b0: 6f74 2062 7920 6368 616e 6769 6e67 2053  ot by changing S
+000007c0: 6574 7469 6e67 7320 2d2d 3e20 4769 7448  ettings --> GitH
+000007d0: 7562 2043 6f70 696c 6f74 2e0a 0a49 2068  ub Copilot...I h
+000007e0: 6176 6520 646f 6e65 2073 6f2e 0a0a       ave done so...
```

### Comparing `hasiihelper-0.1.0/setup.py` & `hasiihelper-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 LICENSE = (HERE / 'LICENSE').read_text()
 
 setup(
     name="hasiihelper",
-    version="0.1.0",
+    version="0.2.0",
     author='Humberto A. Sanchez II',
     author_email='Humberto.A.Sanchez.II@gmail.com',
     maintainer='Humberto A. Sanchez II',
     maintainer_email='humberto.a.sanchez.ii@gmail.com',
     description='Humberto`s Helper Classes',
     long_description=README,
     long_description_content_type="text/markdown",
```

