# Comparing `tmp/gptcache-0.1.7.tar.gz` & `tmp/gptcache-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gptcache-0.1.7.tar", last modified: Mon Apr 10 15:01:21 2023, max compression
+gzip compressed data, was "gptcache-0.1.8.tar", last modified: Tue Apr 11 15:26:01 2023, max compression
```

## Comparing `gptcache-0.1.7.tar` & `gptcache-0.1.8.tar`

### file list

```diff
@@ -1,62 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 15:01:21.880425 gptcache-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (122)     1068 2023-04-10 15:01:12.000000 gptcache-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    16700 2023-04-10 15:01:21.880425 gptcache-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    16162 2023-04-10 15:01:12.000000 gptcache-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 15:01:21.872425 gptcache-0.1.7/gptcache/
--rw-r--r--   0 runner    (1001) docker     (122)     5999 2023-04-10 15:01:12.000000 gptcache-0.1.7/gptcache/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 15:01:21.876425 gptcache-0.1.7/gptcache/adapter/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-10 15:01:12.000000 gptcache-0.1.7/gptcache/adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3957 2023-04-10 15:01:12.000000 gptcache-0.1.7/gptcache/adapter/adapter.py
--rw-r--r--   0 runner    (1001) docker     (122)      670 2023-04-10 15:01:12.000000 gptcache-0.1.7/gptcache/adapter/langchain_llms.py
--rw-r--r--   0 runner    (1001) docker     (122)     2789 2023-04-10 15:01:12.000000 gptcache-0.1.7/gptcache/adapter/openai.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 15:01:21.876425 gptcache-0.1.7/gptcache/embedding/
--rw-r--r--   0 runner    (1001) docker     (122)     1087 2023-04-10 15:01:12.000000 gptcache-0.1.7/gptcache/embedding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      282 2023-04-10 15:01:12.000000 gptcache-0.1.7/gptcache/embedding/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     1768 2023-04-10 15:01:12.000000 gptcache-0.1.7/gptcache/embedding/cohere.py
--rw-r--r--   0 runner    (1001) docker     (122)     1663 2023-04-10 15:01:12.000000 gptcache-0.1.7/gptcache/embedding/fasttext.py
--rw-r--r--   0 runner    (1001) docker     (122)     2561 2023-04-10 15:01:12.000000 gptcache-0.1.7/gptcache/embedding/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (122)     2685 2023-04-10 15:01:12.000000 gptcache-0.1.7/gptcache/embedding/onnx.py
--rw-r--r--   0 runner    (1001) docker     (122)     1893 2023-04-10 15:01:12.000000 gptcache-0.1.7/gptcache/embedding/openai.py
--rw-r--r--   0 runner    (1001) docker     (122)     1542 2023-04-10 15:01:12.000000 gptcache-0.1.7/gptcache/embedding/sbert.py
--rw-r--r--   0 runner    (1001) docker     (122)       46 2023-04-10 15:01:12.000000 gptcache-0.1.7/gptcache/embedding/string.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 15:01:21.876425 gptcache-0.1.7/gptcache/manager/
--rw-r--r--   0 runner    (1001) docker     (122)      157 2023-04-10 15:01:12.000000 gptcache-0.1.7/gptcache/manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5132 2023-04-10 15:01:12.000000 gptcache-0.1.7/gptcache/manager/data_manager.py
--rw-r--r--   0 runner    (1001) docker     (122)     1685 2023-04-10 15:01:12.000000 gptcache-0.1.7/gptcache/manager/eviction.py
--rw-r--r--   0 runner    (1001) docker     (122)     2332 2023-04-10 15:01:12.000000 gptcache-0.1.7/gptcache/manager/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 15:01:21.876425 gptcache-0.1.7/gptcache/manager/scalar_data/
--rw-r--r--   0 runner    (1001) docker     (122)     1607 2023-04-10 15:01:12.000000 gptcache-0.1.7/gptcache/manager/scalar_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      919 2023-04-10 15:01:12.000000 gptcache-0.1.7/gptcache/manager/scalar_data/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     1459 2023-04-10 15:01:12.000000 gptcache-0.1.7/gptcache/manager/scalar_data/manager.py
--rw-r--r--   0 runner    (1001) docker     (122)     5200 2023-04-10 15:01:12.000000 gptcache-0.1.7/gptcache/manager/scalar_data/sqlalchemy.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 15:01:21.876425 gptcache-0.1.7/gptcache/manager/vector_data/
--rw-r--r--   0 runner    (1001) docker     (122)     1479 2023-04-10 15:01:12.000000 gptcache-0.1.7/gptcache/manager/vector_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      601 2023-04-10 15:01:12.000000 gptcache-0.1.7/gptcache/manager/vector_data/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     1598 2023-04-10 15:01:12.000000 gptcache-0.1.7/gptcache/manager/vector_data/chroma.py
--rw-r--r--   0 runner    (1001) docker     (122)     1775 2023-04-10 15:01:12.000000 gptcache-0.1.7/gptcache/manager/vector_data/faiss.py
--rw-r--r--   0 runner    (1001) docker     (122)     3100 2023-04-10 15:01:12.000000 gptcache-0.1.7/gptcache/manager/vector_data/manager.py
--rw-r--r--   0 runner    (1001) docker     (122)     4936 2023-04-10 15:01:12.000000 gptcache-0.1.7/gptcache/manager/vector_data/milvus.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 15:01:21.876425 gptcache-0.1.7/gptcache/processor/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-10 15:01:12.000000 gptcache-0.1.7/gptcache/processor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      162 2023-04-10 15:01:12.000000 gptcache-0.1.7/gptcache/processor/post.py
--rw-r--r--   0 runner    (1001) docker     (122)      434 2023-04-10 15:01:12.000000 gptcache-0.1.7/gptcache/processor/pre.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 15:01:21.880425 gptcache-0.1.7/gptcache/similarity_evaluation/
--rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-04-10 15:01:12.000000 gptcache-0.1.7/gptcache/similarity_evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1796 2023-04-10 15:01:12.000000 gptcache-0.1.7/gptcache/similarity_evaluation/distance.py
--rw-r--r--   0 runner    (1001) docker     (122)     1347 2023-04-10 15:01:12.000000 gptcache-0.1.7/gptcache/similarity_evaluation/exact_match.py
--rw-r--r--   0 runner    (1001) docker     (122)     2200 2023-04-10 15:01:12.000000 gptcache-0.1.7/gptcache/similarity_evaluation/np.py
--rw-r--r--   0 runner    (1001) docker     (122)     4633 2023-04-10 15:01:12.000000 gptcache-0.1.7/gptcache/similarity_evaluation/onnx.py
--rw-r--r--   0 runner    (1001) docker     (122)      349 2023-04-10 15:01:12.000000 gptcache-0.1.7/gptcache/similarity_evaluation/similarity_evaluation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 15:01:21.880425 gptcache-0.1.7/gptcache/utils/
--rw-r--r--   0 runner    (1001) docker     (122)     2001 2023-04-10 15:01:12.000000 gptcache-0.1.7/gptcache/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      536 2023-04-10 15:01:12.000000 gptcache-0.1.7/gptcache/utils/dependency_control.py
--rw-r--r--   0 runner    (1001) docker     (122)      552 2023-04-10 15:01:12.000000 gptcache-0.1.7/gptcache/utils/error.py
--rw-r--r--   0 runner    (1001) docker     (122)      708 2023-04-10 15:01:12.000000 gptcache-0.1.7/gptcache/utils/lazy_import.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 15:01:21.872425 gptcache-0.1.7/gptcache.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    16700 2023-04-10 15:01:21.000000 gptcache-0.1.7/gptcache.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1570 2023-04-10 15:01:21.000000 gptcache-0.1.7/gptcache.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-10 15:01:21.000000 gptcache-0.1.7/gptcache.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       24 2023-04-10 15:01:21.000000 gptcache-0.1.7/gptcache.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-04-10 15:01:21.000000 gptcache-0.1.7/gptcache.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-10 15:01:21.880425 gptcache-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1108 2023-04-10 15:01:12.000000 gptcache-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 15:26:01.326631 gptcache-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (122)     1068 2023-04-11 15:25:50.000000 gptcache-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    16700 2023-04-11 15:26:01.326631 gptcache-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    16162 2023-04-11 15:25:50.000000 gptcache-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 15:26:01.318631 gptcache-0.1.8/gptcache/
+-rw-r--r--   0 runner    (1001) docker     (122)     6022 2023-04-11 15:25:50.000000 gptcache-0.1.8/gptcache/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 15:26:01.318631 gptcache-0.1.8/gptcache/adapter/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 15:25:50.000000 gptcache-0.1.8/gptcache/adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3957 2023-04-11 15:25:50.000000 gptcache-0.1.8/gptcache/adapter/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1605 2023-04-11 15:25:50.000000 gptcache-0.1.8/gptcache/adapter/langchain_llms.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2789 2023-04-11 15:25:50.000000 gptcache-0.1.8/gptcache/adapter/openai.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 15:26:01.322631 gptcache-0.1.8/gptcache/embedding/
+-rw-r--r--   0 runner    (1001) docker     (122)     1087 2023-04-11 15:25:50.000000 gptcache-0.1.8/gptcache/embedding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      282 2023-04-11 15:25:50.000000 gptcache-0.1.8/gptcache/embedding/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1768 2023-04-11 15:25:50.000000 gptcache-0.1.8/gptcache/embedding/cohere.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1663 2023-04-11 15:25:50.000000 gptcache-0.1.8/gptcache/embedding/fasttext.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2561 2023-04-11 15:25:50.000000 gptcache-0.1.8/gptcache/embedding/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2685 2023-04-11 15:25:50.000000 gptcache-0.1.8/gptcache/embedding/onnx.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1893 2023-04-11 15:25:50.000000 gptcache-0.1.8/gptcache/embedding/openai.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1542 2023-04-11 15:25:50.000000 gptcache-0.1.8/gptcache/embedding/sbert.py
+-rw-r--r--   0 runner    (1001) docker     (122)       46 2023-04-11 15:25:50.000000 gptcache-0.1.8/gptcache/embedding/string.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 15:26:01.322631 gptcache-0.1.8/gptcache/manager/
+-rw-r--r--   0 runner    (1001) docker     (122)      157 2023-04-11 15:25:50.000000 gptcache-0.1.8/gptcache/manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5132 2023-04-11 15:25:50.000000 gptcache-0.1.8/gptcache/manager/data_manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1685 2023-04-11 15:25:50.000000 gptcache-0.1.8/gptcache/manager/eviction.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2332 2023-04-11 15:25:50.000000 gptcache-0.1.8/gptcache/manager/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 15:26:01.322631 gptcache-0.1.8/gptcache/manager/scalar_data/
+-rw-r--r--   0 runner    (1001) docker     (122)     1607 2023-04-11 15:25:50.000000 gptcache-0.1.8/gptcache/manager/scalar_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      919 2023-04-11 15:25:50.000000 gptcache-0.1.8/gptcache/manager/scalar_data/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1459 2023-04-11 15:25:50.000000 gptcache-0.1.8/gptcache/manager/scalar_data/manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5200 2023-04-11 15:25:50.000000 gptcache-0.1.8/gptcache/manager/scalar_data/sqlalchemy.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 15:26:01.322631 gptcache-0.1.8/gptcache/manager/vector_data/
+-rw-r--r--   0 runner    (1001) docker     (122)     1686 2023-04-11 15:25:50.000000 gptcache-0.1.8/gptcache/manager/vector_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      601 2023-04-11 15:25:50.000000 gptcache-0.1.8/gptcache/manager/vector_data/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1598 2023-04-11 15:25:50.000000 gptcache-0.1.8/gptcache/manager/vector_data/chroma.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1775 2023-04-11 15:25:50.000000 gptcache-0.1.8/gptcache/manager/vector_data/faiss.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1857 2023-04-11 15:25:50.000000 gptcache-0.1.8/gptcache/manager/vector_data/hnswlib_store.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3621 2023-04-11 15:25:50.000000 gptcache-0.1.8/gptcache/manager/vector_data/manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4936 2023-04-11 15:25:50.000000 gptcache-0.1.8/gptcache/manager/vector_data/milvus.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 15:26:01.322631 gptcache-0.1.8/gptcache/processor/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 15:25:50.000000 gptcache-0.1.8/gptcache/processor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      188 2023-04-11 15:25:50.000000 gptcache-0.1.8/gptcache/processor/post.py
+-rw-r--r--   0 runner    (1001) docker     (122)      621 2023-04-11 15:25:50.000000 gptcache-0.1.8/gptcache/processor/pre.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 15:26:01.322631 gptcache-0.1.8/gptcache/similarity_evaluation/
+-rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-04-11 15:25:50.000000 gptcache-0.1.8/gptcache/similarity_evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1796 2023-04-11 15:25:50.000000 gptcache-0.1.8/gptcache/similarity_evaluation/distance.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1347 2023-04-11 15:25:50.000000 gptcache-0.1.8/gptcache/similarity_evaluation/exact_match.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2200 2023-04-11 15:25:50.000000 gptcache-0.1.8/gptcache/similarity_evaluation/np.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4633 2023-04-11 15:25:50.000000 gptcache-0.1.8/gptcache/similarity_evaluation/onnx.py
+-rw-r--r--   0 runner    (1001) docker     (122)      349 2023-04-11 15:25:50.000000 gptcache-0.1.8/gptcache/similarity_evaluation/similarity_evaluation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 15:26:01.326631 gptcache-0.1.8/gptcache/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)     2184 2023-04-11 15:25:50.000000 gptcache-0.1.8/gptcache/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      582 2023-04-11 15:25:50.000000 gptcache-0.1.8/gptcache/utils/dependency_control.py
+-rw-r--r--   0 runner    (1001) docker     (122)      736 2023-04-11 15:25:50.000000 gptcache-0.1.8/gptcache/utils/error.py
+-rw-r--r--   0 runner    (1001) docker     (122)      708 2023-04-11 15:25:50.000000 gptcache-0.1.8/gptcache/utils/lazy_import.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 15:26:01.318631 gptcache-0.1.8/gptcache.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    16700 2023-04-11 15:26:01.000000 gptcache-0.1.8/gptcache.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1616 2023-04-11 15:26:01.000000 gptcache-0.1.8/gptcache.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-11 15:26:01.000000 gptcache-0.1.8/gptcache.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       24 2023-04-11 15:26:01.000000 gptcache-0.1.8/gptcache.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-04-11 15:26:01.000000 gptcache-0.1.8/gptcache.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-11 15:26:01.326631 gptcache-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1108 2023-04-11 15:25:50.000000 gptcache-0.1.8/setup.py
```

### Comparing `gptcache-0.1.7/LICENSE` & `gptcache-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `gptcache-0.1.7/PKG-INFO` & `gptcache-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gptcache
-Version: 0.1.7
+Version: 0.1.8
 Summary: GPT Cache, a powerful caching library that can be used to speed up and lower the cost of chat applications that rely on the LLM service. GPT Cache works as a memcache for AIGC applications, similar to how Redis works for traditional applications.
 Home-page: https://github.com/zilliztech/GPTCache
 Author: SimFG
 Author-email: bang.fu@zilliz.com
 License: https://opensource.org/license/mit/
 Requires-Python: >=3.8.1
 Description-Content-Type: text/markdown
```

