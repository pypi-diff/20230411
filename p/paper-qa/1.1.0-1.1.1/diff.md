# Comparing `tmp/paper-qa-1.1.0.tar.gz` & `tmp/paper-qa-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paper-qa-1.1.0.tar", last modified: Mon Apr 10 23:45:57 2023, max compression
+gzip compressed data, was "paper-qa-1.1.1.tar", last modified: Tue Apr 11 06:03:49 2023, max compression
```

## Comparing `paper-qa-1.1.0.tar` & `paper-qa-1.1.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 23:45:57.196550 paper-qa-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-10 23:45:30.000000 paper-qa-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11842 2023-04-10 23:45:57.192550 paper-qa-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11407 2023-04-10 23:45:30.000000 paper-qa-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 23:45:57.192550 paper-qa-1.1.0/paper_qa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11842 2023-04-10 23:45:57.000000 paper-qa-1.1.0/paper_qa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-10 23:45:57.000000 paper-qa-1.1.0/paper_qa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 23:45:57.000000 paper-qa-1.1.0/paper_qa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-10 23:45:57.000000 paper-qa-1.1.0/paper_qa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-10 23:45:57.000000 paper-qa-1.1.0/paper_qa.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 23:45:57.192550 paper-qa-1.1.0/paperqa/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-10 23:45:30.000000 paper-qa-1.1.0/paperqa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-04-10 23:45:30.000000 paper-qa-1.1.0/paperqa/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 23:45:57.192550 paper-qa-1.1.0/paperqa/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-10 23:45:30.000000 paper-qa-1.1.0/paperqa/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-04-10 23:45:30.000000 paper-qa-1.1.0/paperqa/contrib/zotero.py
--rw-r--r--   0 runner    (1001) docker     (123)    17084 2023-04-10 23:45:30.000000 paper-qa-1.1.0/paperqa/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-10 23:45:30.000000 paper-qa-1.1.0/paperqa/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-04-10 23:45:30.000000 paper-qa-1.1.0/paperqa/qaprompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-04-10 23:45:30.000000 paper-qa-1.1.0/paperqa/readers.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-04-10 23:45:30.000000 paper-qa-1.1.0/paperqa/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-10 23:45:30.000000 paper-qa-1.1.0/paperqa/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-10 23:45:30.000000 paper-qa-1.1.0/paperqa/version.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 23:45:57.196550 paper-qa-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-04-10 23:45:30.000000 paper-qa-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 23:45:57.192550 paper-qa-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9652 2023-04-10 23:45:30.000000 paper-qa-1.1.0/tests/test_paperqa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:03:49.005178 paper-qa-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-11 06:03:23.000000 paper-qa-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11838 2023-04-11 06:03:49.005178 paper-qa-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11403 2023-04-11 06:03:23.000000 paper-qa-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:03:49.005178 paper-qa-1.1.1/paper_qa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11838 2023-04-11 06:03:48.000000 paper-qa-1.1.1/paper_qa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-11 06:03:49.000000 paper-qa-1.1.1/paper_qa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 06:03:48.000000 paper-qa-1.1.1/paper_qa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-11 06:03:48.000000 paper-qa-1.1.1/paper_qa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-11 06:03:48.000000 paper-qa-1.1.1/paper_qa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:03:49.005178 paper-qa-1.1.1/paperqa/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-11 06:03:23.000000 paper-qa-1.1.1/paperqa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6013 2023-04-11 06:03:23.000000 paper-qa-1.1.1/paperqa/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:03:49.005178 paper-qa-1.1.1/paperqa/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-11 06:03:23.000000 paper-qa-1.1.1/paperqa/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-04-11 06:03:23.000000 paper-qa-1.1.1/paperqa/contrib/zotero.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17104 2023-04-11 06:03:23.000000 paper-qa-1.1.1/paperqa/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-11 06:03:23.000000 paper-qa-1.1.1/paperqa/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-04-11 06:03:23.000000 paper-qa-1.1.1/paperqa/qaprompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-04-11 06:03:23.000000 paper-qa-1.1.1/paperqa/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-04-11 06:03:23.000000 paper-qa-1.1.1/paperqa/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-11 06:03:23.000000 paper-qa-1.1.1/paperqa/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-11 06:03:23.000000 paper-qa-1.1.1/paperqa/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 06:03:49.005178 paper-qa-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-04-11 06:03:23.000000 paper-qa-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:03:49.005178 paper-qa-1.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9893 2023-04-11 06:03:23.000000 paper-qa-1.1.1/tests/test_paperqa.py
```

### Comparing `paper-qa-1.1.0/LICENSE` & `paper-qa-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `paper-qa-1.1.0/PKG-INFO` & `paper-qa-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper-qa
-Version: 1.1.0
+Version: 1.1.1
 Summary: LLM Chain for answering questions from docs 
 Home-page: https://github.com/whitead/paper-qa
 Author: Andrew White
 Author-email: white.d.andrew@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -160,15 +160,14 @@
 which relies on [pyzotero](https://github.com/urschrei/pyzotero).
 
 Install `pyzotero` to use this feature:
 
 ```bash
 pip install pyzotero
 ```
-```
 
 First, note that `paperqa` parses the PDFs of papers to store in the database,
 so all relevant papers should have PDFs stored inside your database.
 You can get Zotero to automatically do this by highlighting the references
 you wish to retrieve, right clicking, and selecting *"Find Available PDFs"*.
 You can also manually drag-and-drop PDFs onto each reference.
