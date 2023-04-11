# Comparing `tmp/txt2tei-1.0.5.tar.gz` & `tmp/txt2tei-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "txt2tei-1.0.5.tar", last modified: Thu Mar 16 13:46:44 2023, max compression
+gzip compressed data, was "txt2tei-1.0.6.tar", last modified: Tue Apr 11 06:31:16 2023, max compression
```

## Comparing `txt2tei-1.0.5.tar` & `txt2tei-1.0.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 fernando  (1000) fernando  (1000)        0 2023-03-16 13:46:44.884926 txt2tei-1.0.5/
--rw-r--r--   0 fernando  (1000) fernando  (1000)    35149 2022-02-02 16:16:01.000000 txt2tei-1.0.5/LICENSE
--rw-r--r--   0 fernando  (1000) fernando  (1000)     5230 2023-03-16 13:46:44.884926 txt2tei-1.0.5/PKG-INFO
--rw-r--r--   0 fernando  (1000) fernando  (1000)     4376 2023-03-16 13:40:33.000000 txt2tei-1.0.5/README.md
--rw-r--r--   0 fernando  (1000) fernando  (1000)       38 2023-03-16 13:46:44.884926 txt2tei-1.0.5/setup.cfg
--rw-r--r--   0 fernando  (1000) fernando  (1000)     1498 2023-03-16 13:40:47.000000 txt2tei-1.0.5/setup.py
-drwxr-xr-x   0 fernando  (1000) fernando  (1000)        0 2023-03-16 13:46:44.884926 txt2tei-1.0.5/txt2tei/
--rw-r--r--   0 fernando  (1000) fernando  (1000)       23 2023-01-31 12:10:06.000000 txt2tei-1.0.5/txt2tei/__init__.py
--rwxr-xr-x   0 fernando  (1000) fernando  (1000)      893 2023-03-09 15:42:07.000000 txt2tei-1.0.5/txt2tei/addmetre.py
--rw-r--r--   0 fernando  (1000) fernando  (1000)     2457 2022-04-08 21:20:27.000000 txt2tei-1.0.5/txt2tei/authors.py
--rw-r--r--   0 fernando  (1000) fernando  (1000)     1422 2022-04-08 21:31:21.000000 txt2tei-1.0.5/txt2tei/authors.xml
--rw-r--r--   0 fernando  (1000) fernando  (1000)      715 2023-01-31 09:11:47.000000 txt2tei-1.0.5/txt2tei/edition.py
--rw-r--r--   0 fernando  (1000) fernando  (1000)    14360 2023-03-16 13:38:58.000000 txt2tei-1.0.5/txt2tei/libtxt2tei.py
--rwxr-xr-x   0 fernando  (1000) fernando  (1000)     1910 2023-01-31 12:06:06.000000 txt2tei-1.0.5/txt2tei/makelist.py
--rw-r--r--   0 fernando  (1000) fernando  (1000)    12011 2022-02-02 16:16:47.000000 txt2tei-1.0.5/txt2tei/sexos.csv
--rwxr-xr-x   0 fernando  (1000) fernando  (1000)     4175 2023-01-30 14:00:22.000000 txt2tei-1.0.5/txt2tei/tei2txt.py
--rwxr-xr-x   0 fernando  (1000) fernando  (1000)    16599 2023-01-31 12:06:06.000000 txt2tei-1.0.5/txt2tei/txt2tei-a.py
--rwxr-xr-x   0 fernando  (1000) fernando  (1000)    20686 2023-03-16 13:46:37.000000 txt2tei-1.0.5/txt2tei/txt2tei.py
-drwxr-xr-x   0 fernando  (1000) fernando  (1000)        0 2023-03-16 13:46:44.884926 txt2tei-1.0.5/txt2tei.egg-info/
--rw-r--r--   0 fernando  (1000) fernando  (1000)     5230 2023-03-16 13:46:44.000000 txt2tei-1.0.5/txt2tei.egg-info/PKG-INFO
--rw-r--r--   0 fernando  (1000) fernando  (1000)      431 2023-03-16 13:46:44.000000 txt2tei-1.0.5/txt2tei.egg-info/SOURCES.txt
--rw-r--r--   0 fernando  (1000) fernando  (1000)        1 2023-03-16 13:46:44.000000 txt2tei-1.0.5/txt2tei.egg-info/dependency_links.txt
--rw-r--r--   0 fernando  (1000) fernando  (1000)       41 2023-03-16 13:46:44.000000 txt2tei-1.0.5/txt2tei.egg-info/entry_points.txt
--rw-r--r--   0 fernando  (1000) fernando  (1000)       31 2023-03-16 13:46:44.000000 txt2tei-1.0.5/txt2tei.egg-info/requires.txt
--rw-r--r--   0 fernando  (1000) fernando  (1000)        8 2023-03-16 13:46:44.000000 txt2tei-1.0.5/txt2tei.egg-info/top_level.txt
+drwxr-xr-x   0 fernando  (1000) fernando  (1000)        0 2023-04-11 06:31:16.631655 txt2tei-1.0.6/
+-rw-r--r--   0 fernando  (1000) fernando  (1000)    35149 2022-02-02 16:16:01.000000 txt2tei-1.0.6/LICENSE
+-rw-r--r--   0 fernando  (1000) fernando  (1000)     5345 2023-04-11 06:31:16.631655 txt2tei-1.0.6/PKG-INFO
+-rw-r--r--   0 fernando  (1000) fernando  (1000)     4491 2023-04-11 05:55:54.000000 txt2tei-1.0.6/README.md
+-rw-r--r--   0 fernando  (1000) fernando  (1000)       38 2023-04-11 06:31:16.631655 txt2tei-1.0.6/setup.cfg
+-rw-r--r--   0 fernando  (1000) fernando  (1000)     1498 2023-04-10 08:19:06.000000 txt2tei-1.0.6/setup.py
+drwxr-xr-x   0 fernando  (1000) fernando  (1000)        0 2023-04-11 06:31:16.619655 txt2tei-1.0.6/txt2tei/
+-rw-r--r--   0 fernando  (1000) fernando  (1000)       23 2023-01-31 12:10:06.000000 txt2tei-1.0.6/txt2tei/__init__.py
+-rwxr-xr-x   0 fernando  (1000) fernando  (1000)      893 2023-03-09 15:42:07.000000 txt2tei-1.0.6/txt2tei/addmetre.py
+-rw-r--r--   0 fernando  (1000) fernando  (1000)     2457 2022-04-08 21:20:27.000000 txt2tei-1.0.6/txt2tei/authors.py
+-rw-r--r--   0 fernando  (1000) fernando  (1000)     1422 2022-04-08 21:31:21.000000 txt2tei-1.0.6/txt2tei/authors.xml
+-rw-r--r--   0 fernando  (1000) fernando  (1000)      715 2023-01-31 09:11:47.000000 txt2tei-1.0.6/txt2tei/edition.py
+-rw-r--r--   0 fernando  (1000) fernando  (1000)    14360 2023-03-16 13:38:58.000000 txt2tei-1.0.6/txt2tei/libtxt2tei.py
+-rwxr-xr-x   0 fernando  (1000) fernando  (1000)     1910 2023-01-31 12:06:06.000000 txt2tei-1.0.6/txt2tei/makelist.py
+-rw-r--r--   0 fernando  (1000) fernando  (1000)    12011 2022-02-02 16:16:47.000000 txt2tei-1.0.6/txt2tei/sexos.csv
+-rwxr-xr-x   0 fernando  (1000) fernando  (1000)     4175 2023-01-30 14:00:22.000000 txt2tei-1.0.6/txt2tei/tei2txt.py
+-rwxr-xr-x   0 fernando  (1000) fernando  (1000)    16599 2023-01-31 12:06:06.000000 txt2tei-1.0.6/txt2tei/txt2tei-a.py
+-rwxr-xr-x   0 fernando  (1000) fernando  (1000)    20920 2023-04-11 06:30:01.000000 txt2tei-1.0.6/txt2tei/txt2tei.py
+drwxr-xr-x   0 fernando  (1000) fernando  (1000)        0 2023-04-11 06:31:16.631655 txt2tei-1.0.6/txt2tei.egg-info/
+-rw-r--r--   0 fernando  (1000) fernando  (1000)     5345 2023-04-11 06:31:16.000000 txt2tei-1.0.6/txt2tei.egg-info/PKG-INFO
+-rw-r--r--   0 fernando  (1000) fernando  (1000)      431 2023-04-11 06:31:16.000000 txt2tei-1.0.6/txt2tei.egg-info/SOURCES.txt
+-rw-r--r--   0 fernando  (1000) fernando  (1000)        1 2023-04-11 06:31:16.000000 txt2tei-1.0.6/txt2tei.egg-info/dependency_links.txt
+-rw-r--r--   0 fernando  (1000) fernando  (1000)       41 2023-04-11 06:31:16.000000 txt2tei-1.0.6/txt2tei.egg-info/entry_points.txt
+-rw-r--r--   0 fernando  (1000) fernando  (1000)       31 2023-04-11 06:31:16.000000 txt2tei-1.0.6/txt2tei.egg-info/requires.txt
+-rw-r--r--   0 fernando  (1000) fernando  (1000)        8 2023-04-11 06:31:16.000000 txt2tei-1.0.6/txt2tei.egg-info/top_level.txt
```

### Comparing `txt2tei-1.0.5/LICENSE` & `txt2tei-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `txt2tei-1.0.5/PKG-INFO` & `txt2tei-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: txt2tei
-Version: 1.0.5
+Version: 1.0.6
 Summary: An aid to encoding plays as XML-TEI
 Home-page: https://github.com/fsanzl/txt2tei
 Author: Fernando Sanz-Lázaro
 Author-email: fsanzl@gmail.com
 License: LGPL
 Project-URL: Source, https://github.com/fsanzl/txt2tei/
 Project-URL: Tracker, https://github.com/fsanzl/txt2tei/issues
@@ -132,15 +132,21 @@
 
 ## Contributions
 
 Feel free to contribute using the [GitHub Issue Tracker](https://github.com/fsanzl/txt2tei/issues) for feedback, suggestions, or bug reports.
 
 ## Changelog
 
-* 1.0.5
+### 1.0.6
 
-** Solved pronouns-related crash
+- Solved empty date crash. 
+- Handling BOM and Hasefroch line terminators
+- Changelog markdown syntax
+
+### 1.0.5
+
+- Solved pronouns-related crash
 
 ## Licence
 
 This project is under GNU GPL 3. See [LICENCE](https://github.com/fsanzl/txt2tei/LICENSE) for details.
```

