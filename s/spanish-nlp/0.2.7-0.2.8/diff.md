# Comparing `tmp/spanish_nlp-0.2.7.tar.gz` & `tmp/spanish_nlp-0.2.8.tar.gz`

## Comparing `spanish_nlp-0.2.7.tar` & `spanish_nlp-0.2.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 spanish_nlp-0.2.7/src/spanish_nlp/__about__.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 spanish_nlp-0.2.7/src/spanish_nlp/__init__.py
--rw-r--r--   0        0        0    10016 2020-02-02 00:00:00.000000 spanish_nlp-0.2.7/src/spanish_nlp/classifiers.py
--rw-r--r--   0        0        0    17009 2020-02-02 00:00:00.000000 spanish_nlp-0.2.7/src/spanish_nlp/preprocess.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 spanish_nlp-0.2.7/src/spanish_nlp/augmentation/__init__.py
--rw-r--r--   0        0        0     4723 2020-02-02 00:00:00.000000 spanish_nlp-0.2.7/src/spanish_nlp/augmentation/abstract.py
--rw-r--r--   0        0        0    12507 2020-02-02 00:00:00.000000 spanish_nlp-0.2.7/src/spanish_nlp/augmentation/masked.py
--rw-r--r--   0        0        0    24055 2020-02-02 00:00:00.000000 spanish_nlp-0.2.7/src/spanish_nlp/augmentation/spelling.py
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 spanish_nlp-0.2.7/src/spanish_nlp/augmentation/data/misspelled_words.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spanish_nlp-0.2.7/src/spanish_nlp/utils/__init__,py
--rw-r--r--   0        0        0     9692 2020-02-02 00:00:00.000000 spanish_nlp-0.2.7/src/spanish_nlp/utils/emo_unicode.py
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 spanish_nlp-0.2.7/src/spanish_nlp/utils/inclusive_words.py
--rw-r--r--   0        0        0    11954 2020-02-02 00:00:00.000000 spanish_nlp-0.2.7/src/spanish_nlp/utils/stopwords.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spanish_nlp-0.2.7/src/spanish_nlp/utils/tokenizers.py
--rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 spanish_nlp-0.2.7/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 spanish_nlp-0.2.7/LICENSE
--rw-r--r--   0        0        0     7822 2020-02-02 00:00:00.000000 spanish_nlp-0.2.7/README.md
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 spanish_nlp-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     9019 2020-02-02 00:00:00.000000 spanish_nlp-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 spanish_nlp-0.2.8/src/spanish_nlp/__about__.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 spanish_nlp-0.2.8/src/spanish_nlp/__init__.py
+-rw-r--r--   0        0        0    10016 2020-02-02 00:00:00.000000 spanish_nlp-0.2.8/src/spanish_nlp/classifiers.py
+-rw-r--r--   0        0        0    17009 2020-02-02 00:00:00.000000 spanish_nlp-0.2.8/src/spanish_nlp/preprocess.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 spanish_nlp-0.2.8/src/spanish_nlp/augmentation/__init__.py
+-rw-r--r--   0        0        0     4723 2020-02-02 00:00:00.000000 spanish_nlp-0.2.8/src/spanish_nlp/augmentation/abstract.py
+-rw-r--r--   0        0        0    12507 2020-02-02 00:00:00.000000 spanish_nlp-0.2.8/src/spanish_nlp/augmentation/masked.py
+-rw-r--r--   0        0        0    25294 2020-02-02 00:00:00.000000 spanish_nlp-0.2.8/src/spanish_nlp/augmentation/spelling.py
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 spanish_nlp-0.2.8/src/spanish_nlp/augmentation/data/misspelled_words.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spanish_nlp-0.2.8/src/spanish_nlp/utils/__init__,py
+-rw-r--r--   0        0        0     9692 2020-02-02 00:00:00.000000 spanish_nlp-0.2.8/src/spanish_nlp/utils/emo_unicode.py
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 spanish_nlp-0.2.8/src/spanish_nlp/utils/inclusive_words.py
+-rw-r--r--   0        0        0    11954 2020-02-02 00:00:00.000000 spanish_nlp-0.2.8/src/spanish_nlp/utils/stopwords.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spanish_nlp-0.2.8/src/spanish_nlp/utils/tokenizers.py
+-rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 spanish_nlp-0.2.8/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 spanish_nlp-0.2.8/LICENSE
+-rw-r--r--   0        0        0     7986 2020-02-02 00:00:00.000000 spanish_nlp-0.2.8/README.md
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 spanish_nlp-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0     9183 2020-02-02 00:00:00.000000 spanish_nlp-0.2.8/PKG-INFO
```

### Comparing `spanish_nlp-0.2.7/src/spanish_nlp/classifiers.py` & `spanish_nlp-0.2.8/src/spanish_nlp/classifiers.py`

 * *Files identical despite different names*

### Comparing `spanish_nlp-0.2.7/src/spanish_nlp/preprocess.py` & `spanish_nlp-0.2.8/src/spanish_nlp/preprocess.py`

 * *Files identical despite different names*

### Comparing `spanish_nlp-0.2.7/src/spanish_nlp/augmentation/abstract.py` & `spanish_nlp-0.2.8/src/spanish_nlp/augmentation/abstract.py`

 * *Files identical despite different names*

### Comparing `spanish_nlp-0.2.7/src/spanish_nlp/augmentation/masked.py` & `spanish_nlp-0.2.8/src/spanish_nlp/augmentation/masked.py`

 * *Files identical despite different names*

### Comparing `spanish_nlp-0.2.7/src/spanish_nlp/augmentation/spelling.py` & `spanish_nlp-0.2.8/src/spanish_nlp/augmentation/spelling.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
             "keyboard",
             "ocr",
             "random",
             "grapheme_spelling",
             "word_spelling",
             "remove_punctuation",
             "remove_accents",
