# Comparing `tmp/jupyter_ai_chatgpt-0.4.0.tar.gz` & `tmp/jupyter_ai_chatgpt-0.5.0.tar.gz`

## Comparing `jupyter_ai_chatgpt-0.4.0.tar` & `jupyter_ai_chatgpt-0.5.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 jupyter_ai_chatgpt-0.4.0/.eslintignore
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 jupyter_ai_chatgpt-0.4.0/.eslintrc.js
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyter_ai_chatgpt-0.4.0/.prettierignore
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 jupyter_ai_chatgpt-0.4.0/.prettierrc
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 jupyter_ai_chatgpt-0.4.0/.stylelintrc
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyter_ai_chatgpt-0.4.0/babel.config.js
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 jupyter_ai_chatgpt-0.4.0/install.json
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 jupyter_ai_chatgpt-0.4.0/jest.config.js
--rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 jupyter_ai_chatgpt-0.4.0/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyter_ai_chatgpt-0.4.0/setup.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 jupyter_ai_chatgpt-0.4.0/tsconfig.json
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 jupyter_ai_chatgpt-0.4.0/jupyter_ai_chatgpt/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyter_ai_chatgpt-0.4.0/jupyter_ai_chatgpt/_version.py
--rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 jupyter_ai_chatgpt-0.4.0/jupyter_ai_chatgpt/engine.py
--rw-r--r--   0        0        0     3607 2020-02-02 00:00:00.000000 jupyter_ai_chatgpt-0.4.0/jupyter_ai_chatgpt/labextension/package.json
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 jupyter_ai_chatgpt-0.4.0/jupyter_ai_chatgpt/labextension/static/568.58d646ba30ad5cce43b0.js
--rw-r--r--   0        0        0     3512 2020-02-02 00:00:00.000000 jupyter_ai_chatgpt-0.4.0/jupyter_ai_chatgpt/labextension/static/643.c1827be98afe184c4f03.js
--rw-r--r--   0        0        0     3904 2020-02-02 00:00:00.000000 jupyter_ai_chatgpt-0.4.0/jupyter_ai_chatgpt/labextension/static/remoteEntry.ec582f0e83f6f33ab335.js
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 jupyter_ai_chatgpt-0.4.0/jupyter_ai_chatgpt/labextension/static/style.js
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 jupyter_ai_chatgpt-0.4.0/jupyter_ai_chatgpt/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 jupyter_ai_chatgpt-0.4.0/jupyter_ai_chatgpt/tests/__init__.py
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 jupyter_ai_chatgpt-0.4.0/src/index.ts
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 jupyter_ai_chatgpt-0.4.0/src/__tests__/jupyter_ai_chatgpt.spec.ts
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 jupyter_ai_chatgpt-0.4.0/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyter_ai_chatgpt-0.4.0/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyter_ai_chatgpt-0.4.0/style/index.js
--rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 jupyter_ai_chatgpt-0.4.0/ui-tests/README.md
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 jupyter_ai_chatgpt-0.4.0/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 jupyter_ai_chatgpt-0.4.0/ui-tests/package.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyter_ai_chatgpt-0.4.0/ui-tests/playwright.config.js
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 jupyter_ai_chatgpt-0.4.0/ui-tests/tests/jupyter_ai_chatgpt.spec.ts
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 jupyter_ai_chatgpt-0.4.0/.gitignore
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 jupyter_ai_chatgpt-0.4.0/LICENSE
--rw-r--r--   0        0        0     3416 2020-02-02 00:00:00.000000 jupyter_ai_chatgpt-0.4.0/README.md
--rw-r--r--   0        0        0     2601 2020-02-02 00:00:00.000000 jupyter_ai_chatgpt-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     6527 2020-02-02 00:00:00.000000 jupyter_ai_chatgpt-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 jupyter_ai_chatgpt-0.5.0/.eslintignore
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 jupyter_ai_chatgpt-0.5.0/.eslintrc.js
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyter_ai_chatgpt-0.5.0/.prettierignore
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 jupyter_ai_chatgpt-0.5.0/.prettierrc
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 jupyter_ai_chatgpt-0.5.0/.stylelintrc
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyter_ai_chatgpt-0.5.0/babel.config.js
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 jupyter_ai_chatgpt-0.5.0/install.json
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 jupyter_ai_chatgpt-0.5.0/jest.config.js
+-rw-r--r--   0        0        0     3547 2020-02-02 00:00:00.000000 jupyter_ai_chatgpt-0.5.0/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyter_ai_chatgpt-0.5.0/setup.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 jupyter_ai_chatgpt-0.5.0/tsconfig.json
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 jupyter_ai_chatgpt-0.5.0/jupyter_ai_chatgpt/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyter_ai_chatgpt-0.5.0/jupyter_ai_chatgpt/_version.py
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 jupyter_ai_chatgpt-0.5.0/jupyter_ai_chatgpt/engine.py
+-rw-r--r--   0        0        0     3689 2020-02-02 00:00:00.000000 jupyter_ai_chatgpt-0.5.0/jupyter_ai_chatgpt/labextension/package.json
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 jupyter_ai_chatgpt-0.5.0/jupyter_ai_chatgpt/labextension/static/568.58d646ba30ad5cce43b0.js
+-rw-r--r--   0        0        0     3512 2020-02-02 00:00:00.000000 jupyter_ai_chatgpt-0.5.0/jupyter_ai_chatgpt/labextension/static/643.c1827be98afe184c4f03.js
+-rw-r--r--   0        0        0     3904 2020-02-02 00:00:00.000000 jupyter_ai_chatgpt-0.5.0/jupyter_ai_chatgpt/labextension/static/remoteEntry.ee237f1652f3483ec858.js
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 jupyter_ai_chatgpt-0.5.0/jupyter_ai_chatgpt/labextension/static/style.js
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 jupyter_ai_chatgpt-0.5.0/jupyter_ai_chatgpt/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 jupyter_ai_chatgpt-0.5.0/jupyter_ai_chatgpt/tests/__init__.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 jupyter_ai_chatgpt-0.5.0/src/index.ts
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 jupyter_ai_chatgpt-0.5.0/src/__tests__/jupyter_ai_chatgpt.spec.ts
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 jupyter_ai_chatgpt-0.5.0/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyter_ai_chatgpt-0.5.0/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyter_ai_chatgpt-0.5.0/style/index.js
+-rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 jupyter_ai_chatgpt-0.5.0/ui-tests/README.md
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 jupyter_ai_chatgpt-0.5.0/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 jupyter_ai_chatgpt-0.5.0/ui-tests/package.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyter_ai_chatgpt-0.5.0/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 jupyter_ai_chatgpt-0.5.0/ui-tests/tests/jupyter_ai_chatgpt.spec.ts
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 jupyter_ai_chatgpt-0.5.0/.gitignore
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 jupyter_ai_chatgpt-0.5.0/LICENSE
+-rw-r--r--   0        0        0     3416 2020-02-02 00:00:00.000000 jupyter_ai_chatgpt-0.5.0/README.md
+-rw-r--r--   0        0        0     2601 2020-02-02 00:00:00.000000 jupyter_ai_chatgpt-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     6527 2020-02-02 00:00:00.000000 jupyter_ai_chatgpt-0.5.0/PKG-INFO
```

### Comparing `jupyter_ai_chatgpt-0.4.0/.eslintrc.js` & `jupyter_ai_chatgpt-0.5.0/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai_chatgpt-0.4.0/jest.config.js` & `jupyter_ai_chatgpt-0.5.0/jest.config.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai_chatgpt-0.4.0/package.json` & `jupyter_ai_chatgpt-0.5.0/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9716540404040405%*

 * *Differences: {"'devDependencies'": "{'@jupyter-ai/core': '^0.5.0'}",*

 * * "'scripts'": "{'dev-install': 'pip install -e . && jupyter labextension develop . --overwrite && "*

 * *              "jupyter server extension enable jupyter_ai_chatgpt', 'dev-uninstall': 'pip "*

 * *              "uninstall jupyter_ai_chatgpt -y', delete: ['setup:dev']}",*

 * * "'version'": "'0.5.0'"}*

