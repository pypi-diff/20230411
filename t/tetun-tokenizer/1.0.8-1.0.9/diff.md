# Comparing `tmp/tetun_tokenizer-1.0.8.tar.gz` & `tmp/tetun_tokenizer-1.0.9.tar.gz`

## Comparing `tetun_tokenizer-1.0.8.tar` & `tetun_tokenizer-1.0.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 tetun_tokenizer-1.0.8/.DS_Store
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 tetun_tokenizer-1.0.8/Pipfile
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 tetun_tokenizer-1.0.8/Pipfile.lock
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 tetun_tokenizer-1.0.8/_token
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tetun_tokenizer-1.0.8/tetuntokenizer/__init__.py
--rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 tetun_tokenizer-1.0.8/tetuntokenizer/tokenizer.py
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 tetun_tokenizer-1.0.8/LICENSE
--rw-r--r--   0        0        0     5080 2020-02-02 00:00:00.000000 tetun_tokenizer-1.0.8/README.md
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 tetun_tokenizer-1.0.8/pyproject.toml
--rw-r--r--   0        0        0     5458 2020-02-02 00:00:00.000000 tetun_tokenizer-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 tetun_tokenizer-1.0.9/.DS_Store
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 tetun_tokenizer-1.0.9/Pipfile
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 tetun_tokenizer-1.0.9/Pipfile.lock
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 tetun_tokenizer-1.0.9/_token
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tetun_tokenizer-1.0.9/tetuntokenizer/__init__.py
+-rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 tetun_tokenizer-1.0.9/tetuntokenizer/tokenizer.py
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 tetun_tokenizer-1.0.9/LICENSE
+-rw-r--r--   0        0        0     5078 2020-02-02 00:00:00.000000 tetun_tokenizer-1.0.9/README.md
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 tetun_tokenizer-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0     5456 2020-02-02 00:00:00.000000 tetun_tokenizer-1.0.9/PKG-INFO
```

### Comparing `tetun_tokenizer-1.0.8/.DS_Store` & `tetun_tokenizer-1.0.9/.DS_Store`

 * *Files identical despite different names*

### Comparing `tetun_tokenizer-1.0.8/Pipfile.lock` & `tetun_tokenizer-1.0.9/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `tetun_tokenizer-1.0.8/tetuntokenizer/tokenizer.py` & `tetun_tokenizer-1.0.9/tetuntokenizer/tokenizer.py`

 * *Files identical despite different names*

### Comparing `tetun_tokenizer-1.0.8/LICENSE` & `tetun_tokenizer-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tetun_tokenizer-1.0.8/README.md` & `tetun_tokenizer-1.0.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -68,23 +68,23 @@
 3. Using `TetunSentenceTokenizer()` to tokenize a given text.
 
 ```python
 from tetuntokenizer.tokenizer import TetunSentenceTokenizer
 
 tetun_tokenizer = TetunSentenceTokenizer()
 
-text = "Ha'u ema-ida ne'ebé baibain de'it. Tebes ká? Ita-nia maluk Dr. ka Ph.D sira hosi U.S.A mós dehan!"
+text = "Ha'u ema-ida ne'ebé baibain de'it. Tebes ga? Ita-nia maluk Dr. ka Ph.D sira hosi U.S.A mós dehan!"
 output = tetun_tokenizer.tokenize(text)
 print(output)
 ```
 
 The output will be:
 
 ```
-["Ha'u ema-ida ne'ebé baibain de'it.", 'Tebes ká?', 'Ita-nia maluk Dr. ka Ph.D sira hosi U.S.A mós dehan!']
+["Ha'u ema-ida ne'ebé baibain de'it.", 'Tebes ga?', 'Ita-nia maluk Dr. ka Ph.D sira hosi U.S.A mós dehan!']
 ```
 
 4. Using `TetunBlankLineTokenizer()` to tokenize a given text.
 
 ```python
 from tetuntokenizer.tokenizer import TetunBlankLineTokenizer
```

### Comparing `tetun_tokenizer-1.0.8/PKG-INFO` & `tetun_tokenizer-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tetun_tokenizer
-Version: 1.0.8
+Version: 1.0.9
 Summary: Tetun tokenizer
 Author-email: Gabriel de Jesus <gabriel.dejesus@timornews.tl>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
@@ -80,23 +80,23 @@
 3. Using `TetunSentenceTokenizer()` to tokenize a given text.
 
 ```python
 from tetuntokenizer.tokenizer import TetunSentenceTokenizer
 
 tetun_tokenizer = TetunSentenceTokenizer()
 
-text = "Ha'u ema-ida ne'ebé baibain de'it. Tebes ká? Ita-nia maluk Dr. ka Ph.D sira hosi U.S.A mós dehan!"
+text = "Ha'u ema-ida ne'ebé baibain de'it. Tebes ga? Ita-nia maluk Dr. ka Ph.D sira hosi U.S.A mós dehan!"
 output = tetun_tokenizer.tokenize(text)
 print(output)
 ```
 
 The output will be:
 
 ```
-["Ha'u ema-ida ne'ebé baibain de'it.", 'Tebes ká?', 'Ita-nia maluk Dr. ka Ph.D sira hosi U.S.A mós dehan!']
+["Ha'u ema-ida ne'ebé baibain de'it.", 'Tebes ga?', 'Ita-nia maluk Dr. ka Ph.D sira hosi U.S.A mós dehan!']
 ```
 
 4. Using `TetunBlankLineTokenizer()` to tokenize a given text.
 
 ```python
 from tetuntokenizer.tokenizer import TetunBlankLineTokenizer
```

