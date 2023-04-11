# Comparing `tmp/temperaturemonitor_mqtt_sldewit-0.0.5.tar.gz` & `tmp/temperaturemonitor_mqtt_sldewit-1.0.0.tar.gz`

## Comparing `temperaturemonitor_mqtt_sldewit-0.0.5.tar` & `temperaturemonitor_mqtt_sldewit-1.0.0.tar`

### file list

```diff
@@ -1,28 +1,37 @@
--rw-r--r--   0        0        0    10291 2020-02-02 00:00:00.000000 temperaturemonitor_mqtt_sldewit-0.0.5/Temperatuur sensoren.xlsx
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 temperaturemonitor_mqtt_sldewit-0.0.5/development-requirements.txt
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 temperaturemonitor_mqtt_sldewit-0.0.5/.github/workflows/python-app.yml
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 temperaturemonitor_mqtt_sldewit-0.0.5/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0    12660 2020-02-02 00:00:00.000000 temperaturemonitor_mqtt_sldewit-0.0.5/Fritzing/Vloerverwarming monitor.fzz
--rw-r--r--   0        0        0   128323 2020-02-02 00:00:00.000000 temperaturemonitor_mqtt_sldewit-0.0.5/Fritzing/Vloerverwarming monitor_schema.svg
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 temperaturemonitor_mqtt_sldewit-0.0.5/TESTDIR/pyvenv.cfg
--rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 temperaturemonitor_mqtt_sldewit-0.0.5/TESTDIR/Scripts/Activate.ps1
--rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 temperaturemonitor_mqtt_sldewit-0.0.5/TESTDIR/Scripts/activate
--rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 temperaturemonitor_mqtt_sldewit-0.0.5/TESTDIR/Scripts/activate.bat
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 temperaturemonitor_mqtt_sldewit-0.0.5/TESTDIR/Scripts/deactivate.bat
--rw-r--r--   0        0        0   106410 2020-02-02 00:00:00.000000 temperaturemonitor_mqtt_sldewit-0.0.5/TESTDIR/Scripts/easy_install-3.7.exe
--rw-r--r--   0        0        0   106410 2020-02-02 00:00:00.000000 temperaturemonitor_mqtt_sldewit-0.0.5/TESTDIR/Scripts/easy_install.exe
--rw-r--r--   0        0        0   106401 2020-02-02 00:00:00.000000 temperaturemonitor_mqtt_sldewit-0.0.5/TESTDIR/Scripts/pip.exe
--rw-r--r--   0        0        0   106401 2020-02-02 00:00:00.000000 temperaturemonitor_mqtt_sldewit-0.0.5/TESTDIR/Scripts/pip3.7.exe
--rw-r--r--   0        0        0   106401 2020-02-02 00:00:00.000000 temperaturemonitor_mqtt_sldewit-0.0.5/TESTDIR/Scripts/pip3.exe
--rw-r--r--   0        0        0   501320 2020-02-02 00:00:00.000000 temperaturemonitor_mqtt_sldewit-0.0.5/TESTDIR/Scripts/python.exe
--rw-r--r--   0        0        0   500296 2020-02-02 00:00:00.000000 temperaturemonitor_mqtt_sldewit-0.0.5/TESTDIR/Scripts/pythonw.exe
--rw-r--r--   0        0        0     3380 2020-02-02 00:00:00.000000 temperaturemonitor_mqtt_sldewit-0.0.5/drafts/test mqtt.py
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 temperaturemonitor_mqtt_sldewit-0.0.5/drafts/test onewire.py
--rw-r--r--   0        0        0     3288 2020-02-02 00:00:00.000000 temperaturemonitor_mqtt_sldewit-0.0.5/drafts/test structure.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 temperaturemonitor_mqtt_sldewit-0.0.5/src/temperature_monitoring_mqtt_sldewit/__init__.py
--rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 temperaturemonitor_mqtt_sldewit-0.0.5/src/temperature_monitoring_mqtt_sldewit/temperatue_monitor_mqtt.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 temperaturemonitor_mqtt_sldewit-0.0.5/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 temperaturemonitor_mqtt_sldewit-0.0.5/LICENSE
--rw-r--r--   0        0        0     2811 2020-02-02 00:00:00.000000 temperaturemonitor_mqtt_sldewit-0.0.5/README.md
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 temperaturemonitor_mqtt_sldewit-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     3437 2020-02-02 00:00:00.000000 temperaturemonitor_mqtt_sldewit-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 temperaturemonitor_mqtt_sldewit-1.0.0/MAC address list.txt
+-rw-r--r--   0        0        0    10497 2020-02-02 00:00:00.000000 temperaturemonitor_mqtt_sldewit-1.0.0/Temperatuur sensoren.xlsx
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 temperaturemonitor_mqtt_sldewit-1.0.0/development-requirements.txt
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 temperaturemonitor_mqtt_sldewit-1.0.0/sensor_list.json
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 temperaturemonitor_mqtt_sldewit-1.0.0/.github/dependabot.yml
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 temperaturemonitor_mqtt_sldewit-1.0.0/.github/workflows/python-app.yml
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 temperaturemonitor_mqtt_sldewit-1.0.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0    12660 2020-02-02 00:00:00.000000 temperaturemonitor_mqtt_sldewit-1.0.0/Fritzing/Vloerverwarming monitor.fzz
+-rw-r--r--   0        0        0   128323 2020-02-02 00:00:00.000000 temperaturemonitor_mqtt_sldewit-1.0.0/Fritzing/Vloerverwarming monitor_schema.svg
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 temperaturemonitor_mqtt_sldewit-1.0.0/TESTDIR/pyvenv.cfg
+-rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 temperaturemonitor_mqtt_sldewit-1.0.0/TESTDIR/Scripts/Activate.ps1
+-rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 temperaturemonitor_mqtt_sldewit-1.0.0/TESTDIR/Scripts/activate
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 temperaturemonitor_mqtt_sldewit-1.0.0/TESTDIR/Scripts/activate.bat
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 temperaturemonitor_mqtt_sldewit-1.0.0/TESTDIR/Scripts/deactivate.bat
+-rw-r--r--   0        0        0   106410 2020-02-02 00:00:00.000000 temperaturemonitor_mqtt_sldewit-1.0.0/TESTDIR/Scripts/easy_install-3.7.exe
+-rw-r--r--   0        0        0   106410 2020-02-02 00:00:00.000000 temperaturemonitor_mqtt_sldewit-1.0.0/TESTDIR/Scripts/easy_install.exe
+-rw-r--r--   0        0        0   106401 2020-02-02 00:00:00.000000 temperaturemonitor_mqtt_sldewit-1.0.0/TESTDIR/Scripts/pip.exe
+-rw-r--r--   0        0        0   106401 2020-02-02 00:00:00.000000 temperaturemonitor_mqtt_sldewit-1.0.0/TESTDIR/Scripts/pip3.7.exe
+-rw-r--r--   0        0        0   106401 2020-02-02 00:00:00.000000 temperaturemonitor_mqtt_sldewit-1.0.0/TESTDIR/Scripts/pip3.exe
+-rw-r--r--   0        0        0   501320 2020-02-02 00:00:00.000000 temperaturemonitor_mqtt_sldewit-1.0.0/TESTDIR/Scripts/python.exe
+-rw-r--r--   0        0        0   500296 2020-02-02 00:00:00.000000 temperaturemonitor_mqtt_sldewit-1.0.0/TESTDIR/Scripts/pythonw.exe
+-rw-r--r--   0        0        0     3380 2020-02-02 00:00:00.000000 temperaturemonitor_mqtt_sldewit-1.0.0/drafts/test mqtt.py
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 temperaturemonitor_mqtt_sldewit-1.0.0/drafts/test onewire.py
+-rw-r--r--   0        0        0     3288 2020-02-02 00:00:00.000000 temperaturemonitor_mqtt_sldewit-1.0.0/drafts/test structure.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 temperaturemonitor_mqtt_sldewit-1.0.0/drafts/TestJSON/T1.json
+-rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 temperaturemonitor_mqtt_sldewit-1.0.0/drafts/TestJSON/TestJSON.py
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 temperaturemonitor_mqtt_sldewit-1.0.0/drafts/TestJSON/_sensor_list.json
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 temperaturemonitor_mqtt_sldewit-1.0.0/drafts/TestJSON/sample.json
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 temperaturemonitor_mqtt_sldewit-1.0.0/drafts/TestJSON/sample2.json
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 temperaturemonitor_mqtt_sldewit-1.0.0/drafts/TestJSON/sensor_list.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 temperaturemonitor_mqtt_sldewit-1.0.0/src/temperature_monitoring_mqtt_sldewit/__init__.py
+-rw-r--r--   0        0        0     4789 2020-02-02 00:00:00.000000 temperaturemonitor_mqtt_sldewit-1.0.0/src/temperature_monitoring_mqtt_sldewit/temperature_monitor_mqtt.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 temperaturemonitor_mqtt_sldewit-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 temperaturemonitor_mqtt_sldewit-1.0.0/LICENSE
+-rw-r--r--   0        0        0     2811 2020-02-02 00:00:00.000000 temperaturemonitor_mqtt_sldewit-1.0.0/README.md
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 temperaturemonitor_mqtt_sldewit-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3437 2020-02-02 00:00:00.000000 temperaturemonitor_mqtt_sldewit-1.0.0/PKG-INFO
```

### Comparing `temperaturemonitor_mqtt_sldewit-0.0.5/Temperatuur sensoren.xlsx` & `temperaturemonitor_mqtt_sldewit-1.0.0/Temperatuur sensoren.xlsx`

 * *Files 19% similar despite different names*