```diff
@@ -10,15 +10,15 @@
     "dependencies": {
         "@jupyterlab/application": "^3.1.0"
     },
     "description": "Jupyter AI module that provides a ChatGPT model engine.",
     "devDependencies": {
         "@babel/core": "^7.0.0",
         "@babel/preset-env": "^7.0.0",
-        "@jupyter-ai/core": "^0.4.0",
+        "@jupyter-ai/core": "^0.5.0",
         "@jupyterlab/builder": "^3.1.0",
         "@jupyterlab/testutils": "^3.0.0",
         "@types/jest": "^26.0.0",
         "@typescript-eslint/eslint-plugin": "^4.8.1",
         "@typescript-eslint/parser": "^4.8.1",
         "eslint": "^7.14.0",
         "eslint-config-prettier": "^6.15.0",
@@ -66,32 +66,33 @@
         "build:lib": "tsc",
         "build:prod": "jlpm clean && jlpm build:lib && jlpm build:labextension",
         "clean": "jlpm clean:lib",
         "clean:all": "jlpm clean:lib && jlpm clean:labextension && jlpm clean:lintcache",
         "clean:labextension": "rimraf jupyter_ai_chatgpt/labextension jupyter_ai_chatgpt/_version.py",
         "clean:lib": "rimraf lib tsconfig.tsbuildinfo",
         "clean:lintcache": "rimraf .eslintcache .stylelintcache",
+        "dev-install": "pip install -e . && jupyter labextension develop . --overwrite && jupyter server extension enable jupyter_ai_chatgpt",
+        "dev-uninstall": "pip uninstall jupyter_ai_chatgpt -y",
         "eslint": "jlpm eslint:check --fix",
         "eslint:check": "eslint . --cache --ext .ts,.tsx",
         "install:extension": "jlpm build",
         "lint": "jlpm stylelint && jlpm prettier && jlpm eslint",
         "lint:check": "jlpm stylelint:check && jlpm prettier:check && jlpm eslint:check",
         "prettier": "jlpm prettier:base --write --list-different",
         "prettier:base": "prettier \"**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}\"",
         "prettier:check": "jlpm prettier:base --check",
-        "setup:dev": "jupyter labextension develop . --overwrite && jupyter server extension enable jupyter_ai_chatgpt",
         "stylelint": "jlpm stylelint:check --fix",
         "stylelint:check": "stylelint --cache \"style/**/*.css\"",
         "test": "jest --coverage",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.4.0"
+    "version": "0.5.0"
 }
```

