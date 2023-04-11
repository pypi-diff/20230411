# Comparing `tmp/Scopul-1.0.1.tar.gz` & `tmp/Scopul-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Scopul-1.0.1.tar", last modified: Mon Apr 10 01:25:56 2023, max compression
+gzip compressed data, was "Scopul-1.0.2.tar", last modified: Tue Apr 11 03:19:33 2023, max compression
```

## Comparing `Scopul-1.0.1.tar` & `Scopul-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 01:25:56.063398 Scopul-1.0.1/
--rw-rw-rw-   0        0        0     1094 2023-02-16 01:23:44.000000 Scopul-1.0.1/LICENSE
--rw-rw-rw-   0        0        0      188 2023-02-16 01:24:10.000000 Scopul-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      873 2023-04-10 01:25:56.063398 Scopul-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2893 2023-03-19 00:09:53.000000 Scopul-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-10 01:25:56.032480 Scopul-1.0.1/Scopul/
-drwxrwxrwx   0        0        0        0 2023-04-10 01:25:56.056421 Scopul-1.0.1/Scopul/Scopul.egg-info/
--rw-rw-rw-   0        0        0      873 2023-04-10 01:25:56.000000 Scopul-1.0.1/Scopul/Scopul.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      429 2023-04-10 01:25:56.000000 Scopul-1.0.1/Scopul/Scopul.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 01:25:56.000000 Scopul-1.0.1/Scopul/Scopul.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 01:25:56.000000 Scopul-1.0.1/Scopul/Scopul.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      283 2023-03-19 00:09:53.000000 Scopul-1.0.1/long_desc.md
--rw-rw-rw-   0        0        0      108 2023-03-19 00:09:53.000000 Scopul-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      736 2023-04-10 01:25:56.065391 Scopul-1.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-10 01:25:56.062401 Scopul-1.0.1/tests/
--rw-rw-rw-   0        0        0     5380 2023-03-19 00:09:53.000000 Scopul-1.0.1/tests/test_sequence.py
--rw-rw-rw-   0        0        0     1150 2023-03-15 22:35:22.000000 Scopul-1.0.1/tests/test_tempo.py
--rw-rw-rw-   0        0        0     1384 2023-03-15 00:11:19.000000 Scopul-1.0.1/tests/test_time_sig.py
+drwxrwxrwx   0        0        0        0 2023-04-11 03:19:33.294281 Scopul-1.0.2/
+-rw-rw-rw-   0        0        0     1094 2023-02-16 01:23:44.000000 Scopul-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0      188 2023-02-16 01:24:10.000000 Scopul-1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      873 2023-04-11 03:19:33.295271 Scopul-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2893 2023-03-19 00:09:53.000000 Scopul-1.0.2/README.md
+-rw-rw-rw-   0        0        0      283 2023-03-19 00:09:53.000000 Scopul-1.0.2/long_desc.md
+-rw-rw-rw-   0        0        0      108 2023-03-19 00:09:53.000000 Scopul-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      730 2023-04-11 03:19:33.297779 Scopul-1.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-11 03:19:33.250658 Scopul-1.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-11 03:19:33.277904 Scopul-1.0.2/src/Scopul/
+-rw-rw-rw-   0        0        0    16368 2023-03-19 00:09:53.000000 Scopul-1.0.2/src/Scopul/Sequence.py
+-rw-rw-rw-   0        0        0      441 2023-03-19 00:09:53.000000 Scopul-1.0.2/src/Scopul/Tempo.py
+-rw-rw-rw-   0        0        0      663 2023-03-19 00:09:53.000000 Scopul-1.0.2/src/Scopul/TimeSignature.py
+-rw-rw-rw-   0        0        0      470 2023-03-15 00:29:53.000000 Scopul-1.0.2/src/Scopul/__init__.py
+-rw-rw-rw-   0        0        0       90 2023-02-17 20:20:00.000000 Scopul-1.0.2/src/Scopul/config_musescore.py
+-rw-rw-rw-   0        0        0     4011 2023-02-12 20:39:00.000000 Scopul-1.0.2/src/Scopul/conversions.py
+-rw-rw-rw-   0        0        0     3560 2023-03-15 00:13:32.000000 Scopul-1.0.2/src/Scopul/helpers.py
+-rw-rw-rw-   0        0        0    15336 2023-03-19 00:09:53.000000 Scopul-1.0.2/src/Scopul/scopul.py
+-rw-rw-rw-   0        0        0      449 2023-02-21 00:22:42.000000 Scopul-1.0.2/src/Scopul/scopul_exception.py
+drwxrwxrwx   0        0        0        0 2023-04-11 03:19:33.287732 Scopul-1.0.2/src/Scopul.egg-info/
+-rw-rw-rw-   0        0        0      873 2023-04-11 03:19:33.000000 Scopul-1.0.2/src/Scopul.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      494 2023-04-11 03:19:33.000000 Scopul-1.0.2/src/Scopul.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 03:19:33.000000 Scopul-1.0.2/src/Scopul.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-11 03:19:33.000000 Scopul-1.0.2/src/Scopul.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-11 03:19:33.293273 Scopul-1.0.2/tests/
+-rw-rw-rw-   0        0        0     5380 2023-03-19 00:09:53.000000 Scopul-1.0.2/tests/test_sequence.py
+-rw-rw-rw-   0        0        0     1150 2023-03-15 22:35:22.000000 Scopul-1.0.2/tests/test_tempo.py
+-rw-rw-rw-   0        0        0     1384 2023-03-15 00:11:19.000000 Scopul-1.0.2/tests/test_time_sig.py
```

### Comparing `Scopul-1.0.1/LICENSE` & `Scopul-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Scopul-1.0.1/PKG-INFO` & `Scopul-1.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Scopul
-Version: 1.0.1
+Version: 1.0.2
 Summary: A MIDI file analyzer which allows you to go through components of a MIDI file and extract data.
 Home-page: https://github.com/SwayamSahoo11742/Scopul
 Author: Swayam Sahoo
 Author-email: swayamsa01@gmail.com
 Project-URL: Bug Tracker, https://github.com/SwayamSahoo11742/Scopul/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Scopul-1.0.1/README.md` & `Scopul-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `Scopul-1.0.1/Scopul/Scopul.egg-info/PKG-INFO` & `Scopul-1.0.2/src/Scopul.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Scopul
