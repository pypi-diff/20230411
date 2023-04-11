# Comparing `tmp/pinecone_text-0.4.1.tar.gz` & `tmp/pinecone_text-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pinecone_text-0.4.1.tar", max compression
+gzip compressed data, was "pinecone_text-0.4.2.tar", max compression
```

## Comparing `pinecone_text-0.4.1.tar` & `pinecone_text-0.4.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    12229 2023-04-05 07:08:59.517552 pinecone_text-0.4.1/LICENSE.txt
--rw-r--r--   0        0        0     6095 2023-04-05 07:08:59.517552 pinecone_text-0.4.1/README.md
--rw-r--r--   0        0        0        1 2023-04-05 07:08:59.517552 pinecone_text-0.4.1/pinecone_text/__init__.py
--rw-r--r--   0        0        0      439 2023-04-05 07:08:59.517552 pinecone_text-0.4.1/pinecone_text/dense/__init__.py
--rw-r--r--   0        0        0      764 2023-04-05 07:08:59.517552 pinecone_text-0.4.1/pinecone_text/dense/base_dense_ecoder.py
--rw-r--r--   0        0        0     1259 2023-04-05 07:08:59.517552 pinecone_text-0.4.1/pinecone_text/dense/sentence_transformer_encoder.py
--rw-r--r--   0        0        0       67 2023-04-05 07:08:59.517552 pinecone_text-0.4.1/pinecone_text/hybrid/__init__.py
--rw-r--r--   0        0        0      998 2023-04-05 07:08:59.517552 pinecone_text-0.4.1/pinecone_text/hybrid/hybrid_convex.py
--rw-r--r--   0        0        0     1716 2023-04-05 07:08:59.517552 pinecone_text-0.4.1/pinecone_text/sparse/__init__.py
--rw-r--r--   0        0        0      818 2023-04-05 07:08:59.517552 pinecone_text-0.4.1/pinecone_text/sparse/base_sparse_encoder.py
--rw-r--r--   0        0        0     9727 2023-04-05 07:08:59.517552 pinecone_text-0.4.1/pinecone_text/sparse/bm25_encoder.py
--rw-r--r--   0        0        0     1760 2023-04-05 07:08:59.517552 pinecone_text-0.4.1/pinecone_text/sparse/bm25_tokenizer.py
--rw-r--r--   0        0        0     3073 2023-04-05 07:08:59.517552 pinecone_text-0.4.1/pinecone_text/sparse/splade_encoder.py
--rw-r--r--   0        0        0      625 2023-04-05 07:08:59.521552 pinecone_text-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     6735 1970-01-01 00:00:00.000000 pinecone_text-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0    12229 2023-04-11 11:35:10.504735 pinecone_text-0.4.2/LICENSE.txt
+-rw-r--r--   0        0        0     6095 2023-04-11 11:35:10.504735 pinecone_text-0.4.2/README.md
+-rw-r--r--   0        0        0       34 2023-04-11 11:35:10.504735 pinecone_text-0.4.2/pinecone_text/__init__.py
+-rw-r--r--   0        0        0      439 2023-04-11 11:35:10.508735 pinecone_text-0.4.2/pinecone_text/dense/__init__.py
+-rw-r--r--   0        0        0      764 2023-04-11 11:35:10.508735 pinecone_text-0.4.2/pinecone_text/dense/base_dense_ecoder.py
+-rw-r--r--   0        0        0     1259 2023-04-11 11:35:10.508735 pinecone_text-0.4.2/pinecone_text/dense/sentence_transformer_encoder.py
+-rw-r--r--   0        0        0       67 2023-04-11 11:35:10.508735 pinecone_text-0.4.2/pinecone_text/hybrid/__init__.py
+-rw-r--r--   0        0        0      998 2023-04-11 11:35:10.508735 pinecone_text-0.4.2/pinecone_text/hybrid/hybrid_convex.py
+-rw-r--r--   0        0        0     1716 2023-04-11 11:35:10.508735 pinecone_text-0.4.2/pinecone_text/sparse/__init__.py
+-rw-r--r--   0        0        0      818 2023-04-11 11:35:10.508735 pinecone_text-0.4.2/pinecone_text/sparse/base_sparse_encoder.py
+-rw-r--r--   0        0        0     9727 2023-04-11 11:35:10.508735 pinecone_text-0.4.2/pinecone_text/sparse/bm25_encoder.py
+-rw-r--r--   0        0        0     1760 2023-04-11 11:35:10.508735 pinecone_text-0.4.2/pinecone_text/sparse/bm25_tokenizer.py
+-rw-r--r--   0        0        0     3073 2023-04-11 11:35:10.508735 pinecone_text-0.4.2/pinecone_text/sparse/splade_encoder.py
+-rw-r--r--   0        0        0      624 2023-04-11 11:35:10.508735 pinecone_text-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     6785 1970-01-01 00:00:00.000000 pinecone_text-0.4.2/PKG-INFO
```

### Comparing `pinecone_text-0.4.1/LICENSE.txt` & `pinecone_text-0.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pinecone_text-0.4.1/README.md` & `pinecone_text-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `pinecone_text-0.4.1/pinecone_text/dense/base_dense_ecoder.py` & `pinecone_text-0.4.2/pinecone_text/dense/base_dense_ecoder.py`

 * *Files identical despite different names*