### Comparing `gptcache-0.1.7/README.md` & `gptcache-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `gptcache-0.1.7/gptcache/__init__.py` & `gptcache-0.1.8/gptcache/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
     def __init__(
         self,
         log_time_func=None,
         similarity_threshold=0.8,
     ):
         if similarity_threshold < 0 or similarity_threshold > 1:
-            raise CacheError("Invalid the similarity threshold param")
+            raise CacheError("Invalid the similarity threshold param, reasonable range: 0-1")
         self.log_time_func = log_time_func
         self.similarity_threshold = similarity_threshold
 
 
 class Report:
     """Get GPTCache report including time and counts for different operations."""
```

### Comparing `gptcache-0.1.7/gptcache/adapter/adapter.py` & `gptcache-0.1.8/gptcache/adapter/adapter.py`

 * *Files identical despite different names*

### Comparing `gptcache-0.1.7/gptcache/adapter/openai.py` & `gptcache-0.1.8/gptcache/adapter/openai.py`

 * *Files identical despite different names*

### Comparing `gptcache-0.1.7/gptcache/embedding/__init__.py` & `gptcache-0.1.8/gptcache/embedding/__init__.py`

 * *Files identical despite different names*

### Comparing `gptcache-0.1.7/gptcache/embedding/cohere.py` & `gptcache-0.1.8/gptcache/embedding/cohere.py`

 * *Files identical despite different names*

### Comparing `gptcache-0.1.7/gptcache/embedding/fasttext.py` & `gptcache-0.1.8/gptcache/embedding/fasttext.py`

 * *Files identical despite different names*

### Comparing `gptcache-0.1.7/gptcache/embedding/huggingface.py` & `gptcache-0.1.8/gptcache/embedding/huggingface.py`

 * *Files identical despite different names*

### Comparing `gptcache-0.1.7/gptcache/embedding/onnx.py` & `gptcache-0.1.8/gptcache/embedding/onnx.py`

 * *Files identical despite different names*

### Comparing `gptcache-0.1.7/gptcache/embedding/openai.py` & `gptcache-0.1.8/gptcache/embedding/openai.py`

 * *Files identical despite different names*

### Comparing `gptcache-0.1.7/gptcache/embedding/sbert.py` & `gptcache-0.1.8/gptcache/embedding/sbert.py`

 * *Files identical despite different names*

### Comparing `gptcache-0.1.7/gptcache/manager/data_manager.py` & `gptcache-0.1.8/gptcache/manager/data_manager.py`

 * *Files identical despite different names*

### Comparing `gptcache-0.1.7/gptcache/manager/eviction.py` & `gptcache-0.1.8/gptcache/manager/eviction.py`

 * *Files identical despite different names*

### Comparing `gptcache-0.1.7/gptcache/manager/factory.py` & `gptcache-0.1.8/gptcache/manager/factory.py`

 * *Files identical despite different names*

### Comparing `gptcache-0.1.7/gptcache/manager/scalar_data/__init__.py` & `gptcache-0.1.8/gptcache/manager/scalar_data/__init__.py`

 * *Files identical despite different names*

### Comparing `gptcache-0.1.7/gptcache/manager/scalar_data/base.py` & `gptcache-0.1.8/gptcache/manager/scalar_data/base.py`

 * *Files identical despite different names*

### Comparing `gptcache-0.1.7/gptcache/manager/scalar_data/manager.py` & `gptcache-0.1.8/gptcache/manager/scalar_data/manager.py`

 * *Files identical despite different names*

### Comparing `gptcache-0.1.7/gptcache/manager/scalar_data/sqlalchemy.py` & `gptcache-0.1.8/gptcache/manager/scalar_data/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `gptcache-0.1.7/gptcache/manager/vector_data/__init__.py` & `gptcache-0.1.8/gptcache/manager/vector_data/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,9 +30,14 @@
     :param secure: whether it is https with Zilliz Cloud, defaults to False.
     :type secures: bool.
     :param index_params: the index parameters for Milvus, defaults to the HNSW index: {'metric_type': 'L2', 'index_type': 'HNSW', 'params': {'M':
                          8, 'efConstruction': 64}}.
     :type index_params: dict
     :param collection_name: the name of the collection for Milvus vector database, defaults to 'gptcache'.
     :type collection_name: str.
+
+    :param index_path: the path to hnswlib index, defaults to 'hnswlib_index.bin'.
+    :type index_path: str.
+    :param max_elements: max_elements of hnswlib, defaults 100000.
+    :type max_elements: int.
     """
     return vector_manager.VectorBase.get(name, **kwargs)
```