### Comparing `jupyter_ai_chatgpt-0.4.0/tsconfig.json` & `jupyter_ai_chatgpt-0.5.0/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyter_ai_chatgpt-0.4.0/jupyter_ai_chatgpt/engine.py` & `jupyter_ai_chatgpt-0.5.0/jupyter_ai_chatgpt/engine.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai_chatgpt-0.4.0/jupyter_ai_chatgpt/labextension/package.json` & `jupyter_ai_chatgpt-0.5.0/jupyter_ai_chatgpt/labextension/package.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.970959595959596%*

 * *Differences: {"'devDependencies'": "{'@jupyter-ai/core': '^0.5.0'}",*

 * * "'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.ee237f1652f3483ec858.js'}}",*

 * * "'scripts'": "{'dev-install': 'pip install -e . && jupyter labextension develop . --overwrite && "*

 * *              "jupyter server extension enable jupyter_ai_chatgpt', 'dev-uninstall': 'pip "*

 * *              "uninstall jupyter_ai_chatgpt -y', delete: ['setup:dev']}",*

 * * "'version'": "'0.5.0'"}*

```diff
@@ -10,15 +10,15 @@
     "dependencies": {
         "@jupyterlab/application": "^3.1.0"
     },
     "description": "Jupyter AI module that provides a ChatGPT model engine.",
     "devDependencies": {
         "@babel/core": "^7.0.0",
         "@babel/preset-env": "^7.0.0",
-        "@jupyter-ai/core": "^0.4.0",
+        "@jupyter-ai/core": "^0.5.0",
         "@jupyterlab/builder": "^3.1.0",
         "@jupyterlab/testutils": "^3.0.0",
         "@types/jest": "^26.0.0",
         "@typescript-eslint/eslint-plugin": "^4.8.1",
         "@typescript-eslint/parser": "^4.8.1",
         "eslint": "^7.14.0",
         "eslint-config-prettier": "^6.15.0",
@@ -39,15 +39,15 @@
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/jupyterlab/jupyter-ai",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.ec582f0e83f6f33ab335.js",
+            "load": "static/remoteEntry.ee237f1652f3483ec858.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "jupyter_ai_chatgpt/labextension"
     },
     "keywords": [
         "jupyter",
@@ -71,32 +71,33 @@
         "build:lib": "tsc",
         "build:prod": "jlpm clean && jlpm build:lib && jlpm build:labextension",
         "clean": "jlpm clean:lib",
         "clean:all": "jlpm clean:lib && jlpm clean:labextension && jlpm clean:lintcache",
         "clean:labextension": "rimraf jupyter_ai_chatgpt/labextension jupyter_ai_chatgpt/_version.py",
         "clean:lib": "rimraf lib tsconfig.tsbuildinfo",
         "clean:lintcache": "rimraf .eslintcache .stylelintcache",
+        "dev-install": "pip install -e . && jupyter labextension develop . --overwrite && jupyter server extension enable jupyter_ai_chatgpt",
+        "dev-uninstall": "pip uninstall jupyter_ai_chatgpt -y",
         "eslint": "jlpm eslint:check --fix",
         "eslint:check": "eslint . --cache --ext .ts,.tsx",
         "install:extension": "jlpm build",
         "lint": "jlpm stylelint && jlpm prettier && jlpm eslint",
         "lint:check": "jlpm stylelint:check && jlpm prettier:check && jlpm eslint:check",
         "prettier": "jlpm prettier:base --write --list-different",
         "prettier:base": "prettier \"**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}\"",
         "prettier:check": "jlpm prettier:base --check",
-        "setup:dev": "jupyter labextension develop . --overwrite && jupyter server extension enable jupyter_ai_chatgpt",
         "stylelint": "jlpm stylelint:check --fix",
         "stylelint:check": "stylelint --cache \"style/**/*.css\"",
         "test": "jest --coverage",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.4.0"
+    "version": "0.5.0"
 }
```

