# Comparing `tmp/extr-0.0.1.tar.gz` & `tmp/extr-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extr-0.0.1.tar", last modified: Tue Apr 11 09:38:10 2023, max compression
+gzip compressed data, was "extr-0.0.2.tar", last modified: Tue Apr 11 09:40:32 2023, max compression
```

## Comparing `extr-0.0.1.tar` & `extr-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 09:38:10.242908 extr-0.0.1/
--rw-rw-rw-   0        0        0     2352 2023-04-11 09:38:10.235119 extr-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1602 2023-04-10 14:08:55.000000 extr-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-11 09:38:10.247288 extr-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      384 2023-04-11 09:36:55.000000 extr-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-11 09:38:10.091383 extr-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-11 09:38:10.148239 extr-0.0.1/src/extr/
--rw-rw-rw-   0        0        0      226 2023-04-10 13:22:29.000000 extr-0.0.1/src/extr/__init__.py
--rw-rw-rw-   0        0        0     1526 2023-04-10 13:35:41.000000 extr-0.0.1/src/extr/entities.py
--rw-rw-rw-   0        0        0      158 2023-04-08 19:56:35.000000 extr-0.0.1/src/extr/iterutils.py
--rw-rw-rw-   0        0        0     1034 2023-04-10 13:02:05.000000 extr-0.0.1/src/extr/models.py
--rw-rw-rw-   0        0        0     2510 2023-04-10 13:19:22.000000 extr-0.0.1/src/extr/regex.py
--rw-rw-rw-   0        0        0     1166 2023-04-10 13:13:58.000000 extr-0.0.1/src/extr/relations.py
-drwxrwxrwx   0        0        0        0 2023-04-11 09:38:10.231459 extr-0.0.1/src/extr.egg-info/
--rw-rw-rw-   0        0        0     2352 2023-04-11 09:38:09.000000 extr-0.0.1/src/extr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-04-11 09:38:09.000000 extr-0.0.1/src/extr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 09:38:09.000000 extr-0.0.1/src/extr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-04-11 09:38:09.000000 extr-0.0.1/src/extr.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-11 09:40:32.624062 extr-0.0.2/
+-rw-rw-rw-   0        0        0     2422 2023-04-11 09:40:32.613041 extr-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1586 2023-04-11 09:38:34.000000 extr-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-11 09:40:32.627345 extr-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      477 2023-04-11 09:40:00.000000 extr-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 09:40:32.482951 extr-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-11 09:40:32.556188 extr-0.0.2/src/extr/
+-rw-rw-rw-   0        0        0      226 2023-04-10 13:22:29.000000 extr-0.0.2/src/extr/__init__.py
+-rw-rw-rw-   0        0        0     1526 2023-04-10 13:35:41.000000 extr-0.0.2/src/extr/entities.py
+-rw-rw-rw-   0        0        0      158 2023-04-08 19:56:35.000000 extr-0.0.2/src/extr/iterutils.py
+-rw-rw-rw-   0        0        0     1034 2023-04-10 13:02:05.000000 extr-0.0.2/src/extr/models.py
+-rw-rw-rw-   0        0        0     2510 2023-04-10 13:19:22.000000 extr-0.0.2/src/extr/regex.py
+-rw-rw-rw-   0        0        0     1166 2023-04-10 13:13:58.000000 extr-0.0.2/src/extr/relations.py
+drwxrwxrwx   0        0        0        0 2023-04-11 09:40:32.610035 extr-0.0.2/src/extr.egg-info/
+-rw-rw-rw-   0        0        0     2422 2023-04-11 09:40:32.000000 extr-0.0.2/src/extr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2023-04-11 09:40:32.000000 extr-0.0.2/src/extr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 09:40:32.000000 extr-0.0.2/src/extr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-04-11 09:40:32.000000 extr-0.0.2/src/extr.egg-info/top_level.txt
```

### Comparing `extr-0.0.1/PKG-INFO` & `extr-0.0.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: extr
-Version: 0.0.1
-Summary: UNKNOWN
+Version: 0.0.2
+Summary: Named Entity Recognition (NER) and Relation Extraction (RE) library using Regular Expressions
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: # Extr - NLP
         
         > Named Entity Recognition (NER) and Relation Extraction (RE) library using Regular Expressions
         
         <br />
         
         ## Install
         
         ```
-        pip install extr-nlp
+        pip install extr
         ```
         
         ## Example
         
         ```python
         text = 'Ted is a Pitcher.'
         ```
         
         ### 1. Entity Extraction
         > Find Named Entities from text.
         
         ```python
-        from extr_nlp import RegEx, RegExLabel, EntityExtactor
+        from extr import RegEx, RegExLabel, EntityExtactor
         
         entity_extractor = EntityExtactor([
             RegExLabel('PERSON', [
                 RegEx([r'ted'], re.IGNORECASE)
             ]),
             RegExLabel('POSITION', [
                 RegEx([r'pitcher'], re.IGNORECASE)
@@ -45,16 +45,16 @@
         ## ]
         ```
         
         ### 2. Relation Extraction
         > Annotate and Extract Relationships between Entities
         
         ```python
-        from extr_nlp import EntityAnnotator
-        from extr_nlp import RegExRelationLabelBuilder, RelationExtractor
+        from extr import EntityAnnotator
+        from extr import RegExRelationLabelBuilder, RelationExtractor
         
         ## define relationship between PERSON and POSITION
         relationship = RegExRelationLabelBuilder('is_a') \
             .add_e1_to_e2(
                 'PERSON', ## e1
                 [
                     ## define how the relationship exists in nature
```

