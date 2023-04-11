# Comparing `tmp/autoresearcher-0.0.2.tar.gz` & `tmp/autoresearcher-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoresearcher-0.0.2.tar", last modified: Tue Apr 11 03:48:40 2023, max compression
+gzip compressed data, was "autoresearcher-0.0.4.tar", last modified: Tue Apr 11 03:31:22 2023, max compression
```

## Comparing `autoresearcher-0.0.2.tar` & `autoresearcher-0.0.4.tar`

### file list

```diff
@@ -1,33 +1,30 @@
-drwxr-xr-x   0 marapelzer   (501) staff       (20)        0 2023-04-11 03:48:40.407389 autoresearcher-0.0.2/
--rw-r--r--   0 marapelzer   (501) staff       (20)     1070 2023-04-11 00:23:06.000000 autoresearcher-0.0.2/LICENSE
--rw-r--r--   0 marapelzer   (501) staff       (20)     2970 2023-04-11 03:48:40.407015 autoresearcher-0.0.2/PKG-INFO
--rw-r--r--   0 marapelzer   (501) staff       (20)     2518 2023-04-11 03:30:54.000000 autoresearcher-0.0.2/README.md
-drwxr-xr-x   0 marapelzer   (501) staff       (20)        0 2023-04-11 03:48:40.391245 autoresearcher-0.0.2/autoresearcher/
--rw-r--r--   0 marapelzer   (501) staff       (20)       77 2023-04-11 00:38:30.000000 autoresearcher-0.0.2/autoresearcher/__init__.py
-drwxr-xr-x   0 marapelzer   (501) staff       (20)        0 2023-04-11 03:48:40.396995 autoresearcher-0.0.2/autoresearcher/data_sources/
--rw-r--r--   0 marapelzer   (501) staff       (20)        0 2023-04-10 23:32:56.000000 autoresearcher-0.0.2/autoresearcher/data_sources/__init__.py
-drwxr-xr-x   0 marapelzer   (501) staff       (20)        0 2023-04-11 03:48:40.399201 autoresearcher-0.0.2/autoresearcher/data_sources/web_apis/
--rw-r--r--   0 marapelzer   (501) staff       (20)        0 2023-04-10 23:32:56.000000 autoresearcher-0.0.2/autoresearcher/data_sources/web_apis/__init__.py
--rw-r--r--   0 marapelzer   (501) staff       (20)      585 2023-04-10 23:32:56.000000 autoresearcher-0.0.2/autoresearcher/data_sources/web_apis/base_web_api_data_loader.py
--rw-r--r--   0 marapelzer   (501) staff       (20)     1627 2023-04-11 03:46:36.000000 autoresearcher-0.0.2/autoresearcher/data_sources/web_apis/semantic_scholar_loader.py
-drwxr-xr-x   0 marapelzer   (501) staff       (20)        0 2023-04-11 03:48:40.400928 autoresearcher-0.0.2/autoresearcher/llms/
--rw-r--r--   0 marapelzer   (501) staff       (20)        0 2023-04-11 03:38:21.000000 autoresearcher-0.0.2/autoresearcher/llms/__init__.py
--rw-r--r--   0 marapelzer   (501) staff       (20)     1204 2023-04-10 23:32:56.000000 autoresearcher-0.0.2/autoresearcher/llms/openai.py
-drwxr-xr-x   0 marapelzer   (501) staff       (20)        0 2023-04-11 03:48:40.404773 autoresearcher-0.0.2/autoresearcher/utils/
--rw-r--r--   0 marapelzer   (501) staff       (20)        0 2023-04-10 23:32:56.000000 autoresearcher-0.0.2/autoresearcher/utils/__init__.py
--rw-r--r--   0 marapelzer   (501) staff       (20)      366 2023-04-10 23:32:56.000000 autoresearcher-0.0.2/autoresearcher/utils/get_citations.py
--rw-r--r--   0 marapelzer   (501) staff       (20)     1632 2023-04-11 01:04:12.000000 autoresearcher-0.0.2/autoresearcher/utils/prompts.py
-drwxr-xr-x   0 marapelzer   (501) staff       (20)        0 2023-04-11 03:48:40.405301 autoresearcher-0.0.2/autoresearcher/workflows/
--rw-r--r--   0 marapelzer   (501) staff       (20)        0 2023-04-11 02:08:49.000000 autoresearcher-0.0.2/autoresearcher/workflows/__init__.py
-drwxr-xr-x   0 marapelzer   (501) staff       (20)        0 2023-04-11 03:48:40.405802 autoresearcher-0.0.2/autoresearcher/workflows/literature_review/
--rw-r--r--   0 marapelzer   (501) staff       (20)        0 2023-04-10 23:32:56.000000 autoresearcher-0.0.2/autoresearcher/workflows/literature_review/__init__.py
--rw-r--r--   0 marapelzer   (501) staff       (20)     5262 2023-04-10 23:32:56.000000 autoresearcher-0.0.2/autoresearcher/workflows/literature_review/literature_review.py
-drwxr-xr-x   0 marapelzer   (501) staff       (20)        0 2023-04-11 03:48:40.396653 autoresearcher-0.0.2/autoresearcher.egg-info/
--rw-r--r--   0 marapelzer   (501) staff       (20)     2970 2023-04-11 03:48:40.000000 autoresearcher-0.0.2/autoresearcher.egg-info/PKG-INFO
--rw-r--r--   0 marapelzer   (501) staff       (20)      796 2023-04-11 03:48:40.000000 autoresearcher-0.0.2/autoresearcher.egg-info/SOURCES.txt
--rw-r--r--   0 marapelzer   (501) staff       (20)        1 2023-04-11 03:48:40.000000 autoresearcher-0.0.2/autoresearcher.egg-info/dependency_links.txt
--rw-r--r--   0 marapelzer   (501) staff       (20)      109 2023-04-11 03:48:40.000000 autoresearcher-0.0.2/autoresearcher.egg-info/requires.txt
--rw-r--r--   0 marapelzer   (501) staff       (20)       15 2023-04-11 03:48:40.000000 autoresearcher-0.0.2/autoresearcher.egg-info/top_level.txt
--rw-r--r--   0 marapelzer   (501) staff       (20)      103 2023-04-11 00:17:53.000000 autoresearcher-0.0.2/pyproject.toml
--rw-r--r--   0 marapelzer   (501) staff       (20)       38 2023-04-11 03:48:40.407500 autoresearcher-0.0.2/setup.cfg
--rw-r--r--   0 marapelzer   (501) staff       (20)      935 2023-04-11 03:34:23.000000 autoresearcher-0.0.2/setup.py
+drwxr-xr-x   0 marapelzer   (501) staff       (20)        0 2023-04-11 03:31:22.797149 autoresearcher-0.0.4/
+-rw-r--r--   0 marapelzer   (501) staff       (20)     1070 2023-04-11 00:23:06.000000 autoresearcher-0.0.4/LICENSE
+-rw-r--r--   0 marapelzer   (501) staff       (20)     2970 2023-04-11 03:31:22.796484 autoresearcher-0.0.4/PKG-INFO
+-rw-r--r--   0 marapelzer   (501) staff       (20)     2518 2023-04-11 03:30:54.000000 autoresearcher-0.0.4/README.md
+drwxr-xr-x   0 marapelzer   (501) staff       (20)        0 2023-04-11 03:31:22.789309 autoresearcher-0.0.4/autoresearcher/
+-rw-r--r--   0 marapelzer   (501) staff       (20)       77 2023-04-11 00:38:30.000000 autoresearcher-0.0.4/autoresearcher/__init__.py
+drwxr-xr-x   0 marapelzer   (501) staff       (20)        0 2023-04-11 03:31:22.791559 autoresearcher-0.0.4/autoresearcher/data_sources/
+-rw-r--r--   0 marapelzer   (501) staff       (20)        0 2023-04-10 23:32:56.000000 autoresearcher-0.0.4/autoresearcher/data_sources/__init__.py
+drwxr-xr-x   0 marapelzer   (501) staff       (20)        0 2023-04-11 03:31:22.792911 autoresearcher-0.0.4/autoresearcher/data_sources/web_apis/
+-rw-r--r--   0 marapelzer   (501) staff       (20)        0 2023-04-10 23:32:56.000000 autoresearcher-0.0.4/autoresearcher/data_sources/web_apis/__init__.py
+-rw-r--r--   0 marapelzer   (501) staff       (20)      585 2023-04-10 23:32:56.000000 autoresearcher-0.0.4/autoresearcher/data_sources/web_apis/base_web_api_data_loader.py
+-rw-r--r--   0 marapelzer   (501) staff       (20)     1813 2023-04-11 01:34:10.000000 autoresearcher-0.0.4/autoresearcher/data_sources/web_apis/semantic_scholar_loader.py
+drwxr-xr-x   0 marapelzer   (501) staff       (20)        0 2023-04-11 03:31:22.794117 autoresearcher-0.0.4/autoresearcher/utils/
+-rw-r--r--   0 marapelzer   (501) staff       (20)        0 2023-04-10 23:32:56.000000 autoresearcher-0.0.4/autoresearcher/utils/__init__.py
+-rw-r--r--   0 marapelzer   (501) staff       (20)      366 2023-04-10 23:32:56.000000 autoresearcher-0.0.4/autoresearcher/utils/get_citations.py
+-rw-r--r--   0 marapelzer   (501) staff       (20)     1632 2023-04-11 01:04:12.000000 autoresearcher-0.0.4/autoresearcher/utils/prompts.py
+drwxr-xr-x   0 marapelzer   (501) staff       (20)        0 2023-04-11 03:31:22.795088 autoresearcher-0.0.4/autoresearcher/workflows/
+-rw-r--r--   0 marapelzer   (501) staff       (20)        0 2023-04-11 02:08:49.000000 autoresearcher-0.0.4/autoresearcher/workflows/__init__.py
+drwxr-xr-x   0 marapelzer   (501) staff       (20)        0 2023-04-11 03:31:22.795546 autoresearcher-0.0.4/autoresearcher/workflows/literature_review/
+-rw-r--r--   0 marapelzer   (501) staff       (20)        0 2023-04-10 23:32:56.000000 autoresearcher-0.0.4/autoresearcher/workflows/literature_review/__init__.py
+-rw-r--r--   0 marapelzer   (501) staff       (20)     5262 2023-04-10 23:32:56.000000 autoresearcher-0.0.4/autoresearcher/workflows/literature_review/literature_review.py
+drwxr-xr-x   0 marapelzer   (501) staff       (20)        0 2023-04-11 03:31:22.791278 autoresearcher-0.0.4/autoresearcher.egg-info/
+-rw-r--r--   0 marapelzer   (501) staff       (20)     2970 2023-04-11 03:31:22.000000 autoresearcher-0.0.4/autoresearcher.egg-info/PKG-INFO
+-rw-r--r--   0 marapelzer   (501) staff       (20)      734 2023-04-11 03:31:22.000000 autoresearcher-0.0.4/autoresearcher.egg-info/SOURCES.txt
+-rw-r--r--   0 marapelzer   (501) staff       (20)        1 2023-04-11 03:31:22.000000 autoresearcher-0.0.4/autoresearcher.egg-info/dependency_links.txt
+-rw-r--r--   0 marapelzer   (501) staff       (20)      109 2023-04-11 03:31:22.000000 autoresearcher-0.0.4/autoresearcher.egg-info/requires.txt
+-rw-r--r--   0 marapelzer   (501) staff       (20)       15 2023-04-11 03:31:22.000000 autoresearcher-0.0.4/autoresearcher.egg-info/top_level.txt
+-rw-r--r--   0 marapelzer   (501) staff       (20)      103 2023-04-11 00:17:53.000000 autoresearcher-0.0.4/pyproject.toml
+-rw-r--r--   0 marapelzer   (501) staff       (20)       38 2023-04-11 03:31:22.797276 autoresearcher-0.0.4/setup.cfg
+-rw-r--r--   0 marapelzer   (501) staff       (20)      935 2023-04-11 03:31:12.000000 autoresearcher-0.0.4/setup.py
```

### Comparing `autoresearcher-0.0.2/LICENSE` & `autoresearcher-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `autoresearcher-0.0.2/PKG-INFO` & `autoresearcher-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoresearcher
-Version: 0.0.2
+Version: 0.0.4
 Summary: Automating scientic workflows with AI
 Home-page: https://github.com/eimenhmdt/autoresearcher
 Author: Eimen Hamedat
 Author-email: eimen.hamedat@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `autoresearcher-0.0.2/README.md` & `autoresearcher-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `autoresearcher-0.0.2/autoresearcher/data_sources/web_apis/base_web_api_data_loader.py` & `autoresearcher-0.0.4/autoresearcher/data_sources/web_apis/base_web_api_data_loader.py`

 * *Files identical despite different names*