-Version: 1.0.1
+Version: 1.0.2
 Summary: A MIDI file analyzer which allows you to go through components of a MIDI file and extract data.
 Home-page: https://github.com/SwayamSahoo11742/Scopul
 Author: Swayam Sahoo
 Author-email: swayamsa01@gmail.com
 Project-URL: Bug Tracker, https://github.com/SwayamSahoo11742/Scopul/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Scopul-1.0.1/setup.cfg` & `Scopul-1.0.2/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2053 636f 7075 6c0d 0a76 6572 7369   = Scopul..versi
-00000020: 6f6e 203d 2031 2e30 2e31 0d0a 6175 7468  on = 1.0.1..auth
+00000020: 6f6e 203d 2031 2e30 2e32 0d0a 6175 7468  on = 1.0.2..auth
 00000030: 6f72 203d 2053 7761 7961 6d20 5361 686f  or = Swayam Saho
 00000040: 6f0d 0a61 7574 686f 725f 656d 6169 6c20  o..author_email 
 00000050: 3d20 7377 6179 616d 7361 3031 4067 6d61  = swayamsa01@gma
 00000060: 696c 2e63 6f6d 0d0a 6465 7363 7269 7074  il.com..descript
 00000070: 696f 6e20 3d20 4120 4d49 4449 2066 696c  ion = A MIDI fil
 00000080: 6520 616e 616c 797a 6572 2077 6869 6368  e analyzer which
 00000090: 2061 6c6c 6f77 7320 796f 7520 746f 2067   allows you to g
@@ -31,16 +31,16 @@
 000001e0: 6e20 3a3a 2033 0d0a 094c 6963 656e 7365  n :: 3...License
 000001f0: 203a 3a20 4f53 4920 4170 7072 6f76 6564   :: OSI Approved
 00000200: 203a 3a20 4d49 5420 4c69 6365 6e73 650d   :: MIT License.
 00000210: 0a09 4f70 6572 6174 696e 6720 5379 7374  ..Operating Syst
 00000220: 656d 203a 3a20 4f53 2049 6e64 6570 656e  em :: OS Indepen
 00000230: 6465 6e74 0d0a 0d0a 5b6f 7074 696f 6e73  dent....[options
 00000240: 5d0d 0a70 6163 6b61 6765 5f64 6972 203d  ]..package_dir =
-00000250: 200d 0a09 3d20 5363 6f70 756c 0d0a 7061   ...= Scopul..pa
-00000260: 636b 6167 6573 203d 2066 696e 643a 0d0a  ckages = find:..
-00000270: 7079 7468 6f6e 5f72 6571 7569 7265 7320  python_requires 
-00000280: 3d20 3e3d 332e 360d 0a0d 0a5b 6f70 7469  = >=3.6....[opti
-00000290: 6f6e 732e 7061 636b 6167 6573 2e66 696e  ons.packages.fin
-000002a0: 645d 0d0a 7768 6572 6520 3d20 5363 6f70  d]..where = Scop
-000002b0: 756c 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d  ul....[egg_info]
-000002c0: 0d0a 7461 675f 6275 696c 6420 3d20 0d0a  ..tag_build = ..
-000002d0: 7461 675f 6461 7465 203d 2030 0d0a 0d0a  tag_date = 0....
+00000250: 200d 0a09 3d20 7372 630d 0a70 6163 6b61   ...= src..packa
+00000260: 6765 7320 3d20 6669 6e64 3a0d 0a70 7974  ges = find:..pyt
+00000270: 686f 6e5f 7265 7175 6972 6573 203d 203e  hon_requires = >
+00000280: 3d33 2e36 0d0a 0d0a 5b6f 7074 696f 6e73  =3.6....[options
+00000290: 2e70 6163 6b61 6765 732e 6669 6e64 5d0d  .packages.find].
+000002a0: 0a77 6865 7265 203d 2073 7263 0d0a 0d0a  .where = src....
+000002b0: 5b65 6767 5f69 6e66 6f5d 0d0a 7461 675f  [egg_info]..tag_
+000002c0: 6275 696c 6420 3d20 0d0a 7461 675f 6461  build = ..tag_da
+000002d0: 7465 203d 2030 0d0a 0d0a                 te = 0....
```

### Comparing `Scopul-1.0.1/tests/test_sequence.py` & `Scopul-1.0.2/tests/test_sequence.py`

 * *Files identical despite different names*

### Comparing `Scopul-1.0.1/tests/test_tempo.py` & `Scopul-1.0.2/tests/test_tempo.py`

 * *Files identical despite different names*

### Comparing `Scopul-1.0.1/tests/test_time_sig.py` & `Scopul-1.0.2/tests/test_time_sig.py`

 * *Files identical despite different names*

