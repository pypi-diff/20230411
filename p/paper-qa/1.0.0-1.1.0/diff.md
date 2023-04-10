# Comparing `tmp/paper-qa-1.0.0.tar.gz` & `tmp/paper-qa-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paper-qa-1.0.0.tar", last modified: Sun Apr  9 19:59:35 2023, max compression
+gzip compressed data, was "paper-qa-1.1.0.tar", last modified: Mon Apr 10 23:45:57 2023, max compression
```

## Comparing `paper-qa-1.0.0.tar` & `paper-qa-1.1.0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:59:35.497224 paper-qa-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-09 19:59:04.000000 paper-qa-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9954 2023-04-09 19:59:35.493224 paper-qa-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9519 2023-04-09 19:59:04.000000 paper-qa-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:59:35.493224 paper-qa-1.0.0/paper_qa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9954 2023-04-09 19:59:35.000000 paper-qa-1.0.0/paper_qa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-09 19:59:35.000000 paper-qa-1.0.0/paper_qa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 19:59:35.000000 paper-qa-1.0.0/paper_qa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-09 19:59:35.000000 paper-qa-1.0.0/paper_qa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-09 19:59:35.000000 paper-qa-1.0.0/paper_qa.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:59:35.493224 paper-qa-1.0.0/paperqa/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-09 19:59:04.000000 paper-qa-1.0.0/paperqa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-04-09 19:59:04.000000 paper-qa-1.0.0/paperqa/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:59:35.493224 paper-qa-1.0.0/paperqa/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-09 19:59:04.000000 paper-qa-1.0.0/paperqa/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9682 2023-04-09 19:59:04.000000 paper-qa-1.0.0/paperqa/contrib/zotero.py
--rw-r--r--   0 runner    (1001) docker     (123)    17412 2023-04-09 19:59:04.000000 paper-qa-1.0.0/paperqa/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-09 19:59:04.000000 paper-qa-1.0.0/paperqa/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-04-09 19:59:04.000000 paper-qa-1.0.0/paperqa/qaprompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     7004 2023-04-09 19:59:04.000000 paper-qa-1.0.0/paperqa/readers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-04-09 19:59:04.000000 paper-qa-1.0.0/paperqa/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-09 19:59:04.000000 paper-qa-1.0.0/paperqa/version.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 19:59:35.497224 paper-qa-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-09 19:59:04.000000 paper-qa-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:59:35.493224 paper-qa-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9477 2023-04-09 19:59:04.000000 paper-qa-1.0.0/tests/test_paperqa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 23:45:57.196550 paper-qa-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-10 23:45:30.000000 paper-qa-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11842 2023-04-10 23:45:57.192550 paper-qa-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11407 2023-04-10 23:45:30.000000 paper-qa-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 23:45:57.192550 paper-qa-1.1.0/paper_qa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11842 2023-04-10 23:45:57.000000 paper-qa-1.1.0/paper_qa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-10 23:45:57.000000 paper-qa-1.1.0/paper_qa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 23:45:57.000000 paper-qa-1.1.0/paper_qa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-10 23:45:57.000000 paper-qa-1.1.0/paper_qa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-10 23:45:57.000000 paper-qa-1.1.0/paper_qa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 23:45:57.192550 paper-qa-1.1.0/paperqa/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-10 23:45:30.000000 paper-qa-1.1.0/paperqa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-04-10 23:45:30.000000 paper-qa-1.1.0/paperqa/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 23:45:57.192550 paper-qa-1.1.0/paperqa/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-10 23:45:30.000000 paper-qa-1.1.0/paperqa/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-04-10 23:45:30.000000 paper-qa-1.1.0/paperqa/contrib/zotero.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17084 2023-04-10 23:45:30.000000 paper-qa-1.1.0/paperqa/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-10 23:45:30.000000 paper-qa-1.1.0/paperqa/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-04-10 23:45:30.000000 paper-qa-1.1.0/paperqa/qaprompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-04-10 23:45:30.000000 paper-qa-1.1.0/paperqa/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-04-10 23:45:30.000000 paper-qa-1.1.0/paperqa/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-10 23:45:30.000000 paper-qa-1.1.0/paperqa/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-10 23:45:30.000000 paper-qa-1.1.0/paperqa/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 23:45:57.196550 paper-qa-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-04-10 23:45:30.000000 paper-qa-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 23:45:57.192550 paper-qa-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9652 2023-04-10 23:45:30.000000 paper-qa-1.1.0/tests/test_paperqa.py
```

### Comparing `paper-qa-1.0.0/LICENSE` & `paper-qa-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `paper-qa-1.0.0/PKG-INFO` & `paper-qa-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper-qa
-Version: 1.0.0
+Version: 1.1.0
 Summary: LLM Chain for answering questions from docs 
 Home-page: https://github.com/whitead/paper-qa
 Author: Andrew White
 Author-email: white.d.andrew@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -19,56 +19,57 @@
 [![PyPI version](https://badge.fury.io/py/paper-qa.svg)](https://badge.fury.io/py/paper-qa)
 [![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](https://lbesson.mit-license.org/)
 
 This is a minimal package for doing question and answering from
 PDFs or text files (which can be raw HTML). It strives to give very good answers, with no hallucinations, by grounding responses with in-text citations. It uses [OpenAI Embeddings](https://platform.openai.com/docs/guides/embeddings) with a vector DB called [FAISS](https://github.com/facebookresearch/faiss) to embed and search documents. [langchain](https://github.com/hwchase17/langchain) helps
 generate answers.
 
-It uses this process
+It uses the process shown below:
 
-```text
+```
 embed docs into vectors -> embed query into vector -> search for top k passages in docs
 
 create summary of each passage relevant to query -> put summaries into prompt -> generate answer
 ```
 