### Comparing `gptcache-0.1.7/gptcache/manager/vector_data/base.py` & `gptcache-0.1.8/gptcache/manager/vector_data/base.py`

 * *Files identical despite different names*

### Comparing `gptcache-0.1.7/gptcache/manager/vector_data/chroma.py` & `gptcache-0.1.8/gptcache/manager/vector_data/chroma.py`

 * *Files identical despite different names*

### Comparing `gptcache-0.1.7/gptcache/manager/vector_data/faiss.py` & `gptcache-0.1.8/gptcache/manager/vector_data/faiss.py`

 * *Files identical despite different names*

### Comparing `gptcache-0.1.7/gptcache/manager/vector_data/manager.py` & `gptcache-0.1.8/gptcache/manager/vector_data/manager.py`

 * *Files 14% similar despite different names*

```diff
@@ -82,10 +82,21 @@
             collection_name = kwargs.get("collection_name", COLLECTION_NAME)
             vector_base = Chromadb(
                 client_settings=client_settings,
                 persist_directory=persist_directory,
                 collection_name=collection_name,
                 top_k=top_k,
             )
+        elif name == "hnswlib":
+            from gptcache.manager.vector_data.hnswlib_store import Hnswlib
+
+            dimension = kwargs.get("dimension", DIMENSION)
+            index_path = kwargs.pop("index_path", "./hnswlib_index.bin")
+            max_elements = kwargs.pop("max_elements", 100000)
+            VectorBase.check_dimension(dimension)
+            vector_base = Hnswlib(
+                index_file_path=index_path, dimension=dimension,
+                top_k=top_k, max_elements=max_elements
+            )
         else:
             raise NotFoundStoreError("vector store", name)
         return vector_base
```