### Comparing `txt2tei-1.0.5/README.md` & `txt2tei-1.0.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -110,15 +110,21 @@
 
 ## Contributions
 
 Feel free to contribute using the [GitHub Issue Tracker](https://github.com/fsanzl/txt2tei/issues) for feedback, suggestions, or bug reports.
 
 ## Changelog
 
-* 1.0.5
+### 1.0.6
 
-** Solved pronouns-related crash
+- Solved empty date crash. 
+- Handling BOM and Hasefroch line terminators
+- Changelog markdown syntax
+
+### 1.0.5
+
+- Solved pronouns-related crash
 
 ## Licence
 
 This project is under GNU GPL 3. See [LICENCE](https://github.com/fsanzl/txt2tei/LICENSE) for details.
```

### Comparing `txt2tei-1.0.5/setup.py` & `txt2tei-1.0.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="txt2tei",
-    version="1.0.5",
+    version="1.0.6",
     python_requires='>=3.5',
     description="An aid to encoding plays as XML-TEI",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/fsanzl/txt2tei",
     project_urls={
         'Source': 'https://github.com/fsanzl/txt2tei/',
```

### Comparing `txt2tei-1.0.5/txt2tei/addmetre.py` & `txt2tei-1.0.6/txt2tei/addmetre.py`

 * *Files identical despite different names*

### Comparing `txt2tei-1.0.5/txt2tei/authors.py` & `txt2tei-1.0.6/txt2tei/authors.py`

 * *Files identical despite different names*

### Comparing `txt2tei-1.0.5/txt2tei/authors.xml` & `txt2tei-1.0.6/txt2tei/authors.xml`

 * *Files identical despite different names*

### Comparing `txt2tei-1.0.5/txt2tei/edition.py` & `txt2tei-1.0.6/txt2tei/edition.py`

 * *Files identical despite different names*

### Comparing `txt2tei-1.0.5/txt2tei/libtxt2tei.py` & `txt2tei-1.0.6/txt2tei/libtxt2tei.py`

 * *Files identical despite different names*

### Comparing `txt2tei-1.0.5/txt2tei/makelist.py` & `txt2tei-1.0.6/txt2tei/makelist.py`

 * *Files identical despite different names*

### Comparing `txt2tei-1.0.5/txt2tei/sexos.csv` & `txt2tei-1.0.6/txt2tei/sexos.csv`

 * *Files identical despite different names*

### Comparing `txt2tei-1.0.5/txt2tei/tei2txt.py` & `txt2tei-1.0.6/txt2tei/tei2txt.py`

 * *Files identical despite different names*

### Comparing `txt2tei-1.0.5/txt2tei/txt2tei-a.py` & `txt2tei-1.0.6/txt2tei/txt2tei-a.py`

 * *Files identical despite different names*

### Comparing `txt2tei-1.0.5/txt2tei/txt2tei.py` & `txt2tei-1.0.6/txt2tei/txt2tei.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,36 +2,37 @@
 import re
 from unidecode import unidecode
 import pandas as pd
 import lxml.etree as etree
 from lxml.etree import Element, SubElement, parse
 from datetime import datetime
 import sys
+import chardet
 if sys.version_info < (3, 9):
     # importlib.resources either doesn't exist or lacks the files()
     # function, so use the PyPI version:
     import importlib_resources
 else:
     # importlib.resources has files(), so use that:
     import importlib.resources as importlib_resources
 import os.path
 
 ###############################################################################
 # Please, edit this part if necessary
 editor = 'Fernando Sanz-Lázaro'
 authority = 'University of Vienna, Institute of Romance Languages '\
     'and Literatures'
-publisher_id = 'dracor'
-publisher_name = 'DraCor'
+publisher_id = ''
+publisher_name = ''
 licence = 'CC BY 3.0'
 licence_url = 'https://creativecommons.org/publicdomain/by/3.0/'
 hodie = datetime.today().strftime('%Y-%m-%d')
 nunc = datetime.today().strftime('%H:%M:%S')
 authority = ''
-publisher = ('DraCor', 'dracor', 'https://dracor.org')
+publisher = ('', '', '')
 licence = 'CC BY'
 licence_url = 'https://creativecommons.org/publicdomain/BY/3.0/'
 xml_model = '<?xml-model href="https://dracor.org/schema.rng" type="applicati'\
         'on/xml" schematypens="http://relaxng.org/ns/structure/1.0"?>'
 ###############################################################################
 
 
@@ -79,15 +80,17 @@
     standoff = make_standoff(standoff, date)
 
     SubElement(root, 'text')
     return tree
 
 
 def parse_date(date):
-    if '-' in date:
+    if not date or len(date) == 0:
+        date = {'notbefore': '1550', 'notafter': '1699'}
+    elif '-' in date:
         date = {'notbefore': date.split('-')[0],
                 'notafter': date.split('-')[1]}
     elif '?' in date:
         date = {'when': date.strip('?'), 'cert': 'medium'}
     else:
         date = {'when': date, 'cert': 'medium'}
     return date
@@ -443,15 +446,15 @@
     SubElement(speech, 'speaker').text = speaker
     return (speech, on_stage)
 
 
 header_labels = {'t': 'title', 'tt': 'subtitle', 'a': 'author',
                  'g': 'genre', 's': 'subgenre', 'o': 'source',
                  'f': 'date', 'x': 'comment'}
-rev_header_lavels = dict((v, k) for k, v in header_labels.items())
+rev_header_labels = dict((v, k) for k, v in header_labels.items())
 body_labels = {'j': 'act', '<e>': 'echo', '<p>': 'prose',
                '<i>': 'stage_direction', '<x>': 'comment'}
 subtitle = ''
 author = ''
 genre = ''
 subgenre = ''
 # date = ''
@@ -463,42 +466,49 @@
              '3.º': 'III', '4º': 'IV', '4.º': 'IV', 'PRIMERO': 'I',
              'SEGUNDO': 'II', 'TERCERO': 'III', 'CUARTO': 'IV',
              '1ª': 'i', '1.ª': 'i', '2ª': 'ii', '2.ª': 'ii', '3ª': 'iii',
              '3.ª': 'iii', '4ª': 'iv', '4.ª': 'iv', 'PRIMERA': 'i',
              'SEGUNDA': 'ii', 'TERCERA': 'iii', 'CUARTA': 'iv'}
 
 
+def unixfy(filename):
+    with open(filename, 'rb') as file:
+        raw = file.read(32)
+        encoding = chardet.detect(raw)['encoding']
+    return encoding
+
+
 def main(input_arguments=sys.argv):
     input_file = input_arguments[1]
     output = f'{input_file.rsplit(".", 1)[0]}.xml'
-    with open(input_file) as f:
+    enc = unixfy(input_file)
+    with open(input_file, 'rU', encoding=enc) as f:
         characters_list = find_characters(f)
-    with open(input_file) as g:
-        lines = g.readlines()
+        f.seek(0)
+        lines = f.readlines()
     author = date = title = n = sp = ''
     for line in lines:
         if line.startswith('<'):
             label = re.search(r'^\s*<(\w*)>', line.strip()).group(1)
             if label in header_labels.keys():
                 header_labels[label] = line.strip(f'<{label}>').strip()
             else:
                 break
         else:
             break
-        if header_labels['f']:
-            date = parse_date(header_labels['f'])
-
+    if header_labels['f']:
+        date = parse_date(header_labels['f'])
+    else:
+        date = parse_date('')
     author = parse_author(header_labels['a'])
     title = header_labels['t']
     subtitle = header_labels['tt']
     genre = header_labels['g']
     subgenre = header_labels['s']
     source = header_labels['o']
-    if not header_labels['f']:
-        date = parse_date('')
     tree = make_tree(
         title,
         subtitle,
         author,
         genre,
         subgenre,
         source,
```

### Comparing `txt2tei-1.0.5/txt2tei.egg-info/PKG-INFO` & `txt2tei-1.0.6/txt2tei.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: txt2tei
-Version: 1.0.5
+Version: 1.0.6
 Summary: An aid to encoding plays as XML-TEI
 Home-page: https://github.com/fsanzl/txt2tei
 Author: Fernando Sanz-Lázaro
 Author-email: fsanzl@gmail.com
 License: LGPL
 Project-URL: Source, https://github.com/fsanzl/txt2tei/
 Project-URL: Tracker, https://github.com/fsanzl/txt2tei/issues
@@ -132,15 +132,21 @@
 
 ## Contributions
 
 Feel free to contribute using the [GitHub Issue Tracker](https://github.com/fsanzl/txt2tei/issues) for feedback, suggestions, or bug reports.
 
 ## Changelog
 
-* 1.0.5
+### 1.0.6
 
-** Solved pronouns-related crash
+- Solved empty date crash. 
+- Handling BOM and Hasefroch line terminators
+- Changelog markdown syntax
+
+### 1.0.5
+
+- Solved pronouns-related crash
 
 ## Licence
 
 This project is under GNU GPL 3. See [LICENCE](https://github.com/fsanzl/txt2tei/LICENSE) for details.
```

