# Comparing `tmp/embedding_explorer-0.1.1.tar.gz` & `tmp/embedding_explorer-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embedding_explorer-0.1.1.tar", max compression
+gzip compressed data, was "embedding_explorer-0.1.2.tar", max compression
```

## Comparing `embedding_explorer-0.1.1.tar` & `embedding_explorer-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1095 2023-03-13 11:52:25.053838 embedding_explorer-0.1.1/LICENSE
--rw-r--r--   0        0        0       95 2023-03-13 11:52:25.057838 embedding_explorer-0.1.1/README.md
--rw-r--r--   0        0        0      142 2023-03-27 13:50:12.710655 embedding_explorer-0.1.1/embedding_explorer/__init__.py
--rw-r--r--   0        0        0     3930 2023-03-27 13:59:02.583495 embedding_explorer-0.1.1/embedding_explorer/app.py
--rw-r--r--   0        0        0    16170 2023-03-21 14:13:23.726074 embedding_explorer-0.1.1/embedding_explorer/assets/favicon.ico
--rw-r--r--   0        0        0     2128 2023-03-27 13:51:30.306787 embedding_explorer-0.1.1/embedding_explorer/blueprints/dashboard.py
--rw-r--r--   0        0        0     3189 2023-03-27 13:44:45.950000 embedding_explorer-0.1.1/embedding_explorer/blueprints/explorer.py
--rw-r--r--   0        0        0     2277 2023-03-27 13:27:51.091877 embedding_explorer-0.1.1/embedding_explorer/components/model_card.py
--rw-r--r--   0        0        0     2000 2023-03-27 13:28:01.367900 embedding_explorer-0.1.1/embedding_explorer/components/network.py
--rw-r--r--   0        0        0     1106 2023-03-17 13:45:00.203784 embedding_explorer-0.1.1/embedding_explorer/components/slider.py
--rw-r--r--   0        0        0     2343 2023-03-27 13:27:41.987856 embedding_explorer-0.1.1/embedding_explorer/components/word_selector.py
--rw-r--r--   0        0        0      853 2023-03-27 13:36:18.356965 embedding_explorer-0.1.1/embedding_explorer/model.py
--rw-r--r--   0        0        0     4907 2023-03-20 14:01:46.998402 embedding_explorer-0.1.1/embedding_explorer/plots/network.py
--rw-r--r--   0        0        0     5843 2023-03-27 14:42:08.501085 embedding_explorer-0.1.1/embedding_explorer/prepare/semkern.py
--rw-r--r--   0        0        0     1125 2023-03-27 14:47:02.041747 embedding_explorer-0.1.1/embedding_explorer/prepare/thumbnails.py
--rw-r--r--   0        0        0      725 2023-03-27 13:47:49.818369 embedding_explorer-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1250 1970-01-01 00:00:00.000000 embedding_explorer-0.1.1/setup.py
--rw-r--r--   0        0        0     1165 1970-01-01 00:00:00.000000 embedding_explorer-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1095 2023-03-13 11:52:25.053838 embedding_explorer-0.1.2/LICENSE
+-rw-r--r--   0        0        0       95 2023-03-13 11:52:25.057838 embedding_explorer-0.1.2/README.md
+-rw-r--r--   0        0        0      142 2023-03-27 13:50:12.710655 embedding_explorer-0.1.2/embedding_explorer/__init__.py
+-rw-r--r--   0        0        0     4578 2023-04-11 10:33:13.278666 embedding_explorer-0.1.2/embedding_explorer/app.py
+-rw-r--r--   0        0        0    16170 2023-03-21 14:13:23.726074 embedding_explorer-0.1.2/embedding_explorer/assets/favicon.ico
+-rw-r--r--   0        0        0     2170 2023-04-11 10:30:36.606316 embedding_explorer-0.1.2/embedding_explorer/blueprints/dashboard.py
+-rw-r--r--   0        0        0     3250 2023-04-11 10:30:00.242235 embedding_explorer-0.1.2/embedding_explorer/blueprints/explorer.py
+-rw-r--r--   0        0        0     2277 2023-03-27 13:27:51.091877 embedding_explorer-0.1.2/embedding_explorer/components/model_card.py
+-rw-r--r--   0        0        0     2000 2023-03-27 13:28:01.367900 embedding_explorer-0.1.2/embedding_explorer/components/network.py
+-rw-r--r--   0        0        0     1106 2023-03-17 13:45:00.203784 embedding_explorer-0.1.2/embedding_explorer/components/slider.py
+-rw-r--r--   0        0        0     3239 2023-04-11 10:28:39.678054 embedding_explorer-0.1.2/embedding_explorer/components/word_selector.py
+-rw-r--r--   0        0        0      853 2023-03-27 13:36:18.356965 embedding_explorer-0.1.2/embedding_explorer/model.py
+-rw-r--r--   0        0        0     4907 2023-03-20 14:01:46.998402 embedding_explorer-0.1.2/embedding_explorer/plots/network.py
+-rw-r--r--   0        0        0     5843 2023-03-27 14:42:08.501085 embedding_explorer-0.1.2/embedding_explorer/prepare/semkern.py
+-rw-r--r--   0        0        0     1125 2023-03-27 14:47:02.041747 embedding_explorer-0.1.2/embedding_explorer/prepare/thumbnails.py
+-rw-r--r--   0        0        0      684 2023-04-11 10:36:05.899051 embedding_explorer-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1177 1970-01-01 00:00:00.000000 embedding_explorer-0.1.2/setup.py
+-rw-r--r--   0        0        0     1064 1970-01-01 00:00:00.000000 embedding_explorer-0.1.2/PKG-INFO
```

### Comparing `embedding_explorer-0.1.1/LICENSE` & `embedding_explorer-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `embedding_explorer-0.1.1/embedding_explorer/assets/favicon.ico` & `embedding_explorer-0.1.2/embedding_explorer/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `embedding_explorer-0.1.1/embedding_explorer/blueprints/dashboard.py` & `embedding_explorer-0.1.2/embedding_explorer/blueprints/dashboard.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from dash_extensions.enrich import Dash, DashBlueprint, dash, dcc, html
 
 from embedding_explorer.blueprints.explorer import create_explorer
 from embedding_explorer.components.model_card import create_card
 from embedding_explorer.model import Model
 
 