### Comparing `gptcache-0.1.7/gptcache/manager/vector_data/milvus.py` & `gptcache-0.1.8/gptcache/manager/vector_data/milvus.py`

 * *Files identical despite different names*

### Comparing `gptcache-0.1.7/gptcache/similarity_evaluation/__init__.py` & `gptcache-0.1.8/gptcache/similarity_evaluation/__init__.py`

 * *Files identical despite different names*

### Comparing `gptcache-0.1.7/gptcache/similarity_evaluation/distance.py` & `gptcache-0.1.8/gptcache/similarity_evaluation/distance.py`

 * *Files identical despite different names*

### Comparing `gptcache-0.1.7/gptcache/similarity_evaluation/exact_match.py` & `gptcache-0.1.8/gptcache/similarity_evaluation/exact_match.py`

 * *Files identical despite different names*

### Comparing `gptcache-0.1.7/gptcache/similarity_evaluation/np.py` & `gptcache-0.1.8/gptcache/similarity_evaluation/np.py`

 * *Files identical despite different names*

### Comparing `gptcache-0.1.7/gptcache/similarity_evaluation/onnx.py` & `gptcache-0.1.8/gptcache/similarity_evaluation/onnx.py`

 * *Files identical despite different names*

### Comparing `gptcache-0.1.7/gptcache/utils/__init__.py` & `gptcache-0.1.8/gptcache/utils/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 __all__ = [
     "import_pymilvus",
     "import_huggingface_hub",
     "import_faiss",