### Comparing `extr-0.0.1/README.md` & `extr-0.0.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -3,28 +3,28 @@
 > Named Entity Recognition (NER) and Relation Extraction (RE) library using Regular Expressions
 
 <br />
 
 ## Install
 
 ```
-pip install extr-nlp
+pip install extr
 ```
 
 ## Example
 
 ```python
 text = 'Ted is a Pitcher.'
 ```
 
 ### 1. Entity Extraction
 > Find Named Entities from text.
 
 ```python
-from extr_nlp import RegEx, RegExLabel, EntityExtactor
+from extr import RegEx, RegExLabel, EntityExtactor
 
 entity_extractor = EntityExtactor([
     RegExLabel('PERSON', [
         RegEx([r'ted'], re.IGNORECASE)
     ]),
     RegExLabel('POSITION', [
         RegEx([r'pitcher'], re.IGNORECASE)
@@ -39,16 +39,16 @@
 ## ]
 ```
 
 ### 2. Relation Extraction
 > Annotate and Extract Relationships between Entities
 
 ```python
-from extr_nlp import EntityAnnotator
-from extr_nlp import RegExRelationLabelBuilder, RelationExtractor
+from extr import EntityAnnotator
+from extr import RegExRelationLabelBuilder, RelationExtractor
 
 ## define relationship between PERSON and POSITION
 relationship = RegExRelationLabelBuilder('is_a') \
     .add_e1_to_e2(
         'PERSON', ## e1
         [
             ## define how the relationship exists in nature
```

### Comparing `extr-0.0.1/src/extr/entities.py` & `extr-0.0.2/src/extr/entities.py`

 * *Files identical despite different names*

### Comparing `extr-0.0.1/src/extr/models.py` & `extr-0.0.2/src/extr/models.py`

 * *Files identical despite different names*

### Comparing `extr-0.0.1/src/extr/regex.py` & `extr-0.0.2/src/extr/regex.py`

 * *Files identical despite different names*

### Comparing `extr-0.0.1/src/extr/relations.py` & `extr-0.0.2/src/extr/relations.py`

 * *Files identical despite different names*

### Comparing `extr-0.0.1/src/extr.egg-info/PKG-INFO` & `extr-0.0.2/src/extr.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: extr
-Version: 0.0.1
-Summary: UNKNOWN
+Version: 0.0.2
+Summary: Named Entity Recognition (NER) and Relation Extraction (RE) library using Regular Expressions
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: # Extr - NLP
         
         > Named Entity Recognition (NER) and Relation Extraction (RE) library using Regular Expressions
         
         <br />
         
         ## Install
         
         ```
-        pip install extr-nlp
+        pip install extr
         ```
         
         ## Example
         
         ```python
         text = 'Ted is a Pitcher.'
         ```
         
         ### 1. Entity Extraction
         > Find Named Entities from text.
         
         ```python
-        from extr_nlp import RegEx, RegExLabel, EntityExtactor
+        from extr import RegEx, RegExLabel, EntityExtactor
         
         entity_extractor = EntityExtactor([
             RegExLabel('PERSON', [
                 RegEx([r'ted'], re.IGNORECASE)
             ]),
             RegExLabel('POSITION', [
                 RegEx([r'pitcher'], re.IGNORECASE)
@@ -45,16 +45,16 @@
         ## ]
         ```
         
         ### 2. Relation Extraction
         > Annotate and Extract Relationships between Entities
         
         ```python
-        from extr_nlp import EntityAnnotator
-        from extr_nlp import RegExRelationLabelBuilder, RelationExtractor
+        from extr import EntityAnnotator
+        from extr import RegExRelationLabelBuilder, RelationExtractor
         
         ## define relationship between PERSON and POSITION
         relationship = RegExRelationLabelBuilder('is_a') \
             .add_e1_to_e2(
                 'PERSON', ## e1
                 [
                     ## define how the relationship exists in nature
```

