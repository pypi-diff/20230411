# Comparing `tmp/goodreadsscraper-0.3.tar.gz` & `tmp/goodreadsscraper-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goodreadsscraper-0.3.tar", last modified: Mon Apr 10 16:28:32 2023, max compression
+gzip compressed data, was "goodreadsscraper-0.4.tar", last modified: Tue Apr 11 12:26:01 2023, max compression
```

## Comparing `goodreadsscraper-0.3.tar` & `goodreadsscraper-0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rwxr-xr-x   0        0        0     1098 2023-04-02 18:42:33.763559 goodreadsscraper-0.3/LICENSE
--rwxr-xr-x   0        0        0    27708 2023-04-05 14:39:21.394653 goodreadsscraper-0.3/geckodriver.log
--rwxr-xr-x   0        0        0    25305 2023-04-10 16:28:27.508161 goodreadsscraper-0.3/goodreadsscraper/__init__.py
--rwxr-xr-x   0        0        0     3660 2023-04-02 22:30:15.644596 goodreadsscraper-0.3/goodreadsscraper/author.py
--rwxr-xr-x   0        0        0     2876 2023-04-02 18:42:33.769060 goodreadsscraper-0.3/goodreadsscraper/book.py
--rwxr-xr-x   0        0        0     2152 2023-04-10 15:25:43.633380 goodreadsscraper-0.3/goodreadsscraper/review.py
--rwxr-xr-x   0        0        0        0 2023-04-05 21:14:32.340995 goodreadsscraper-0.3/goodreadsscraper/test/debug.html
--rwxr-xr-x   0        0        0    12709 2023-04-10 16:22:02.668138 goodreadsscraper-0.3/goodreadsscraper/utils.py
--rwxr-xr-x   0        0        0      550 2023-04-10 16:28:29.238615 goodreadsscraper-0.3/pyproject.toml
--rwxr-xr-x   0        0        0     8669 2023-04-10 16:28:22.834903 goodreadsscraper-0.3/readme.md
--rwxr-xr-x   0        0        0     1996 2023-04-10 15:25:43.652881 goodreadsscraper-0.3/reviewanalyser/__init__.py
--rwxr-xr-x   0        0        0  5329000 2023-04-10 15:25:43.697879 goodreadsscraper-0.3/reviewanalyser/model/review_analyser.h5
--rwxr-xr-x   0        0        0   138845 2023-04-10 15:25:43.705879 goodreadsscraper-0.3/reviewanalyser/model/tv_layer.pkl
--rw-r--r--   0        0        0     8848 1970-01-01 00:00:00.000000 goodreadsscraper-0.3/PKG-INFO
+-rwxr-xr-x   0        0        0     1098 2023-04-02 18:42:33.763559 goodreadsscraper-0.4/LICENSE
+-rwxr-xr-x   0        0        0    27708 2023-04-05 14:39:21.394653 goodreadsscraper-0.4/geckodriver.log
+-rwxr-xr-x   0        0        0    25305 2023-04-11 12:15:38.302801 goodreadsscraper-0.4/goodreadsscraper/__init__.py
+-rwxr-xr-x   0        0        0     3660 2023-04-02 22:30:15.644596 goodreadsscraper-0.4/goodreadsscraper/author.py
+-rwxr-xr-x   0        0        0     2876 2023-04-02 18:42:33.769060 goodreadsscraper-0.4/goodreadsscraper/book.py
+-rwxr-xr-x   0        0        0     2152 2023-04-10 15:25:43.633380 goodreadsscraper-0.4/goodreadsscraper/review.py
+-rwxr-xr-x   0        0        0        0 2023-04-05 21:14:32.340995 goodreadsscraper-0.4/goodreadsscraper/test/debug.html
+-rwxr-xr-x   0        0        0    12926 2023-04-11 12:16:56.682616 goodreadsscraper-0.4/goodreadsscraper/utils.py
+-rwxr-xr-x   0        0        0      550 2023-04-10 16:28:29.238615 goodreadsscraper-0.4/pyproject.toml
+-rwxr-xr-x   0        0        0     8778 2023-04-11 12:15:25.707368 goodreadsscraper-0.4/readme.md
+-rwxr-xr-x   0        0        0     1996 2023-04-10 15:25:43.652881 goodreadsscraper-0.4/reviewanalyser/__init__.py
+-rwxr-xr-x   0        0        0  5329000 2023-04-10 15:25:43.697879 goodreadsscraper-0.4/reviewanalyser/model/review_analyser.h5
+-rwxr-xr-x   0        0        0   138845 2023-04-10 15:25:43.705879 goodreadsscraper-0.4/reviewanalyser/model/tv_layer.pkl
+-rw-r--r--   0        0        0     8954 1970-01-01 00:00:00.000000 goodreadsscraper-0.4/PKG-INFO
```

### Comparing `goodreadsscraper-0.3/LICENSE` & `goodreadsscraper-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `goodreadsscraper-0.3/geckodriver.log` & `goodreadsscraper-0.4/geckodriver.log`

 * *Files identical despite different names*

### Comparing `goodreadsscraper-0.3/goodreadsscraper/__init__.py` & `goodreadsscraper-0.4/goodreadsscraper/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #! /usr/bin/env python3
 """Module to scrap book information from goodreads
 """
 
-__version__ = '0.3'
+__version__ = '0.4'
 
 __description__ = 'Module to scrap book information from goodreads'
 
 import os
 import time
 import re
 import json