+    "import_hnswlib",
     "import_chromadb",
     "import_sqlalchemy",
     "import_sql_client",
     "import_huggingface",
     "import_torch",
     "import_sbert",
     "import_onnxruntime",
@@ -58,15 +59,19 @@
 
 
 def import_onnxruntime():
     _check_library("onnxruntime")
 
 
 def import_faiss():
-    _check_library("faiss", package="faiss-cpu==1.6.5")
+    _check_library("faiss", package="faiss-cpu")
+
+
+def import_hnswlib():
+    _check_library("hnswlib")
 
 
 def import_chromadb():
     _check_library("chromadb")
 
 
 def import_sqlalchemy():
@@ -97,7 +102,15 @@
         import_postgresql()
     elif db_name in ["mysql", "mariadb"]:
         import_pymysql()
     elif db_name == "sqlserver":
         import_pyodbc()
     elif db_name == "oracle":
         import_cxoracle()
+
+
+def import_pydantic():
+    _check_library("pydantic")
+
+
+def import_langchain():
+    _check_library("langchain")
```

### Comparing `gptcache-0.1.7/gptcache/utils/dependency_control.py` & `gptcache-0.1.8/gptcache/utils/dependency_control.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import subprocess
 
+from gptcache.utils.error import PipInstallError
+
 
 def prompt_install(package: str, warn: bool = False):  # pragma: no cover
     """
     Function used to prompt user to install a package.
     """
     cmd = f"pip install {package}"
     try:
         if warn and input(f"Install {package}? Y/n: ") != "Y":
             raise ModuleNotFoundError(f"No module named {package}")
         subprocess.check_call(cmd, shell=True)
         print(f"{package} installed successfully!")