+            "remove_spaces",
             "lowercase",
             "uppercase",
             "randomcase",
             "all",
         ]
 
         if self.method not in available_methods:
@@ -78,14 +79,16 @@
             return self._random_augment_(text, num_samples)
         elif self.method == "grapheme_spelling":
             return self._grapheme_spelling_augment_(text, num_samples)
         elif self.method == "word_spelling":
             return self._word_spelling_augmentation_(text, num_samples)
         elif self.method == "remove_punctuation":
             return self._remove_punctuation_augment_(text, num_samples)
+        elif self.method == "remove_spaces":
+            return self._remove_spaces_augment_(text, num_samples)
         elif self.method == "remove_accents":
             return self._remove_accents_augmentation_(text, num_samples)
         elif self.method == "lowercase":
             return self._lowercase_augmentation_(text, num_samples)
         elif self.method == "uppercase":
             return self._uppercase_augmentation_(text, num_samples)
         elif self.method == "randomcase":
@@ -439,14 +442,40 @@
             elements = random.sample(indices, num_aug)
             for e in elements:
                 new_text = new_text[:e] + new_text[e + 1 :]
             # Append the augmented text to the list
             output_texts.append(new_text)
         return output_texts
 
+    def _remove_spaces_augment_(self, text, num_samples):
+        """Remove spaces in the text according to the aug_percent
+
+        Args:
+            text (str): text to augment
+            num_samples (int): number of samples to generate
+        """
+        # List to save the augmented texts
+        output_texts = []
+        # List with the punctuation to eliminate
+        num_text_spaces = [c for c in text if c == " "]
+        num_aug = len(num_text_spaces) * self.aug_percent
+        # Round by the upper integer
+        num_aug = ceil(num_aug)
+        for i in range(num_samples):
+            new_text = text
+            # Get the indices of the punctuation to eliminate
+            indices = [i for i, c in enumerate(new_text) if c == " "]
+            # Create a list with num_aug elements in indices without repetition
+            elements = random.sample(indices, num_aug)
+            for e in elements:
+                new_text = new_text[:e] + new_text[e + 1:]
+            # Append the augmented text to the list
+            output_texts.append(new_text)
+        return output_texts
+
     def _remove_accents_augmentation_(self, text, num_samples):
         """Remove accents in the text according to the aug_percent
 
         Args:
             text (str): text to augment
             num_samples (int): number of samples to generate
         """