```

### Comparing `paper-qa-1.1.0/README.md` & `paper-qa-1.1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -146,15 +146,14 @@
 which relies on [pyzotero](https://github.com/urschrei/pyzotero).
 
 Install `pyzotero` to use this feature:
 
 ```bash
 pip install pyzotero
 ```
-```
 
 First, note that `paperqa` parses the PDFs of papers to store in the database,
 so all relevant papers should have PDFs stored inside your database.
 You can get Zotero to automatically do this by highlighting the references
 you wish to retrieve, right clicking, and selecting *"Find Available PDFs"*.
 You can also manually drag-and-drop PDFs onto each reference.
```

### Comparing `paper-qa-1.1.0/paper_qa.egg-info/PKG-INFO` & `paper-qa-1.1.1/paper_qa.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper-qa
-Version: 1.1.0
+Version: 1.1.1
 Summary: LLM Chain for answering questions from docs 
 Home-page: https://github.com/whitead/paper-qa
 Author: Andrew White
 Author-email: white.d.andrew@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -160,15 +160,14 @@
 which relies on [pyzotero](https://github.com/urschrei/pyzotero).
 
 Install `pyzotero` to use this feature:
 
 ```bash
 pip install pyzotero
 ```
-```
 
 First, note that `paperqa` parses the PDFs of papers to store in the database,
 so all relevant papers should have PDFs stored inside your database.
 You can get Zotero to automatically do this by highlighting the references
 you wish to retrieve, right clicking, and selecting *"Find Available PDFs"*.
 You can also manually drag-and-drop PDFs onto each reference.
```

### Comparing `paper-qa-1.1.0/paperqa/contrib/zotero.py` & `paper-qa-1.1.1/paperqa/contrib/zotero.py`

 * *Files identical despite different names*

### Comparing `paper-qa-1.1.0/paperqa/docs.py` & `paper-qa-1.1.1/paperqa/docs.py`

 * *Files 0% similar despite different names*

```diff
@@ -393,20 +393,20 @@
         answer: Optional[Answer] = None,
         key_filter: Optional[bool] = None,
     ) -> Answer:
         if k < max_sources:
             raise ValueError("k should be greater than max_sources")
         if answer is None:
             answer = Answer(query)
-        if key_filter or (key_filter is None and len(self.docs) > 5):
-            with get_openai_callback() as cb:
-                keys = self.doc_match(answer.question)
-            answer.tokens += cb.total_tokens
-            answer.cost += cb.total_cost
         if len(answer.contexts) == 0:
+            if key_filter or (key_filter is None and len(self.docs) > 5):
+                with get_openai_callback() as cb:
+                    keys = self.doc_match(answer.question)
+                answer.tokens += cb.total_tokens
+                answer.cost += cb.total_cost
             answer = await self.aget_evidence(
                 answer,
                 k=k,
                 max_sources=max_sources,
                 marginal_relevance=marginal_relevance,
                 key_filter=keys if key_filter else None,
             )
```

### Comparing `paper-qa-1.1.0/paperqa/qaprompts.py` & `paper-qa-1.1.1/paperqa/qaprompts.py`

 * *Files identical despite different names*

### Comparing `paper-qa-1.1.0/paperqa/readers.py` & `paper-qa-1.1.1/paperqa/readers.py`

 * *Files identical despite different names*

### Comparing `paper-qa-1.1.0/paperqa/types.py` & `paper-qa-1.1.1/paperqa/types.py`

 * *Files identical despite different names*

### Comparing `paper-qa-1.1.0/paperqa/utils.py` & `paper-qa-1.1.1/paperqa/utils.py`

 * *Files identical despite different names*

### Comparing `paper-qa-1.1.0/setup.py` & `paper-qa-1.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `paper-qa-1.1.0/tests/test_paperqa.py` & `paper-qa-1.1.1/tests/test_paperqa.py`

 * *Files 4% similar despite different names*

```diff
@@ -253,7 +253,17 @@
     # the filter shouldn't trigger, so just checking that it doesn't crash
 
 
 def disabled_test_agent():
     docs = paperqa.Docs()
     answer = paperqa.run_agent(docs, "What compounds target AKT1")
     print(answer)
+
+def test_zotera():
+    from paperqa.contrib import ZoteroDB
+
+    docs = paperqa.Docs()
+    try:
+        zotero = ZoteroDB(library_type="user")  # "group" if group library
+    except ValueError:
+        # close enough
+        return
```

