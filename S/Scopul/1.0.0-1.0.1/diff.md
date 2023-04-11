# Comparing `tmp/scopul-1.0.0.tar.gz` & `tmp/Scopul-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scopul-1.0.0.tar", last modified: Sat Mar 18 23:20:16 2023, max compression
+gzip compressed data, was "Scopul-1.0.1.tar", last modified: Mon Apr 10 01:25:56 2023, max compression
```

## Comparing `scopul-1.0.0.tar` & `Scopul-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-03-18 23:20:16.464995 scopul-1.0.0/
--rw-rw-rw-   0        0        0     1094 2023-02-16 01:23:44.000000 scopul-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      188 2023-02-16 01:24:10.000000 scopul-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0      873 2023-03-18 23:20:16.465992 scopul-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     3398 2023-03-17 23:27:45.000000 scopul-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-03-18 23:20:16.442191 scopul-1.0.0/Scopul/
-drwxrwxrwx   0        0        0        0 2023-03-18 23:20:16.460008 scopul-1.0.0/Scopul/scopul.egg-info/
--rw-rw-rw-   0        0        0      873 2023-03-18 23:20:16.000000 scopul-1.0.0/Scopul/scopul.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      429 2023-03-18 23:20:16.000000 scopul-1.0.0/Scopul/scopul.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-18 23:20:16.000000 scopul-1.0.0/Scopul/scopul.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-03-18 23:20:16.000000 scopul-1.0.0/Scopul/scopul.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      283 2023-03-18 23:19:58.000000 scopul-1.0.0/long_desc.md
--rw-rw-rw-   0        0        0      108 2023-03-18 23:01:21.000000 scopul-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0      738 2023-03-18 23:20:16.469981 scopul-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-03-18 23:20:16.463997 scopul-1.0.0/tests/
--rw-rw-rw-   0        0        0     5380 2023-03-18 22:51:31.000000 scopul-1.0.0/tests/test_sequence.py
--rw-rw-rw-   0        0        0     1150 2023-03-15 22:35:22.000000 scopul-1.0.0/tests/test_tempo.py
--rw-rw-rw-   0        0        0     1384 2023-03-15 00:11:19.000000 scopul-1.0.0/tests/test_time_sig.py
+drwxrwxrwx   0        0        0        0 2023-04-10 01:25:56.063398 Scopul-1.0.1/
+-rw-rw-rw-   0        0        0     1094 2023-02-16 01:23:44.000000 Scopul-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      188 2023-02-16 01:24:10.000000 Scopul-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      873 2023-04-10 01:25:56.063398 Scopul-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2893 2023-03-19 00:09:53.000000 Scopul-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-10 01:25:56.032480 Scopul-1.0.1/Scopul/
+drwxrwxrwx   0        0        0        0 2023-04-10 01:25:56.056421 Scopul-1.0.1/Scopul/Scopul.egg-info/
+-rw-rw-rw-   0        0        0      873 2023-04-10 01:25:56.000000 Scopul-1.0.1/Scopul/Scopul.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      429 2023-04-10 01:25:56.000000 Scopul-1.0.1/Scopul/Scopul.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 01:25:56.000000 Scopul-1.0.1/Scopul/Scopul.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 01:25:56.000000 Scopul-1.0.1/Scopul/Scopul.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      283 2023-03-19 00:09:53.000000 Scopul-1.0.1/long_desc.md
+-rw-rw-rw-   0        0        0      108 2023-03-19 00:09:53.000000 Scopul-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0      736 2023-04-10 01:25:56.065391 Scopul-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-10 01:25:56.062401 Scopul-1.0.1/tests/
+-rw-rw-rw-   0        0        0     5380 2023-03-19 00:09:53.000000 Scopul-1.0.1/tests/test_sequence.py
+-rw-rw-rw-   0        0        0     1150 2023-03-15 22:35:22.000000 Scopul-1.0.1/tests/test_tempo.py
+-rw-rw-rw-   0        0        0     1384 2023-03-15 00:11:19.000000 Scopul-1.0.1/tests/test_time_sig.py
```

### Comparing `scopul-1.0.0/LICENSE` & `Scopul-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scopul-1.0.0/PKG-INFO` & `Scopul-1.0.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: scopul
-Version: 1.0.0
+Name: Scopul
+Version: 1.0.1
 Summary: A MIDI file analyzer which allows you to go through components of a MIDI file and extract data.
 Home-page: https://github.com/SwayamSahoo11742/Scopul
 Author: Swayam Sahoo
 Author-email: swayamsa01@gmail.com
 Project-URL: Bug Tracker, https://github.com/SwayamSahoo11742/Scopul/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `scopul-1.0.0/README.md` & `Scopul-1.0.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -35,32 +35,23 @@
 ## Future Plans
 🟡 = In progress
 
 🟠 = To-Do
 
 🟢 = Done
 