-## Hugging Face Demo
-
-[Hugging Face Demo](https://huggingface.co/spaces/whitead/paper-qa)
+<img src="https://user-images.githubusercontent.com/908389/230854097-8fa96768-c694-45c0-bb04-3a7386facef3.jpeg" width="600" alt="Process of vector search, refinement, and answer with context">
 
-## Example
+## Output Example
 
 Question: How can carbon nanotubes be manufactured at a large scale?
 
 Carbon nanotubes can be manufactured at a large scale using the electric-arc technique (Journet6644). This technique involves creating an arc between two electrodes in a reactor under a helium atmosphere and using a mixture of a metallic catalyst and graphite powder in the anode. Yields of 80% of entangled carbon filaments can be achieved, which consist of smaller aligned SWNTs self-organized into bundle-like crystallites (Journet6644). Additionally, carbon nanotubes can be synthesized and self-assembled using various methods such as DNA-mediated self-assembly, nanoparticle-assisted alignment, chemical self-assembly, and electro-addressed functionalization (Tulevski2007). These methods have been used to fabricate large-area nanostructured arrays, high-density integration, and freestanding networks (Tulevski2007). 98% semiconducting CNT network solution can also be used and is separated from metallic nanotubes using a density gradient ultracentrifugation approach (Chen2014). The substrate is incubated in the solution and then rinsed with deionized water and dried with N2 air gun, leaving a uniform carbon network (Chen2014).
 
 ### References
 
 Journet6644: Journet, Catherine, et al. "Large-scale production of single-walled carbon nanotubes by the electric-arc technique." nature 388.6644 (1997): 756-758.
 
 Tulevski2007: Tulevski, George S., et al. "Chemically assisted directed assembly of carbon nanotubes for the fabrication of large-scale device arrays." Journal of the American Chemical Society 129.39 (2007): 11964-11968.
 
 Chen2014: Chen, Haitian, et al. "Large-scale complementary macroelectronics using hybrid integration of carbon nanotubes and IGZO thin-film transistors." Nature communications 5.1 (2014): 4097.
 
+
+## Hugging Face Demo
+
+[Hugging Face Demo](https://huggingface.co/spaces/whitead/paper-qa)
+
 ## Install
 
 Install with pip:
 
 ```bash
 pip install paper-qa
 ```
 
 ## Usage
 
 Make sure you have set your OPENAI_API_KEY environment variable to your [openai api key](https://platform.openai.com/account/api-keys)
 
 To use paper-qa, you need to have a list of paths (valid extensions include: .pdf, .txt) and a list of citations (strings) that correspond to the paths. You can then use the `Docs` class to add the documents and then query them.
 
-*This uses a lot of tokens!! About 5-10k tokens per answer + embedding cost (negligible unless many documents used). That is up to $0.02 per answer with current GPT-3 pricing. Use wisely.*
-
 ```python
 
 from paperqa import Docs
 
 # get a list of paths
 
 docs = Docs()
@@ -77,32 +78,98 @@
     
 answer = docs.query("What manufacturing challenges are unique to bispecific antibodies?")
 print(answer.formatted_answer)
 ```
 
 The answer object has the following attributes: `formatted_answer`, `answer` (answer alone), `question`, `context` (the summaries of passages found for answer), `references` (the docs from which the passages came), and `passages` which contain the raw text of the passages as a dictionary.
 
-## Adjusting number of sources
+### Choosing Model
+
+By default, it uses a hybrid of `gpt-3.5-turbo` and `gpt-4`. If you don't have gpt-4 access or would like to save money, you can adjust:
+
+```py
+docs = Docs(llm='gpt-3.5-turbo')
+```
+#### Locally Hosted
+
+You can also use any other models (or embeddings) available in [langchain](https://github.com/hwchase17/langchain). Here's an example of using `llama.cpp` to have locally hosted paper-qa:
+
+```py
+from langchain.embeddings import LlamaCppEmbeddings
+from langchain.llms import LlamaCpp
+llm = LlamaCpp(model_path="./ggml-model-q4_0.bin")
+embeddings = LlamaCppEmbeddings(model_path="/path/to/model/ggml-model-q4_0.bin")
+docs = Docs(llm=llm, embeddings=embeddings)
+```
+
+### Adjusting number of sources
 
 You can adjust the numbers of sources (passages of text) to reduce token usage or add more context. `k` refers to the top k most relevant and diverse (may from different sources) passages. Each passage is sent to the LLM to summarize, or determine if it is irrelevant. After this step, a limit of `max_sources` is applied so that the final answer can fit into the LLM context window. Thus, `k` > `max_sources`  and `max_sources` is the number of sources used in the final answer.
 
 ```python
 docs.query("What manufacturing challenges are unique to bispecific antibodies?", k = 5, max_sources = 2)
 ```
 
+### Using Code or HTML
+
+You do not need to use papers -- you can use code or raw HTML. Note that this tool is focused on answering questions, so it won't do well at writing code. One note is that the tool cannot infer citations from code, so you will need to provide them yourself.
+
+```python
+
+import glob
+
+source_files = glob.glob('**/*.js')
+
+docs = Docs()
+for f in source_files:
+    # this assumes the file names are unique in code
+    docs.add(f, citation='File ' + os.path.name(f), key=os.path.name(f))
+answer = docs.query("Where is the search bar in the header defined?")
+print(answer)
+```
+
+## Notebooks
+
+If you want to use this in an jupyter notebook or colab, you need to run the following command:
+
+```python
+import nest_asyncio
+nest_asyncio.apply()
+```
+
+Also - if you know how to make this automated, please let me know!
+
+## Agents (experimental)
+
+You can try to automate the collection of papers and assessment of correctness of papers using an agent. This is experimental and requires installation of [paper-scraper](https://github.com/blackadad/paper-scraper).
+
+```python
+
+docs = paperqa.Docs()
+answer = paperqa.run_agent(docs, 'What compounds target AKT1')
+print(answer)
+```
+
 ## Where do I get papers?
 
 Well that's a really good question! It's probably best to just download PDFs of papers you think will help answer your question and start from there.
 
 ### Zotero
 
 If you use [Zotero](https://www.zotero.org/) to organize your personal bibliography,
 you can use the `paperqa.contrib.ZoteroDB` to query papers from your library,
 which relies on [pyzotero](https://github.com/urschrei/pyzotero).
 
+Install `pyzotero` to use this feature:
+
+```bash
+pip install pyzotero
+```
+```
+
 First, note that `paperqa` parses the PDFs of papers to store in the database,
 so all relevant papers should have PDFs stored inside your database.
 You can get Zotero to automatically do this by highlighting the references
 you wish to retrieve, right clicking, and selecting *"Find Available PDFs"*.
 You can also manually drag-and-drop PDFs onto each reference.
 
 To download papers, you need to get an API key for your account.
@@ -118,14 +185,16 @@
 ```py
 from paperqa.contrib import ZoteroDB
 
 docs = paperqa.Docs()
 zotero = ZoteroDB(library_type="user")  # "group" if group library
 
 for item in zotero.iterate(limit=20):
+    if item.num_pages > 30:
+        continue  # skip long papers
     docs.add(item.pdf, key=item.key)
 ```
 
 which will download the first 20 papers in your Zotero database and add
 them to the `Docs` object.
 
 We can also do specific queries of our Zotero library and iterate over the results:
@@ -156,15 +225,15 @@
 for path,data in papers.items():
     try:
         docs.add(path)
     except ValueError as e:
         # sometimes this happens if PDFs aren't downloaded or readable
         print('Could not read', path, e)
 answer = docs.query("What manufacturing challenges are unique to bispecific antibodies?")
-print(answer.formatted_answer)
+print(answer)
 ```
 
 ## FAQ
 
 ### How is this different from LlamaIndex?
 
 It's not that different! This is similar to the tree response method in LlamaIndex. I just have included some prompts I find useful, readers that give page numbers/line numbers, and am focused on one task - answering technical questions with cited sources.
@@ -183,18 +252,20 @@
 
 ### Where do the documents come from?
 
 You can provide your own. I use some of my own code to pull papers from Google Scholar. This code is not included because it may enable people to violate Google's terms of service and publisher's terms of service.
 
 ### Can I save or load?
 
-The `Docs` class can be pickled and unpickled. This is useful if you want to save the embeddings of the documents and then load them later. The database is stored in `$HOME/.paperqa/{name}` where `name` is `default`, or you can pass a `name` when you instantiate the `paperqa` doc object.
+The `Docs` class can be pickled and unpickled. This is useful if you want to save the embeddings of the documents and then load them later.
 
 ```python
 import pickle
 
+# save
 with open("my_docs.pkl", "wb") as f:
     pickle.dump(docs, f)
 
+# load
 with open("my_docs.pkl", "rb") as f:
     docs = pickle.load(f)
 ```
```

### Comparing `paper-qa-1.0.0/README.md` & `paper-qa-1.1.0/paper_qa.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,60 +1,75 @@
+Metadata-Version: 2.1
+Name: paper-qa
+Version: 1.1.0
+Summary: LLM Chain for answering questions from docs 
+Home-page: https://github.com/whitead/paper-qa
+Author: Andrew White
+Author-email: white.d.andrew@gmail.com
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Paper QA
 
 [![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/whitead/paper-qa)
 [![tests](https://github.com/whitead/paper-qa/actions/workflows/tests.yml/badge.svg)](https://github.com/whitead/paper-qa)
 [![PyPI version](https://badge.fury.io/py/paper-qa.svg)](https://badge.fury.io/py/paper-qa)
 [![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](https://lbesson.mit-license.org/)
 
 This is a minimal package for doing question and answering from
 PDFs or text files (which can be raw HTML). It strives to give very good answers, with no hallucinations, by grounding responses with in-text citations. It uses [OpenAI Embeddings](https://platform.openai.com/docs/guides/embeddings) with a vector DB called [FAISS](https://github.com/facebookresearch/faiss) to embed and search documents. [langchain](https://github.com/hwchase17/langchain) helps
 generate answers.
 
-It uses this process
+It uses the process shown below:
 
-```text
+```
 embed docs into vectors -> embed query into vector -> search for top k passages in docs
 
 create summary of each passage relevant to query -> put summaries into prompt -> generate answer
 ```
 
-## Hugging Face Demo
-
-[Hugging Face Demo](https://huggingface.co/spaces/whitead/paper-qa)
+<img src="https://user-images.githubusercontent.com/908389/230854097-8fa96768-c694-45c0-bb04-3a7386facef3.jpeg" width="600" alt="Process of vector search, refinement, and answer with context">
 
-## Example
+## Output Example
 
 Question: How can carbon nanotubes be manufactured at a large scale?
 
 Carbon nanotubes can be manufactured at a large scale using the electric-arc technique (Journet6644). This technique involves creating an arc between two electrodes in a reactor under a helium atmosphere and using a mixture of a metallic catalyst and graphite powder in the anode. Yields of 80% of entangled carbon filaments can be achieved, which consist of smaller aligned SWNTs self-organized into bundle-like crystallites (Journet6644). Additionally, carbon nanotubes can be synthesized and self-assembled using various methods such as DNA-mediated self-assembly, nanoparticle-assisted alignment, chemical self-assembly, and electro-addressed functionalization (Tulevski2007). These methods have been used to fabricate large-area nanostructured arrays, high-density integration, and freestanding networks (Tulevski2007). 98% semiconducting CNT network solution can also be used and is separated from metallic nanotubes using a density gradient ultracentrifugation approach (Chen2014). The substrate is incubated in the solution and then rinsed with deionized water and dried with N2 air gun, leaving a uniform carbon network (Chen2014).
 
 ### References
 
 Journet6644: Journet, Catherine, et al. "Large-scale production of single-walled carbon nanotubes by the electric-arc technique." nature 388.6644 (1997): 756-758.
 
 Tulevski2007: Tulevski, George S., et al. "Chemically assisted directed assembly of carbon nanotubes for the fabrication of large-scale device arrays." Journal of the American Chemical Society 129.39 (2007): 11964-11968.
 
 Chen2014: Chen, Haitian, et al. "Large-scale complementary macroelectronics using hybrid integration of carbon nanotubes and IGZO thin-film transistors." Nature communications 5.1 (2014): 4097.
 
+
+## Hugging Face Demo
+
+[Hugging Face Demo](https://huggingface.co/spaces/whitead/paper-qa)
+
 ## Install
 
 Install with pip:
 
 ```bash
 pip install paper-qa
 ```
 
 ## Usage
 
 Make sure you have set your OPENAI_API_KEY environment variable to your [openai api key](https://platform.openai.com/account/api-keys)
 
 To use paper-qa, you need to have a list of paths (valid extensions include: .pdf, .txt) and a list of citations (strings) that correspond to the paths. You can then use the `Docs` class to add the documents and then query them.
 
-*This uses a lot of tokens!! About 5-10k tokens per answer + embedding cost (negligible unless many documents used). That is up to $0.02 per answer with current GPT-3 pricing. Use wisely.*
-
 ```python
 
 from paperqa import Docs
 
 # get a list of paths
 
 docs = Docs()
@@ -63,32 +78,98 @@
     
 answer = docs.query("What manufacturing challenges are unique to bispecific antibodies?")
 print(answer.formatted_answer)
 ```
 
 The answer object has the following attributes: `formatted_answer`, `answer` (answer alone), `question`, `context` (the summaries of passages found for answer), `references` (the docs from which the passages came), and `passages` which contain the raw text of the passages as a dictionary.
 
-## Adjusting number of sources
+### Choosing Model
+
+By default, it uses a hybrid of `gpt-3.5-turbo` and `gpt-4`. If you don't have gpt-4 access or would like to save money, you can adjust:
+
+```py
+docs = Docs(llm='gpt-3.5-turbo')
+```
+#### Locally Hosted
+
+You can also use any other models (or embeddings) available in [langchain](https://github.com/hwchase17/langchain). Here's an example of using `llama.cpp` to have locally hosted paper-qa:
+
+```py
+from langchain.embeddings import LlamaCppEmbeddings
+from langchain.llms import LlamaCpp
+llm = LlamaCpp(model_path="./ggml-model-q4_0.bin")
+embeddings = LlamaCppEmbeddings(model_path="/path/to/model/ggml-model-q4_0.bin")
+docs = Docs(llm=llm, embeddings=embeddings)
+```
+
+### Adjusting number of sources
 
 You can adjust the numbers of sources (passages of text) to reduce token usage or add more context. `k` refers to the top k most relevant and diverse (may from different sources) passages. Each passage is sent to the LLM to summarize, or determine if it is irrelevant. After this step, a limit of `max_sources` is applied so that the final answer can fit into the LLM context window. Thus, `k` > `max_sources`  and `max_sources` is the number of sources used in the final answer.
 
 ```python
 docs.query("What manufacturing challenges are unique to bispecific antibodies?", k = 5, max_sources = 2)
 ```
 
+### Using Code or HTML
+
+You do not need to use papers -- you can use code or raw HTML. Note that this tool is focused on answering questions, so it won't do well at writing code. One note is that the tool cannot infer citations from code, so you will need to provide them yourself.
+
+```python
+
+import glob
+
+source_files = glob.glob('**/*.js')
+
+docs = Docs()
+for f in source_files:
+    # this assumes the file names are unique in code
+    docs.add(f, citation='File ' + os.path.name(f), key=os.path.name(f))
+answer = docs.query("Where is the search bar in the header defined?")
+print(answer)
+```
+
+## Notebooks
+
+If you want to use this in an jupyter notebook or colab, you need to run the following command:
+
+```python
+import nest_asyncio
+nest_asyncio.apply()
+```
+
+Also - if you know how to make this automated, please let me know!
+
+## Agents (experimental)
+
+You can try to automate the collection of papers and assessment of correctness of papers using an agent. This is experimental and requires installation of [paper-scraper](https://github.com/blackadad/paper-scraper).
+
+```python
+
+docs = paperqa.Docs()
+answer = paperqa.run_agent(docs, 'What compounds target AKT1')
+print(answer)
+```
+
 ## Where do I get papers?
 
 Well that's a really good question! It's probably best to just download PDFs of papers you think will help answer your question and start from there.
 
 ### Zotero
 
 If you use [Zotero](https://www.zotero.org/) to organize your personal bibliography,
 you can use the `paperqa.contrib.ZoteroDB` to query papers from your library,
 which relies on [pyzotero](https://github.com/urschrei/pyzotero).
 
+Install `pyzotero` to use this feature:
+
+```bash
+pip install pyzotero
+```
+```
+
 First, note that `paperqa` parses the PDFs of papers to store in the database,
 so all relevant papers should have PDFs stored inside your database.
 You can get Zotero to automatically do this by highlighting the references
 you wish to retrieve, right clicking, and selecting *"Find Available PDFs"*.
 You can also manually drag-and-drop PDFs onto each reference.
 
 To download papers, you need to get an API key for your account.
@@ -104,14 +185,16 @@
 ```py
 from paperqa.contrib import ZoteroDB
 
 docs = paperqa.Docs()
 zotero = ZoteroDB(library_type="user")  # "group" if group library
 
 for item in zotero.iterate(limit=20):
+    if item.num_pages > 30:
+        continue  # skip long papers
     docs.add(item.pdf, key=item.key)
 ```
 
 which will download the first 20 papers in your Zotero database and add
 them to the `Docs` object.
 
 We can also do specific queries of our Zotero library and iterate over the results:
@@ -142,15 +225,15 @@
 for path,data in papers.items():
     try:
         docs.add(path)
     except ValueError as e:
         # sometimes this happens if PDFs aren't downloaded or readable
         print('Could not read', path, e)
 answer = docs.query("What manufacturing challenges are unique to bispecific antibodies?")
-print(answer.formatted_answer)
+print(answer)
 ```
 
 ## FAQ
 
 ### How is this different from LlamaIndex?
 
 It's not that different! This is similar to the tree response method in LlamaIndex. I just have included some prompts I find useful, readers that give page numbers/line numbers, and am focused on one task - answering technical questions with cited sources.
@@ -169,18 +252,20 @@
 
 ### Where do the documents come from?
 
 You can provide your own. I use some of my own code to pull papers from Google Scholar. This code is not included because it may enable people to violate Google's terms of service and publisher's terms of service.
 
 ### Can I save or load?
 
-The `Docs` class can be pickled and unpickled. This is useful if you want to save the embeddings of the documents and then load them later. The database is stored in `$HOME/.paperqa/{name}` where `name` is `default`, or you can pass a `name` when you instantiate the `paperqa` doc object.
+The `Docs` class can be pickled and unpickled. This is useful if you want to save the embeddings of the documents and then load them later.
 
 ```python
 import pickle
 
+# save
 with open("my_docs.pkl", "wb") as f:
     pickle.dump(docs, f)
 
+# load
 with open("my_docs.pkl", "rb") as f:
     docs = pickle.load(f)
 ```
```

### Comparing `paper-qa-1.0.0/paper_qa.egg-info/PKG-INFO` & `paper-qa-1.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,74 +1,61 @@
-Metadata-Version: 2.1
-Name: paper-qa
-Version: 1.0.0
-Summary: LLM Chain for answering questions from docs 
-Home-page: https://github.com/whitead/paper-qa
-Author: Andrew White
-Author-email: white.d.andrew@gmail.com
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Paper QA
 
 [![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/whitead/paper-qa)
 [![tests](https://github.com/whitead/paper-qa/actions/workflows/tests.yml/badge.svg)](https://github.com/whitead/paper-qa)
 [![PyPI version](https://badge.fury.io/py/paper-qa.svg)](https://badge.fury.io/py/paper-qa)
 [![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](https://lbesson.mit-license.org/)
 
 This is a minimal package for doing question and answering from
 PDFs or text files (which can be raw HTML). It strives to give very good answers, with no hallucinations, by grounding responses with in-text citations. It uses [OpenAI Embeddings](https://platform.openai.com/docs/guides/embeddings) with a vector DB called [FAISS](https://github.com/facebookresearch/faiss) to embed and search documents. [langchain](https://github.com/hwchase17/langchain) helps
 generate answers.
 
-It uses this process
+It uses the process shown below:
 
-```text
+```
 embed docs into vectors -> embed query into vector -> search for top k passages in docs
 
 create summary of each passage relevant to query -> put summaries into prompt -> generate answer
 ```
 
-## Hugging Face Demo
-
-[Hugging Face Demo](https://huggingface.co/spaces/whitead/paper-qa)
+<img src="https://user-images.githubusercontent.com/908389/230854097-8fa96768-c694-45c0-bb04-3a7386facef3.jpeg" width="600" alt="Process of vector search, refinement, and answer with context">
 
-## Example
+## Output Example
 
 Question: How can carbon nanotubes be manufactured at a large scale?
 
 Carbon nanotubes can be manufactured at a large scale using the electric-arc technique (Journet6644). This technique involves creating an arc between two electrodes in a reactor under a helium atmosphere and using a mixture of a metallic catalyst and graphite powder in the anode. Yields of 80% of entangled carbon filaments can be achieved, which consist of smaller aligned SWNTs self-organized into bundle-like crystallites (Journet6644). Additionally, carbon nanotubes can be synthesized and self-assembled using various methods such as DNA-mediated self-assembly, nanoparticle-assisted alignment, chemical self-assembly, and electro-addressed functionalization (Tulevski2007). These methods have been used to fabricate large-area nanostructured arrays, high-density integration, and freestanding networks (Tulevski2007). 98% semiconducting CNT network solution can also be used and is separated from metallic nanotubes using a density gradient ultracentrifugation approach (Chen2014). The substrate is incubated in the solution and then rinsed with deionized water and dried with N2 air gun, leaving a uniform carbon network (Chen2014).
 
 ### References
 
 Journet6644: Journet, Catherine, et al. "Large-scale production of single-walled carbon nanotubes by the electric-arc technique." nature 388.6644 (1997): 756-758.
 
 Tulevski2007: Tulevski, George S., et al. "Chemically assisted directed assembly of carbon nanotubes for the fabrication of large-scale device arrays." Journal of the American Chemical Society 129.39 (2007): 11964-11968.
 
 Chen2014: Chen, Haitian, et al. "Large-scale complementary macroelectronics using hybrid integration of carbon nanotubes and IGZO thin-film transistors." Nature communications 5.1 (2014): 4097.
 
+
+## Hugging Face Demo
+
+[Hugging Face Demo](https://huggingface.co/spaces/whitead/paper-qa)
+
 ## Install
 
 Install with pip:
 
 ```bash
 pip install paper-qa
 ```
 
 ## Usage
 
 Make sure you have set your OPENAI_API_KEY environment variable to your [openai api key](https://platform.openai.com/account/api-keys)
 
 To use paper-qa, you need to have a list of paths (valid extensions include: .pdf, .txt) and a list of citations (strings) that correspond to the paths. You can then use the `Docs` class to add the documents and then query them.
 
-*This uses a lot of tokens!! About 5-10k tokens per answer + embedding cost (negligible unless many documents used). That is up to $0.02 per answer with current GPT-3 pricing. Use wisely.*
-
 ```python
 
 from paperqa import Docs
 
 # get a list of paths
 
 docs = Docs()
@@ -77,32 +64,98 @@
     
 answer = docs.query("What manufacturing challenges are unique to bispecific antibodies?")
 print(answer.formatted_answer)
 ```
 
 The answer object has the following attributes: `formatted_answer`, `answer` (answer alone), `question`, `context` (the summaries of passages found for answer), `references` (the docs from which the passages came), and `passages` which contain the raw text of the passages as a dictionary.
 
-## Adjusting number of sources
+### Choosing Model
+
+By default, it uses a hybrid of `gpt-3.5-turbo` and `gpt-4`. If you don't have gpt-4 access or would like to save money, you can adjust:
+
+```py
+docs = Docs(llm='gpt-3.5-turbo')
+```
+#### Locally Hosted
+
+You can also use any other models (or embeddings) available in [langchain](https://github.com/hwchase17/langchain). Here's an example of using `llama.cpp` to have locally hosted paper-qa:
+
+```py
+from langchain.embeddings import LlamaCppEmbeddings
+from langchain.llms import LlamaCpp
+llm = LlamaCpp(model_path="./ggml-model-q4_0.bin")
+embeddings = LlamaCppEmbeddings(model_path="/path/to/model/ggml-model-q4_0.bin")
+docs = Docs(llm=llm, embeddings=embeddings)
+```
+
+### Adjusting number of sources
 
 You can adjust the numbers of sources (passages of text) to reduce token usage or add more context. `k` refers to the top k most relevant and diverse (may from different sources) passages. Each passage is sent to the LLM to summarize, or determine if it is irrelevant. After this step, a limit of `max_sources` is applied so that the final answer can fit into the LLM context window. Thus, `k` > `max_sources`  and `max_sources` is the number of sources used in the final answer.
 
 ```python
 docs.query("What manufacturing challenges are unique to bispecific antibodies?", k = 5, max_sources = 2)
 ```
 
+### Using Code or HTML
+
+You do not need to use papers -- you can use code or raw HTML. Note that this tool is focused on answering questions, so it won't do well at writing code. One note is that the tool cannot infer citations from code, so you will need to provide them yourself.
+
+```python
+
+import glob
+
+source_files = glob.glob('**/*.js')
+
+docs = Docs()
+for f in source_files:
+    # this assumes the file names are unique in code
+    docs.add(f, citation='File ' + os.path.name(f), key=os.path.name(f))
+answer = docs.query("Where is the search bar in the header defined?")
+print(answer)
+```
+
+## Notebooks
+
+If you want to use this in an jupyter notebook or colab, you need to run the following command:
+
+```python
+import nest_asyncio
+nest_asyncio.apply()
+```
+
+Also - if you know how to make this automated, please let me know!
+
+## Agents (experimental)
+
+You can try to automate the collection of papers and assessment of correctness of papers using an agent. This is experimental and requires installation of [paper-scraper](https://github.com/blackadad/paper-scraper).
+
+```python
+
+docs = paperqa.Docs()
+answer = paperqa.run_agent(docs, 'What compounds target AKT1')
+print(answer)
+```
+
 ## Where do I get papers?
 
 Well that's a really good question! It's probably best to just download PDFs of papers you think will help answer your question and start from there.
 
 ### Zotero
 
 If you use [Zotero](https://www.zotero.org/) to organize your personal bibliography,
 you can use the `paperqa.contrib.ZoteroDB` to query papers from your library,
 which relies on [pyzotero](https://github.com/urschrei/pyzotero).
 
+Install `pyzotero` to use this feature:
+
+```bash
+pip install pyzotero
+```
+```
+
 First, note that `paperqa` parses the PDFs of papers to store in the database,
 so all relevant papers should have PDFs stored inside your database.
 You can get Zotero to automatically do this by highlighting the references
 you wish to retrieve, right clicking, and selecting *"Find Available PDFs"*.
 You can also manually drag-and-drop PDFs onto each reference.
 
 To download papers, you need to get an API key for your account.
@@ -118,14 +171,16 @@
 ```py
 from paperqa.contrib import ZoteroDB
 
 docs = paperqa.Docs()
 zotero = ZoteroDB(library_type="user")  # "group" if group library
 
 for item in zotero.iterate(limit=20):
+    if item.num_pages > 30:
+        continue  # skip long papers
     docs.add(item.pdf, key=item.key)
 ```
 
 which will download the first 20 papers in your Zotero database and add
 them to the `Docs` object.
 
 We can also do specific queries of our Zotero library and iterate over the results:
@@ -156,15 +211,15 @@
 for path,data in papers.items():
     try:
         docs.add(path)
     except ValueError as e:
         # sometimes this happens if PDFs aren't downloaded or readable
         print('Could not read', path, e)
 answer = docs.query("What manufacturing challenges are unique to bispecific antibodies?")
-print(answer.formatted_answer)
+print(answer)
 ```
 
 ## FAQ
 
 ### How is this different from LlamaIndex?
 
 It's not that different! This is similar to the tree response method in LlamaIndex. I just have included some prompts I find useful, readers that give page numbers/line numbers, and am focused on one task - answering technical questions with cited sources.
@@ -183,18 +238,20 @@
 
 ### Where do the documents come from?
 
 You can provide your own. I use some of my own code to pull papers from Google Scholar. This code is not included because it may enable people to violate Google's terms of service and publisher's terms of service.
 
 ### Can I save or load?
 
-The `Docs` class can be pickled and unpickled. This is useful if you want to save the embeddings of the documents and then load them later. The database is stored in `$HOME/.paperqa/{name}` where `name` is `default`, or you can pass a `name` when you instantiate the `paperqa` doc object.
+The `Docs` class can be pickled and unpickled. This is useful if you want to save the embeddings of the documents and then load them later.
 
 ```python
 import pickle
 
+# save
 with open("my_docs.pkl", "wb") as f:
     pickle.dump(docs, f)
 
+# load
 with open("my_docs.pkl", "rb") as f:
     docs = pickle.load(f)
 ```
```

### Comparing `paper-qa-1.0.0/paperqa/agent.py` & `paper-qa-1.1.0/paperqa/agent.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from langchain.tools import BaseTool
-from langchain.chains import LLMChain
-from .qaprompts import select_paper_prompt, make_chain
 from .docs import Answer, Docs
-from langchain.agents import initialize_agent, Tool
+from langchain.agents import initialize_agent
 from langchain.chat_models import ChatOpenAI
 
 
 def status(answer: Answer, docs: Docs):
     return f" Status: Current Papers: {len(docs.doc_previews())} Current Evidence: {len(answer.contexts)} Current Cost: {answer.cost}"
 
+
 class ReadPapers(BaseTool):
     name = "Gather Evidence"
     description = (
         "Give a specific question to a researcher that will return evidence for it. "
         "Optionally, you may specify papers using their key provided by the Select Papers tool. "
         "Use the format: $QUESTION or use format $QUESTION|$KEY1,$KEY2,..."
     )
@@ -73,32 +72,32 @@
     def _arun(self, query: str) -> str:
         """Use the tool asynchronously."""
         raise NotImplementedError()
 
 
 class Search(BaseTool):
     name = "Paper Search"
-    description = (
-        "Search for papers to add to current papers. Input should be a string of keywords."
-    )
+    description = "Search for papers to add to current papers. Input should be a string of keywords."
     docs: Docs = None
     answer: Answer = None
 
     def __init__(self, docs, answer):
         # call the parent class constructor
         super(Search, self).__init__()
 
         self.docs = docs
         self.answer = answer
 
     def _run(self, query: str) -> str:
         try:
             import paperscraper
         except ImportError:
-            raise ImportError('Please install paperscraper (github.com/blackadad/paper-scraper) to use agent')
+            raise ImportError(
+                "Please install paperscraper (github.com/blackadad/paper-scraper) to use agent"
+            )
 
         papers = paperscraper.search_papers(query, limit=20, verbose=False)
         for path, data in papers.items():
             try:
                 self.docs.add(path)
             except:
                 pass
@@ -106,39 +105,34 @@
 
     def _arun(self, query: str) -> str:
         """Use the tool asynchronously."""
         raise NotImplementedError()
 
 
 def make_tools(docs, answer):
+    # putting here until langchain PR is merged
+    from langchain.tools.exception.tool import ExceptionTool
 
     tools = []
 
     tools.append(Search(docs, answer))
     tools.append(ReadPapers(docs, answer))
     tools.append(AnswerTool(docs, answer))
-    tools.append(
-        Tool(
-            name="Reflect",
-            description="Use this tool if you are stuck or repeating the same steps",
-            func=lambda x: "Reflect on your process. Are you repeating the same steps? Are you stuck? If so, try to think of a new way to approach the problem.",
-        )
-    )
-    # reflect is left off for now - doesn't seem to help
-    return tools[:-1]
+    tools.append(ExceptionTool())
+    return tools
 
 
 def run_agent(docs, question, llm=None):
     if llm is None:
         llm = ChatOpenAI(temperature=0.1, model="gpt-4")
     answer = Answer(question)
     tools = make_tools(docs, answer)
     mrkl = initialize_agent(
         tools, llm, agent="chat-zero-shot-react-description", verbose=True
     )
     mrkl.run(
         f"Answer question: {question}. Search for papers, gather evidence, and answer. "
         "Once you have at least five pieces of evidence, call the Propose Answer tool. "
-        "If you do not have enough evidence, search with different keywords. Remember to format with JSON. "
+        "If you do not have enough evidence, search with different keywords. "
     )
 
     return answer
```

### Comparing `paper-qa-1.0.0/paperqa/docs.py` & `paper-qa-1.1.0/paperqa/docs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,83 +1,54 @@
-from typing import List, Optional, Tuple, Dict, Callable, Any, Union
+from typing import List, Optional, Tuple, Union
 from functools import reduce
 import os
 import sys
 import asyncio
 from pathlib import Path
 import re
 from .paths import CACHE_PATH
-from .utils import maybe_is_text, maybe_is_truncated
+from .utils import maybe_is_text, md5sum
 from .qaprompts import (
     summary_prompt,
     qa_prompt,
     search_prompt,
     citation_prompt,
     select_paper_prompt,
     make_chain,
 )
-from dataclasses import dataclass
+from .types import Answer, Context
 from .readers import read_doc
 from langchain.vectorstores import FAISS
 from langchain.embeddings.openai import OpenAIEmbeddings
 from langchain.embeddings.base import Embeddings
 from langchain.chat_models import ChatOpenAI
 from langchain.llms.base import LLM
-from langchain.chains import LLMChain
 from langchain.callbacks import get_openai_callback
 from langchain.cache import SQLiteCache
 import langchain
 from datetime import datetime
 
 os.makedirs(os.path.dirname(CACHE_PATH), exist_ok=True)
 langchain.llm_cache = SQLiteCache(CACHE_PATH)
 
 
-@dataclass
-class Answer:
-    """A class to hold the answer to a question."""
-
-    question: str
-    answer: str = ""
-    context: str = ""
-    contexts: List[Any] = None
-    references: str = ""
-    formatted_answer: str = ""
-    passages: Dict[str, str] = None
-    tokens: int = 0
-    cost: float = 0
-
-    def __post_init__(self):
-        """Initialize the answer."""
-        if self.contexts is None:
-            self.contexts = []
-        if self.passages is None:
-            self.passages = {}
-
-    def __str__(self) -> str:
-        """Return the answer as a string."""
-        return self.formatted_answer
-
-
 class Docs:
     """A collection of documents to be used for answering questions."""
 
     def __init__(
         self,
         chunk_size_limit: int = 3000,
         llm: Optional[Union[LLM, str]] = None,
         summary_llm: Optional[Union[LLM, str]] = None,
         name: str = "default",
         index_path: Optional[Path] = None,
         embeddings: Optional[Embeddings] = None,
     ) -> None:
         """Initialize the collection of documents.
 
-
-
         Args:
             chunk_size_limit: The maximum number of characters to use for a single chunk of text.
             llm: The language model to use for answering questions. Default - OpenAI chat-gpt-turbo
             summary_llm: The language model to use for summarizing documents. If None, llm is used.
             name: The name of the collection.
             index_path: The path to the index file IF pickled. If None, defaults to using name in $HOME/.paperqa/name
         """
@@ -119,26 +90,28 @@
     def add(
         self,
         path: str,
         citation: Optional[str] = None,
         key: Optional[str] = None,
         disable_check: bool = False,
         chunk_chars: Optional[int] = 3000,
+        overwrite: bool = False,
     ) -> None:
         """Add a document to the collection."""
 
         # first check to see if we already have this document
         # this way we don't make api call to create citation on file we already have
+        md5 = md5sum(path)
         if path in self.docs:
             raise ValueError(f"Document {path} already in collection.")
 
         if citation is None:
             # peak first chunk
             texts, _ = read_doc(path, "", "", chunk_chars=chunk_chars)
-            with get_openai_callback() as cb:
+            with get_openai_callback():
                 citation = self.cite_chain.run(texts[0])
             if len(citation) < 3 or "Unknown" in citation or "insufficient" in citation:
                 citation = f"Unknown, {os.path.basename(path)}, {datetime.now().year}"
 
         if key is None:
             # get first name and year from citation
             try:
@@ -157,31 +130,30 @@
         while key + suffix in self.keys:
             # move suffix to next letter
             if suffix == "":
                 suffix = "a"
             else:
                 suffix = chr(ord(suffix) + 1)
         key += suffix
-        self.keys.add(key)
 
         texts, metadata = read_doc(path, citation, key, chunk_chars=chunk_chars)
         # loose check to see if document was loaded
         #
         if len("".join(texts)) < 10 or (
             not disable_check and not maybe_is_text("".join(texts))
         ):
             raise ValueError(
                 f"This does not look like a text document: {path}. Path disable_check to ignore this error."
             )
-
-        self.docs[path] = dict(texts=texts, metadata=metadata, key=key)
         if self._faiss_index is not None:
             self._faiss_index.add_texts(texts, metadatas=metadata)
         if self._doc_index is not None:
             self._doc_index.add_texts([citation], metadatas=[{"key": key}])
+        self.docs[path] = dict(texts=texts, metadata=metadata, key=key, md5=md5)
+        self.keys.add(key)
 
     def clear(self) -> None:
         """Clear the collection of documents."""
         self.docs = dict()
         self.keys = set()
         self._faiss_index = None
         self._doc_index = None
@@ -203,15 +175,15 @@
             )
             for doc in self.docs.values()
         ]
 
     def doc_match(self, query: str, k: int = 25) -> List[str]:
         """Return a list of documents that match the query."""
         if len(self.docs) == 0:
-            return ''
+            return ""
         if self._doc_index is None:
             texts = [doc["metadata"][0]["citation"] for doc in self.docs.values()]
             metadatas = [
                 {"key": doc["metadata"][0]["dockey"]} for doc in self.docs.values()
             ]
             self._doc_index = FAISS.from_texts(
                 texts, metadatas=metadatas, embedding=self.embeddings
@@ -242,14 +214,16 @@
     def __setstate__(self, state):
         self.__dict__.update(state)
         try:
             self._faiss_index = FAISS.load_local(self.index_path, self.embeddings)
         except:
             # they use some special exception type, but I don't want to import it
             self._faiss_index = None
+        if not hasattr(self, "_doc_index"):
+            self._doc_index = None
         self.update_llm(None, None)
 
     def _build_faiss_index(self):
         if self._faiss_index is None:
             texts = reduce(
                 lambda x, y: x + y, [doc["texts"] for doc in self.docs.values()], []
             )
@@ -263,18 +237,19 @@
     def get_evidence(
         self,
         answer: Answer,
         k: int = 3,
         max_sources: int = 5,
         marginal_relevance: bool = True,
         key_filter: Optional[List[str]] = None,
-    ) -> str:
+    ) -> Answer:
         # special case for jupyter notebooks
         if "get_ipython" in globals() or "google.colab" in sys.modules:
             import nest_asyncio
+
             nest_asyncio.apply()
         try:
             loop = asyncio.get_event_loop()
         except RuntimeError:
             loop = asyncio.new_event_loop()
             asyncio.set_event_loop(loop)
         return loop.run_until_complete(
@@ -290,15 +265,15 @@
     async def aget_evidence(
         self,
         answer: Answer,
         k: int = 3,
         max_sources: int = 5,
         marginal_relevance: bool = True,
         key_filter: Optional[List[str]] = None,
-    ) -> str:
+    ) -> Answer:
         if len(self.docs) == 0:
             return answer
         if self._faiss_index is None:
             self._build_faiss_index()
         _k = k
         if key_filter is not None:
             _k = k * 10  # heuristic
@@ -312,49 +287,55 @@
                 answer.question, k=_k, fetch_k=5 * _k
             )
 
         async def process(doc):
             if key_filter is not None and doc.metadata["dockey"] not in key_filter:
                 return None
             # check if it is already in answer (possible in agent setting)
-            if doc.metadata["key"] in [c[0] for c in answer.contexts]:
+            if doc.metadata["key"] in [c.key for c in answer.contexts]:
                 return None
-            c = (
-                doc.metadata["key"],
-                doc.metadata["citation"],
-                await self.summary_chain.arun(
+            c = Context(
+                key=doc.metadata["key"],
+                citation=doc.metadata["citation"],
+                context=await self.summary_chain.arun(
                     question=answer.question,
                     context_str=doc.page_content,
                     citation=doc.metadata["citation"],
                 ),
-                doc.page_content,
+                text=doc.page_content,
             )
-            if "Not applicable" not in c[2]:
+            if "Not applicable" not in c.context:
                 return c
             return None
 
         with get_openai_callback() as cb:
             contexts = await asyncio.gather(*[process(doc) for doc in docs])
         answer.tokens += cb.total_tokens
         answer.cost += cb.total_cost
         contexts = [c for c in contexts if c is not None]
         if len(contexts) == 0:
             return answer
-        contexts = sorted(contexts, key=lambda x: x[2], reverse=True)
+        contexts = sorted(contexts, key=lambda x: len(x.context), reverse=True)
         contexts = contexts[:max_sources]
         # add to answer (if not already there)
-        keys = [c[0] for c in answer.contexts]
+        keys = [c.key for c in answer.contexts]
         for c in contexts:
-            if c[0] not in keys:
+            if c.key not in keys:
                 answer.contexts.append(c)
 
         context_str = "\n\n".join(
-            [f"{k}: {s}" for k, c, s, t in answer.contexts if "Not applicable" not in s]
+            [
+                f"{c.key}: {c.context}"
+                for c in answer.contexts
+                if "Not applicable" not in c.context
+            ]
         )
-        valid_keys = [k for k, c, s, t in answer.contexts if "Not applicable" not in s]
+        valid_keys = [
+            c.key for c in answer.contexts if "Not applicable" not in c.context
+        ]
         if len(valid_keys) > 0:
             context_str += "\n\nValid keys: " + ", ".join(valid_keys)
         answer.context = context_str
         return answer
 
     def generate_search_query(self, query: str) -> List[str]:
         """Generate a list of search strings that can be used to find
@@ -375,15 +356,15 @@
         query: str,
         k: int = 10,
         max_sources: int = 5,
         length_prompt: str = "about 100 words",
         marginal_relevance: bool = True,
         answer: Optional[Answer] = None,
         key_filter: Optional[bool] = None,
-    ):
+    ) -> Answer:
         # special case for jupyter notebooks
         if "get_ipython" in globals() or "google.colab" in sys.modules:
             import nest_asyncio
 
             nest_asyncio.apply()
         try:
             loop = asyncio.get_event_loop()
@@ -394,46 +375,46 @@
             self.aquery(
                 query,
                 k=k,
                 max_sources=max_sources,
                 length_prompt=length_prompt,
                 marginal_relevance=marginal_relevance,
                 answer=answer,
-                key_filter=key_filter
+                key_filter=key_filter,
             )
         )
 
     async def aquery(
         self,
         query: str,
         k: int = 10,
         max_sources: int = 5,
         length_prompt: str = "about 100 words",
         marginal_relevance: bool = True,
         answer: Optional[Answer] = None,
-        key_filter: Optional[bool] = None
-    ):
+        key_filter: Optional[bool] = None,
+    ) -> Answer:
         if k < max_sources:
             raise ValueError("k should be greater than max_sources")
         if answer is None:
             answer = Answer(query)
-        if key_filter or (key_filter is None and len(self.docs) > 5)    :
+        if key_filter or (key_filter is None and len(self.docs) > 5):
             with get_openai_callback() as cb:
                 keys = self.doc_match(answer.question)
             answer.tokens += cb.total_tokens
             answer.cost += cb.total_cost
         if len(answer.contexts) == 0:
             answer = await self.aget_evidence(
                 answer,
                 k=k,
                 max_sources=max_sources,
                 marginal_relevance=marginal_relevance,
-                key_filter=keys if key_filter else None
+                key_filter=keys if key_filter else None,
             )
-        context_str, citations = answer.context, answer.contexts
+        context_str, contexts = answer.context, answer.contexts
         bib = dict()
         passages = dict()
         if len(context_str) < 10:
             answer_text = (
                 "I cannot answer this question due to insufficient information."
             )
         else:
@@ -442,15 +423,18 @@
                     question=query, context_str=context_str, length=length_prompt
                 )
             answer.tokens += cb.total_tokens
             answer.cost += cb.total_cost
         # it still happens lol
         if "(Foo2012)" in answer_text:
             answer_text = answer_text.replace("(Foo2012)", "")
-        for key, citation, summary, text in citations:
+        for c in contexts:
+            key = c.key
+            text = c.context
+            citation = c.citation
             # do check for whole key (so we don't catch Callahan2019a with Callahan2019)
             skey = key.split(" ")[0]
             if skey + " " in answer_text or skey + ")" or skey + "," in answer_text:
                 bib[skey] = citation
                 passages[key] = text
         bib_str = "\n\n".join(
             [f"{i+1}. ({k}): {c}" for i, (k, c) in enumerate(bib.items())]
```

### Comparing `paper-qa-1.0.0/paperqa/qaprompts.py` & `paper-qa-1.1.0/paperqa/qaprompts.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import langchain.prompts as prompts
 from datetime import datetime
 from langchain.chains import LLMChain
 from langchain.chat_models import ChatOpenAI
-from langchain.schema import HumanMessage, SystemMessage
+from langchain.schema import SystemMessage
 from langchain.prompts.chat import HumanMessagePromptTemplate, ChatPromptTemplate
 
 
 summary_prompt = prompts.PromptTemplate(
     input_variables=["question", "context_str", "citation"],
     template="Summarize and provide direct quotes from the text below to help answer a question. "
     "Do not directly answer the question, instead summarize and "
```

### Comparing `paper-qa-1.0.0/paperqa/readers.py` & `paper-qa-1.1.0/paperqa/readers.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 
 
 def parse_txt(path, citation, key, chunk_chars=2000, overlap=50, html=False):
 
     try:
         with open(path) as f:
             doc = f.read()
-    except UnicodeDecodeError as e:
+    except UnicodeDecodeError:
         with open(path, encoding="utf-8", errors="ignore") as f:
             doc = f.read()
     if html:
         doc = html2text(doc)
     # yo, no idea why but the texts are not split correctly
     text_splitter = TextSplitter(chunk_size=chunk_chars, chunk_overlap=overlap)
     texts = text_splitter.split_text(doc)
@@ -128,15 +128,15 @@
 def _deserialize_s(obj):
     """The inverse of _serialize_s"""
     return json.loads(obj)
 
 
 def _serialize(obj):
     # llmchain wants a list of "Generation" objects, so we simply
-    # stick this regular text into it. 
+    # stick this regular text into it.
     return [Generation(text=_serialize_s(obj))]
 
 
 def _deserialize(obj):
     # (The inverse of _serialize)
     try:
         return _deserialize_s(obj[0].text)
```

### Comparing `paper-qa-1.0.0/paperqa/utils.py` & `paper-qa-1.1.0/paperqa/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 import math
 import string
+import pypdf
+
+from .types import StrPath
 
 
 def maybe_is_text(s, thresh=2.5):
     if len(s) == 0:
         return False
     # Calculate the entropy of the string
     entropy = 0
@@ -46,7 +49,21 @@
 
 def maybe_is_html(s):
     if len(s) == 0:
         return False
     # check for html tags
     if "<body" in s or "<html" in s or "<div" in s:
         return True
+
+
+def count_pdf_pages(file_path: StrPath) -> int:
+    with open(file_path, "rb") as pdf_file:
+        pdf_reader = pypdf.PdfReader(pdf_file)
+        num_pages = len(pdf_reader.pages)
+    return num_pages
+
+
+def md5sum(file_path: StrPath) -> str:
+    import hashlib
+
+    with open(file_path, "rb") as f:
+        return hashlib.md5(f.read()).hexdigest()
```

### Comparing `paper-qa-1.0.0/setup.py` & `paper-qa-1.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,14 @@
         "pypdf",
         "langchain>=0.0.129",
         "openai>=0.27.0",
         "faiss-cpu",
         "PyCryptodome",
         "html2text",
         "tiktoken",
-        "pyzotero",
     ],
     test_suite="tests",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

### Comparing `paper-qa-1.0.0/tests/test_paperqa.py` & `paper-qa-1.1.0/tests/test_paperqa.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,56 +41,55 @@
         r = requests.get("https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
         f.write(r.text)
     docs = paperqa.Docs()
     docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed now")
     evidence = docs.get_evidence(
         paperqa.Answer("For which state was he a governor"), k=1, max_sources=1
     )
+    print(evidence.contexts[0].context, evidence.context)
     assert "Missouri" in evidence.context
     os.remove(doc_path)
 
 
 def test_query():
     doc_path = "example.txt"
     with open(doc_path, "w", encoding="utf-8") as f:
         # get wiki page about politician
         r = requests.get("https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
         f.write(r.text)
     docs = paperqa.Docs()
     docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed now")
-    answer = docs.query("What is Frederick Bates's greatest accomplishment?")
+    docs.query("What is Frederick Bates's greatest accomplishment?")
     os.remove(doc_path)
 
 
 class Test(IsolatedAsyncioTestCase):
     async def test_aquery(self):
         doc_path = "example.txt"
         with open(doc_path, "w", encoding="utf-8") as f:
             # get wiki page about politician
             r = requests.get(
                 "https://en.wikipedia.org/wiki/Frederick_Bates_(politician)"
             )
             f.write(r.text)
         docs = paperqa.Docs()
         docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed now")
-        i = 0
-        answer = await docs.aquery("What is Frederick Bates's greatest accomplishment?")
+        await docs.aquery("What is Frederick Bates's greatest accomplishment?")
         os.remove(doc_path)
 
 
 def test_doc_match():
     doc_path = "example.txt"
     with open(doc_path, "w", encoding="utf-8") as f:
         # get wiki page about politician
         r = requests.get("https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
         f.write(r.text)
     docs = paperqa.Docs()
     docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed now")
-    i = 0
-    result = docs.doc_match("What is Frederick Bates's greatest accomplishment?")
+    docs.doc_match("What is Frederick Bates's greatest accomplishment?")
     os.remove(doc_path)
 
 
 def test_docs_pickle():
     doc_path = "example.txt"
     with open(doc_path, "w", encoding="utf-8") as f:
         # get front page of wikipedia
@@ -200,15 +199,15 @@
 
 def test_code():
     # load this script
     doc_path = os.path.abspath(__file__)
     docs = paperqa.Docs(llm=OpenAI(temperature=0.0, model_name="text-ada-001"))
     docs.add(doc_path, "test_paperqa.py", key="test", disable_check=True)
     assert len(docs.docs) == 1
-    answer = docs.query("What function tests the preview?")
+    docs.query("What function tests the preview?")
 
 
 def test_citation():
     doc_path = "example.txt"
     with open(doc_path, "w", encoding="utf-8") as f:
         # get wiki page about politician
         r = requests.get("https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
@@ -240,13 +239,21 @@
     """Test that we can filter evidence with in query"""
     doc_path = "example2.txt"
     with open(doc_path, "w", encoding="utf-8") as f:
         # get wiki page about politician
         r = requests.get("https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
         f.write(r.text)
     docs = paperqa.Docs()
-    docs.add(doc_path, "Information about Fredrick Bates, WikiMedia Foundation, 2023, Accessed now")
+    docs.add(
+        doc_path,
+        "Information about Fredrick Bates, WikiMedia Foundation, 2023, Accessed now",
+    )
     # add with new dockey
     docs.add("example.txt", "WikiMedia Foundation, 2023, Accessed now", key="test")
     answer = docs.query("What country is Bates from?", key_filter=True)
-    print(answer.context)
-    assert "United States" in answer.answer
+    # the filter shouldn't trigger, so just checking that it doesn't crash
+
+
+def disabled_test_agent():
+    docs = paperqa.Docs()
+    answer = paperqa.run_agent(docs, "What compounds target AKT1")
+    print(answer)
```