### Comparing `pinecone_text-0.4.1/pinecone_text/dense/sentence_transformer_encoder.py` & `pinecone_text-0.4.2/pinecone_text/dense/sentence_transformer_encoder.py`

 * *Files identical despite different names*

### Comparing `pinecone_text-0.4.1/pinecone_text/hybrid/hybrid_convex.py` & `pinecone_text-0.4.2/pinecone_text/hybrid/hybrid_convex.py`

 * *Files identical despite different names*

### Comparing `pinecone_text-0.4.1/pinecone_text/sparse/__init__.py` & `pinecone_text-0.4.2/pinecone_text/sparse/__init__.py`

 * *Files identical despite different names*

### Comparing `pinecone_text-0.4.1/pinecone_text/sparse/base_sparse_encoder.py` & `pinecone_text-0.4.2/pinecone_text/sparse/base_sparse_encoder.py`

 * *Files identical despite different names*

### Comparing `pinecone_text-0.4.1/pinecone_text/sparse/bm25_encoder.py` & `pinecone_text-0.4.2/pinecone_text/sparse/bm25_encoder.py`

 * *Files identical despite different names*

### Comparing `pinecone_text-0.4.1/pinecone_text/sparse/bm25_tokenizer.py` & `pinecone_text-0.4.2/pinecone_text/sparse/bm25_tokenizer.py`

 * *Files identical despite different names*

### Comparing `pinecone_text-0.4.1/pinecone_text/sparse/splade_encoder.py` & `pinecone_text-0.4.2/pinecone_text/sparse/splade_encoder.py`

 * *Files identical despite different names*

### Comparing `pinecone_text-0.4.1/pyproject.toml` & `pinecone_text-0.4.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "pinecone-text"
-version = "0.4.1"
+version = "0.4.2"
 description = "Text utilities library by Pinecone.io"
 authors = ["Pinecone.io"]
 readme = "README.md"
 packages = [{include = "pinecone_text"}]
 
 [tool.poetry.dependencies]
-python = ">=3.8 <3.11"
+python = ">=3.8,<4.0"
 torch = "^1.13.1"
 transformers = "^4.26.1"
 sentence-transformers = "^2.0.0"
 wget = "^3.2"
 mmh3 = "^3.1.0"
 nltk = "^3.6.5"
```

### Comparing `pinecone_text-0.4.1/PKG-INFO` & `pinecone_text-0.4.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: pinecone-text
-Version: 0.4.1
+Version: 0.4.2
 Summary: Text utilities library by Pinecone.io
 Author: Pinecone.io
-Requires-Python: >=3.8,<3.11
+Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: mmh3 (>=3.1.0,<4.0.0)
 Requires-Dist: nltk (>=3.6.5,<4.0.0)
 Requires-Dist: sentence-transformers (>=2.0.0,<3.0.0)
 Requires-Dist: torch (>=1.13.1,<2.0.0)
 Requires-Dist: transformers (>=4.26.1,<5.0.0)
 Requires-Dist: wget (>=3.2,<4.0)
 Description-Content-Type: text/markdown
```