```diff
@@ -104,541 +104,554 @@
 00000670: edad 86b0 b737 a0ea 93cf 9b7f d796 a6e9  .....7..........
 00000680: 0d3f 8839 4cec d299 15c8 7362 67d9 ae7c  .?.9L.....sbg..|
 00000690: c86c 21f5 f91a 5553 6839 69b0 629e 723a  .l!...USh9i.b.r:
 000006a0: 2279 5f64 6cc0 f344 9bbf 13fd 7c2d 4e9c  "y_dl..D....|-N.
 000006b0: c852 2234 12f8 32cf 47c7 25a0 f57f 5ab4  .R"4..2.G.%...Z.
 000006c0: 34f1 cb9d 79c4 3709 c3ab c8f0 c982 8b1f  4...y.7.........
 000006d0: a8de 0100 00ff ff03 0050 4b03 0414 0006  .........PK.....
-000006e0: 0008 0000 0021 008d de29 17f4 0200 00d6  .....!...)......
+000006e0: 0008 0000 0021 0030 549e 8be6 0200 00c0  .....!.0T.......
 000006f0: 0600 000f 0000 0078 6c2f 776f 726b 626f  .......xl/workbo
-00000700: 6f6b 2e78 6d6c ac55 db6e a330 107d 5f69  ok.xml.U.n.0.}_i
-00000710: ffc1 f23b 0513 4808 2aad 9a90 6a23 6d57  ...;..H.*...j#mW
-00000720: 55db 6d5f 2255 2e38 c10d d8ac 6d9a 5455  U.m_"U.8....m.TU
-00000730: ff7d c750 7acb 4bb7 5d94 f8c2 c0f1 9999  .}.Pz.K.].......
-00000740: 33c3 fee1 b62a d11d 539a 4b91 60b2 e761  3....*..S.K.`..a
-00000750: c444 2673 2e56 09fe 7d71 ec44 1869 4345  .D&s.V..}q.D.iCE
-00000760: 4e4b 2958 82ef 99c6 8707 dfbf ed6f a45a  NK)X.........o.Z
-00000770: df48 b946 0020 7482 0b63 ead8 7575 56b0  .H.F. t..c..uuV.
-00000780: 8aea 3d59 3301 96a5 5415 35b0 552b 57d7  ..=Y3...T.5.U+W.
-00000790: 8ad1 5c17 8c99 aa74 7dcf 1bba 15e5 0277  ..\....t}......w
-000007a0: 08b1 fa08 865c 2e79 c652 9935 1513 a603  .....\.y.R.5....
-000007b0: 51ac a406 e8eb 82d7 ba47 abb2 8fc0 5554  Q........G....UT
-000007c0: ad9b dac9 6455 03c4 0d2f b9b9 6f41 31aa  ....dU.../..oA1.
-000007d0: b278 be12 52d1 9b12 dcde 9210 6d15 fc86  .x..R.......m...
-000007e0: f027 1e0c 7e7f 1298 768e aa78 a6a4 964b  .'..~...v..x...K
-000007f0: b307 d06e 477a c77f e2b9 84bc 09c1 7637  ...nGz........v7
-00000800: 061f 430a 5cc5 eeb8 cde1 332b 35fc 24ab  ..C.\.....3+5.$.
-00000810: e133 d6f0 058c 785f 4623 20ad 562b 3104  .3....x_F# .V+1.
-00000820: ef93 68e1 3337 1f1f ec2f 79c9 2e3b e922  ..h.37.../y..;."
-00000830: 5ad7 bf68 6533 5562 5452 6d66 3937 2c4f  Z..he3UbTRmf97,O
-00000840: f008 b672 c35e 6e80 57aa a927 0d2f c1ea  ...r.^n.W..'./..
-00000850: 87d1 8060 f7e0 59ce a70a 3690 fba3 d230  ...`..Y...6....0
-00000860: 25a8 6153 290c 48ed 89fa 5765 d562 4f0b  %.aS).H...We.bO.
-00000870: 0922 4667 ec4f c315 83da 0109 813b 30d2  ."Fg.O.......;0.
-00000880: 2ca6 37fa 949a 0235 aa4c f062 9172 bd3e  ,.7....5.L.b.r.>
-00000890: 37ad be17 2935 7471 c26f 05aa 95bc 6519  7...)5tq.o....e.
-000008a0: f05a 9c48 c18d 5450 aee8 ae94 4c41 296f  .Z.H..TP....LA)o
-000008b0: a8aa 60bf 7825 50ba 5b0d ff20 519a d908  ..`.x%P.[.. Q...
-000008c0: b910 958e 79b7 7e1f 2170 40c5 bd0c 4f8d  ....y.~.!p@...O.
-000008d0: 42b0 9ea7 3f21 15e7 f40e 1203 e9cf 9fea  B...?!..........
-000008e0: 760e 9127 836b 91a9 985c 3f90 209d 1e87  v..'.k...\?. ...
-000008f0: 5ee4 4413 df73 8241 1a39 93d1 d1d8 89d2  ^.D..s.A.9......
-00000900: 239f 7847 a3c8 f3c7 8fe0 8c1a c699 a48d  #.xG............
-00000910: 299e 726e a113 1c40 8277 4c27 74db 5b88  ).rn...@.wL't.[.
-00000920: 1737 3c7f a1f1 e03d 5d8e 9ddf 0dbd edd1  .7<....=].......
-00000930: 3a6c bbdb 2567 1bfd a20e bb45 db2b 2e72  :l..%g.....E.+.r
-00000940: b969 3dba efd7 be1f 62b4 690d 573c 3705  .i=.....b.i.W<7.
-00000950: 482b 8a3c f0b9 bbf7 83f1 5501 6c49 180c  H+.<......U.lI..
-00000960: e041 a800 cb2a c16f d8a4 1d9b 63b8 1c3b  .A...*.o....c..;
-00000970: bc61 e3be a2d3 f650 a0d5 ce48 b4ba 3fb7  .a.....P...H..?.
-00000980: 7d95 40b3 b673 1b60 d079 6ccf 50f3 bc95  }.@..s.`.yl.P...
-00000990: b8db bf96 d132 3b55 c84e ed83 437f 4c06  .....2;U.N..C.L.
-000009a0: d663 b635 3fb5 6967 d01f 077a 2480 0478  .c.5?.ig...z$..x
-000009b0: e3c0 f166 83d0 09a2 b1ef 44c1 c077 a641  ...f......D..w.A
-000009c0: eacf c2d1 2c9d 4d42 9b1b fb0d 88ff 4727  ....,.MB......G'
-000009d0: 6ccb 20ee 3f2e 9665 4195 b950 345b 83a6  l. .?..eA..P4[..
-000009e0: cfd8 7242 3588 a973 08f8 8216 7bd6 6eff  ..rB5..s....{.n.
-000009f0: d6c1 5f00 0000 ffff 0300 504b 0304 1400  .._.......PK....
-00000a00: 0600 0800 0000 2100 813e 9497 f300 0000  ......!..>......
-00000a10: ba02 0000 1a00 0801 786c 2f5f 7265 6c73  ........xl/_rels
-00000a20: 2f77 6f72 6b62 6f6f 6b2e 786d 6c2e 7265  /workbook.xml.re
-00000a30: 6c73 20a2 0401 28a0 0001 0000 0000 0000  ls ...(.........
+00000700: 6f6b 2e78 6d6c ac55 df6f 9b30 107e 9fb4  ok.xml.U.o.0.~..
+00000710: ff01 f99d 8209 9014 954c f9b9 556a a7ac  .........L..Uj..
+00000720: cdda 974a 9503 4eb0 0236 b34d 93aa eaff  ...J..N..6.M....
+00000730: be33 84a4 6d5e ba76 28f1 61ce fefc dddd  .3..m^.v(.a.....
+00000740: c771 f66d 5be4 d603 958a 091e 237c e222  .q.m[.......#|."
+00000750: 8bf2 44a4 8caf 62f4 7b3e b57b c852 9af0  ..D...b.{>.{.R..
+00000760: 94e4 82d3 183d 5285 bef5 bf7e 39db 08b9  .....=R....~9...
+00000770: 5e08 b1b6 0080 ab18 655a 9791 e3a8 24a3  ^.......eZ....$.
+00000780: 0551 27a2 a41c 3c4b 210b a261 2a57 8e2a  .Q'...<K!..a*W.*
+00000790: 2525 a9ca 28d5 45ee 78ae 1b3a 0561 1c35  %%..(.E.x..:.a.5
+000007a0: 0891 7c0f 8658 2e59 42c7 22a9 0aca 7503  ..|..X.YB."...u.
+000007b0: 2269 4e34 d057 192b 558b 5624 ef81 2b88  "iN4.W.+U.V$..+.
+000007c0: 5c57 a59d 88a2 0488 05cb 997e ac41 9155  \W.........~.A.U
+000007d0: 24d1 f98a 0b49 1639 84bd c581 b595 f00b  $....I.9........
+000007e0: e18f 5d18 bcf6 2470 1d1d 55b0 440a 2596  ..]...$p..U.D.%.
+000007f0: fa04 a09d 86f4 51fc d875 307e 9582 ed71  ......Q..u0~...q
+00000800: 0ede 87e4 3b92 3e30 53c3 3d2b 197e 9055  ....;.>0S.=+.~.U
+00000810: b8c7 0a0f 60d8 fd34 1a06 69d5 5a89 2079  ....`..4..i.Z. y
+00000820: 1f44 0bf6 dc3c d43f 5bb2 9cde 34d2 b548  .D...<.?[...4..H
+00000830: 59fe 2485 a954 8eac 9c28 3d49 99a6 698c  Y.$..T...(=I..i.
+00000840: ba30 151b 7a78 0051 c9aa 1c56 2c07 af17  .0..zx.Q...V,...
+00000850: 7a5e 1739 fdbd 9c67 1226 50fb 41ae a9e4  z^.9...g.&P.A...
+00000860: 44d3 91e0 1aa4 b6a3 fe59 59d5 d8a3 4c80  D........YY...L.
+00000870: 88ad 2bfa a762 92c2 bb03 1282 7060 2449  ..+..b......p`$I
+00000880: 4416 6a46 7466 5532 8fd1 38ba fbce 7456  D.jFtfU2..8...tV
+00000890: 2dee e6b4 28a9 24ba 92f4 5270 a685 bcbf  -...(.$...Rp....
+000008a0: fc35 9fdf bd50 2139 96fc 3fe8 9024 260d  .5...P!9..?..$&.
+000008b0: 0e84 ded0 6bee dfa6 0158 caa8 d5da 4c4b  ....k....X....LK
+000008c0: 0bee cfc7 1790 ef6b f200 d987 1aa7 bb97  .......k........
+000008d0: f31c d28b 3bf7 3c91 11be 7f1a f9dd b137  ....;.<........7
+000008e0: 1cba b6e7 8f02 db0f fca9 3dec 4e3d bb3b  ..........=.N=.;
+000008f0: 1804 43cf f307 7ee8 3e43 3032 8c12 412a  ..C...~.>C02..A*
+00000900: 9ded 0a6b a063 e443 158f 5c97 64db 7ab0  ...k.c.C..\.d.z.
+00000910: 1b55 2c3d d078 7277 976d ec9b a1f5 3d9b  .U,=.xrw.m....=.
+00000920: 804d 0bbb 6174 a30e 1230 536b 7bcb 782a  .M..at...0Sk{.x*
+00000930: 36a0 9020 e806 c87a 6ce7 9d9e 0f41 6e6a  6.. ...zl....Anj
+00000940: ef2d 4b75 064b 70e8 ee9f fda0 6c95 0165  .-Ku.Kp.....l..e
+00000950: 1cf8 1dd8 075a 37d4 62f4 8ad2 b8a1 3485  .....Z7.b.....4.
+00000960: cb36 c32b 4ace 0b4e 75b7 046e b5b5 78ad  .6.+J..Nu..n..x.
+00000970: f06b d341 31b4 6563 eb2c 83a2 2373 863c  .k.A1.ec.,..#s.<
+00000980: 4f71 5dc5 765b 42f2 6426 2d63 ea85 a177  Oq].v[B.d&-c...w
+00000990: 8a3b 6605 ddea 0ba5 6b0b 4a63 400f fbee  .;f.....k.Jc@...
+000009a0: a0eb 9efa b63b e940 817a a79e ddf3 3b9e  .....;.@.z....;.
+000009b0: 3df2 c7de 24e8 4ec6 9361 600a 64ba 7df4  =...$.N..a`.d.}.
+000009c0: 3f7a 5e2d f8a8 fd8c 1896 1991 7a2e 49b2  ?z^-........z.I.
+000009d0: 868f cf15 5d0e 8902 4535 0101 5f10 64cb  ....]...E5.._.d.
+000009e0: da69 77f5 ff02 0000 ffff 0300 504b 0304  .iw.........PK..
+000009f0: 1400 0600 0800 0000 2100 813e 9497 f300  ........!..>....
+00000a00: 0000 ba02 0000 1a00 0801 786c 2f5f 7265  ..........xl/_re
+00000a10: 6c73 2f77 6f72 6b62 6f6f 6b2e 786d 6c2e  ls/workbook.xml.
+00000a20: 7265 6c73 20a2 0401 28a0 0001 0000 0000  rels ...(.......
+00000a30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000a40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000a50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000a60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000a70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000a80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000a90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000aa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ab0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ac0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ad0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ae0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000af0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000b00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000b10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000b20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000b30: 0000 0000 0000 0000 0000 ac52 4d4b c430  ...........RMK.0
-00000b40: 10bd 0bfe 8730 779b 7615 11d9 742f 22ec  .....0w.v...t/".
-00000b50: 55eb 0f08 c9b4 29db 2621 337e f4df 1b2a  U.....).&!3~...*
-00000b60: ba5d 58d6 4b2f 036f 8679 efcd c776 f735  .]X.K/.o.y...v.5
-00000b70: 0ee2 0313 f5c1 2ba8 8a12 047a 136c ef3b  ......+....z.l.;
-00000b80: 056f cdf3 cd03 0862 edad 1e82 4705 1312  .o.....b....G...
-00000b90: ecea ebab ed0b 0e9a 7313 b93e 92c8 2c9e  ........s..>..,.
-00000ba0: 1438 e6f8 2825 1987 a3a6 2244 f4b9 d286  .8..(%...."D....
-00000bb0: 346a ce30 7532 6a73 d01d ca4d 59de cbb4  4j.0u2js...MY...
-00000bc0: e480 fa84 53ec ad82 b4b7 b720 9a29 66e5  ....S...... .)f.
-00000bd0: ffb9 43db f606 9f82 791f d1f3 1909 493c  ..C.....y.....I<
-00000be0: 0d79 00d1 e8d4 212b f8c1 45f6 08f2 bcfc  .y....!+..E.....
-00000bf0: 664d 79ce 6bc1 a3fa 0ce5 1cab 4b1e aa35  fMy.k.......K..5
-00000c00: 3d7c 8674 2087 c847 1f7f 2992 73e5 a299  =|.t ..G..).s...
-00000c10: bb55 efe1 7442 fbca 29bf dbf2 2ccb f4ef  .U..tB..)...,...
-00000c20: 66e4 c9c7 d5df 0000 00ff ff03 0050 4b03  f............PK.
-00000c30: 0414 0006 0008 0000 0021 0098 7c3d 912c  .........!..|=.,
-00000c40: 0300 002d 0700 0018 0000 0078 6c2f 776f  ...-.......xl/wo
-00000c50: 726b 7368 6565 7473 2f73 6865 6574 312e  rksheets/sheet1.
-00000c60: 786d 6c9c 93db 8e9b 3010 86ef 2bf5 1d2c  xml.....0...+..,
-00000c70: df07 0309 6c82 20ab b6ab a87b 57f5 78ed  ....l. ....{W.x.
-00000c80: 9821 58b1 31b5 9d93 aabe 7bc7 9043 a5dc  .!X.1.....{..C..
-00000c90: 448b c036 f6f8 fb67 f04f f97c d48a ecc1  D..6...g.O.|....
-00000ca0: 3a69 ba8a 2651 4c09 74c2 d4b2 db54 f4c7  :i..&QL.t....T..
-00000cb0: f7d5 644e 89f3 bcab b932 1d54 f404 8e3e  ..dN.....2.T...>
-00000cc0: 2fdf bf2b 0fc6 6e5d 0be0 0912 3a57 d1d6  /..+..n]....:W..
-00000cd0: fbbe 60cc 8916 3477 91e9 a1c3 95c6 58cd  ..`...4w......X.
-00000ce0: 3dbe da0d 73bd 055e 0f9b b462 691c e74c  =...s..^...bi..L
-00000cf0: 73d9 d191 50d8 4718 a669 a480 1723 761a  s...P.G..i...#v.
-00000d00: 3a3f 422c 28ee 317f d7ca de5d 685a 3c82  :?B,(.1....]hZ<.
-00000d10: d3dc 6e77 fd44 18dd 2362 2d95 f4a7 014a  ..nw.D..#b-....J
-00000d20: 8916 c5eb a633 96af 15d6 7d4c 665c 90a3  .....3....}Lf\..
-00000d30: c53b c567 7a91 19e6 ef94 b414 d638 d3f8  .;.gz........8..
-00000d40: 08c9 6ccc f9be fc05 5b30 2eae a4fb fa1f  ..l.....[0......
-00000d50: c224 3366 612f c301 de50 e9db 524a b22b  .$3fa/...P..RJ.+
-00000d60: 2bbd c1a6 6f84 e557 58f8 5cb6 d8c9 baa2  +...o..WX.\.....
-00000d70: 7fe2 f335 c13e 094d 7c6b 2e6b 7fe9 b2ac  ...5.>.M|k.k....
-00000d80: 259e 70a8 8a58 682a fa21 293e e694 2dcb  %.p..Xh*.!)>..-.
-00000d90: c13f 3f25 1cdc 7f63 e2f9 fa1b 2810 1e50  .??%...c....(..P
-00000da0: 23a1 24d8 736d cc36 04be e254 8c44 3704  #.$.sm.6...T.D7.
-00000db0: 0422 175e eee1 1328 85e0 1c1d fe7b d418  .".^...(.....{..
-00000dc0: 04d8 5561 59de c617 b5d5 60e8 2f96 d4d0  ..UaY.....`./...
-00000dd0: f09d f25f cde1 33c8 4deb 5136 c332 834f  ..._..3.M.Q6.2.O
-00000de0: 8afa f402 4ea0 4151 384a b390 b630 0a11  ....N.AQ8J...0..
-00000df0: d812 2dc3 9f86 06e3 c731 5559 fb16 478b  ..-......1UY..G.
-00000e00: 287b 8aa7 0986 9335 38bf 9201 4989 d839  ({.....58...I..9
-00000e10: 6ff4 af73 d019 3542 f08c 0608 f687 713d  o..s..5B......q=
-00000e20: 9d45 f32c 9be5 f327 a4dc ef64 4316 ff00  .E.,...'...dC...
-00000e30: 0000 ffff 0000 00ff ff94 d241 0ec2 2010  ...........A.. .
-00000e40: 05d0 ab10 0e20 8542 170d 25d1 f422 0449  ..... .B..%..".I
-00000e50: 5c55 d321 b5de de19 6350 0c0b d901 f3f3  \U.!....cP......
-00000e60: fe2c b070 8931 cd3e 7967 d7eb 9dad 1397  .,.p.1.>yg......
-00000e70: 9cc1 cd2f 80a7 5171 b64b edc3 787e cc11  .../..Qq.K..x~..
-00000e80: 425c d2c4 bb83 32dc d940 d923 86f1 09f0  B\....2..@.#....
-00000e90: beb9 ce8a cd59 11de b3d3 f74c e699 c09a  .....Y.....L....
-00000ea0: dc85 feff 5d14 7ead 971b 555d ed5b 540a  ....].~...U].[T.
-00000eb0: 976a 5f57 758b 4ae1 52d5 75d5 b4a8 142e  .j_Wu.J.R.u.....
-00000ec0: 5553 5787 1695 c2a5 3afc a8e2 f34b 9e00  USW.....:....K..
-00000ed0: 0000 ffff 0000 00ff ff4c 8ecd 0ac2 400c  .........L....@.
-00000ee0: 845f 65c9 0368 ad3f 65c5 edc9 8b07 41f0  ._e..h.?e.....A.
-00000ef0: 09b6 36b6 c1ba 59d2 54c1 a777 2b16 bde5  ..6...Y.T..w+...
-00000f00: 9b19 26b3 8bbe c1a3 9786 426f 3abc aa83  ..&.......Bo:...
-00000f10: 6c56 8011 6ada e956 8e1f 750d a662 55be  lV..j..V..u..bU.
-00000f20: 4fd4 a2af 5146 5a82 b932 eb04 f372 37f6  O...QFZ..2...r7.
-00000f30: 9e51 8768 a28f 2867 7aa1 030b 8685 30a8  .Q.h..(gz.....0.
-00000f40: 57e2 e020 b2a8 7852 306d d25f 9c8c 6e1f  W.. ..xR0m._..n.
-00000f50: c9c1 2ab7 2bbb 2972 9b8a 1f28 4a97 af91  ..*.+.)r...(J...
-00000f60: a569 5baa 1dc8 a15e 40fa a3be eaf0 e445  .i[....^@......E
-00000f70: 7b73 e121 a4cd 0bf8 537f e97c 4ccf 7ff1  {s.!....S..|L...
-00000f80: 044f 965b df22 6af9 0600 00ff ff03 0050  .O.[."j........P
-00000f90: 4b03 0414 0006 0008 0000 0021 0075 3e99  K..........!.u>.
-00000fa0: 6993 0600 008c 1a00 0013 0000 0078 6c2f  i............xl/
-00000fb0: 7468 656d 652f 7468 656d 6531 2e78 6d6c  theme/theme1.xml
-00000fc0: ec59 5b8b db46 147e 2ff4 3f08 bd3b be49  .Y[..F.~/.?..;.I
-00000fd0: b2bd c41b 6cd9 4eda ec26 21eb a4e4 716c  ....l.N..&!...ql
-00000fe0: 8fad c98e 3446 33de 8d09 8192 3cf5 a550  ....4F3.....<..P
-00000ff0: 484b 5f0a 7deb 4329 0d34 d0d0 97fe 9885  HK_.}.C).4......
-00001000: 8436 fd11 3d33 92ad 99f5 389b cba6 b425  .6..=3....8....%
-00001010: 6b58 a4d1 77ce 7c73 ced1 3717 5dbc 742f  kX..w.|s..7.].t/
-00001020: a6ce 114e 3961 49db ad5e a8b8 0e4e c66c  ...N9aI..^...N.l
-00001030: 4292 59db bd35 1c94 9aae c305 4a26 88b2  B.Y..5......J&..
-00001040: 04b7 dd25 e6ee a5dd 8f3f ba88 7644 8463  ...%.....?..vD.c
-00001050: ec80 7dc2 7750 db8d 8498 ef94 cb7c 0ccd  ..}.wP.......|..
-00001060: 885f 6073 9cc0 b329 4b63 24e0 369d 9527  ._`s...)Kc$.6..'
-00001070: 293a 06bf 312d d72a 95a0 1c23 92b8 4e82  ):..1-.*...#..N.
-00001080: 6270 7b7d 3a25 63ec 0ca5 4b77 77e5 bc4f  bp{}:%c...Kww..O
-00001090: e136 115c 368c 697a 205d 63c3 4261 2787  .6.\6.iz ]c.Ba'.
-000010a0: 5589 e04b 1ed2 d439 42b4 ed42 3f13 763c  U..K...9B..B?.v<
-000010b0: c4f7 84eb 50c4 053c 68bb 15f5 e796 772f  ....P..<h.....w/
-000010c0: 96d1 4e6e 44c5 165b cd6e a0fe 72bb dc60  ..NnD..[.n..r..`
-000010d0: 7258 537d a6b3 d1ba 53cf f3bd a0b3 f6af  rXS}....S.......
-000010e0: 0054 6ce2 fa8d 7ed0 0fd6 fe14 008d c730  .Tl...~........0
-000010f0: d28c 8bee d3ef b6ba 3d3f c76a a0ec d2e2  ........=?.j....
-00001100: bbd7 e8d5 ab06 5ef3 5fdf e0dc f1e5 cfc0  ......^._.......
-00001110: 2b50 e6df dbc0 0f06 2144 d1c0 2b50 86f7  +P......!D..+P..
-00001120: 2d31 69d4 42cf c02b 5086 0f36 f08d 4aa7  -1i.B..+P..6..J.
-00001130: e735 0cbc 0245 9424 871b e88a 1fd4 c3d5  .5...E.$........
-00001140: 68d7 9029 a357 acf0 96ef 0d1a b5dc 7981  h..).W........y.
-00001150: 826a 5857 97ec 62ca 12b1 add6 6274 97a5  .jXW..b.....bt..
-00001160: 0300 4820 4582 248e 58ce f114 8da1 8a43  ..H E.$.X......C
-00001170: 44c9 2825 ce1e 9945 5078 7394 300e cd95  D.(%...EPxs.0...
-00001180: 5a65 50a9 c37f f9f3 d495 8a08 dac1 48b3  ZeP...........H.
-00001190: 96bc 8009 df68 927c 1c3e 4ec9 5cb4 dd4f  .....h.|.>N.\..O
-000011a0: c1ab ab41 9e3f 7b76 f2f0 e9c9 c35f 4f1e  ...A.?{v....._O.
-000011b0: 3d3a 79f8 73de b772 65d8 5d41 c94c b77b  =:y.s..re.]A.L.{
-000011c0: f9c3 577f 7df7 b9f3 e72f dfbf 7cfc 75d6  ..W.}..../..|.u.
-000011d0: f569 3cd7 f12f 7efa e2c5 6fbf bfca 3d8c  .i<../~...o...=.
-000011e0: b808 c5f3 6f9e bc78 fae4 f9b7 5ffe f1e3  ....o..x...._...
-000011f0: 638b f74e 8a46 3a7c 4862 cc9d 6bf8 d8b9  c..N.F:|Hb..k...
-00001200: c962 18a0 853f 1ea5 6f66 318c 1031 2c50  .b...?..of1..1,P
-00001210: 04be 2dae fb22 3280 d796 88da 705d 6c86  ..-.."2.....p]l.
-00001220: f076 0a2a 6303 5e5e dc35 b81e 44e9 4210  .v.*c.^^.5..D.B.
-00001230: 4bcf 57a3 d800 ee33 46bb 2cb5 06e0 aaec  K.W....3F.,.....
-00001240: 4b8b f070 91cc ec9d a70b 1d77 13a1 235b  K..p.......w..#[
-00001250: df21 4a8c 04f7 1773 9057 6273 1946 d8a0  .!J....s.Wbs.F..
-00001260: 7983 a244 a019 4eb0 70e4 3376 88b1 6574  y..D..N.p.3v..et
-00001270: 7708 31e2 ba4f c629 e36c 2a9c 3bc4 e922  w.1..O.).l*.;.."
-00001280: 620d c990 8c8c 422a 8cae 9018 f2b2 b411  b.....B*........
-00001290: 8454 1bb1 d9bf ed74 19b5 8dba 878f 4c24  .T.....t......L$
-000012a0: bc16 885a c80f 3135 c278 192d 048a 6d2e  ...Z..15.x.-..m.
-000012b0: 8728 a67a c0f7 9088 6c24 0f96 e958 c7f5  .(.z....l$...X..
-000012c0: b980 4ccf 3065 4e7f 8239 b7d9 5c4f 61bc  ..L.0eN..9..\Oa.
-000012d0: 5ad2 af82 c2d8 d3be 4f97 b189 4c05 39b4  Z.......O...L.9.
-000012e0: f9dc 438c e9c8 1e3b 0c23 14cf ad9c 4912  ..C....;.#....I.
-000012f0: e9d8 4ff8 2194 2872 6e30 6183 ef33 f30d  ..O.!.(rn0a..3..
-00001300: 91f7 9007 946c 4df7 6d82 8d74 9f2d 04b7  .....lM.m..t.-..
-00001310: 405c 754a 4581 c827 8bd4 92cb cb98 99ef  @\uJE..'........
-00001320: e392 4e11 562a 03da 6f48 7a4c 9233 f5fd  ..N.V*..oHzL.3..
-00001330: 94b2 fbff 8cb2 db35 fa1c 34dd eef8 5dd4  .......5..4...].
-00001340: bc93 12eb 3b75 e594 866f c3fd 0795 bb87  ....;u...o......
-00001350: 16c9 0d0c 2fcb e6cc f541 b83f 08b7 fbbf  ..../....A.?....
-00001360: 17ee 6def f2f9 cb75 a1d0 20de c55a 5dad  ..m....u.. ..Z].
-00001370: dce3 ad0b f729 a1f4 402c 29de e36a edce  .....)..@,)..j..
-00001380: 615e 9a0c a051 6d2a d4ce 72bd 919b 4770  a^...Qm*..r...Gp
-00001390: 996f 130c dc2c 45ca c649 99f8 8c88 e820  .o...,E..I..... 
-000013a0: 4273 58e0 57d5 3674 c673 d733 eecc 1987  BsX.W.6t.s.3....
-000013b0: 75bf 6a56 1b62 7cca b7da 3d2c e27d 36c9  u.jV.b|...=,.}6.
-000013c0: f6ab d5aa dc9b 66e2 c191 28da 2bfe ba1d  ......f...(.+...
-000013d0: f61a 2243 078d 620f b676 af76 b533 b557  .."C..b..v.v.3.W
-000013e0: 5e11 90b6 6f42 42eb cc24 51b7 9068 ac1a  ^...oBB..$Q..h..
-000013f0: 210b af22 a146 762e 2c5a 1616 4de9 7e95  !..".Fv.,Z..M.~.
-00001400: aa55 16d7 a100 6aeb acc0 c2c9 81e5 56db  .U....j.......V.
-00001410: f5bd ec1c 00b6 5488 e289 cc53 7624 b0ca  ......T....Sv$..
-00001420: ae4c ceb9 667a 5b30 a95e 01b0 8a58 5540  .L..fz[0.^...XU@
-00001430: 91e9 96e4 ba75 7872 7459 a9bd 46a6 0d12  .....uxrtY..F...
-00001440: 5ab9 9924 b432 8cd0 04e7 d5a9 1f9c 9c67  Z..$.2.........g
-00001450: ae5b 454a 0d7a 3214 abb7 a1a0 d168 be8f  .[EJ.z2......h..
-00001460: 5c4b 1139 a50d 34d1 9582 26ce 71db 0dea  \K.9..4...&.q...
-00001470: 3e9c 8d8d d1bc ed4e 61df 0f97 f11c 6a87  >......Na.....j.
-00001480: cb05 2fa2 3338 3c1b 8b34 7be1 df46 59e6  ../.38<..4{..FY.
-00001490: 2917 3dc4 a32c e04a 7432 3588 89c0 a943  ).=..,.Jt25....C
-000014a0: 49dc 76e5 f0d7 d540 13a5 218a 5bb5 0682  I.v....@..!.[...
-000014b0: f0af 25d7 0259 f9b7 9183 a49b 49c6 d329  ..%..Y......I..)
-000014c0: 1e0b 3ded 5a8b 8c74 760b 0a9f 6985 f5a9  ..=.Z..tv...i...
-000014d0: 327f 7bb0 b464 0b48 f741 3439 7646 7491  2.{..d.H.A49vFt.
-000014e0: de44 5062 7ea3 2a03 3821 1c8e 7faa 5934  .DPb~.*.8!....Y4
-000014f0: 2704 ce33 d742 56d4 dfa9 8929 975d fd40  '..3.BV....).].@
-00001500: 51d5 50d6 8ee8 3c42 f98c a28b 7906 5722  Q.P...<B....y.W"
-00001510: baa6 a3ee d631 d0ee f231 4340 3743 389a  .....1...1C@7C8.
-00001520: c909 f69d 67dd b3a7 6a19 394d 348b 39d3  ....g...j.9M4.9.
-00001530: 5015 396b dac5 f4fd 4df2 1aab 6212 3558  P.9k....M...b.5X
-00001540: 65d2 adb6 0dbc d0ba d64a eba0 50ad b3c4  e........J..P...
-00001550: 19b3 ee6b 4c08 1ab5 a233 839a 64bc 29c3  ...kL....3..d.).
-00001560: 52b3 f356 93da 392e 08b4 4804 5be2 b69e  R..V..9...H.[...
-00001570: 23ac 9178 db99 1fec 4e57 ad9c 2056 eb4a  #..x....NW.. V.J
-00001580: 55f8 eac3 87fe 6d82 8dee 8278 f4e0 1478  U.....m....x...x
-00001590: 4105 57a9 842f 0f29 8245 5f76 8e9c c906  A.W../.).E_v....
-000015a0: bc22 f744 be46 842b 6791 92b6 7bbf e277  .".D.F.+g...{..w
-000015b0: bcb0 e687 a54a d3ef 97bc ba57 2935 fd4e  .....J.....W)5.N
-000015c0: bdd4 f1fd 7ab5 ef57 2bbd 6eed 014c 2c22  ....z..W+.n..L,"
-000015d0: 8aab 7ef6 d165 0007 5174 997f 7a51 ed1b  ..~..e..Qt..zQ..
-000015e0: 9f5f e2d5 59db 8531 8bcb 4c7d 5e29 2be2  ._..Y..1..L}^)+.
-000015f0: eaf3 4bb5 b6fd f38b 4340 74ee 07b5 41ab  ..K.....C@t...A.
-00001600: deea 06a5 56bd 3328 79bd 6eb3 d40a 836e  ....V.3(y.n....n
-00001610: a917 848d dea0 17fa cdd6 e081 eb1c 29b0  ..............).
-00001620: d7a9 875e d06f 9682 6a18 96bc a022 e937  ...^.o..j....".7
-00001630: 5ba5 8657 ab75 bc46 a7d9 f73a 0ff2 650c  [..W.u.F...:..e.
-00001640: 8c3c 938f 3c16 105e c56b f76f 0000 00ff  .<..<..^.k.o....
-00001650: ff03 0050 4b03 0414 0006 0008 0000 0021  ...PK..........!
-00001660: 0097 e7f0 ba0f 0300 00cf 0700 000d 0000  ................
-00001670: 0078 6c2f 7374 796c 6573 2e78 6d6c a455  .xl/styles.xml.U
-00001680: 5d8f 9b3a 107d afd4 ff60 f99d 35b0 214d  ]..:.}...`..5.!M
-00001690: 22a0 6a36 8b54 a9b7 aab4 5ba9 af0e 98c4  ".j6.T....[.....
-000016a0: 5a7f 20db ec92 56f7 bf77 0c24 21fd eef6  Z. ...V..w.$!...
-000016b0: 2519 8fed e333 3367 86f4 7527 057a 64c6  %....33g..u'.zd.
-000016c0: 72ad 321c 5d85 1831 55ea 8aab 5d86 3fde  r.2.]..1U...].?.
-000016d0: 17c1 0223 eba8 aaa8 d08a 65f8 c02c 7e9d  ...#......e..,~.
-000016e0: bf7c 915a 7710 ec6e cf98 4300 a16c 86f7  .|.Zw..n..C..l..
-000016f0: ce35 2b42 6cb9 6792 da2b dd30 053b b536  .5+Bl.g..+.0.;.6
-00001700: 923a 589a 1db1 8d61 b4b2 fe92 1424 0ec3  .:X....a.....$..
-00001710: 3991 942b 3c20 ac64 f927 2092 9a87 b609  9..+< .d.' .....
-00001720: 4a2d 1bea f896 0bee 0e3d 1646 b25c bddd  J-.......=.F.\..
-00001730: 296d e856 00d5 2e9a d112 75d1 dcc4 a833  )m.V......u....3
-00001740: c747 7aef 77ef 485e 1a6d 75ed ae00 97e8  .Gz.w.H^.mu.....
-00001750: bae6 25fb 9eee 922c 092d cf48 80fc 3ca4  ..%....,.-.H..<.
-00001760: 2821 617c 117b 679e 8934 2386 3d72 5f3e  (!a|.{g..4#.=r_>
-00001770: 9ca7 b556 cea2 52b7 ca65 3806 a23e 05ab  ...V..R..e8..>..
-00001780: 07a5 9f54 e1b7 a0c2 e3a9 3cb5 9fd1 2315  ...T......<...#.
-00001790: e089 30c9 d352 0b6d 9083 d241 e67a 8fa2  ..0..R.m...A.z..
-000017a0: 920d 276e a8e0 5bc3 fdb1 9a4a 2e0e 833b  ..'n..[....J...;
-000017b0: f68e beda e339 c921 f7de 493c 8f81 cd5f  .....9.!..I<..._
-000017c0: bda3 5bc3 9941 efd9 d3b7 6f5d 4f60 7b74  ..[..A....o]O`{t
-000017d0: 0bf0 5c88 49b0 8323 4f41 158e 1955 c02e  ..\.I..#OA...U..
-000017e0: 1aed fb43 0351 2910 f000 035b bf3d bd33  ...C.Q)....[.=.3
-000017f0: f410 c5c9 e402 e91f ccd3 ad36 1534 cc31  ...........6.4.1
-00001800: cd3e a383 2b4f 05ab 1dc4 6ff8 6eef ff9d  .>..+O....o.n...
-00001810: 6ee0 77ab 9d03 51e5 69c5 e94e 2b2a 7c86  n.w...Q.i..N+*|.
-00001820: 8e37 4603 c229 9910 77be a93e d517 d85d  .7F..)..w..>...]
-00001830: 8d54 2b0b e9de 5619 86f6 f4b9 3d9a 10c8  .T+...V.....=...
-00001840: 680e 78c3 c2e3 4fd1 06ec 096c 0c94 ff1e  h.x...O....l....
-00001850: 1675 f509 ff67 b723 e0f7 6352 a7db 8836  .u...g.#..cR...6
-00001860: 8d38 7839 8e42 ebb9 02bb 490a 2e12 700a  .8x9.B....I...p.
-00001870: 0579 4966 f8bd 9f28 02c4 3dd2 41db 960b  .yIf...(..=.A...
-00001880: c7d5 0f82 07cc aabb 4c27 ac4f ca74 863f  ........L'.O.t.?
-00001890: 8cda 0d7d a175 eb04 5753 8fdd d34a 3f0d  ...}.u..WS...J?.
-000018a0: 7aef 8fb4 837d d412 4c4e f746 f09d 1adc  z....}..LN.F....
-000018b0: 5b6a 9947 e83b e3cf fbeb 37ba 9ff6 d859  [j.G.;....7....Y
-000018c0: c47d 8b91 3e1c ff0b a13a 3ff7 7a09 9df2  .}..>....:?.z...
-000018d0: 077a a958 4d5b e1ee 4f9b 193e dbff b18a  .z.XM[..O..>....
-000018e0: b712 26c5 78ea 037f d4ae 87c8 f0d9 7ee7  ..&.x.........~.
-000018f0: f51c cd7d 54ac 73ef 2cf4 36fc 23e8 d60c  ...}T.s.,.6.#...
-00001900: 7fb9 5dbf 5a6e 6e8b 3858 84eb 4530 bb66  ..].Znn.8X..E0.f
-00001910: 49b0 4cd6 9b20 99dd ac37 9b62 19c6 e1cd  I.L.. ...7.b....
-00001920: ff93 e9fb 0fb3 b7ff 5880 74a3 d9ca 0a98  ........X.t.....
-00001930: d066 0c76 247f 77f6 6578 b218 e8f7 9d0c  .f.v$.w.ex......
-00001940: b4a7 dc97 f13c 7c93 4461 505c 8751 309b  .....<|.DaP\.Q0.
-00001950: d345 b098 5f27 4191 44f1 663e 5bdf 2645  .E.._'A.D.f>[.&E
-00001960: 32e1 9e3c 7346 8724 8a86 69ef c927 2bc7  2..<sF.$..i..'+.
-00001970: 652f 934b faf7 532f 1409 96bf 0882 1c2b  e/.K..S/.......+
-00001980: 41ce 5fe2 fc2b 0000 00ff ff03 0050 4b03  A._..+.......PK.
-00001990: 0414 0006 0008 0000 0021 0065 2d2a 77c7  .........!.e-*w.
-000019a0: 0000 005e 0100 0014 0000 0078 6c2f 7368  ...^.......xl/sh
-000019b0: 6172 6564 5374 7269 6e67 732e 786d 6c7c  aredStrings.xml|
-000019c0: 9031 4ec4 3010 457b 24ee 604d cf3a 1b41  .1N.0.E{$.`M.:.A
-000019d0: 368b 6c6f 0142 a206 0e60 e299 8da5 781c  6.lo.B...`....x.
-000019e0: 3c0e 82db 1384 6880 a57c ffe9 35df 1cde  <.....h..|..5...
-000019f0: d2a4 5eb1 48cc 6c61 bb69 4021 0f39 443e  ..^.H.la.i@!.9D>
-00001a00: 5a78 7abc bbe8 4149 f51c fc94 192d bca3  Zxz...AI.....-..
-00001a10: c0c1 9d9f 1991 aad6 96c5 c258 eb7c adb5  ...........X.|..
-00001a20: 0c23 262f 9b3c 23af 8672 49be ae58 8e5a  .#&/.<#..rI..X.Z
-00001a30: e682 3ec8 8858 d3a4 dba6 e974 f291 410d  ..>..X.....t..A.
-00001a40: 79e1 6a61 076a e1f8 b2e0 cd37 3b23 d199  y.ja.j.....7;#..
-00001a50: eaee 6f8d aece e84f fa5a 1e90 2597 9f6b  ..o....O.Z..%..k
-00001a60: db07 1aba abdd 96ba 4ba2 bf6c d89f b66d  ........K..l...m
-00001a70: 4f74 da7a 4fe1 9ff6 99f0 b7d5 eb3f ee03  Ot.zO........?..
-00001a80: 0000 ffff 0300 504b 0304 1400 0600 0800  ......PK........
-00001a90: 0000 2100 41bf f860 d900 0000 ca01 0000  ..!.A..`........
-00001aa0: 2300 0000 786c 2f77 6f72 6b73 6865 6574  #...xl/worksheet
-00001ab0: 732f 5f72 656c 732f 7368 6565 7431 2e78  s/_rels/sheet1.x
-00001ac0: 6d6c 2e72 656c 73ac 91c1 4ec3 300c 40ef  ml.rels...N.0.@.
-00001ad0: 48fc 43e4 3b49 bb03 4268 e92e 0869 5718  H.C.;I..Bh...iW.
-00001ae0: 1fe0 a56e 1bd1 3a51 6c10 fb7b 8276 a1d3  ...n..:Ql..{.v..
-00001af0: 242e 9c2c dbf2 f393 bddd 7d2d b3f9 a422  $..,......}-..."
-00001b00: 31b1 87d6 3660 8843 ea23 8f1e de0e cf77  1...6`.C.#.....w
-00001b10: 0f60 4491 7b9c 1393 8713 09ec badb 9bed  .`D.{...........
-00001b20: 0bcd a875 48a6 98c5 540a 8b87 4935 3f3a  ...uH...T...I5?:
-00001b30: 2761 a205 c5a6 4c5c 3b43 2a0b 6a4d cbe8  'a....L\;C*.jM..
-00001b40: 3286 771c c96d 9ae6 de95 df0c e856 4cb3  2.w..m.......VL.
-00001b50: ef3d 947d bf01 7338 e5ba f96f 761a 8618  .=.}..s8...ov...
-00001b60: e829 858f 8558 afac 708a c799 2a10 cb48  .)...X..p...*..H
-00001b70: eac1 da73 45ce a1b5 5516 dc75 8ff6 3f3d  ...sE...U..u..?=
-00001b80: 7289 ac54 5e49 b51e 5a56 4617 3d77 91b7  r..T^I..ZVF.=w..
-00001b90: f618 f947 d2ad 3ed0 7d03 0000 ffff 0300  ...G..>.}.......
-00001ba0: 504b 0304 1400 0600 0800 0000 2100 1157  PK..........!..W
-00001bb0: 5b9e 7c01 0000 d40d 0000 2700 0000 786c  [.|.......'...xl
-00001bc0: 2f70 7269 6e74 6572 5365 7474 696e 6773  /printerSettings
-00001bd0: 2f70 7269 6e74 6572 5365 7474 696e 6773  /printerSettings
-00001be0: 312e 6269 6eec 57bd 4a03 4110 feee 47c8  1.bin.W.J.A...G.
-00001bf0: e915 56c1 4e3b 1b0b d1b3 5763 2504 8358  ..V.N;....Wc%..X
-00001c00: 5ca9 100b 9b28 26bd f80c 76be 854f e20b  \....(&...v..O..
-00001c10: 046c 047d 008b 3472 ce77 b981 756f ef44  .l.}..4r.w..uo.D
-00001c20: 4821 b273 4c66 7676 6676 f6cb c0cd f570  H!.sLfvvfv.....p
-00001c30: 8111 ae85 37d0 478e 3dec 605b f431 2e71  ....7.G.=.`[.1.q
-00001c40: 8b2b f91d cb6a 50ea 234c 4a2b 0c0a e224  .+...jP.#LJ+...$
-00001c50: 9d62 9646 2ff7 5180 048f 2b59 6788 00dd  .b.F/.Q...+Yg...
-00001c60: e0b3 0845 4238 c001 3233 6841 3ab3 87e5  ...EB8..23hA:...
-00001c70: 093c a54e b314 383c 3eea 2722 49d3 0ef0  .<.N..8<>.'"I...
-00001c80: 2c92 acc4 b8ce 2910 4f80 2d59 9c09 9f9f  ,.....).O.-Y....
-00001c90: 00af 37f5 b5ed 47df 0f87 bfda 359f ed97  ..7...G.....5...
-00001ca0: 8779 b8b6 200c 7c9a 3a02 ab9b 1e15 8f80  .y.. .|.:.......
-00001cb0: 47c0 23f0 f710 e0fb 2aaa 98d5 cddf 91ae  G.#.....*.......
-00001cc0: 3ac3 d2cf ff87 1e01 2290 c8a3 7dc3 1eb2  :......."...}...
-00001cd0: 2916 0367 19fa 7445 a124 b9e6 22da b9af  )..g..tE.$.."...
-00001ce0: b393 ed37 1443 22ac f30e f7ed b5d6 309f  ...7.C".......0.
-00001cf0: f09a cfa9 cac0 832a 22f7 97e7 fe8c 5d37  .......*".....]7
-00001d00: eca6 cabd a2f8 be29 6135 72dd afe9 cee6  .......)a5r.....
-00001d10: 3ded dc36 a69a a329 9789 0d7d ee2c 36cf  =..6...)...}.,6.
-00001d20: a2fe 2680 5bd7 71de bcad f606 a85a 3171  ..&.[.q......Z1q
-00001d30: 61c6 5a7e a225 c341 b131 fbc5 8e7f af72  a.Z~.%.A.1.....r
-00001d40: ba70 6bc2 963d aba4 7dd4 5657 5baf fd06  .pk..=..}.VW[...
-00001d50: b7de 3ffe e6e9 654f bb5f 0000 00ff ff03  ..?...eO._......
-00001d60: 0050 4b03 0414 0006 0008 0000 0021 0090  .PK..........!..
-00001d70: 52f4 5fe1 0100 0094 0300 0014 0000 0078  R._............x
-00001d80: 6c2f 7461 626c 6573 2f74 6162 6c65 312e  l/tables/table1.
-00001d90: 786d 6c9c 93cd 8e9b 3014 85f7 95fa 0ec8  xml.....0.......
-00001da0: 7b07 cc8f 0328 6414 fea4 486d 17cd f401  {....(d...Hm....
-00001db0: 3c60 12ab d846 b699 4954 f5dd 6b60 2693  <`...F..IT..k`&.
-00001dc0: 5136 6d77 70e0 7e3e e75c d83c 9c79 ef3c  Q6mwp.~>.\.<.y.<
-00001dd0: 53a5 9914 1940 2b0f 3854 34b2 65e2 9881  S....@+.8T4.e...
-00001de0: 1f8f 358c 81a3 0d11 2de9 a5a0 19b8 500d  ..5.....-.....P.
-00001df0: 1eb6 9f3f 6d0c 79ea a963 a785 cec0 c998  ...?m.y..c......
-00001e00: 2175 5ddd 9c28 277a 2507 2aec 934e 2a4e  !u]..('z%.*..N*N
-00001e10: 8cbd 5547 570f 8a92 569f 2835 bc77 7dcf  ..UGW...V.(5.w}.
-00001e20: c32e 274c 8085 90f2 e66f 209c a89f e300  ..'L.....o .....
-00001e30: 1bc9 0762 d813 eb99 b9cc 2ce0 f026 dd1f  ...b......,..&..
-00001e40: 8554 93ab 0c9c 9573 56c1 1bfc acee e09c  .T.....sV.......
-00001e50: 354a 6ad9 9995 85b9 b2eb 5843 ef3c a2d0  5Jj.......XC.<..
-00001e60: 55f4 994d d5bc a382 ff64 e12b cbfa 62ad  U..M.....d.+..b.
-00001e70: edda 3255 3a4e 97bf 0a54 2751 5814 d0cb  ..2U:N...T'QX...
-00001e80: eb00 86bb b282 715c 2288 bd22 2ce2 a02a  ......q\"..",..*
-00001e90: 6b54 fe06 8e20 dc86 7b9c 32da e996 e9a1  kT... ..{.2.....
-00001ea0: 2797 6f1f 4445 bb0c ec50 9a63 e018 6948  '.o.DE...P.c..iH
-00001eb0: afbf cb97 c349 bed8 ed7a 60bb 21a3 9135  .....I...z`.!..5
-00001ec0: eb0d 55ce edab ffe8 c4dd 2efb 2f64 3f72  ..U........./d?r
-00001ed0: a19d 468e c264 c0b7 07cc dfc5 a2bf c70c  ..F..d..........
-00001ee0: 5e73 c67e 5e57 38a9 6098 ac23 1816 810f  ^s.~^W8.`..#....
-00001ef0: 93a0 4e20 4aa2 2a8a 50be db05 f535 e7be  ..N J.*.P....5..
-00001f00: b419 8921 e5b9 dbdb 923c f0f1 d499 ee4f  ...!.....<.....O
-00001f10: 25be d1eb 2441 798e 13b8 5e63 04c3 38c6  %...$Ay...^c..8.
-00001f20: 30f7 6d8b 090e 8a1c 57eb 1887 d595 7ea0  0.m.....W.....~.
-00001f30: 424b 3531 dd1b cbfa 35c0 c15c 7aba 179d  BK51....5..\z...
-00001f40: bced 7c16 bfd2 968d dcb6 ab6d a935 53da  ..|........m.5S.
-00001f50: 2c61 2783 b3f6 85dc 49d3 0a8c 6203 b5bf  ,a'.....I...b...
-00001f60: 8a5d dc34 b90c 5dd5 39dc 6264 fb07 0000  .].4..].9.bd....
-00001f70: ffff 0300 504b 0304 1400 0600 0800 0000  ....PK..........
-00001f80: 2100 afec c69b 4b01 0000 6d02 0000 1100  !.....K...m.....
-00001f90: 0801 646f 6350 726f 7073 2f63 6f72 652e  ..docProps/core.
-00001fa0: 786d 6c20 a204 0128 a000 0100 0000 0000  xml ...(........
-00001fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002000: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002010: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002020: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002030: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002040: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002050: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002060: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000b20: 0000 0000 0000 0000 0000 0000 ac52 4d4b  .............RMK
+00000b30: c430 10bd 0bfe 8730 779b 7615 11d9 742f  .0.....0w.v...t/
+00000b40: 22ec 55eb 0f08 c9b4 29db 2621 337e f4df  ".U.....).&!3~..
+00000b50: 1b2a ba5d 58d6 4b2f 036f 8679 efcd c776  .*.]X.K/.o.y...v
+00000b60: f735 0ee2 0313 f5c1 2ba8 8a12 047a 136c  .5......+....z.l
+00000b70: ef3b 056f cdf3 cd03 0862 edad 1e82 4705  .;.o.....b....G.
+00000b80: 1312 ecea ebab ed0b 0e9a 7313 b93e 92c8  ..........s..>..
+00000b90: 2c9e 1438 e6f8 2825 1987 a3a6 2244 f4b9  ,..8..(%...."D..
+00000ba0: d286 346a ce30 7532 6a73 d01d ca4d 59de  ..4j.0u2js...MY.
+00000bb0: cbb4 e480 fa84 53ec ad82 b4b7 b720 9a29  ......S...... .)
+00000bc0: 66e5 ffb9 43db f606 9f82 791f d1f3 1909  f...C.....y.....
+00000bd0: 493c 0d79 00d1 e8d4 212b f8c1 45f6 08f2  I<.y....!+..E...
+00000be0: bcfc 664d 79ce 6bc1 a3fa 0ce5 1cab 4b1e  ..fMy.k.......K.
+00000bf0: aa35 3d7c 8674 2087 c847 1f7f 2992 73e5  .5=|.t ..G..).s.
+00000c00: a299 bb55 efe1 7442 fbca 29bf dbf2 2ccb  ...U..tB..)...,.
+00000c10: f4ef 66e4 c9c7 d5df 0000 00ff ff03 0050  ..f............P
+00000c20: 4b03 0414 0006 0008 0000 0021 0072 bfc9  K..........!.r..
+00000c30: 908c 0300 0006 0a00 0018 0000 0078 6c2f  .............xl/
+00000c40: 776f 726b 7368 6565 7473 2f73 6865 6574  worksheets/sheet
+00000c50: 312e 786d 6c9c 93db 8e9b 3010 86ef 2bf5  1.xml.....0...+.
+00000c60: 1d2c df07 0309 39a0 9055 db55 d4bd abba  .,....9..U.U....
+00000c70: 3d5c 3b66 0856 6c4c 6d93 83aa be7b c790  =\;f.VlLm....{..
+00000c80: c34a b989 1681 6dec f1f7 cfe0 9fe5 d351  .J....m........Q
+00000c90: 2bb2 07eb a469 0a9a 4431 25d0 0853 ca66  +....i..D1%..S.f
+00000ca0: 5bd0 9f3f d6a3 3925 cef3 a6e4 ca34 50d0  [..?..9%.....4P.
+00000cb0: 1338 fab4 faf8 6179 3076 e76a 004f 90d0  .8....ay0v.j.O..
+00000cc0: b882 d6de b739 634e d4a0 b98b 4c0b 0dae  .....9cN....L...
+00000cd0: 54c6 6aee f1d5 6e99 6b2d f0b2 dfa4 154b  T.j...n.k-.....K
+00000ce0: e378 ca34 970d 1d08 b97d 8461 aa4a 0a78  .x.4.....}.a.J.x
+00000cf0: 36a2 d3d0 f801 6241 718f f9bb 5ab6 ee42  6.....bAq...Z..B
+00000d00: d3e2 119c e676 d7b5 2361 748b 888d 54d2  .....v..#at...T.
+00000d10: 9f7a 2825 5ae4 2fdb c658 be51 58f7 3199  .z(%Z./..X.QX.1.
+00000d20: 7041 8e16 ef14 9ff1 45a6 9fbf 53d2 5258  pA......E...S.RX
+00000d30: e34c e523 24b3 21e7 fbf2 176c c1b8 b892  .L.#$.!....l....
+00000d40: eeeb 7f08 934c 9885 bd0c 0778 43a5 ef4b  .....L.....xC..K
+00000d50: 29c9 aeac f406 1bbf 1336 bdc2 c2e7 b279  )........6.....y
+00000d60: 27cb 82fe 8dcf d708 fb24 34f1 adb9 acfd  '........$4.....
+00000d70: a3ab 6529 f184 4355 c442 55d0 4f49 fe39  ..e)..CU.BU.OI.9
+00000d80: 4928 5b2d 7b03 fd92 7070 6fc6 c4f3 cd2b  I([-{...ppo....+
+00000d90: 2810 1e50 24a1 24f8 7363 cc2e 04be e054  (..P$.$.sc.....T
+00000da0: 8c48 d707 0424 175e eee1 0b28 85e4 195a  .H...$.^...(...Z
+00000db0: fccf 2032 0b02 ecaa f076 7c51 5bf7 8efe  .. 2.....v|Q[...
+00000dc0: 6649 0915 ef94 ff6e 0e5f 416e 6b8f b219  fI.....n._Ank...
+00000dd0: d619 8c92 97a7 6770 021d 8ac2 519a 05aa  ......gp....Q...
+00000de0: 300a 11d8 122d c3af 860e e3c7 2155 59fa  0....-......!UY.
+00000df0: 1a47 8b28 9bc5 e304 c3c9 069c 5fcb 80a4  .G.(........_...
+00000e00: 4474 ce1b fdfb 1c74 460d 103c a41e 82fd  Dt.....tF..<....
+00000e10: 6158 4f27 d13c cb26 d3f9 0c29 f73b 599f  aXO'.<.&...).;Y.
+00000e20: c57f 0000 00ff ff00 0000 ffff 94d4 6d0a  ..............m.
+00000e30: 8240 1080 e1ab c81e 205d bf95 5528 bc88  .@...... ]..U(..
+00000e40: 98d0 2f0b 57ac 6edf 8cc4 ae3b b9d0 fccb  ../.W.n....;....
+00000e50: f6c5 4719 1ca5 6fe3 b874 fdd2 b76a be3f  ..G...o..t...j.?
+00000e60: 83b9 1152 04fa d14f 1a7e d5b1 085e 32ed  ...R...O.~...^2.
+00000e70: 87fa faee 463d 8cd3 d288 e814 67a2 5503  ....F=......g.U.
+00000e80: b667 88e1 2f0d d76b 1ba9 706d 5538 7ccf  .g../..k..pmU8|.
+00000e90: 2efb 3369 ce42 608c 05f7 ffdf c278 7b3c  ..3i.B`......x{<
+00000ea0: 23c6 4484 c29c 15c7 62c2 1131 76c5 8488  #.D.....b..1v...
+00000eb0: 5018 b13c 1653 8e88 b12b a644 84c2 88d5  P..<.S...+.D....
+00000ec0: b198 7144 8c5d 3123 2214 4694 76c8 ce20  ..qD.]1#".F.v.. 
+00000ed0: 730e 89b1 4b4a 3a49 48ac e919 65c1 3131  s...KJ:IH...e.11
+00000ee0: 2626 9d25 24d6 f40c b3e4 9818 1393 4e13  &&.%$.........N.
+00000ef0: 126b 7ac6 5971 4c8c 8949 e709 89fd 823c  .kz.YqL..I.....<
+00000f00: f394 1107 dd6a 57cd e932 801b da37 f5ac  .....jW..2...7..
+00000f10: 03c9 db3d 5893 77fd 61f7 4b28 a66c 68b7  ...=X.w.a.K(.lh.
+00000f20: df07 0000 ffff 0000 00ff ff4c 8ecd 0ac2  ...........L....
+00000f30: 400c 845f 65c9 0368 ad3f 65c5 edc9 8b07  @.._e..h.?e.....
+00000f40: 41f0 09b6 36b6 c1ba 59d2 54c1 a777 2b16  A...6...Y.T..w+.
+00000f50: bde5 9b19 26b3 8bbe c1a3 9786 426f 3abc  ....&.......Bo:.
+00000f60: aa83 6c56 8011 6ada e956 8e1f 750d a662  ..lV..j..V..u..b
+00000f70: 55be 4fd4 a2af 5146 5a82 b932 eb04 f372  U.O...QFZ..2...r
+00000f80: 37f6 9e51 8768 a28f 2867 7aa1 030b 8685  7..Q.h..(gz.....
+00000f90: 30a8 57e2 e020 b2a8 7852 306d d25f 9c8c  0.W.. ..xR0m._..
+00000fa0: 6e1f c9c1 2ab7 2bbb 2972 9b8a 1f28 4a97  n...*.+.)r...(J.
+00000fb0: af91 a569 5baa 1dc8 a15e 40fa a3be eaf0  ...i[....^@.....
+00000fc0: e445 7b73 e121 a4cd 0bf8 537f e97c 4ccf  .E{s.!....S..|L.
+00000fd0: 7ff1 044f 965b df22 6af9 0600 00ff ff03  ...O.[."j.......
+00000fe0: 0050 4b03 0414 0006 0008 0000 0021 0075  .PK..........!.u
+00000ff0: 3e99 6993 0600 008c 1a00 0013 0000 0078  >.i............x
+00001000: 6c2f 7468 656d 652f 7468 656d 6531 2e78  l/theme/theme1.x
+00001010: 6d6c ec59 5b8b db46 147e 2ff4 3f08 bd3b  ml.Y[..F.~/.?..;
+00001020: be49 b2bd c41b 6cd9 4eda ec26 21eb a4e4  .I....l.N..&!...
+00001030: 716c 8fad c98e 3446 33de 8d09 8192 3cf5  ql....4F3.....<.
+00001040: a550 484b 5f0a 7deb 4329 0d34 d0d0 97fe  .PHK_.}.C).4....
+00001050: 9885 8436 fd11 3d33 92ad 99f5 389b cba6  ...6..=3....8...
+00001060: b425 6b58 a4d1 77ce 7c73 ced1 3717 5dbc  .%kX..w.|s..7.].
+00001070: 742f a6ce 114e 3961 49db ad5e a8b8 0e4e  t/...N9aI..^...N
+00001080: c66c 4292 59db bd35 1c94 9aae c305 4a26  .lB.Y..5......J&
+00001090: 88b2 04b7 dd25 e6ee a5dd 8f3f ba88 7644  .....%.....?..vD
+000010a0: 8463 ec80 7dc2 7750 db8d 8498 ef94 cb7c  .c..}.wP.......|
+000010b0: 0ccd 885f 6073 9cc0 b329 4b63 24e0 369d  ..._`s...)Kc$.6.
+000010c0: 9527 293a 06bf 312d d72a 95a0 1c23 92b8  .'):..1-.*...#..
+000010d0: 4e82 6270 7b7d 3a25 63ec 0ca5 4b77 77e5  N.bp{}:%c...Kww.
+000010e0: bc4f e136 115c 368c 697a 205d 63c3 4261  .O.6.\6.iz ]c.Ba
+000010f0: 2787 5589 e04b 1ed2 d439 42b4 ed42 3f13  '.U..K...9B..B?.
+00001100: 763c c4f7 84eb 50c4 053c 68bb 15f5 e796  v<....P..<h.....
+00001110: 772f 96d1 4e6e 44c5 165b cd6e a0fe 72bb  w/..NnD..[.n..r.
+00001120: dc60 7258 537d a6b3 d1ba 53cf f3bd a0b3  .`rXS}....S.....
+00001130: f6af 0054 6ce2 fa8d 7ed0 0fd6 fe14 008d  ...Tl...~.......
+00001140: c730 d28c 8bee d3ef b6ba 3d3f c76a a0ec  .0........=?.j..
+00001150: d2e2 bbd7 e8d5 ab06 5ef3 5fdf e0dc f1e5  ........^._.....
+00001160: cfc0 2b50 e6df dbc0 0f06 2144 d1c0 2b50  ..+P......!D..+P
+00001170: 86f7 2d31 69d4 42cf c02b 5086 0f36 f08d  ..-1i.B..+P..6..
+00001180: 4aa7 e735 0cbc 0245 9424 871b e88a 1fd4  J..5...E.$......
+00001190: c3d5 68d7 9029 a357 acf0 96ef 0d1a b5dc  ..h..).W........
+000011a0: 7981 826a 5857 97ec 62ca 12b1 add6 6274  y..jXW..b.....bt
+000011b0: 97a5 0300 4820 4582 248e 58ce f114 8da1  ....H E.$.X.....
+000011c0: 8a43 44c9 2825 ce1e 9945 5078 7394 300e  .CD.(%...EPxs.0.
+000011d0: cd95 5a65 50a9 c37f f9f3 d495 8a08 dac1  ..ZeP...........
+000011e0: 48b3 96bc 8009 df68 927c 1c3e 4ec9 5cb4  H......h.|.>N.\.
+000011f0: dd4f c1ab ab41 9e3f 7b76 f2f0 e9c9 c35f  .O...A.?{v....._
+00001200: 4f1e 3d3a 79f8 73de b772 65d8 5d41 c94c  O.=:y.s..re.]A.L
+00001210: b77b f9c3 577f 7df7 b9f3 e72f dfbf 7cfc  .{..W.}..../..|.
+00001220: 75d6 f569 3cd7 f12f 7efa e2c5 6fbf bfca  u..i<../~...o...
+00001230: 3d8c b808 c5f3 6f9e bc78 fae4 f9b7 5ffe  =.....o..x...._.
+00001240: f1e3 638b f74e 8a46 3a7c 4862 cc9d 6bf8  ..c..N.F:|Hb..k.
+00001250: d8b9 c962 18a0 853f 1ea5 6f66 318c 1031  ...b...?..of1..1
+00001260: 2c50 04be 2dae fb22 3280 d796 88da 705d  ,P..-.."2.....p]
+00001270: 6c86 f076 0a2a 6303 5e5e dc35 b81e 44e9  l..v.*c.^^.5..D.
+00001280: 4210 4bcf 57a3 d800 ee33 46bb 2cb5 06e0  B.K.W....3F.,...
+00001290: aaec 4b8b f070 91cc ec9d a70b 1d77 13a1  ..K..p.......w..
+000012a0: 235b df21 4a8c 04f7 1773 9057 6273 1946  #[.!J....s.Wbs.F
+000012b0: d8a0 7983 a244 a019 4eb0 70e4 3376 88b1  ..y..D..N.p.3v..
+000012c0: 6574 7708 31e2 ba4f c629 e36c 2a9c 3bc4  etw.1..O.).l*.;.
+000012d0: e922 620d c990 8c8c 422a 8cae 9018 f2b2  ."b.....B*......
+000012e0: b411 8454 1bb1 d9bf ed74 19b5 8dba 878f  ...T.....t......
+000012f0: 4c24 bc16 885a c80f 3135 c278 192d 048a  L$...Z..15.x.-..
+00001300: 6d2e 8728 a67a c0f7 9088 6c24 0f96 e958  m..(.z....l$...X
+00001310: c7f5 b980 4ccf 3065 4e7f 8239 b7d9 5c4f  ....L.0eN..9..\O
+00001320: 61bc 5ad2 af82 c2d8 d3be 4f97 b189 4c05  a.Z.......O...L.
+00001330: 39b4 f9dc 438c e9c8 1e3b 0c23 14cf ad9c  9...C....;.#....
+00001340: 4912 e9d8 4ff8 2194 2872 6e30 6183 ef33  I...O.!.(rn0a..3
+00001350: f30d 91f7 9007 946c 4df7 6d82 8d74 9f2d  .......lM.m..t.-
+00001360: 04b7 405c 754a 4581 c827 8bd4 92cb cb98  ..@\uJE..'......
+00001370: 99ef e392 4e11 562a 03da 6f48 7a4c 9233  ....N.V*..oHzL.3
+00001380: f5fd 94b2 fbff 8cb2 db35 fa1c 34dd eef8  .........5..4...
+00001390: 5dd4 bc93 12eb 3b75 e594 866f c3fd 0795  ].....;u...o....
+000013a0: bb87 16c9 0d0c 2fcb e6cc f541 b83f 08b7  ....../....A.?..
+000013b0: fbbf 17ee 6def f2f9 cb75 a1d0 20de c55a  ....m....u.. ..Z
+000013c0: 5dad dce3 ad0b f729 a1f4 402c 29de e36a  ]......)..@,)..j
+000013d0: edce 615e 9a0c a051 6d2a d4ce 72bd 919b  ..a^...Qm*..r...
+000013e0: 4770 996f 130c dc2c 45ca c649 99f8 8c88  Gp.o...,E..I....
+000013f0: e820 4273 58e0 57d5 3674 c673 d733 eecc  . BsX.W.6t.s.3..
+00001400: 1987 75bf 6a56 1b62 7cca b7da 3d2c e27d  ..u.jV.b|...=,.}
+00001410: 36c9 f6ab d5aa dc9b 66e2 c191 28da 2bfe  6.......f...(.+.
+00001420: ba1d f61a 2243 078d 620f b676 af76 b533  ...."C..b..v.v.3
+00001430: b557 5e11 90b6 6f42 42eb cc24 51b7 9068  .W^...oBB..$Q..h
+00001440: ac1a 210b af22 a146 762e 2c5a 1616 4de9  ..!..".Fv.,Z..M.
+00001450: 7e95 aa55 16d7 a100 6aeb acc0 c2c9 81e5  ~..U....j.......
+00001460: 56db f5bd ec1c 00b6 5488 e289 cc53 7624  V.......T....Sv$
+00001470: b0ca ae4c ceb9 667a 5b30 a95e 01b0 8a58  ...L..fz[0.^...X
+00001480: 5540 91e9 96e4 ba75 7872 7459 a9bd 46a6  U@.....uxrtY..F.
+00001490: 0d12 5ab9 9924 b432 8cd0 04e7 d5a9 1f9c  ..Z..$.2........
+000014a0: 9c67 ae5b 454a 0d7a 3214 abb7 a1a0 d168  .g.[EJ.z2......h
+000014b0: be8f 5c4b 1139 a50d 34d1 9582 26ce 71db  ..\K.9..4...&.q.
+000014c0: 0dea 3e9c 8d8d d1bc ed4e 61df 0f97 f11c  ..>......Na.....
+000014d0: 6a87 cb05 2fa2 3338 3c1b 8b34 7be1 df46  j.../.38<..4{..F
+000014e0: 59e6 2917 3dc4 a32c e04a 7432 3588 89c0  Y.).=..,.Jt25...
+000014f0: a943 49dc 76e5 f0d7 d540 13a5 218a 5bb5  .CI.v....@..!.[.
+00001500: 0682 f0af 25d7 0259 f9b7 9183 a49b 49c6  ....%..Y......I.
+00001510: d329 1e0b 3ded 5a8b 8c74 760b 0a9f 6985  .)..=.Z..tv...i.
+00001520: f5a9 327f 7bb0 b464 0b48 f741 3439 7646  ..2.{..d.H.A49vF
+00001530: 7491 de44 5062 7ea3 2a03 3821 1c8e 7faa  t..DPb~.*.8!....
+00001540: 5934 2704 ce33 d742 56d4 dfa9 8929 975d  Y4'..3.BV....).]
+00001550: fd40 51d5 50d6 8ee8 3c42 f98c a28b 7906  .@Q.P...<B....y.
+00001560: 5722 baa6 a3ee d631 d0ee f231 4340 3743  W".....1...1C@7C
+00001570: 389a c909 f69d 67dd b3a7 6a19 394d 348b  8.....g...j.9M4.
+00001580: 39d3 5015 396b dac5 f4fd 4df2 1aab 6212  9.P.9k....M...b.
+00001590: 3558 65d2 adb6 0dbc d0ba d64a eba0 50ad  5Xe........J..P.
+000015a0: b3c4 19b3 ee6b 4c08 1ab5 a233 839a 64bc  .....kL....3..d.
+000015b0: 29c3 52b3 f356 93da 392e 08b4 4804 5be2  ).R..V..9...H.[.
+000015c0: b69e 23ac 9178 db99 1fec 4e57 ad9c 2056  ..#..x....NW.. V
+000015d0: eb4a 55f8 eac3 87fe 6d82 8dee 8278 f4e0  .JU.....m....x..
+000015e0: 1478 4105 57a9 842f 0f29 8245 5f76 8e9c  .xA.W../.).E_v..
+000015f0: c906 bc22 f744 be46 842b 6791 92b6 7bbf  ...".D.F.+g...{.
+00001600: e277 bcb0 e687 a54a d3ef 97bc ba57 2935  .w.....J.....W)5
+00001610: fd4e bdd4 f1fd 7ab5 ef57 2bbd 6eed 014c  .N....z..W+.n..L
+00001620: 2c22 8aab 7ef6 d165 0007 5174 997f 7a51  ,"..~..e..Qt..zQ
+00001630: ed1b 9f5f e2d5 59db 8531 8bcb 4c7d 5e29  ..._..Y..1..L}^)
+00001640: 2be2 eaf3 4bb5 b6fd f38b 4340 74ee 07b5  +...K.....C@t...
+00001650: 41ab deea 06a5 56bd 3328 79bd 6eb3 d40a  A.....V.3(y.n...
+00001660: 836e a917 848d dea0 17fa cdd6 e081 eb1c  .n..............
+00001670: 29b0 d7a9 875e d06f 9682 6a18 96bc a022  )....^.o..j...."
+00001680: e937 5ba5 8657 ab75 bc46 a7d9 f73a 0ff2  .7[..W.u.F...:..
+00001690: 650c 8c3c 938f 3c16 105e c56b f76f 0000  e..<..<..^.k.o..
+000016a0: 00ff ff03 0050 4b03 0414 0006 0008 0000  .....PK.........
+000016b0: 0021 00b0 22e5 a930 0300 000c 0800 000d  .!.."..0........
+000016c0: 0000 0078 6c2f 7374 796c 6573 2e78 6d6c  ...xl/styles.xml
+000016d0: a455 4d6f db38 10bd 17d8 ff40 f0ae 5092  .UMo.8.....@..P.
+000016e0: 2dd7 3624 75eb 3802 0ab4 c102 c902 7ba5  -.6$u.8.......{.
+000016f0: 25ca 26c2 0f81 a212 b945 ff7b 8794 6ccb  %.&......E.{..l.
+00001700: db62 db66 2ff6 7048 3ebe 9979 334a dff5  .b.f/.pH>..y3J..
+00001710: 52a0 6766 5aae 5586 a39b 1023 a64a 5d71  R.gfZ.U....#.J]q
+00001720: b5cf f0df 8f45 b0c4 a8b5 5455 5468 c532  .....E....TUTh.2
+00001730: 7c64 2d7e 97ff f126 6ded 51b0 8703 6316  |d-~...&m.Q...c.
+00001740: 0184 6a33 7cb0 b659 13d2 9607 2669 7ba3  ..j3|..Y....&i{.
+00001750: 1ba6 60a7 d646 520b 4bb3 276d 6318 ad5a  ..`..FR.K.'mc..Z
+00001760: 7749 0a12 87e1 8248 ca15 1e10 d6b2 fc15  wI.....H........
+00001770: 1049 cd53 d704 a596 0db5 7cc7 05b7 478f  .I.S......|...G.
+00001780: 8591 2cd7 1ff6 4a1b ba13 40b5 8fe6 b444  ..,...J...@....D
+00001790: 7db4 3031 eacd e911 effd ee1d c94b a35b  }.01.........K.[
+000017a0: 5ddb 1bc0 25ba ae79 c9be a7bb 222b 42cb  ]...%..y...."+B.
+000017b0: 0b12 20bf 0e29 4a48 185f c5de 9b57 22cd  .. ..)JH._...W".
+000017c0: 8961 cfdc 950f e769 ad95 6d51 a93b 6533  .a.....i..mQ.;e3
+000017d0: 1c03 5197 82f5 93d2 2faa 705b 50e1 f154  ..Q...../.p[P..T
+000017e0: 9eb6 9fd1 3315 e089 30c9 d352 0b6d 9085  ....3...0..R.m..
+000017f0: d241 e6bc 4751 c986 13b7 54f0 9de1 ee58  .A..GQ....T....X
+00001800: 4d25 17c7 c11d 3b87 aff6 784e 72c8 bd73  M%....;...xNr..s
+00001810: 12c7 6360 f35b efe8 ce70 66d0 3d7b f9f7  ..c`.[...pf.={..
+00001820: 5bb3 09ac 476f 019e 0b31 0976 70e4 29a8  [...Go...1.vp.).
+00001830: c232 a30a d845 a3fd 786c 202a 0502 1e60  .2...E..xl *...`
+00001840: 60eb a7a7 f786 1ea3 3899 5c20 fec1 3cdd  `.......8.\ ..<.
+00001850: 6953 41c3 9cd2 ec32 3ab8 f254 b0da 42fc  iSA....2:..T..B.
+00001860: 86ef 0fee dfea 067e 77da 5a10 559e 569c  .......~w.Z.U.V.
+00001870: eeb5 a2c2 65e8 7463 3420 9c92 09f1 e09a  ....e.tc4 ......
+00001880: ea9f fa0a bbaf 91ea 6421 ed87 2ac3 d09e  ........d!..*...
+00001890: 2eb7 2713 0219 cd01 6f58 38fc 29da 803d  ..'.....oX8.)..=
+000018a0: 818d 81f2 efc3 a2be 3ee3 5fdd 9eaf 2eac  ........>._.....
+000018b0: 2230 7fcc ea7c 1dd1 a611 c7fb 4eee 9829  "0...|......N..)
+000018c0: fc74 708a 1bbc 4ea5 a3fe 7c08 407a 9299  .tp...N...|.@z..
+000018d0: abbc 9c23 444e a919 be77 5002 343f b244  ...#DN...wP.4?.D
+000018e0: bb8e 0bcb d50f 7202 9855 7f9d 6558 9f05  ......r..U..eX..
+000018f0: 6b0d 7f1a 251d bafa ebce 0aae a69e f640  k...%..........@
+00001900: 2bfd 32b4 813f d20d f649 6230 50ed 7bc1  +.2..?...Ib0P.{.
+00001910: f76a 70ef 68cb 1c82 6f98 5f6f bb9f b4c3  .jp.h...o._o....
+00001920: b4f5 2eda f69d 3708 66a2 9b99 178e 9bc4  ......7.f.......
+00001930: b7ba 8264 fde9 75ed 8326 2e15 a055 3734  ...d..u..&...U74
+00001940: bdfe ce59 863b 15ab 6927 ece3 7933 c317  ...Y.;..i'..y3..
+00001950: fb13 ab78 2761 cc8c a7fe e2cf da7a 880c  ...x'a.......z..
+00001960: 5fec 8fae 19a2 857b 90f5 f663 0b83 01fe  _......{...c....
+00001970: 11b4 7a86 bfdc 6dde aeb6 7745 1c2c c3cd  ..z...m...wE.,..
+00001980: 3298 cf58 12ac 92cd 3648 e6b7 9bed b658  2..X....6H.....X
+00001990: 8571 78fb 7532 baff c7e0 f65f 1ad0 7d34  .qx.u2....._..}4
+000019a0: 5fb7 02c6 bb19 831d c93f 5c7c 199e 2c06  _........?\|..,.
+000019b0: fa3e 5d40 7bca 7d15 2fc2 f749 1406 c52c  .>]@{.}./..I...,
+000019c0: 8c82 f982 2e83 e562 9604 4512 c5db c57c  .......b..E....|
+000019d0: 7397 14c9 847b f2ca 011f 9228 1a3e 158e  s....{.....(.>..
+000019e0: 7cb2 b65c 7a31 5dd3 7f9c 7aa1 48b0 fc8f  |..\z1]...z.H...
+000019f0: 20c8 a912 e4f2 19cf bf01 0000 ffff 0300   ...............
+00001a00: 504b 0304 1400 0600 0800 0000 2100 a72b  PK..........!..+
+00001a10: 97e9 1e01 0000 1703 0000 1400 0000 786c  ..............xl
+00001a20: 2f73 6861 7265 6453 7472 696e 6773 2e78  /sharedStrings.x
+00001a30: 6d6c 7cd2 cd4e c420 1405 e0bd 89ef 40d8  ml|..N. ......@.
+00001a40: 3bb4 77e8 9f69 3b31 1a13 e352 7d00 84cb  ;.w..i;1...R}...
+00001a50: b449 0bb5 d089 bebd 9831 b3e8 b45d 72bf  .I.......1...]r.
+00001a60: 9c00 07ca c377 df91 138e aeb5 a6a2 f12e  .....w..........
+00001a70: a204 8db4 aa35 c78a 7ebc 3fdf e594 382f  .....5..~.?...8/
+00001a80: 8c12 9d35 58d1 1f74 f450 dfde 94ce 7912  ...5X..t.P....y.
+00001a90: b2c6 55b4 f17e b867 ccc9 067b e176 7640  ..U..~.g...{.vv@
+00001aa0: 1344 dbb1 173e 2cc7 2373 c388 42b9 06d1  .D...>,.#s..B...
+00001ab0: f71d 8328 4a59 2f5a 4389 b493 f115 05a0  ...(JY/ZC.......
+00001ac0: 6432 edd7 848f 9741 5dba b62e 7dfd f254  d2.....A]...}..T
+00001ad0: 325f 97ec 6f75 9ebc a171 769c 4f21 575a  2_..ou...qv.O!WZ
+00001ae0: a649 16eb 946b bda4 aa58 57c8 b55e 5721  .I...k...XW..^W!
+00001af0: b4da c87e 6a5c d3d7 3134 4962 2284 3959  ...~j\..14Ib".9Y
+00001b00: bc3a f485 f5ba c276 38f0 62f8 6179 47c8  .:.....v8.b.ayG.
+00001b10: a30c 208d f7e1 1120 bbae e95f a1e0 52ae  .. .... ..._..R.
+00001b20: 2997 5951 440b 5a00 243c 51b1 cec5 9a66  ).YQD.Z.$<Q....f
+00001b30: 59ca 81cf f5dc c37e fba6 8137 6ae2 dbe1  Y......~...7j...
+00001b40: c0cb 35cd a62c 7cec fa17 0000 ffff 0300  ..5..,|.........
+00001b50: 504b 0304 1400 0600 0800 0000 2100 41bf  PK..........!.A.
+00001b60: f860 d900 0000 ca01 0000 2300 0000 786c  .`........#...xl
+00001b70: 2f77 6f72 6b73 6865 6574 732f 5f72 656c  /worksheets/_rel
+00001b80: 732f 7368 6565 7431 2e78 6d6c 2e72 656c  s/sheet1.xml.rel
+00001b90: 73ac 91c1 4ec3 300c 40ef 48fc 43e4 3b49  s...N.0.@.H.C.;I
+00001ba0: bb03 4268 e92e 0869 5718 1fe0 a56e 1bd1  ..Bh...iW....n..
+00001bb0: 3a51 6c10 fb7b 8276 a1d3 242e 9c2c dbf2  :Ql..{.v..$..,..
+00001bc0: f393 bddd 7d2d b3f9 a422 31b1 87d6 3660  ....}-..."1...6`
+00001bd0: 8843 ea23 8f1e de0e cf77 0f60 4491 7b9c  .C.#.....w.`D.{.
+00001be0: 1393 8713 09ec badb 9bed 0bcd a875 48a6  .............uH.
+00001bf0: 98c5 540a 8b87 4935 3f3a 2761 a205 c5a6  ..T...I5?:'a....
+00001c00: 4c5c 3b43 2a0b 6a4d cbe8 3286 771c c96d  L\;C*.jM..2.w..m
+00001c10: 9ae6 de95 df0c e856 4cb3 ef3d 947d bf01  .......VL..=.}..
+00001c20: 7338 e5ba f96f 761a 8618 e829 858f 8558  s8...ov....)...X
+00001c30: afac 708a c799 2a10 cb48 eac1 da73 45ce  ..p...*..H...sE.
+00001c40: a1b5 5516 dc75 8ff6 3f3d 7289 ac54 5e49  ..U..u..?=r..T^I
+00001c50: b51e 5a56 4617 3d77 91b7 f618 f947 d2ad  ..ZVF.=w.....G..
+00001c60: 3ed0 7d03 0000 ffff 0300 504b 0304 1400  >.}.......PK....
+00001c70: 0600 0800 0000 2100 1157 5b9e 7c01 0000  ......!..W[.|...
+00001c80: d40d 0000 2700 0000 786c 2f70 7269 6e74  ....'...xl/print
+00001c90: 6572 5365 7474 696e 6773 2f70 7269 6e74  erSettings/print
+00001ca0: 6572 5365 7474 696e 6773 312e 6269 6eec  erSettings1.bin.
+00001cb0: 57bd 4a03 4110 feee 47c8 e915 56c1 4e3b  W.J.A...G...V.N;
+00001cc0: 1b0b d1b3 5763 2504 8358 5ca9 100b 9b28  ....Wc%..X\....(
+00001cd0: 26bd f80c 76be 854f e20b 046c 047d 008b  &...v..O...l.}..
+00001ce0: 3472 ce77 b981 756f ef44 4821 b273 4c66  4r.w..uo.DH!.sLf
+00001cf0: 7676 6676 f6cb c0cd f570 8111 ae85 37d0  vvfv.....p....7.
+00001d00: 478e 3dec 605b f431 2e71 8b2b f91d cb6a  G.=.`[.1.q.+...j
+00001d10: 50ea 234c 4a2b 0c0a e224 9d62 9646 2ff7  P.#LJ+...$.b.F/.
+00001d20: 5180 048f 2b59 6788 00dd e0b3 0845 4238  Q...+Yg......EB8
+00001d30: c001 3233 6841 3ab3 87e5 093c a54e b314  ..23hA:....<.N..
+00001d40: 383c 3eea 2722 49d3 0ef0 2c92 acc4 b8ce  8<>.'"I...,.....
+00001d50: 2910 4f80 2d59 9c09 9f9f 00af 37f5 b5ed  ).O.-Y......7...
+00001d60: 47df 0f87 bfda 359f ed97 8779 b8b6 200c  G.....5....y.. .
+00001d70: 7c9a 3a02 ab9b 1e15 8f80 47c0 23f0 f710  |.:.......G.#...
+00001d80: e0fb 2aaa 98d5 cddf 91ae 3ac3 d2cf ff87  ..*.......:.....
+00001d90: 1e01 2290 c8a3 7dc3 1eb2 2916 0367 19fa  .."...}...)..g..
+00001da0: 7445 a124 b9e6 22da b9af b393 ed37 1443  tE.$.."......7.C
+00001db0: 22ac f30e f7ed b5d6 309f f09a cfa9 cac0  ".......0.......
+00001dc0: 832a 22f7 97e7 fe8c 5d37 eca6 cabd a2f8  .*".....]7......
+00001dd0: be29 6135 72dd afe9 cee6 3ded dc36 a69a  .)a5r.....=..6..
+00001de0: a329 9789 0d7d ee2c 36cf a2fe 2680 5bd7  .)...}.,6...&.[.
+00001df0: 71de bcad f606 a85a 3171 61c6 5a7e a225  q......Z1qa.Z~.%
+00001e00: c341 b131 fbc5 8e7f af72 ba70 6bc2 963d  .A.1.....r.pk..=
+00001e10: aba4 7dd4 5657 5baf fd06 b7de 3ffe e6e9  ..}.VW[.....?...
+00001e20: 654f bb5f 0000 00ff ff03 0050 4b03 0414  eO._.......PK...
+00001e30: 0006 0008 0000 0021 009e b9cd ace3 0100  .......!........
+00001e40: 0096 0300 0014 0000 0078 6c2f 7461 626c  .........xl/tabl
+00001e50: 6573 2f74 6162 6c65 312e 786d 6c9c 93cd  es/table1.xml...
+00001e60: 8e9b 3014 85f7 95fa 0ec8 7b07 cc8f 0328  ..0.......{....(
+00001e70: 6414 fea4 486d 17cd f401 3c60 12ab d846  d...Hm....<`...F
+00001e80: b699 4954 f5dd 6b60 2633 5136 6d77 70ed  ..IT..k`&3Q6mwp.
+00001e90: fbf9 9c73 edcd c399 f7ce 3355 9a49 9101  ...s......3U.I..
+00001ea0: b4f2 8043 4523 5b26 8e19 f8f1 58c3 1838  ...CE#[&....X..8
+00001eb0: da10 d192 5e0a 9a81 0bd5 e061 fbf9 d3c6  ....^......a....
+00001ec0: 90a7 9e3a b65b e80c 9c8c 1952 d7d5 cd89  ...:.[.....R....
+00001ed0: 72a2 5772 a0c2 ae74 5271 62ec af3a ba7a  r.Wr...tRqb..:.z
+00001ee0: 5094 b4fa 44a9 e1bd eb7b 1e76 3961 022c  P...D....{.v9a.,
+00001ef0: 8494 377f 03e1 44fd 1c07 d848 3e10 c39e  ..7...D....H>...
+00001f00: 58cf cc65 6601 8737 e9fe 28a4 9a54 65e0  X..ef..7..(..Te.
+00001f10: ac9c b30a dee0 6775 07e7 ac51 52cb ceac  ......gu...QR...
+00001f20: 2ccc 955d c71a 7aa7 1185 aea2 cf6c 8ae6  ,..]..z......l..
+00001f30: 1d15 fc27 0b5f 5956 176b 6dd6 96a9 d271  ...'._YV.km....q
+00001f40: fafc 55a0 3a89 c2a2 805e 5e07 30dc 9515  ..U.:....^^.0...
+00001f50: 8ce3 1241 ec15 6111 0755 59a3 f237 7004  ...A..a..UY..7p.
+00001f60: e1d6 dce3 e4d1 76b7 4c0f 3db9 7cbb 292a  ......v.L.=.|.)*
+00001f70: da65 6087 d21c d91d 461a d2eb eff2 e570  .e`.....F......p
+00001f80: 922f 76bc 1ed8 6ec8 6864 cd7a 4395 73b3  ./v...n.hd.zC.s.
+00001f90: f71f b5b8 dbe5 0614 b21f b9d0 4e23 4761  ............N#Ga
+00001fa0: 32e0 db13 e69b b1d4 df8d 06af 4e63 3faf  2...........Nc?.
+00001fb0: 2b9c 5430 4cd6 110c 8bc0 8749 5027 1025  +.T0L......IP'.%
+00001fc0: 5115 4528 dfed 82fa ea74 5f5a 97c4 90f2  Q.E(.....t_Z....
+00001fd0: dced 6d4c 1eb8 3d75 a6fb 538c 6ff4 3a49  ..mL..=u..S.o.:I
+00001fe0: 509e e304 aed7 18c1 308e 31cc 7d9b 6382  P.......0.1.}.c.
+00001ff0: 8322 c7d5 3ac6 6175 a51f a8d0 524d 4cf7  ."..:.au....RML.
+00002000: 8364 fd6a e060 2e3d dd8b 4e7e 4c7d 2e7e  .d.j.`.=..N~L}.~
+00002010: a52d 1b39 b6ef c2a6 5a33 a5cd 6276 1238  .-.9....Z3..bv.8
+00002020: d7be 90bb d234 03a3 d840 ed63 b183 993a  .....4...@.c...:
+00002030: 97a6 6b75 36b7 08d9 fe01 0000 ffff 0300  ..ku6...........
+00002040: 504b 0304 1400 0600 0800 0000 2100 5fc3  PK..........!._.
+00002050: 7062 4d01 0000 6d02 0000 1100 0801 646f  pbM...m.......do
+00002060: 6350 726f 7073 2f63 6f72 652e 786d 6c20  cProps/core.xml 
+00002070: a204 0128 a000 0100 0000 0000 0000 0000  ...(............
 00002080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000020a0: 0000 0000 0000 0000 0000 007c 9251 4bc3  ...........|.QK.
-000020b0: 3014 85df 05ff 43c9 7b9b a463 7384 b603  0.....C.{..cs...
-000020c0: 953d 3910 5651 7c0b c9dd 566c d290 44bb  .=9.VQ|...Vl..D.
-000020d0: fd7b d376 ab95 898f c939 f7cb 3997 64ab  .{.v.....9..9.d.
-000020e0: a3aa a32f b0ae 6a74 8e68 4250 045a 34b2  .../..jt.hBP.Z4.
-000020f0: d2fb 1cbd 94eb 7889 22e7 b996 bc6e 34e4  ......x."....n4.
-00002100: e804 0ead 8adb 9b4c 1826 1a0b cfb6 3160  .......L.&....1`
-00002110: 7d05 2e0a 24ed 9830 393a 786f 18c6 4e1c  }...$..09:xo..N.
-00002120: 4071 9704 870e e2ae b18a fb70 b47b 6cb8  @q.........p.{l.
-00002130: f8e0 7bc0 2921 0bac c073 c93d c71d 3036  ..{.)!...s.=..06
-00002140: 2311 9d91 528c 48f3 69eb 1e20 0586 1a14  #...R.H.i.. ....
-00002150: 68ef 304d 28fe f17a b0ca fd39 d02b 13a7  h.0M(..z...9.+..
-00002160: aafc c984 4ee7 b853 b614 8338 ba8f ae1a  ....N..S...8....
-00002170: 8d6d db26 edac 8f11 f253 fcb6 79da f655  .m.&.....S..y..U
-00002180: e34a 77bb 1280 8a4c 0a26 2c70 dfd8 62eb  .Jw....L.&,p..b.
-00002190: c11c b88e 2444 af95 cff0 44ea d658 73e7  ....$D....D..Xs.
-000021a0: 3761 e3bb 0ae4 fde9 ca7d ed08 ecbe caf0  7a.......}......
-000021b0: 00c8 2884 6343 958b f23a 7b78 2cd7 a848  ..(.cC...:{x,..H
-000021c0: 099d c764 1193 7949 978c deb1 94bc 7701  ...d..yI......w.
-000021d0: 7ecd 7761 870b 758e f12f 319d c584 0668  ~.wa..u../1....h
-000021e0: 1970 64ce 089d 102f 8022 c357 1fa4 f806  .pd..../.".W....
-000021f0: 0000 ffff 0300 504b 0304 1400 0600 0800  ......PK........
-00002200: 0000 2100 6149 0910 8901 0000 1103 0000  ..!.aI..........
-00002210: 1000 0801 646f 6350 726f 7073 2f61 7070  ....docProps/app
-00002220: 2e78 6d6c 20a2 0401 28a0 0001 0000 0000  .xml ...(.......
-00002230: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002240: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002250: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002260: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002270: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002280: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002290: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000022a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000022b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000022c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000022d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000022e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000022f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000020a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000020b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000020c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000020d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000020e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000020f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002100: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002110: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002120: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002130: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002140: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002150: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002160: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002170: 0000 0000 0000 007c 9251 4bc3 3014 85df  .......|.QK.0...
+00002180: 05ff 43c9 7b9b a475 7384 b603 953d 3910  ..C.{..us....=9.
+00002190: 5699 f816 92bb add8 a621 8976 fbf7 a6ed  V........!.v....
+000021a0: 562b 131f 9373 ee97 732e 4997 c7ba 0abe  V+...s..s.I.....
+000021b0: c0d8 b251 19a2 1141 0128 d1c8 52ed 33f4  ...Q...A.(..R.3.
+000021c0: 5aac c205 0aac e34a f2aa 5190 a113 58b4  Z......J..Q...X.
+000021d0: cc6f 6f52 a199 680c bc98 4683 7125 d8c0  .ooR..h...F.q%..
+000021e0: 9394 6542 67e8 e09c 6618 5b71 809a dbc8  ..eBg...f.[q....
+000021f0: 3b94 1777 8da9 b9f3 47b3 c79a 8b0f be07  ;..w....G.......
+00002200: 1c13 32c7 3538 2eb9 e3b8 0386 7a24 a233  ..2.58......z$.3
+00002210: 528a 11a9 3f4d d503 a4c0 5041 0dca 594c  R...?M....PA..YL
+00002220: 238a 7fbc 0e4c 6dff 1ce8 9589 b32e dd49  #....Lm........I
+00002230: fb4e e7b8 53b6 1483 38ba 8fb6 1c8d 6ddb  .N..S...8.....m.
+00002240: 466d d2c7 f0f9 297e 5b3f 6ffa aa61 a9ba  Fm....)~[?o..a..
+00002250: 5d09 4079 2a05 1306 b86b 4cbe 71a0 0f5c  ].@y*....kL.q..\
+00002260: 0512 826d e952 3c91 ba35 56dc bab5 dff8  ...m.R<..5V.....
+00002270: ae04 f970 ba72 5f3b 3cbb af32 3c00 32f0  ...p.r_;<..2<.2.
+00002280: e1d8 50e5 a26c 93c7 a762 85f2 98d0 5948  ..P..l...b....YH
+00002290: e621 9915 74c1 e83d 8bc9 7b17 e0d7 7c17  .!..t..=..{...|.
+000022a0: 76b8 a8cf 31fe 25c6 4948 ee42 4a0b 9ab0  v...1.%.IH.BJ...
+000022b0: 84b0 f87e 42bc 00f2 145f 7d90 fc1b 0000  ...~B...._}.....
+000022c0: ffff 0300 504b 0304 1400 0600 0800 0000  ....PK..........
+000022d0: 2100 6149 0910 8901 0000 1103 0000 1000  !.aI............
+000022e0: 0801 646f 6350 726f 7073 2f61 7070 2e78  ..docProps/app.x
+000022f0: 6d6c 20a2 0401 28a0 0001 0000 0000 0000  ml ...(.........
 00002300: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002310: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002320: 0000 0000 0000 0000 0000 0000 9c92 416f  ..............Ao
-00002330: db30 0c85 ef03 fa1f 0cdd 1b39 dd50 0c81  .0.........9.P..
-00002340: ac62 4857 f4b0 6101 92b6 674d a663 a1b2  .bHW..a...gM.c..
-00002350: 2488 ac91 ecd7 8fb6 d1d4 d97a ea8d e47b  $..........z...{
-00002360: 78fa 4449 dd1c 3a5f f490 d1c5 5089 e5a2  x.DI..:_....P...
-00002370: 1405 041b 6b17 f695 78d8 dd5d 7e15 0592  ....k...x..]~...
-00002380: 09b5 f131 4025 8e80 e246 5f7c 529b 1c13  ...1@%...F_|R...
-00002390: 6472 8005 4704 ac44 4b94 5652 a26d a133  dr..G..DK.VR.m.3
-000023a0: b860 39b0 d2c4 dc19 e236 ef65 6c1a 67e1  .`9......6.el.g.
-000023b0: 36da 970e 02c9 abb2 bc96 7020 0835 d497  6.........p .5..
-000023c0: e914 28a6 c455 4f1f 0dad a31d f8f0 7177  ..(..UO.......qw
-000023d0: 4c0c acd5 b794 bcb3 86f8 96fa a7b3 3962  L.............9b
-000023e0: 6ca8 f87e b0e0 959c 8b8a e9b6 605f b2a3  l..~........`_..
-000023f0: a32e 959c b76a 6b8d 8735 07eb c678 0425  .....jk..5...x.%
-00002400: df06 ea1e ccb0 b48d 7119 b5ea 69d5 83a5  ........q...i...
-00002410: 980b 747f 786d 57a2 f86d 1006 9c4a f426  ..t.xmW..m...J.&
-00002420: 3b13 88b1 06db d48c b54f 4859 3fc5 fc8c  ;........OHY?...
-00002430: 2d00 a192 6c98 8663 39f7 ce6b f745 2f47  -...l..c9..k.E/G
-00002440: 0317 e7c6 2160 0261 e11c 71e7 c803 fe6a  ....!`.a..q....j
-00002450: 3626 d33b c4cb 39f1 c830 f14e 38db 816f  6&.;..9..0.N8..o
-00002460: 3a73 ce37 5e99 4ffa 277b 1dbb 64c2 9185  :s.7^.O.'{..d...
-00002470: 53f5 c385 677c 48bb 786b 085e d779 3e54  S...g|H.xk.^.y>T
-00002480: dbd6 64a8 f905 4eeb 3e0d d43d 6f32 fb21  ..d...N.>..=o2.!
-00002490: 64dd 9ab0 87fa d5f3 bf30 3cfe e3f4 c3f5  d........0<.....
-000024a0: f27a 517e 2ef9 5d67 3325 dffe b2fe 0b00  .zQ~..]g3%......
-000024b0: 00ff ff03 0050 4b01 022d 0014 0006 0008  .....PK..-......
-000024c0: 0000 0021 0037 31bd 917b 0100 0084 0500  ...!.71..{......
-000024d0: 0013 0000 0000 0000 0000 0000 0000 0000  ................
-000024e0: 0000 005b 436f 6e74 656e 745f 5479 7065  ...[Content_Type
-000024f0: 735d 2e78 6d6c 504b 0102 2d00 1400 0600  s].xmlPK..-.....
-00002500: 0800 0000 2100 b555 3023 f400 0000 4c02  ....!..U0#....L.
-00002510: 0000 0b00 0000 0000 0000 0000 0000 0000  ................
-00002520: b403 0000 5f72 656c 732f 2e72 656c 7350  ...._rels/.relsP
-00002530: 4b01 022d 0014 0006 0008 0000 0021 008d  K..-.........!..
-00002540: de29 17f4 0200 00d6 0600 000f 0000 0000  .)..............
-00002550: 0000 0000 0000 0000 00d9 0600 0078 6c2f  .............xl/
-00002560: 776f 726b 626f 6f6b 2e78 6d6c 504b 0102  workbook.xmlPK..
-00002570: 2d00 1400 0600 0800 0000 2100 813e 9497  -.........!..>..
-00002580: f300 0000 ba02 0000 1a00 0000 0000 0000  ................
-00002590: 0000 0000 0000 fa09 0000 786c 2f5f 7265  ..........xl/_re
-000025a0: 6c73 2f77 6f72 6b62 6f6f 6b2e 786d 6c2e  ls/workbook.xml.
-000025b0: 7265 6c73 504b 0102 2d00 1400 0600 0800  relsPK..-.......
-000025c0: 0000 2100 987c 3d91 2c03 0000 2d07 0000  ..!..|=.,...-...
-000025d0: 1800 0000 0000 0000 0000 0000 0000 2d0c  ..............-.
-000025e0: 0000 786c 2f77 6f72 6b73 6865 6574 732f  ..xl/worksheets/
-000025f0: 7368 6565 7431 2e78 6d6c 504b 0102 2d00  sheet1.xmlPK..-.
-00002600: 1400 0600 0800 0000 2100 753e 9969 9306  ........!.u>.i..
-00002610: 0000 8c1a 0000 1300 0000 0000 0000 0000  ................
-00002620: 0000 0000 8f0f 0000 786c 2f74 6865 6d65  ........xl/theme
-00002630: 2f74 6865 6d65 312e 786d 6c50 4b01 022d  /theme1.xmlPK..-
-00002640: 0014 0006 0008 0000 0021 0097 e7f0 ba0f  .........!......
-00002650: 0300 00cf 0700 000d 0000 0000 0000 0000  ................
-00002660: 0000 0000 0053 1600 0078 6c2f 7374 796c  .....S...xl/styl
-00002670: 6573 2e78 6d6c 504b 0102 2d00 1400 0600  es.xmlPK..-.....
-00002680: 0800 0000 2100 652d 2a77 c700 0000 5e01  ....!.e-*w....^.
-00002690: 0000 1400 0000 0000 0000 0000 0000 0000  ................
-000026a0: 8d19 0000 786c 2f73 6861 7265 6453 7472  ....xl/sharedStr
-000026b0: 696e 6773 2e78 6d6c 504b 0102 2d00 1400  ings.xmlPK..-...
-000026c0: 0600 0800 0000 2100 41bf f860 d900 0000  ......!.A..`....
-000026d0: ca01 0000 2300 0000 0000 0000 0000 0000  ....#...........
-000026e0: 0000 861a 0000 786c 2f77 6f72 6b73 6865  ......xl/workshe
-000026f0: 6574 732f 5f72 656c 732f 7368 6565 7431  ets/_rels/sheet1
-00002700: 2e78 6d6c 2e72 656c 7350 4b01 022d 0014  .xml.relsPK..-..
-00002710: 0006 0008 0000 0021 0011 575b 9e7c 0100  .......!..W[.|..
-00002720: 00d4 0d00 0027 0000 0000 0000 0000 0000  .....'..........
-00002730: 0000 00a0 1b00 0078 6c2f 7072 696e 7465  .......xl/printe
-00002740: 7253 6574 7469 6e67 732f 7072 696e 7465  rSettings/printe
-00002750: 7253 6574 7469 6e67 7331 2e62 696e 504b  rSettings1.binPK
-00002760: 0102 2d00 1400 0600 0800 0000 2100 9052  ..-.........!..R
-00002770: f45f e101 0000 9403 0000 1400 0000 0000  ._..............
-00002780: 0000 0000 0000 0000 611d 0000 786c 2f74  ........a...xl/t
-00002790: 6162 6c65 732f 7461 626c 6531 2e78 6d6c  ables/table1.xml
-000027a0: 504b 0102 2d00 1400 0600 0800 0000 2100  PK..-.........!.
-000027b0: afec c69b 4b01 0000 6d02 0000 1100 0000  ....K...m.......
-000027c0: 0000 0000 0000 0000 0000 741f 0000 646f  ..........t...do
-000027d0: 6350 726f 7073 2f63 6f72 652e 786d 6c50  cProps/core.xmlP
-000027e0: 4b01 022d 0014 0006 0008 0000 0021 0061  K..-.........!.a
-000027f0: 4909 1089 0100 0011 0300 0010 0000 0000  I...............
-00002800: 0000 0000 0000 0000 00f6 2100 0064 6f63  ..........!..doc
-00002810: 5072 6f70 732f 6170 702e 786d 6c50 4b05  Props/app.xmlPK.
-00002820: 0600 0000 000d 000d 0068 0300 00b5 2400  .........h....$.
-00002830: 0000 00                                  ...
+00002320: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002330: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002340: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002350: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002360: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002370: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002380: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002390: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000023a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000023b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000023c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000023d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000023e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000023f0: 0000 0000 0000 0000 0000 9c92 416f db30  ............Ao.0
+00002400: 0c85 ef03 fa1f 0cdd 1b39 dd50 0c81 ac62  .........9.P...b
+00002410: 4857 f4b0 6101 92b6 674d a663 a1b2 2488  HW..a...gM.c..$.
+00002420: ac91 ecd7 8fb6 d1d4 d97a ea8d e47b 78fa  .........z...{x.
+00002430: 4449 dd1c 3a5f f490 d1c5 5089 e5a2 1405  DI..:_....P.....
+00002440: 041b 6b17 f695 78d8 dd5d 7e15 0592 09b5  ..k...x..]~.....
+00002450: f131 4025 8e80 e246 5f7c 529b 1c13 6472  .1@%...F_|R...dr
+00002460: 8005 4704 ac44 4b94 5652 a26d a133 b860  ..G..DK.VR.m.3.`
+00002470: 39b0 d2c4 dc19 e236 ef65 6c1a 67e1 36da  9......6.el.g.6.
+00002480: 970e 02c9 abb2 bc96 7020 0835 d497 e914  ........p .5....
+00002490: 28a6 c455 4f1f 0dad a31d f8f0 7177 4c0c  (..UO.......qwL.
+000024a0: acd5 b794 bcb3 86f8 96fa a7b3 3962 6ca8  ............9bl.
+000024b0: f87e b0e0 959c 8b8a e9b6 605f b2a3 a32e  .~........`_....
+000024c0: 959c b76a 6b8d 8735 07eb c678 0425 df06  ...jk..5...x.%..
+000024d0: ea1e ccb0 b48d 7119 b5ea 69d5 83a5 980b  ......q...i.....
+000024e0: 747f 786d 57a2 f86d 1006 9c4a f426 3b13  t.xmW..m...J.&;.
+000024f0: 88b1 06db d48c b54f 4859 3fc5 fc8c 2d00  .......OHY?...-.
+00002500: a192 6c98 8663 39f7 ce6b f745 2f47 0317  ..l..c9..k.E/G..
+00002510: e7c6 2160 0261 e11c 71e7 c803 fe6a 3626  ..!`.a..q....j6&
+00002520: d33b c4cb 39f1 c830 f14e 38db 816f 3a73  .;..9..0.N8..o:s
+00002530: ce37 5e99 4ffa 277b 1dbb 64c2 9185 53f5  .7^.O.'{..d...S.
+00002540: c385 677c 48bb 786b 085e d779 3e54 dbd6  ..g|H.xk.^.y>T..
+00002550: 64a8 f905 4eeb 3e0d d43d 6f32 fb21 64dd  d...N.>..=o2.!d.
+00002560: 9ab0 87fa d5f3 bf30 3cfe e3f4 c3f5 f27a  .......0<......z
+00002570: 517e 2ef9 5d67 3325 dffe b2fe 0b00 00ff  Q~..]g3%........
+00002580: ff03 0050 4b01 022d 0014 0006 0008 0000  ...PK..-........
+00002590: 0021 0037 31bd 917b 0100 0084 0500 0013  .!.71..{........
+000025a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000025b0: 005b 436f 6e74 656e 745f 5479 7065 735d  .[Content_Types]
+000025c0: 2e78 6d6c 504b 0102 2d00 1400 0600 0800  .xmlPK..-.......
+000025d0: 0000 2100 b555 3023 f400 0000 4c02 0000  ..!..U0#....L...
+000025e0: 0b00 0000 0000 0000 0000 0000 0000 b403  ................
+000025f0: 0000 5f72 656c 732f 2e72 656c 7350 4b01  .._rels/.relsPK.
+00002600: 022d 0014 0006 0008 0000 0021 0030 549e  .-.........!.0T.
+00002610: 8be6 0200 00c0 0600 000f 0000 0000 0000  ................
+00002620: 0000 0000 0000 00d9 0600 0078 6c2f 776f  ...........xl/wo
+00002630: 726b 626f 6f6b 2e78 6d6c 504b 0102 2d00  rkbook.xmlPK..-.
+00002640: 1400 0600 0800 0000 2100 813e 9497 f300  ........!..>....
+00002650: 0000 ba02 0000 1a00 0000 0000 0000 0000  ................
+00002660: 0000 0000 ec09 0000 786c 2f5f 7265 6c73  ........xl/_rels
+00002670: 2f77 6f72 6b62 6f6f 6b2e 786d 6c2e 7265  /workbook.xml.re
+00002680: 6c73 504b 0102 2d00 1400 0600 0800 0000  lsPK..-.........
+00002690: 2100 72bf c990 8c03 0000 060a 0000 1800  !.r.............
+000026a0: 0000 0000 0000 0000 0000 0000 1f0c 0000  ................
+000026b0: 786c 2f77 6f72 6b73 6865 6574 732f 7368  xl/worksheets/sh
+000026c0: 6565 7431 2e78 6d6c 504b 0102 2d00 1400  eet1.xmlPK..-...
+000026d0: 0600 0800 0000 2100 753e 9969 9306 0000  ......!.u>.i....
+000026e0: 8c1a 0000 1300 0000 0000 0000 0000 0000  ................
+000026f0: 0000 e10f 0000 786c 2f74 6865 6d65 2f74  ......xl/theme/t
+00002700: 6865 6d65 312e 786d 6c50 4b01 022d 0014  heme1.xmlPK..-..
+00002710: 0006 0008 0000 0021 00b0 22e5 a930 0300  .......!.."..0..
+00002720: 000c 0800 000d 0000 0000 0000 0000 0000  ................
+00002730: 0000 00a5 1600 0078 6c2f 7374 796c 6573  .......xl/styles
+00002740: 2e78 6d6c 504b 0102 2d00 1400 0600 0800  .xmlPK..-.......
+00002750: 0000 2100 a72b 97e9 1e01 0000 1703 0000  ..!..+..........
+00002760: 1400 0000 0000 0000 0000 0000 0000 001a  ................
+00002770: 0000 786c 2f73 6861 7265 6453 7472 696e  ..xl/sharedStrin
+00002780: 6773 2e78 6d6c 504b 0102 2d00 1400 0600  gs.xmlPK..-.....
+00002790: 0800 0000 2100 41bf f860 d900 0000 ca01  ....!.A..`......
+000027a0: 0000 2300 0000 0000 0000 0000 0000 0000  ..#.............
+000027b0: 501b 0000 786c 2f77 6f72 6b73 6865 6574  P...xl/worksheet
+000027c0: 732f 5f72 656c 732f 7368 6565 7431 2e78  s/_rels/sheet1.x
+000027d0: 6d6c 2e72 656c 7350 4b01 022d 0014 0006  ml.relsPK..-....
+000027e0: 0008 0000 0021 0011 575b 9e7c 0100 00d4  .....!..W[.|....
+000027f0: 0d00 0027 0000 0000 0000 0000 0000 0000  ...'............
+00002800: 006a 1c00 0078 6c2f 7072 696e 7465 7253  .j...xl/printerS
+00002810: 6574 7469 6e67 732f 7072 696e 7465 7253  ettings/printerS
+00002820: 6574 7469 6e67 7331 2e62 696e 504b 0102  ettings1.binPK..
+00002830: 2d00 1400 0600 0800 0000 2100 9eb9 cdac  -.........!.....
+00002840: e301 0000 9603 0000 1400 0000 0000 0000  ................
+00002850: 0000 0000 0000 2b1e 0000 786c 2f74 6162  ......+...xl/tab
+00002860: 6c65 732f 7461 626c 6531 2e78 6d6c 504b  les/table1.xmlPK
+00002870: 0102 2d00 1400 0600 0800 0000 2100 5fc3  ..-.........!._.
+00002880: 7062 4d01 0000 6d02 0000 1100 0000 0000  pbM...m.........
+00002890: 0000 0000 0000 0000 4020 0000 646f 6350  ........@ ..docP
+000028a0: 726f 7073 2f63 6f72 652e 786d 6c50 4b01  rops/core.xmlPK.
+000028b0: 022d 0014 0006 0008 0000 0021 0061 4909  .-.........!.aI.
+000028c0: 1089 0100 0011 0300 0010 0000 0000 0000  ................
+000028d0: 0000 0000 0000 00c4 2200 0064 6f63 5072  ........"..docPr
+000028e0: 6f70 732f 6170 702e 786d 6c50 4b05 0600  ops/app.xmlPK...
+000028f0: 0000 000d 000d 0068 0300 0083 2500 0000  .......h....%...
+00002900: 00                                       .
```

### Comparing `temperaturemonitor_mqtt_sldewit-0.0.5/.github/workflows/python-app.yml` & `temperaturemonitor_mqtt_sldewit-1.0.0/.github/workflows/python-app.yml`

 * *Files identical despite different names*

### Comparing `temperaturemonitor_mqtt_sldewit-0.0.5/.github/workflows/python-publish.yml` & `temperaturemonitor_mqtt_sldewit-1.0.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `temperaturemonitor_mqtt_sldewit-0.0.5/Fritzing/Vloerverwarming monitor.fzz` & `temperaturemonitor_mqtt_sldewit-1.0.0/Fritzing/Vloerverwarming monitor.fzz`

 * *Files identical despite different names*

### Comparing `temperaturemonitor_mqtt_sldewit-0.0.5/Fritzing/Vloerverwarming monitor_schema.svg` & `temperaturemonitor_mqtt_sldewit-1.0.0/Fritzing/Vloerverwarming monitor_schema.svg`

 * *Files identical despite different names*

### Comparing `temperaturemonitor_mqtt_sldewit-0.0.5/TESTDIR/Scripts/Activate.ps1` & `temperaturemonitor_mqtt_sldewit-1.0.0/TESTDIR/Scripts/Activate.ps1`

 * *Files identical despite different names*

### Comparing `temperaturemonitor_mqtt_sldewit-0.0.5/TESTDIR/Scripts/activate` & `temperaturemonitor_mqtt_sldewit-1.0.0/TESTDIR/Scripts/activate`

 * *Files identical despite different names*

### Comparing `temperaturemonitor_mqtt_sldewit-0.0.5/TESTDIR/Scripts/activate.bat` & `temperaturemonitor_mqtt_sldewit-1.0.0/TESTDIR/Scripts/activate.bat`

 * *Files identical despite different names*

### Comparing `temperaturemonitor_mqtt_sldewit-0.0.5/TESTDIR/Scripts/easy_install-3.7.exe` & `temperaturemonitor_mqtt_sldewit-1.0.0/TESTDIR/Scripts/easy_install-3.7.exe`

 * *Files identical despite different names*

### Comparing `temperaturemonitor_mqtt_sldewit-0.0.5/TESTDIR/Scripts/easy_install.exe` & `temperaturemonitor_mqtt_sldewit-1.0.0/TESTDIR/Scripts/easy_install.exe`

 * *Files identical despite different names*

### Comparing `temperaturemonitor_mqtt_sldewit-0.0.5/TESTDIR/Scripts/pip.exe` & `temperaturemonitor_mqtt_sldewit-1.0.0/TESTDIR/Scripts/pip.exe`

 * *Files identical despite different names*

### Comparing `temperaturemonitor_mqtt_sldewit-0.0.5/TESTDIR/Scripts/pip3.7.exe` & `temperaturemonitor_mqtt_sldewit-1.0.0/TESTDIR/Scripts/pip3.7.exe`

 * *Files identical despite different names*

### Comparing `temperaturemonitor_mqtt_sldewit-0.0.5/TESTDIR/Scripts/pip3.exe` & `temperaturemonitor_mqtt_sldewit-1.0.0/TESTDIR/Scripts/pip3.exe`

 * *Files identical despite different names*

### Comparing `temperaturemonitor_mqtt_sldewit-0.0.5/TESTDIR/Scripts/python.exe` & `temperaturemonitor_mqtt_sldewit-1.0.0/TESTDIR/Scripts/python.exe`

 * *Files identical despite different names*

### Comparing `temperaturemonitor_mqtt_sldewit-0.0.5/TESTDIR/Scripts/pythonw.exe` & `temperaturemonitor_mqtt_sldewit-1.0.0/TESTDIR/Scripts/pythonw.exe`

 * *Files identical despite different names*

### Comparing `temperaturemonitor_mqtt_sldewit-0.0.5/drafts/test mqtt.py` & `temperaturemonitor_mqtt_sldewit-1.0.0/drafts/test mqtt.py`

 * *Files identical despite different names*

### Comparing `temperaturemonitor_mqtt_sldewit-0.0.5/drafts/test onewire.py` & `temperaturemonitor_mqtt_sldewit-1.0.0/drafts/test onewire.py`

 * *Files identical despite different names*

### Comparing `temperaturemonitor_mqtt_sldewit-0.0.5/drafts/test structure.py` & `temperaturemonitor_mqtt_sldewit-1.0.0/drafts/test structure.py`

 * *Files identical despite different names*

### Comparing `temperaturemonitor_mqtt_sldewit-0.0.5/src/temperature_monitoring_mqtt_sldewit/temperatue_monitor_mqtt.py` & `temperaturemonitor_mqtt_sldewit-1.0.0/src/temperature_monitoring_mqtt_sldewit/temperature_monitor_mqtt.py`

 * *Files 26% similar despite different names*

```diff
@@ -26,37 +26,39 @@
             self.sensorstate = "not found"
             print(f"Exception initializing sensor: {pi1wire_exception}")
 
     def read(self):
         """Sensor read function"""
         if self.temperaturesensor != 0:
             try:
-                self.temperature = self.temperaturesensor.get_temperature()
+                self.temperature = round(self.temperaturesensor.get_temperature(),1)
                 self.sensorstate = "online"
             except Exception as sensor_exception:
                 self.sensorstate = "offline"
                 print(f"Exception while reading sensor: {sensor_exception}")
         else: #simulate in case not really there
             self.temperature += 0.1
             print(f"Simulate sensor: {self.topic} - {self.temperature}")
 
     def publish(self):
         """Sensor publish to MQTT function"""
+        sensor_value = f"{{\"temperatuur\":\"{self.temperature}\"}}"
+        # pylint: disable-next=C0301
+        sensor_attr = f"{{\"mac_address\":\"{self.sensoraddress}\",\"status\":\"{self.sensorstate}\"}}"
+        print(f"Publish {self.topic} as {self.temperature}")
         try:
-            sensor_value = f'{"temperatuur":"self.temperature.1f"}'
             self.mqtt_broker.publish(self.topic,
                                      payload = sensor_value,
                                      qos=0, retain=True)
-            sensor_attr = f'{"mac_address":"{self.sensoraddress}","status":"{self.sensorstate}"}'
             self.mqtt_broker.publish(self.topic+'/attributes',
                                      payload = sensor_attr,
                                      qos=0,
                                      retain=False)
         except Exception as mqtt_exception:
-            print(f"MQTT publish failed: {mqtt_exception}")
+            print(f"MQTT publish failed on topic {self.topic} : {mqtt_exception}")
 
 # pylint: disable-next=W0613
 def on_connect(client, userdata, flags, return_code):
     """On connect event"""
     if return_code == 0:
         print("Connected success")
     else:
@@ -79,27 +81,32 @@
                 sensor.publish()
 
 try:
     mqtt_client = mqtt.Client()
     mqtt_client.on_connect = on_connect
     mqtt_client.will_set('vloerverwarming/status', "offline")
     mqtt_client.username_pw_set("mqtt","test_mqtt")
-    mqtt_client.connect("ha.de-wit.me", 1883, 60)
+    mqtt_client.connect("192.168.2.209", 1883, 60)
     mqtt_client.publish('vloerverwarming/status',payload = "online", qos=0, retain=True)
     mqtt_client.publish('vloerverwarming/version/installed',payload = "1.0.0", qos=0, retain=True)
     mqtt_client.publish('vloerverwarming/version/latest',payload = "1.0.0", qos=0, retain=True)
     mqtt_client.loop_start()
 except Exception as connect_exception:
     print(f"Failed to connect to MQTT: {connect_exception}")
     sys.exit()
 
 SENSORS = []
 
 SENSORS.append(TemperatureSensor('vloerverwarming/kring1/aanvoertemp',"28dfc6571f64ff",mqtt_client))
 SENSORS.append(TemperatureSensor('vloerverwarming/kring1/afvoertemp',"28dfd9571f64ff",mqtt_client))
 SENSORS.append(TemperatureSensor('vloerverwarming/kring2/aanvoertemp',"2828ff571f64ff",mqtt_client))
 SENSORS.append(TemperatureSensor('vloerverwarming/kring2/afvoertemp',"28aafd571f64ff",mqtt_client))
+SENSORS.append(TemperatureSensor('vloerverwarming/kring3/aanvoertemp',"28072261300627",mqtt_client))
+SENSORS.append(TemperatureSensor('vloerverwarming/kring3/afvoertemp',"280722613294cc",mqtt_client))
+SENSORS.append(TemperatureSensor('vloerverwarming/kring4/aanvoertemp',"280722614c7990",mqtt_client))
+SENSORS.append(TemperatureSensor('vloerverwarming/kring4/afvoertemp',"280922545d1f8a",mqtt_client))
 SENSORS.append(TemperatureSensor('vloerverwarming/aanvoertemp',"282bfe571f64ff",mqtt_client))
+SENSORS.append(TemperatureSensor('vloerverwarming/afvoertemp',"28092254776424",mqtt_client))
 
 stop_flag = Event()
 thread= MyThread(stop_flag, 10)
 thread.start()
```

### Comparing `temperaturemonitor_mqtt_sldewit-0.0.5/.gitignore` & `temperaturemonitor_mqtt_sldewit-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `temperaturemonitor_mqtt_sldewit-0.0.5/LICENSE` & `temperaturemonitor_mqtt_sldewit-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `temperaturemonitor_mqtt_sldewit-0.0.5/README.md` & `temperaturemonitor_mqtt_sldewit-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `temperaturemonitor_mqtt_sldewit-0.0.5/pyproject.toml` & `temperaturemonitor_mqtt_sldewit-1.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "TemperatureMonitor_MQTT_sldewit"
-version = "0.0.5"
+version = "1.0.0"
 authors = [
   { name="Stephan de Wit", email="stephan@de-wit.me" },
 ]
 description = "Temperature Monitoring system using MQTT"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `temperaturemonitor_mqtt_sldewit-0.0.5/PKG-INFO` & `temperaturemonitor_mqtt_sldewit-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TemperatureMonitor_MQTT_sldewit
-Version: 0.0.5
+Version: 1.0.0
 Summary: Temperature Monitoring system using MQTT
 Project-URL: Homepage, https://github.com/sldewit/TemperatureMonitor_MQTT
 Project-URL: Bug Tracker, https://github.com/sldewit/TemperatureMonitor_MQTT/issues
 Author-email: Stephan de Wit <stephan@de-wit.me>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