```

### Comparing `goodreadsscraper-0.3/goodreadsscraper/author.py` & `goodreadsscraper-0.4/goodreadsscraper/author.py`

 * *Files identical despite different names*

### Comparing `goodreadsscraper-0.3/goodreadsscraper/book.py` & `goodreadsscraper-0.4/goodreadsscraper/book.py`

 * *Files identical despite different names*

### Comparing `goodreadsscraper-0.3/goodreadsscraper/review.py` & `goodreadsscraper-0.4/goodreadsscraper/review.py`

 * *Files identical despite different names*

### Comparing `goodreadsscraper-0.3/goodreadsscraper/utils.py` & `goodreadsscraper-0.4/goodreadsscraper/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -142,15 +142,16 @@
                                output = args.output,
                                logging = args.logging,
                                errors = args.errors,
                                reviews_simple = args.reviews_simple,
                                reviews = args.reviews,
                                reviews_range = args.reviews_range,
                                reviews_language = args.reviews_language,
-                               reviews_output = args.reviews_output)
+                               reviews_output = args.reviews_output,
+                               verbose = args.verbose)
 
         books.append(book)
 
     #Apenas um author
     elif args.author:
         author = SimpleNamespace(author = args.author,
                                  maxworks = args.maxworks,
@@ -179,15 +180,16 @@
                                output = args.output,
                                logging = args.logging,
                                errors = args.errors,
                                reviews_simple = args.reviews_simple,
                                reviews = args.reviews,
                                reviews_range = args.reviews_range,
                                reviews_language = args.reviews_language,
-                               reviews_output = None)
+                               reviews_output = None,
+                               verbose = args.verbose)
 
                 if 'isbn' in book_json:
                     book.isbn = book_json['isbn']
                 if 'id' in book_json:
                     book.id = book_json['id']
                 if 'name' in book_json:
                     book.btitle = book_json['name']
@@ -204,14 +206,16 @@
                         book.reviews_range = book_json['reviews_range']
                     else:
                         invalid = True
                 if 'reviews_language' in book_json:
                     book.reviews_language = book_json['reviews_language']
                 if 'reviews_output' in book_json:
                     book.reviews_output = book_json['reviews_output']
+                if 'verbose' in book_json:
+                        book.verbose = book_json['verbose']
 
                 if not (book.isbn or book.id or book.btitle):
                     invalid = True
                 else: 
                     books.append(book)
                 if invalid:
                     error(args,f"Error in dic \n {book_json}")
```

### Comparing `goodreadsscraper-0.3/pyproject.toml` & `goodreadsscraper-0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `goodreadsscraper-0.3/readme.md` & `goodreadsscraper-0.4/readme.md`

 * *Files 3% similar despite different names*

```diff
@@ -191,22 +191,25 @@
             {
                 "name" : "Coraline",
                 "author" : "Neil Gaiman", 
                 "output" : "coraline.txt",
                 "reviews" : true,
                 "reviews_output" : "caroline_reviews.csv",
                 "reviews_range" : [40,60],
-                "reviews_language" : "pt"
+                "reviews_language" : "pt",
+                "verbose" : true
 
             }
         ],
         "authors" : [
             {
-                "name" : "abel ferreira",
-                "output" : "abel.txt"
+                "name" : "Neil Gaiman",
+                "output" : "neil_gaiman.txt",
+                "maxworks" : 20,
+                "verbose" : true
             }
         ]
 }
 
 Where the first key *books* represents all the books that are meant to be scraped. Each book can have its task costumized to only search for the basic info, its output, gather reviews in a range and so on. The flags explained before are also available here in the same contexts, whereas in this case their full name has to be given, as exemplefied, for ease of legibility (special case for 'btitle' and 'a' which both are recognized as 'name').  
 As mentioned before, if a book does not have a review output defined, they will either go to the default output or, if a global review output is given with the flag **-ro**, they will be appended there.
```

### Comparing `goodreadsscraper-0.3/reviewanalyser/__init__.py` & `goodreadsscraper-0.4/reviewanalyser/__init__.py`

 * *Files identical despite different names*

### Comparing `goodreadsscraper-0.3/reviewanalyser/model/review_analyser.h5` & `goodreadsscraper-0.4/reviewanalyser/model/review_analyser.h5`

 * *Files identical despite different names*

### Comparing `goodreadsscraper-0.3/reviewanalyser/model/tv_layer.pkl` & `goodreadsscraper-0.4/reviewanalyser/model/tv_layer.pkl`

 * *Files identical despite different names*

### Comparing `goodreadsscraper-0.3/PKG-INFO` & `goodreadsscraper-0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goodreadsscraper
-Version: 0.3
+Version: 0.4
 Summary: Module to scrap book information from goodreads
 Author-email: brazafonso <a93178@uminho.pt>, Tiago Silva <a93277@uminho.pt>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: jellyfish
 Requires-Dist: pandas
 Requires-Dist: bs4
@@ -204,22 +204,25 @@
             {
                 "name" : "Coraline",
                 "author" : "Neil Gaiman", 
                 "output" : "coraline.txt",
                 "reviews" : true,
                 "reviews_output" : "caroline_reviews.csv",
                 "reviews_range" : [40,60],
-                "reviews_language" : "pt"
+                "reviews_language" : "pt",
+                "verbose" : true
 
             }
         ],
         "authors" : [
             {
-                "name" : "abel ferreira",
-                "output" : "abel.txt"
+                "name" : "Neil Gaiman",
+                "output" : "neil_gaiman.txt",
+                "maxworks" : 20,
+                "verbose" : true
             }
         ]
 }
 
 Where the first key *books* represents all the books that are meant to be scraped. Each book can have its task costumized to only search for the basic info, its output, gather reviews in a range and so on. The flags explained before are also available here in the same contexts, whereas in this case their full name has to be given, as exemplefied, for ease of legibility (special case for 'btitle' and 'a' which both are recognized as 'name').  
 As mentioned before, if a book does not have a review output defined, they will either go to the default output or, if a global review output is given with the flag **-ro**, they will be appended there.
```