-def create_dashboard(models: Dict[str, Model]):
+def create_dashboard(models: Dict[str, Model], fuzzy_search: bool = False):
     """Creates dashboard for all embedding models.
 
     Parameters
     ----------
     models: dict of str to Model
         Mapping of names to models.
     """
@@ -23,16 +23,15 @@
 
     # Collecting cards and registering pages
     cards = []
     pages = {}
     for model_name, model in models.items():
         cards.append(create_card(model=model, model_name=model_name))
         page = create_explorer(
-            model=model,
-            model_name=model_name,
+            model=model, model_name=model_name, fuzzy_search=fuzzy_search
         )
         page.register_callbacks(dashboard)
         pages[model_name] = page.layout
 
     dashboard.layout = html.Div(
         children=[
             html.Div(
```

### Comparing `embedding_explorer-0.1.1/embedding_explorer/blueprints/explorer.py` & `embedding_explorer-0.1.2/embedding_explorer/blueprints/explorer.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,18 +4,20 @@
 from dash_extensions.enrich import DashBlueprint, dcc, html
 
 from embedding_explorer.components.network import create_network
 from embedding_explorer.components.word_selector import create_word_selector
 from embedding_explorer.model import Model
 
 
-def create_explorer(model: Model, model_name: str = "") -> DashBlueprint:
+def create_explorer(
+    model: Model, model_name: str = "", fuzzy_search: bool = False
+) -> DashBlueprint:
     # --------[ Collecting blueprints ]--------
     word_selector = create_word_selector(
-        vocab=model.vocab, model_name=model_name
+        vocab=model.vocab, model_name=model_name, fuzzy_search=fuzzy_search
     )
     network = create_network(
         vocab=model.vocab, embeddings=model.embeddings, model_name=model_name
     )
     blueprints = [
         word_selector,
         network,
```

### Comparing `embedding_explorer-0.1.1/embedding_explorer/components/model_card.py` & `embedding_explorer-0.1.2/embedding_explorer/components/model_card.py`

 * *Files identical despite different names*

### Comparing `embedding_explorer-0.1.1/embedding_explorer/components/network.py` & `embedding_explorer-0.1.2/embedding_explorer/components/network.py`

 * *Files identical despite different names*

### Comparing `embedding_explorer-0.1.1/embedding_explorer/components/slider.py` & `embedding_explorer-0.1.2/embedding_explorer/components/slider.py`

 * *Files identical despite different names*

### Comparing `embedding_explorer-0.1.1/embedding_explorer/components/word_selector.py` & `embedding_explorer-0.1.2/embedding_explorer/components/word_selector.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,72 +7,103 @@
     DashBlueprint,
     Input,
     Output,
     State,
     dcc,
     exceptions,
 )
-from thefuzz import process
+from neofuzz import Process
+from sklearn.decomposition import NMF
+from sklearn.feature_extraction.text import TfidfVectorizer
+from sklearn.pipeline import make_pipeline
 from typing_extensions import TypedDict
 
 
 class Option(TypedDict):
     value: int
     label: str
+    search: str
+
+
+class DummyProcess:
+    def query(self, search_terms, limit):
+        return np.array([]), np.array([])
 
 
 def create_word_selector(
-    vocab: np.ndarray, model_name: str = ""
+    vocab: np.ndarray, model_name: str = "", fuzzy_search: bool = False
 ) -> DashBlueprint:
     """Creates word selector component blueprint."""
 
     word_selector = DashBlueprint()
     vocab_lookup = {word: index for index, word in enumerate(vocab)}
-
-    word_selector.layout = dmc.MultiSelect(
-        label="Seeds",
-        description="Select words that are going to be used as"
-        "the basis of semantic association.",
+    if fuzzy_search:
+        print("Indexing vocabulary for fuzzy search")
+        vectorizer = make_pipeline(
+            TfidfVectorizer(
+                analyzer="char", ngram_range=(1, 5), max_features=50_000
+            ),
+            NMF(n_components=10),
+        )
+        fuzzy_process = Process(
+            vectorizer,
+            metric="euclidean",
+            low_memory=True,
+        )
+        fuzzy_process.index(vocab)
+        print("Indexing done")
+    else:
+        fuzzy_process = DummyProcess()
+
+    word_selector.layout = dcc.Dropdown(
+        # label="Seeds",
+        # description="Select words that are going to be used as"
+        # "the basis of semantic association.",
         id=f"{model_name}_word_selector",
         placeholder="Search for words...",
         value=[],
-        data=[],
+        # data=[],
+        options=[],
         searchable=True,
         clearable=True,
-        size="lg",
+        # size="lg",
+        multi=True,
     )
 
     @word_selector.callback(
-        Output(f"{model_name}_word_selector", "data"),
-        Input(f"{model_name}_word_selector", "searchValue"),
+        Output(f"{model_name}_word_selector", "options"),
+        Input(f"{model_name}_word_selector", "search_value"),
         State(f"{model_name}_word_selector", "value"),
     )
     def update_options(
         search_value: str, selected_values: List[int]
     ) -> List[Option]:
         if not search_value:
             raise exceptions.PreventUpdate
         # Collecting already chosen options
         selected_options = [
-            Option(value=index, label=vocab[index])
+            dict(value=index, label=vocab[index], search=search_value)
             for index in selected_values
         ]
         # Lowercasing search value
         search_value = search_value.lower()
         # Trying to find exact match
         if search_value in vocab_lookup:
-            exact_match = Option(
-                value=vocab_lookup[search_value], label=search_value
+            exact_match = dict(
+                value=vocab_lookup[search_value],
+                label=search_value,
+                search=search_value,
             )
             return [exact_match] + selected_options
-        # Trying to fuzzy find 5 closest terms
-        fuzzy_process_result = process.extract(search_value, vocab, limit=5)
-        # Getting only the terms
-        fuzzy_match_terms = [term for term, score in fuzzy_process_result]
+        # Fuzzy finding 5 closest
+        fuzzy_indices, _ = fuzzy_process.query(
+            search_terms=[search_value], limit=5
+        )
+        fuzzy_indices = np.ravel(fuzzy_indices)
         # Collecting options
         fuzzy_matches = [
-            Option(value=vocab_lookup[term], label=term)
-            for term in fuzzy_match_terms
+            dict(value=index, label=vocab[index], search=search_value)
+            for index in fuzzy_indices
         ]
         return fuzzy_matches + selected_options
 
     return word_selector
```

### Comparing `embedding_explorer-0.1.1/embedding_explorer/model.py` & `embedding_explorer-0.1.2/embedding_explorer/model.py`

 * *Files identical despite different names*

### Comparing `embedding_explorer-0.1.1/embedding_explorer/plots/network.py` & `embedding_explorer-0.1.2/embedding_explorer/plots/network.py`

 * *Files identical despite different names*

### Comparing `embedding_explorer-0.1.1/embedding_explorer/prepare/semkern.py` & `embedding_explorer-0.1.2/embedding_explorer/prepare/semkern.py`

 * *Files identical despite different names*

### Comparing `embedding_explorer-0.1.1/embedding_explorer/prepare/thumbnails.py` & `embedding_explorer-0.1.2/embedding_explorer/prepare/thumbnails.py`

 * *Files identical despite different names*

### Comparing `embedding_explorer-0.1.1/pyproject.toml` & `embedding_explorer-0.1.2/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -2,32 +2,30 @@
 line-length=79
 
 [tool.ruff]
 line-length=79
 
 [tool.poetry]
 name = "embedding-explorer"
-version = "0.1.1"
+version = "0.1.2"
 description = "Tools for interactive visual inspection of static word embedding models."
 authors = ["Márton Kardos <power.up1163@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "embedding_explorer"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8.0"
 dash = "~2.7.1"
 dash-extensions = "~0.1.10"
 dash-mantine-components = "~0.11.1"
 dash-iconify = "~0.1.2"
-joblib = "~1.2.0"
-scikit-learn = "~1.2.0"
-numpy = "^1.24.1"
+scikit-learn = "~1.1.0"
+numpy = ">=1.23.0"
 pandas = "~1.5.2"
 wordcloud = "~1.8.2.2"
-thefuzz = "~0.19.0"
-levenshtein = "~0.20.9"
+neofuzz = ">=0.1.2"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `embedding_explorer-0.1.1/setup.py` & `embedding_explorer-0.1.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,25 +12,23 @@
 {'': ['*'], 'embedding_explorer': ['assets/*']}
 
 install_requires = \
 ['dash-extensions>=0.1.10,<0.2.0',
  'dash-iconify>=0.1.2,<0.2.0',
  'dash-mantine-components>=0.11.1,<0.12.0',
  'dash>=2.7.1,<2.8.0',
- 'joblib>=1.2.0,<1.3.0',
- 'levenshtein>=0.20.9,<0.21.0',
- 'numpy>=1.24.1,<2.0.0',
+ 'neofuzz>=0.1.2',
+ 'numpy>=1.23.0',
  'pandas>=1.5.2,<1.6.0',
- 'scikit-learn>=1.2.0,<1.3.0',
- 'thefuzz>=0.19.0,<0.20.0',
+ 'scikit-learn>=1.1.0,<1.2.0',
  'wordcloud>=1.8.2.2,<1.9.0.0']
 
 setup_kwargs = {
     'name': 'embedding-explorer',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': 'Tools for interactive visual inspection of static word embedding models.',
     'long_description': '# embedding-explorer\nTools for interactive visual exploration of static word embedding models.\n',
     'author': 'Márton Kardos',
     'author_email': 'power.up1163@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `embedding_explorer-0.1.1/PKG-INFO` & `embedding_explorer-0.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embedding-explorer
-Version: 0.1.1
+Version: 0.1.2
 Summary: Tools for interactive visual inspection of static word embedding models.
 License: MIT
 Author: Márton Kardos
 Author-email: power.up1163@gmail.com
 Requires-Python: >=3.8.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -12,19 +12,17 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: dash (>=2.7.1,<2.8.0)
 Requires-Dist: dash-extensions (>=0.1.10,<0.2.0)
 Requires-Dist: dash-iconify (>=0.1.2,<0.2.0)
 Requires-Dist: dash-mantine-components (>=0.11.1,<0.12.0)
-Requires-Dist: joblib (>=1.2.0,<1.3.0)
-Requires-Dist: levenshtein (>=0.20.9,<0.21.0)
-Requires-Dist: numpy (>=1.24.1,<2.0.0)
+Requires-Dist: neofuzz (>=0.1.2)
+Requires-Dist: numpy (>=1.23.0)
 Requires-Dist: pandas (>=1.5.2,<1.6.0)
-Requires-Dist: scikit-learn (>=1.2.0,<1.3.0)
-Requires-Dist: thefuzz (>=0.19.0,<0.20.0)
+Requires-Dist: scikit-learn (>=1.1.0,<1.2.0)
 Requires-Dist: wordcloud (>=1.8.2.2,<1.9.0.0)
 Description-Content-Type: text/markdown
 
 # embedding-explorer
 Tools for interactive visual exploration of static word embedding models.
```