-    except subprocess.CalledProcessError:
-        print(f"Ran into error installing {package}.")
+    except subprocess.CalledProcessError as e:
+        raise PipInstallError(package) from e
```

### Comparing `gptcache-0.1.7/gptcache/utils/lazy_import.py` & `gptcache-0.1.8/gptcache/utils/lazy_import.py`

 * *Files identical despite different names*

### Comparing `gptcache-0.1.7/gptcache.egg-info/PKG-INFO` & `gptcache-0.1.8/gptcache.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gptcache
-Version: 0.1.7
+Version: 0.1.8
 Summary: GPT Cache, a powerful caching library that can be used to speed up and lower the cost of chat applications that rely on the LLM service. GPT Cache works as a memcache for AIGC applications, similar to how Redis works for traditional applications.
 Home-page: https://github.com/zilliztech/GPTCache
 Author: SimFG
 Author-email: bang.fu@zilliz.com
 License: https://opensource.org/license/mit/
 Requires-Python: >=3.8.1
 Description-Content-Type: text/markdown
```

### Comparing `gptcache-0.1.7/gptcache.egg-info/SOURCES.txt` & `gptcache-0.1.8/gptcache.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 gptcache/manager/scalar_data/base.py
 gptcache/manager/scalar_data/manager.py
 gptcache/manager/scalar_data/sqlalchemy.py
 gptcache/manager/vector_data/__init__.py
 gptcache/manager/vector_data/base.py
 gptcache/manager/vector_data/chroma.py
 gptcache/manager/vector_data/faiss.py
+gptcache/manager/vector_data/hnswlib_store.py
 gptcache/manager/vector_data/manager.py
 gptcache/manager/vector_data/milvus.py
 gptcache/processor/__init__.py
 gptcache/processor/post.py
 gptcache/processor/pre.py
 gptcache/similarity_evaluation/__init__.py
 gptcache/similarity_evaluation/distance.py
```

### Comparing `gptcache-0.1.7/setup.py` & `gptcache-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
             if require.strip() and not require.startswith('#')
         ]
 
 
 setuptools.setup(
     name="gptcache",
     packages=find_packages(),
-    version="0.1.7",
+    version="0.1.8",
     author="SimFG",
     author_email="bang.fu@zilliz.com",
     description="GPT Cache, a powerful caching library that can be used to speed up and lower the cost of chat "
                 "applications that rely on the LLM service. GPT Cache works as a memcache for AIGC applications, "
                 "similar to how Redis works for traditional applications.",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