```

### Comparing `spanish_nlp-0.2.7/src/spanish_nlp/augmentation/data/misspelled_words.json` & `spanish_nlp-0.2.8/src/spanish_nlp/augmentation/data/misspelled_words.json`

 * *Files identical despite different names*

### Comparing `spanish_nlp-0.2.7/src/spanish_nlp/utils/emo_unicode.py` & `spanish_nlp-0.2.8/src/spanish_nlp/utils/emo_unicode.py`

 * *Files identical despite different names*

### Comparing `spanish_nlp-0.2.7/src/spanish_nlp/utils/inclusive_words.py` & `spanish_nlp-0.2.8/src/spanish_nlp/utils/inclusive_words.py`

 * *Files identical despite different names*

### Comparing `spanish_nlp-0.2.7/src/spanish_nlp/utils/stopwords.py` & `spanish_nlp-0.2.8/src/spanish_nlp/utils/stopwords.py`

 * *Files identical despite different names*

### Comparing `spanish_nlp-0.2.7/.gitignore` & `spanish_nlp-0.2.8/.gitignore`

 * *Files identical despite different names*

### Comparing `spanish_nlp-0.2.7/LICENSE` & `spanish_nlp-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `spanish_nlp-0.2.7/README.md` & `spanish_nlp-0.2.8/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -72,14 +72,15 @@
 ```
 ### Classification
 
 See more information in the [Jupyter Notebook example](https://github.com/jorgeortizfuentes/spanish_nlp/blob/main/examples/Classify.ipynb)
 #### Available classifiers
 
 * Hate Speech (hate_speech)
+* Incivility (incivility)
 * Toxic Speech (toxic_speech)
 * Sentiment Analysis (sentiment_analysis)
 * Emotion Analysis (emotion_analysis)
 * Irony Analysis (irony_analysis)
 * Sexist Analysis (sexist_analysis)
 * Racism Analysis (racism_analysis)
 
@@ -113,18 +114,24 @@
 ### Augmentation
 
 See more information in the [Jupyter Notebook example](https://github.com/jorgeortizfuentes/spanish_nlp/blob/main/examples/Data%20Augmentation.ipynb)
 
 #### Available Augmentation Models
 
 - Spelling augmentation
-  - Keyboard method
-  - OCR method
-  - Random method
-  - Orthography method
+  - Keyboard spelling method
+  - OCR spelling method
+  - Random spelling replace method
+  - Grapheme spelling
+  - Word spelling
+  - Remove punctuation
+  - Remove accents
+  - Lowercase
+  - Uppercase
+  - Randomcase
   - All method
 - Masked augmentation
   - Sustitute method
   - Insert method
 - Others models under development (such as Synonyms, WordEmbeddings, GenerativeOpenSource, GenerativeOpenAI, BackTranslation, AbstractiveSummarization)
 
 
@@ -187,8 +194,8 @@
 
 ## Acknowledgements
 
 We would like to express our gratitude to the Millennium Institute For Foundational Research and Department of Computer Science at the University of Chile for supporting the development of Spanish NLP. Special thanks to Felipe Bravo-Marquéz, Ricardo Cordova and Hernán Sarmiento for their knowledge, support and invaluable contribution to the project.
 
 ## Contributing
 
-Contributions to Spanish NLP are welcome! Please see the [contributing guide](https://github.com/users/jorgeortizfuentes/projects/1) for more information.
+Contributions to Spanish NLP are welcome! Please see the [contributing guide](https://github.com/users/jorgeortizfuentes/projects/1) for more information.
```

### Comparing `spanish_nlp-0.2.7/pyproject.toml` & `spanish_nlp-0.2.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spanish_nlp-0.2.7/PKG-INFO` & `spanish_nlp-0.2.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spanish_nlp
-Version: 0.2.7
+Version: 0.2.8
 Summary: A package for NLP in Spanish
 Project-URL: Homepage, https://github.com/jorgeortizfuentes/spanish_nlp
 Author-email: Jorge Ortiz-Fuentes <jorge@ortizfuentes.com>
 License-Expression: GPL-3.0-or-later
 License-File: LICENSE
 Keywords: augmentation,clasificacion,classifier,español,language,lenguaje,nlp,pln,preprocesamiento,preprocess,spanish
 Classifier: Development Status :: 3 - Alpha
@@ -103,14 +103,15 @@
 ```
 ### Classification
 
 See more information in the [Jupyter Notebook example](https://github.com/jorgeortizfuentes/spanish_nlp/blob/main/examples/Classify.ipynb)
 #### Available classifiers
 
 * Hate Speech (hate_speech)
+* Incivility (incivility)
 * Toxic Speech (toxic_speech)
 * Sentiment Analysis (sentiment_analysis)
 * Emotion Analysis (emotion_analysis)
 * Irony Analysis (irony_analysis)
 * Sexist Analysis (sexist_analysis)
 * Racism Analysis (racism_analysis)
 
@@ -144,18 +145,24 @@
 ### Augmentation
 
 See more information in the [Jupyter Notebook example](https://github.com/jorgeortizfuentes/spanish_nlp/blob/main/examples/Data%20Augmentation.ipynb)
 
 #### Available Augmentation Models
 
 - Spelling augmentation
-  - Keyboard method
-  - OCR method
-  - Random method
-  - Orthography method
+  - Keyboard spelling method
+  - OCR spelling method
+  - Random spelling replace method
+  - Grapheme spelling
+  - Word spelling
+  - Remove punctuation
+  - Remove accents
+  - Lowercase
+  - Uppercase
+  - Randomcase
   - All method
 - Masked augmentation
   - Sustitute method
   - Insert method
 - Others models under development (such as Synonyms, WordEmbeddings, GenerativeOpenSource, GenerativeOpenAI, BackTranslation, AbstractiveSummarization)
 
 
@@ -218,8 +225,8 @@
 
 ## Acknowledgements
 
 We would like to express our gratitude to the Millennium Institute For Foundational Research and Department of Computer Science at the University of Chile for supporting the development of Spanish NLP. Special thanks to Felipe Bravo-Marquéz, Ricardo Cordova and Hernán Sarmiento for their knowledge, support and invaluable contribution to the project.
 
 ## Contributing
 
-Contributions to Spanish NLP are welcome! Please see the [contributing guide](https://github.com/users/jorgeortizfuentes/projects/1) for more information.
+Contributions to Spanish NLP are welcome! Please see the [contributing guide](https://github.com/users/jorgeortizfuentes/projects/1) for more information.
```