### Comparing `jupyter_ai_chatgpt-0.4.0/jupyter_ai_chatgpt/labextension/static/643.c1827be98afe184c4f03.js` & `jupyter_ai_chatgpt-0.5.0/jupyter_ai_chatgpt/labextension/static/643.c1827be98afe184c4f03.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai_chatgpt-0.4.0/jupyter_ai_chatgpt/labextension/static/remoteEntry.ec582f0e83f6f33ab335.js` & `jupyter_ai_chatgpt-0.5.0/jupyter_ai_chatgpt/labextension/static/remoteEntry.ee237f1652f3483ec858.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -106,15 +106,15 @@
                     var n = i[e] = i[e] || {},
                         l = n[t];
                     (!l || !l.loaded && (1 != !l.eager ? a : u > l.from)) && (n[t] = {
                         get: () => o.e(568).then((() => () => o(568))),
                         from: u,
                         eager: !1
                     })
-                })("@jupyter-ai/chatgpt", "0.4.0"), e[r] = l.length ? Promise.all(l).then((() => e[r] = 1)) : 1
+                })("@jupyter-ai/chatgpt", "0.5.0"), e[r] = l.length ? Promise.all(l).then((() => e[r] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         o.g.importScripts && (e = o.g.location + "");
         var t = o.g.document;
         if (!e && t && (t.currentScript && (e = t.currentScript.src), !e)) {
```

### Comparing `jupyter_ai_chatgpt-0.4.0/jupyter_ai_chatgpt/labextension/static/third-party-licenses.json` & `jupyter_ai_chatgpt-0.5.0/jupyter_ai_chatgpt/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyter_ai_chatgpt-0.4.0/ui-tests/README.md` & `jupyter_ai_chatgpt-0.5.0/ui-tests/README.md`

 * *Files identical despite different names*

### Comparing `jupyter_ai_chatgpt-0.4.0/ui-tests/jupyter_server_test_config.py` & `jupyter_ai_chatgpt-0.5.0/ui-tests/jupyter_server_test_config.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai_chatgpt-0.4.0/ui-tests/tests/jupyter_ai_chatgpt.spec.ts` & `jupyter_ai_chatgpt-0.5.0/ui-tests/tests/jupyter_ai_chatgpt.spec.ts`

 * *Files identical despite different names*

### Comparing `jupyter_ai_chatgpt-0.4.0/.gitignore` & `jupyter_ai_chatgpt-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyter_ai_chatgpt-0.4.0/LICENSE` & `jupyter_ai_chatgpt-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_ai_chatgpt-0.4.0/README.md` & `jupyter_ai_chatgpt-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `jupyter_ai_chatgpt-0.4.0/pyproject.toml` & `jupyter_ai_chatgpt-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyter_ai_chatgpt-0.4.0/PKG-INFO` & `jupyter_ai_chatgpt-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter_ai_chatgpt
-Version: 0.4.0
+Version: 0.5.0
 Summary: Jupyter AI module that provides a ChatGPT model engine.
 Project-URL: Homepage, https://github.com/jupyterlab/jupyter-ai
 Project-URL: Bug Tracker, https://github.com/jupyterlab/jupyter-ai/issues
 Project-URL: Repository, https://github.com/jupyterlab/jupyter-ai.git
 Author-email: Project Jupyter <jupyter@googlegroups.com>
 License: BSD 3-Clause License
```

