# Comparing `tmp/hearthstone-6.4.0.tar.gz` & `tmp/hearthstone-6.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hearthstone-6.4.0.tar", last modified: Wed Apr  5 17:45:16 2023, max compression
+gzip compressed data, was "hearthstone-6.5.0.tar", last modified: Tue Apr 11 17:10:50 2023, max compression
```

## Comparing `hearthstone-6.4.0.tar` & `hearthstone-6.5.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:45:16.153609 hearthstone-6.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-05 17:45:12.000000 hearthstone-6.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-04-05 17:45:16.153609 hearthstone-6.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-04-05 17:45:12.000000 hearthstone-6.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:45:16.153609 hearthstone-6.4.0/hearthstone/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-05 17:45:12.000000 hearthstone-6.4.0/hearthstone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-04-05 17:45:12.000000 hearthstone-6.4.0/hearthstone/bountyxml.py
--rw-r--r--   0 runner    (1001) docker     (123)    12903 2023-04-05 17:45:12.000000 hearthstone-6.4.0/hearthstone/cardxml.py
--rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-04-05 17:45:12.000000 hearthstone-6.4.0/hearthstone/dbf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-04-05 17:45:12.000000 hearthstone-6.4.0/hearthstone/deckstrings.py
--rw-r--r--   0 runner    (1001) docker     (123)    10283 2023-04-05 17:45:12.000000 hearthstone-6.4.0/hearthstone/entities.py
--rw-r--r--   0 runner    (1001) docker     (123)    58797 2023-04-05 17:45:12.000000 hearthstone-6.4.0/hearthstone/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     6985 2023-04-05 17:45:12.000000 hearthstone-6.4.0/hearthstone/mercenaryxml.py
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-04-05 17:45:12.000000 hearthstone-6.4.0/hearthstone/stringsfile.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-05 17:45:12.000000 hearthstone-6.4.0/hearthstone/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:45:16.153609 hearthstone-6.4.0/hearthstone/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    11209 2023-04-05 17:45:12.000000 hearthstone-6.4.0/hearthstone/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-05 17:45:12.000000 hearthstone-6.4.0/hearthstone/xmlutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:45:16.153609 hearthstone-6.4.0/hearthstone.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-04-05 17:45:16.000000 hearthstone-6.4.0/hearthstone.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-05 17:45:16.000000 hearthstone-6.4.0/hearthstone.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 17:45:16.000000 hearthstone-6.4.0/hearthstone.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-05 17:45:16.000000 hearthstone-6.4.0/hearthstone.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-05 17:45:16.000000 hearthstone-6.4.0/hearthstone.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 17:45:16.000000 hearthstone-6.4.0/hearthstone.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-05 17:45:16.153609 hearthstone-6.4.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)       62 2023-04-05 17:45:12.000000 hearthstone-6.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:10:50.447475 hearthstone-6.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-11 17:10:45.000000 hearthstone-6.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-04-11 17:10:50.447475 hearthstone-6.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-04-11 17:10:45.000000 hearthstone-6.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:10:50.447475 hearthstone-6.5.0/hearthstone/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-11 17:10:45.000000 hearthstone-6.5.0/hearthstone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-04-11 17:10:45.000000 hearthstone-6.5.0/hearthstone/bountyxml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12903 2023-04-11 17:10:45.000000 hearthstone-6.5.0/hearthstone/cardxml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-04-11 17:10:45.000000 hearthstone-6.5.0/hearthstone/dbf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-04-11 17:10:45.000000 hearthstone-6.5.0/hearthstone/deckstrings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10283 2023-04-11 17:10:45.000000 hearthstone-6.5.0/hearthstone/entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58839 2023-04-11 17:10:45.000000 hearthstone-6.5.0/hearthstone/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6985 2023-04-11 17:10:45.000000 hearthstone-6.5.0/hearthstone/mercenaryxml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-04-11 17:10:45.000000 hearthstone-6.5.0/hearthstone/stringsfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-11 17:10:45.000000 hearthstone-6.5.0/hearthstone/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:10:50.447475 hearthstone-6.5.0/hearthstone/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    11424 2023-04-11 17:10:45.000000 hearthstone-6.5.0/hearthstone/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-11 17:10:45.000000 hearthstone-6.5.0/hearthstone/xmlutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:10:50.447475 hearthstone-6.5.0/hearthstone.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-04-11 17:10:50.000000 hearthstone-6.5.0/hearthstone.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-11 17:10:50.000000 hearthstone-6.5.0/hearthstone.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 17:10:50.000000 hearthstone-6.5.0/hearthstone.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-11 17:10:50.000000 hearthstone-6.5.0/hearthstone.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-11 17:10:50.000000 hearthstone-6.5.0/hearthstone.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 17:10:50.000000 hearthstone-6.5.0/hearthstone.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-11 17:10:50.447475 hearthstone-6.5.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)       62 2023-04-11 17:10:45.000000 hearthstone-6.5.0/setup.py
```

### Comparing `hearthstone-6.4.0/LICENSE` & `hearthstone-6.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hearthstone-6.4.0/PKG-INFO` & `hearthstone-6.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hearthstone
-Version: 6.4.0
+Version: 6.5.0
 Summary: CardDefs.xml parser and Hearthstone enums for Python
 Home-page: https://github.com/HearthSim/python-hearthstone/
 Download-URL: https://github.com/HearthSim/python-hearthstone/tarball/master
 Author: Jerome Leclanche
 Author-email: jerome@leclan.ch
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `hearthstone-6.4.0/README.md` & `hearthstone-6.5.0/README.md`

 * *Files identical despite different names*

### Comparing `hearthstone-6.4.0/hearthstone/bountyxml.py` & `hearthstone-6.5.0/hearthstone/bountyxml.py`

 * *Files identical despite different names*