-### Things to look forward in the next release, any suggestions will be appreciated
-- Time signature conversions 🟢
-- Tempo conversions 🟢
-- Extract a specific rhythm 🟢
-- Ability to save as MIDI 🟢
-- Altering MIDI (adding/Deleting measures or notes)🟢
-- Refactoring and adding documentation for the changes 🟡
-- CONTRIBUTING.md will be updated with actual useful info 🟡
-
-### Things for the distant future, any suggestions will be appreciated
+### Things to look forward in the next major release, any suggestions will be appreciated
 - Chord extraction: Allow the extraction of chord progressions from the MIDI file.🟠
 - Key detection: Implement a function to detect the key of the MIDI file.🟠
 - Melody extraction: Allow the extraction of the melody from the MIDI file.🟠
 - Harmonic analysis: Provide harmonic analysis of the MIDI file by identifying chords and their progressions.🟠
+
+### Things for the distant future, any suggestions will be appreciated
 - Drum track extraction: Allow the extraction of the drum track from the MIDI file.🟠
-- Time signature detection: Implement a function to detect the time signature of the MIDI file.🟠
 - Quantization: Implement a function to quantize the notes in the MIDI file to a particular grid size.🟠
-- Instrument recognition: Provide functionality to recognize the instruments used in the MIDI file.
 - MIDI file validation: Implement a function to validate the structure of the MIDI file and detect any errors.🟠
 - Export to other formats: Allow the export of the MIDI data to other formats such as CSV, JSON, or XML.🟠
 
 ## Links
 Documentation - [https://swayamsahoo11742.github.io/](https://swayamsahoo11742.github.io/)
 
 Documentation Source Code - [https://github.com/SwayamSahoo11742/SwayamSahoo11742.github.io/](https://github.com/SwayamSahoo11742/SwayamSahoo11742.github.io/)
```

### Comparing `scopul-1.0.0/Scopul/scopul.egg-info/PKG-INFO` & `Scopul-1.0.1/Scopul/Scopul.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: scopul
-Version: 1.0.0
+Name: Scopul
+Version: 1.0.1
 Summary: A MIDI file analyzer which allows you to go through components of a MIDI file and extract data.
 Home-page: https://github.com/SwayamSahoo11742/Scopul
 Author: Swayam Sahoo
 Author-email: swayamsa01@gmail.com
 Project-URL: Bug Tracker, https://github.com/SwayamSahoo11742/Scopul/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `scopul-1.0.0/setup.cfg` & `Scopul-1.0.1/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
-00000010: 203d 2073 636f 7075 6c0d 0a76 6572 7369   = scopul..versi
-00000020: 6f6e 203d 2031 2e30 2e30 0d0a 6175 7468  on = 1.0.0..auth
+00000010: 203d 2053 636f 7075 6c0d 0a76 6572 7369   = Scopul..versi
+00000020: 6f6e 203d 2031 2e30 2e31 0d0a 6175 7468  on = 1.0.1..auth
 00000030: 6f72 203d 2053 7761 7961 6d20 5361 686f  or = Swayam Saho
 00000040: 6f0d 0a61 7574 686f 725f 656d 6169 6c20  o..author_email 
 00000050: 3d20 7377 6179 616d 7361 3031 4067 6d61  = swayamsa01@gma
 00000060: 696c 2e63 6f6d 0d0a 6465 7363 7269 7074  il.com..descript
 00000070: 696f 6e20 3d20 4120 4d49 4449 2066 696c  ion = A MIDI fil
 00000080: 6520 616e 616c 797a 6572 2077 6869 6368  e analyzer which
 00000090: 2061 6c6c 6f77 7320 796f 7520 746f 2067   allows you to g
@@ -31,17 +31,16 @@
 000001e0: 6e20 3a3a 2033 0d0a 094c 6963 656e 7365  n :: 3...License
 000001f0: 203a 3a20 4f53 4920 4170 7072 6f76 6564   :: OSI Approved
 00000200: 203a 3a20 4d49 5420 4c69 6365 6e73 650d   :: MIT License.
 00000210: 0a09 4f70 6572 6174 696e 6720 5379 7374  ..Operating Syst
 00000220: 656d 203a 3a20 4f53 2049 6e64 6570 656e  em :: OS Indepen
 00000230: 6465 6e74 0d0a 0d0a 5b6f 7074 696f 6e73  dent....[options
 00000240: 5d0d 0a70 6163 6b61 6765 5f64 6972 203d  ]..package_dir =
-00000250: 200d 0a09 3d20 5363 6f70 756c 2f0d 0a70   ...= Scopul/..p
-00000260: 6163 6b61 6765 7320 3d20 6669 6e64 3a0d  ackages = find:.
-00000270: 0a70 7974 686f 6e5f 7265 7175 6972 6573  .python_requires
-00000280: 203d 203e 3d33 2e36 0d0a 0d0a 5b6f 7074   = >=3.6....[opt
-00000290: 696f 6e73 2e70 6163 6b61 6765 732e 6669  ions.packages.fi
-000002a0: 6e64 5d0d 0a77 6865 7265 203d 2053 636f  nd]..where = Sco
-000002b0: 7075 6c2f 0d0a 0d0a 5b65 6767 5f69 6e66  pul/....[egg_inf
-000002c0: 6f5d 0d0a 7461 675f 6275 696c 6420 3d20  o]..tag_build = 
-000002d0: 0d0a 7461 675f 6461 7465 203d 2030 0d0a  ..tag_date = 0..
-000002e0: 0d0a                                     ..
+00000250: 200d 0a09 3d20 5363 6f70 756c 0d0a 7061   ...= Scopul..pa
+00000260: 636b 6167 6573 203d 2066 696e 643a 0d0a  ckages = find:..
+00000270: 7079 7468 6f6e 5f72 6571 7569 7265 7320  python_requires 
+00000280: 3d20 3e3d 332e 360d 0a0d 0a5b 6f70 7469  = >=3.6....[opti
+00000290: 6f6e 732e 7061 636b 6167 6573 2e66 696e  ons.packages.fin
+000002a0: 645d 0d0a 7768 6572 6520 3d20 5363 6f70  d]..where = Scop
+000002b0: 756c 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d  ul....[egg_info]
+000002c0: 0d0a 7461 675f 6275 696c 6420 3d20 0d0a  ..tag_build = ..
+000002d0: 7461 675f 6461 7465 203d 2030 0d0a 0d0a  tag_date = 0....
```

### Comparing `scopul-1.0.0/tests/test_sequence.py` & `Scopul-1.0.1/tests/test_sequence.py`

 * *Files identical despite different names*

### Comparing `scopul-1.0.0/tests/test_tempo.py` & `Scopul-1.0.1/tests/test_tempo.py`

 * *Files identical despite different names*

### Comparing `scopul-1.0.0/tests/test_time_sig.py` & `Scopul-1.0.1/tests/test_time_sig.py`

 * *Files identical despite different names*