### Comparing `autoresearcher-0.0.2/autoresearcher/data_sources/web_apis/semantic_scholar_loader.py` & `autoresearcher-0.0.4/autoresearcher/data_sources/web_apis/semantic_scholar_loader.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,10 +31,14 @@
         for paper in papers:
             similarity = jellyfish.jaro_similarity(search_query, paper['title'])
             normalized_citation_count = paper['citationCount'] / max_citations
             paper['combined_score'] = (weight_similarity * similarity) + ((1 - weight_similarity) * normalized_citation_count)
 
         sorted_papers = sorted(papers, key=lambda x: x['combined_score'], reverse=True)
 
+        print("Top 20 papers:") 
+        for paper in sorted_papers[:top_n]:
+            print(paper['citationCount'], paper['title'], f"Combined Score: {paper['combined_score']:.2f}")
+
         return sorted_papers[:top_n]
```

### Comparing `autoresearcher-0.0.2/autoresearcher/utils/prompts.py` & `autoresearcher-0.0.4/autoresearcher/utils/prompts.py`

 * *Files identical despite different names*

### Comparing `autoresearcher-0.0.2/autoresearcher/workflows/literature_review/literature_review.py` & `autoresearcher-0.0.4/autoresearcher/workflows/literature_review/literature_review.py`

 * *Files identical despite different names*

### Comparing `autoresearcher-0.0.2/autoresearcher.egg-info/PKG-INFO` & `autoresearcher-0.0.4/autoresearcher.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoresearcher
-Version: 0.0.2
+Version: 0.0.4
 Summary: Automating scientic workflows with AI
 Home-page: https://github.com/eimenhmdt/autoresearcher
 Author: Eimen Hamedat
 Author-email: eimen.hamedat@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `autoresearcher-0.0.2/autoresearcher.egg-info/SOURCES.txt` & `autoresearcher-0.0.4/autoresearcher.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,13 @@
 autoresearcher.egg-info/dependency_links.txt
 autoresearcher.egg-info/requires.txt
 autoresearcher.egg-info/top_level.txt
 autoresearcher/data_sources/__init__.py
 autoresearcher/data_sources/web_apis/__init__.py
 autoresearcher/data_sources/web_apis/base_web_api_data_loader.py
 autoresearcher/data_sources/web_apis/semantic_scholar_loader.py
-autoresearcher/llms/__init__.py
-autoresearcher/llms/openai.py
 autoresearcher/utils/__init__.py
 autoresearcher/utils/get_citations.py
 autoresearcher/utils/prompts.py
 autoresearcher/workflows/__init__.py
 autoresearcher/workflows/literature_review/__init__.py
 autoresearcher/workflows/literature_review/literature_review.py
```

### Comparing `autoresearcher-0.0.2/setup.py` & `autoresearcher-0.0.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="autoresearcher",
-    version="0.0.2",
+    version="0.0.4",
     author="Eimen Hamedat",
     author_email="eimen.hamedat@gmail.com",
     description="Automating scientic workflows with AI",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/eimenhmdt/autoresearcher",
     classifiers=[
```