### Comparing `hearthstone-6.4.0/hearthstone/cardxml.py` & `hearthstone-6.5.0/hearthstone/cardxml.py`

 * *Files identical despite different names*

### Comparing `hearthstone-6.4.0/hearthstone/dbf.py` & `hearthstone-6.5.0/hearthstone/dbf.py`

 * *Files identical despite different names*

### Comparing `hearthstone-6.4.0/hearthstone/deckstrings.py` & `hearthstone-6.5.0/hearthstone/deckstrings.py`

 * *Files identical despite different names*

### Comparing `hearthstone-6.4.0/hearthstone/entities.py` & `hearthstone-6.5.0/hearthstone/entities.py`

 * *Files identical despite different names*

### Comparing `hearthstone-6.4.0/hearthstone/enums.py` & `hearthstone-6.5.0/hearthstone/enums.py`

 * *Files 0% similar despite different names*

```diff
@@ -1101,14 +1101,15 @@
 			CardSet.DARKMOON_FAIRE,
 			CardSet.THE_BARRENS,
 			CardSet.ALTERAC_VALLEY,
 			CardSet.LEGACY,
 			CardSet.THE_SUNKEN_CITY,
 			CardSet.RETURN_OF_THE_LICH_KING,
 			CardSet.PATH_OF_ARTHAS,
+			CardSet.BATTLE_OF_THE_BANDS,
 		)
 
 	@property
 	def name_global(self):
 		# Newer sets use a 2-3 letter set code
 		from .utils import CARDSET_GLOBAL_STRING_MAP
 		custom = CARDSET_GLOBAL_STRING_MAP.get(self)
@@ -2368,14 +2369,15 @@
 	KRAKEN = 1
 	MAMMOTH = 2
 	RAVEN = 3
 	DRAGON = 4
 	PHOENIX = 5
 	GRYPHON = 6
 	HYDRA = 7
+	WOLF = 8
 
 	@property
 	def standard_card_sets(self):
 		from .utils import STANDARD_SETS
 		return STANDARD_SETS.get(self, [])
 
 	@classmethod
```

### Comparing `hearthstone-6.4.0/hearthstone/mercenaryxml.py` & `hearthstone-6.5.0/hearthstone/mercenaryxml.py`

 * *Files identical despite different names*

### Comparing `hearthstone-6.4.0/hearthstone/stringsfile.py` & `hearthstone-6.5.0/hearthstone/stringsfile.py`

 * *Files identical despite different names*

### Comparing `hearthstone-6.4.0/hearthstone/utils/__init__.py` & `hearthstone-6.5.0/hearthstone/utils/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -170,14 +170,19 @@
 	ZodiacYear.HYDRA: [
 		CardSet.CORE,
 		CardSet.THE_BARRENS, CardSet.WAILING_CAVERNS, CardSet.STORMWIND,
 		CardSet.ALTERAC_VALLEY, CardSet.THE_SUNKEN_CITY, CardSet.REVENDRETH,
 		CardSet.RETURN_OF_THE_LICH_KING, CardSet.PATH_OF_ARTHAS,
 		CardSet.BATTLE_OF_THE_BANDS,
 	],
+	ZodiacYear.WOLF: [
+		CardSet.CORE,
+		CardSet.THE_SUNKEN_CITY, CardSet.REVENDRETH, CardSet.RETURN_OF_THE_LICH_KING,
+		CardSet.PATH_OF_ARTHAS, CardSet.BATTLE_OF_THE_BANDS,
+	]
 }
 
 
 try:
 	_EPOCH = datetime.fromtimestamp(0)
 except OSError:
 	# https://bugs.python.org/issue29097 (Windows-only)
@@ -189,14 +194,15 @@
 	ZodiacYear.KRAKEN: datetime(2016, 4, 26),
 	ZodiacYear.MAMMOTH: datetime(2017, 4, 7),
 	ZodiacYear.RAVEN: datetime(2018, 4, 12),
 	ZodiacYear.DRAGON: datetime(2019, 4, 9),
 	ZodiacYear.PHOENIX: datetime(2020, 4, 7),
 	ZodiacYear.GRYPHON: datetime(2021, 3, 30),
 	ZodiacYear.HYDRA: datetime(2022, 4, 12),
+	ZodiacYear.WOLF: datetime(2023, 4, 11),
 }
 
 
 # QuestController.cs
 QUEST_REWARDS = {
 	"UNG_940": "UNG_940t8",
 	"UNG_954": "UNG_954t1",
```

### Comparing `hearthstone-6.4.0/hearthstone/xmlutils.py` & `hearthstone-6.5.0/hearthstone/xmlutils.py`

 * *Files identical despite different names*

### Comparing `hearthstone-6.4.0/hearthstone.egg-info/PKG-INFO` & `hearthstone-6.5.0/hearthstone.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hearthstone
-Version: 6.4.0
+Version: 6.5.0
 Summary: CardDefs.xml parser and Hearthstone enums for Python
 Home-page: https://github.com/HearthSim/python-hearthstone/
 Download-URL: https://github.com/HearthSim/python-hearthstone/tarball/master
 Author: Jerome Leclanche
 Author-email: jerome@leclan.ch
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `hearthstone-6.4.0/hearthstone.egg-info/SOURCES.txt` & `hearthstone-6.5.0/hearthstone.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hearthstone-6.4.0/setup.cfg` & `hearthstone-6.5.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = hearthstone
-version = 6.4.0
+version = 6.5.0
 description = CardDefs.xml parser and Hearthstone enums for Python
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Jerome Leclanche
 author_email = jerome@leclan.ch
 url = https://github.com/HearthSim/python-hearthstone/
 download_url = https://github.com/HearthSim/python-hearthstone/tarball/master
```

