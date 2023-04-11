# Comparing `tmp/text_mods-1.22.tar.gz` & `tmp/text_mods-1.30.tar.gz`

## Comparing `text_mods-1.22.tar` & `text_mods-1.30.tar`

### file list

```diff
@@ -1,12 +1,18 @@
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 text_mods-1.22/src/Example.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 text_mods-1.22/src/__init__.py
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 text_mods-1.22/src/setup.py
--rw-r--r--   0        0        0     2357 2020-02-02 00:00:00.000000 text_mods-1.22/src/text_mods.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 text_mods-1.22/text_mods.egg-info/PKG-INFO
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 text_mods-1.22/text_mods.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 text_mods-1.22/text_mods.egg-info/dependency_links.txt
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 text_mods-1.22/text_mods.egg-info/top_level.txt
--rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 text_mods-1.22/LICENSE.txt
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 text_mods-1.22/README.md
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 text_mods-1.22/pyproject.toml
--rw-r--r--   0        0        0     2043 2020-02-02 00:00:00.000000 text_mods-1.22/PKG-INFO
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 text_mods-1.30/src/Example.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 text_mods-1.30/src/__init__.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 text_mods-1.30/src/setup.py
+-rw-r--r--   0        0        0     4842 2020-02-02 00:00:00.000000 text_mods-1.30/src/text_mods.py
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 text_mods-1.30/src/dist/text_mods-1.30-py3-none-any.whl
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 text_mods-1.30/src/dist/text_mods-1.30.tar.gz
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 text_mods-1.30/src/text_mods.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 text_mods-1.30/src/text_mods.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 text_mods-1.30/src/text_mods.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 text_mods-1.30/src/text_mods.egg-info/top_level.txt
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 text_mods-1.30/text_mods.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 text_mods-1.30/text_mods.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 text_mods-1.30/text_mods.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 text_mods-1.30/text_mods.egg-info/top_level.txt
+-rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 text_mods-1.30/LICENSE.txt
+-rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 text_mods-1.30/README.md
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 text_mods-1.30/pyproject.toml
+-rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 text_mods-1.30/PKG-INFO
```

### Comparing `text_mods-1.22/LICENSE.txt` & `text_mods-1.30/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `text_mods-1.22/README.md` & `text_mods-1.30/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,36 +1,45 @@
 # Text Formatting Toolkit
 
-text_mods is a Python module for formatting text strings in various ways. It includes functions for removing HTML tags and punctuation, replacing words with synonyms, and applying different formatting styles such as bold, italic, and colored text.
+text_mods is a Python module for formatting text strings in various ways. It includes functions for removing HTML tags and punctuation, replacing words with synonyms, applying different formatting styles such as bold, italic and colored text. In addition it performs natural language processing tasks such as entity recognition, word frequency counting and text summarization.
 
 ## Requirements+
 
 * Python 3.6 or higher
 * NLTK library
 * WordNet database
+* gensim library
+* googletrans library
+* spacy library
+* en_core_web_sm package for Spacy
 
 ## Installation
 
 * Install Python 3.6 or higher from the official website: [Here] (<https://www.python.org/downloads/>)
-* Install the NLTK library by running pip install nltk in your terminal or command prompt.
+* Install the NLTK library by running ```pip install nltk``` in your terminal or command prompt.
 * Download the WordNet database by running the following commands in a Python interpreter:
 arduino
 
 ``` Python
 import nltk
 nltk.download('wordnet')
 ```
 
-* Download or clone the code from the Github repository: [GitHub] (<https://github.com/Ilija-nik1/text_mods>)
+* Install the gensim, googletrans, and spacy libraries by running
+
+```pip install gensim googletrans spacy```
+
+* Download the en_core_web_sm package for Spacy by running ```python -m spacy download en_core_web_sm```
+* Download or clone the code from the Github repository: [Github] (<https://github.com/Ilija-nik1/text_mods>)
 
 ### Clone
 
-Clone the repository using git:
+Clone the repository using git
 
-```bash
+``` bash
 git clone https://github.com/Ilija-nik1/text_mods.git
 ```
 
 ## Usage
 
 Here are some examples of how to use the functions in the module
 
@@ -52,8 +61,8 @@
 
 ## Contributing
 
 If you find any bugs or have suggestions for new features, please open an issue or pull request on the Github repository.
 
 ## License
 
-This code is licensed under the MIT License.
+This code is licensed under the MIT License.
```

### Comparing `text_mods-1.22/PKG-INFO` & `text_mods-1.30/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,48 +1,57 @@
 Metadata-Version: 2.1
 Name: text_mods
-Version: 1.22
+Version: 1.30
 Summary: This code defines a collection of functions for formatting and modifying text
 Project-URL: Homepage, https://github.com/Ilija-nik1/text_mods
 Author: I_N-01
 License-File: LICENSE.txt
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.1
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # Text Formatting Toolkit
 
-text_mods is a Python module for formatting text strings in various ways. It includes functions for removing HTML tags and punctuation, replacing words with synonyms, and applying different formatting styles such as bold, italic, and colored text.
+text_mods is a Python module for formatting text strings in various ways. It includes functions for removing HTML tags and punctuation, replacing words with synonyms, applying different formatting styles such as bold, italic and colored text. In addition it performs natural language processing tasks such as entity recognition, word frequency counting and text summarization.
 
 ## Requirements+
 
 * Python 3.6 or higher
 * NLTK library
 * WordNet database
+* gensim library
+* googletrans library
+* spacy library
+* en_core_web_sm package for Spacy
 
 ## Installation
 
 * Install Python 3.6 or higher from the official website: [Here] (<https://www.python.org/downloads/>)
-* Install the NLTK library by running pip install nltk in your terminal or command prompt.
+* Install the NLTK library by running ```pip install nltk``` in your terminal or command prompt.
 * Download the WordNet database by running the following commands in a Python interpreter:
 arduino
 
 ``` Python
 import nltk
 nltk.download('wordnet')
 ```
 
-* Download or clone the code from the Github repository: [GitHub] (<https://github.com/Ilija-nik1/text_mods>)
+* Install the gensim, googletrans, and spacy libraries by running
+
+```pip install gensim googletrans spacy```
+
+* Download the en_core_web_sm package for Spacy by running ```python -m spacy download en_core_web_sm```
+* Download or clone the code from the Github repository: [Github] (<https://github.com/Ilija-nik1/text_mods>)
 
 ### Clone
 
-Clone the repository using git:
+Clone the repository using git
 
-```bash
+``` bash
 git clone https://github.com/Ilija-nik1/text_mods.git
 ```
 
 ## Usage
 
 Here are some examples of how to use the functions in the module
 
@@ -64,8 +73,8 @@
 
 ## Contributing
 
 If you find any bugs or have suggestions for new features, please open an issue or pull request on the Github repository.
 
 ## License
 
-This code is licensed under the MIT License.
+This code is licensed under the MIT License.
```

