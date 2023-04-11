# Comparing `tmp/jupyter_ai_dalle-0.4.0.tar.gz` & `tmp/jupyter_ai_dalle-0.5.0.tar.gz`

## Comparing `jupyter_ai_dalle-0.4.0.tar` & `jupyter_ai_dalle-0.5.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 jupyter_ai_dalle-0.4.0/.eslintignore
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 jupyter_ai_dalle-0.4.0/.eslintrc.js
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 jupyter_ai_dalle-0.4.0/.prettierignore
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 jupyter_ai_dalle-0.4.0/.prettierrc
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 jupyter_ai_dalle-0.4.0/.stylelintrc
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyter_ai_dalle-0.4.0/babel.config.js
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 jupyter_ai_dalle-0.4.0/install.json
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 jupyter_ai_dalle-0.4.0/jest.config.js
--rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 jupyter_ai_dalle-0.4.0/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyter_ai_dalle-0.4.0/setup.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 jupyter_ai_dalle-0.4.0/tsconfig.json
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 jupyter_ai_dalle-0.4.0/jupyter_ai_dalle/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyter_ai_dalle-0.4.0/jupyter_ai_dalle/_version.py
--rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 jupyter_ai_dalle-0.4.0/jupyter_ai_dalle/engine.py
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 jupyter_ai_dalle-0.4.0/jupyter_ai_dalle/tasks.py
--rw-r--r--   0        0        0     3623 2020-02-02 00:00:00.000000 jupyter_ai_dalle-0.4.0/jupyter_ai_dalle/labextension/package.json
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 jupyter_ai_dalle-0.4.0/jupyter_ai_dalle/labextension/static/568.360c80aecf15fb74bd5d.js
--rw-r--r--   0        0        0     3508 2020-02-02 00:00:00.000000 jupyter_ai_dalle-0.4.0/jupyter_ai_dalle/labextension/static/643.9e0e6dc147127c5f5b07.js
--rw-r--r--   0        0        0     6353 2020-02-02 00:00:00.000000 jupyter_ai_dalle-0.4.0/jupyter_ai_dalle/labextension/static/remoteEntry.2a61b3d6ed7e5b7aa159.js
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 jupyter_ai_dalle-0.4.0/jupyter_ai_dalle/labextension/static/style.js
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 jupyter_ai_dalle-0.4.0/jupyter_ai_dalle/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 jupyter_ai_dalle-0.4.0/jupyter_ai_dalle/tests/__init__.py
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 jupyter_ai_dalle-0.4.0/src/index.ts
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 jupyter_ai_dalle-0.4.0/src/__tests__/jupyter_ai_dalle.spec.ts
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 jupyter_ai_dalle-0.4.0/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyter_ai_dalle-0.4.0/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyter_ai_dalle-0.4.0/style/index.js
--rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 jupyter_ai_dalle-0.4.0/ui-tests/README.md
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 jupyter_ai_dalle-0.4.0/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 jupyter_ai_dalle-0.4.0/ui-tests/package.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyter_ai_dalle-0.4.0/ui-tests/playwright.config.js
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 jupyter_ai_dalle-0.4.0/ui-tests/tests/jupyter_ai_dalle.spec.ts
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 jupyter_ai_dalle-0.4.0/.gitignore
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 jupyter_ai_dalle-0.4.0/LICENSE
--rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 jupyter_ai_dalle-0.4.0/README.md
--rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 jupyter_ai_dalle-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     6559 2020-02-02 00:00:00.000000 jupyter_ai_dalle-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 jupyter_ai_dalle-0.5.0/.eslintignore
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 jupyter_ai_dalle-0.5.0/.eslintrc.js
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 jupyter_ai_dalle-0.5.0/.prettierignore
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 jupyter_ai_dalle-0.5.0/.prettierrc
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 jupyter_ai_dalle-0.5.0/.stylelintrc
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyter_ai_dalle-0.5.0/babel.config.js
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 jupyter_ai_dalle-0.5.0/install.json
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 jupyter_ai_dalle-0.5.0/jest.config.js
+-rw-r--r--   0        0        0     3555 2020-02-02 00:00:00.000000 jupyter_ai_dalle-0.5.0/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyter_ai_dalle-0.5.0/setup.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 jupyter_ai_dalle-0.5.0/tsconfig.json
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 jupyter_ai_dalle-0.5.0/jupyter_ai_dalle/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyter_ai_dalle-0.5.0/jupyter_ai_dalle/_version.py
+-rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 jupyter_ai_dalle-0.5.0/jupyter_ai_dalle/engine.py
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 jupyter_ai_dalle-0.5.0/jupyter_ai_dalle/tasks.py
+-rw-r--r--   0        0        0     3697 2020-02-02 00:00:00.000000 jupyter_ai_dalle-0.5.0/jupyter_ai_dalle/labextension/package.json
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 jupyter_ai_dalle-0.5.0/jupyter_ai_dalle/labextension/static/568.360c80aecf15fb74bd5d.js
+-rw-r--r--   0        0        0     3508 2020-02-02 00:00:00.000000 jupyter_ai_dalle-0.5.0/jupyter_ai_dalle/labextension/static/643.9e0e6dc147127c5f5b07.js
+-rw-r--r--   0        0        0     6353 2020-02-02 00:00:00.000000 jupyter_ai_dalle-0.5.0/jupyter_ai_dalle/labextension/static/remoteEntry.5f267942fa0b6ca3ba8e.js
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 jupyter_ai_dalle-0.5.0/jupyter_ai_dalle/labextension/static/style.js
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 jupyter_ai_dalle-0.5.0/jupyter_ai_dalle/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 jupyter_ai_dalle-0.5.0/jupyter_ai_dalle/tests/__init__.py
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 jupyter_ai_dalle-0.5.0/src/index.ts
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 jupyter_ai_dalle-0.5.0/src/__tests__/jupyter_ai_dalle.spec.ts
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 jupyter_ai_dalle-0.5.0/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyter_ai_dalle-0.5.0/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyter_ai_dalle-0.5.0/style/index.js
+-rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 jupyter_ai_dalle-0.5.0/ui-tests/README.md
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 jupyter_ai_dalle-0.5.0/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 jupyter_ai_dalle-0.5.0/ui-tests/package.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyter_ai_dalle-0.5.0/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 jupyter_ai_dalle-0.5.0/ui-tests/tests/jupyter_ai_dalle.spec.ts
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 jupyter_ai_dalle-0.5.0/.gitignore
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 jupyter_ai_dalle-0.5.0/LICENSE
+-rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 jupyter_ai_dalle-0.5.0/README.md
+-rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 jupyter_ai_dalle-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     6559 2020-02-02 00:00:00.000000 jupyter_ai_dalle-0.5.0/PKG-INFO
```

### Comparing `jupyter_ai_dalle-0.4.0/.eslintrc.js` & `jupyter_ai_dalle-0.5.0/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai_dalle-0.4.0/jest.config.js` & `jupyter_ai_dalle-0.5.0/jest.config.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai_dalle-0.4.0/package.json` & `jupyter_ai_dalle-0.5.0/package.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9716540404040405%*

 * *Differences: {"'devDependencies'": "{'@jupyter-ai/core': '^0.5.0'}",*

 * * "'scripts'": "{'dev-install': 'pip install -e . && jupyter labextension develop . --overwrite && "*

 * *              "jupyter server extension enable jupyter_ai', 'dev-uninstall': 'pip uninstall "*

 * *              "jupyter_ai_dalle -y', delete: ['setup:dev']}",*

 * * "'version'": "'0.5.0'"}*

```diff
@@ -10,15 +10,15 @@
     "dependencies": {
         "@jupyterlab/application": "^3.1.0"
     },
     "description": "A JupyterLab extension that adds a DALL-E model engine and image insertion modes.",
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
         "clean:labextension": "rimraf jupyter_ai_dalle/labextension jupyter_ai_dalle/_version.py",
         "clean:lib": "rimraf lib tsconfig.tsbuildinfo",
         "clean:lintcache": "rimraf .eslintcache .stylelintcache",
+        "dev-install": "pip install -e . && jupyter labextension develop . --overwrite && jupyter server extension enable jupyter_ai",
+        "dev-uninstall": "pip uninstall jupyter_ai_dalle -y",
         "eslint": "jlpm eslint:check --fix",
         "eslint:check": "eslint . --cache --ext .ts,.tsx",
         "install:extension": "jlpm build",
         "lint": "jlpm stylelint && jlpm prettier && jlpm eslint",
         "lint:check": "jlpm stylelint:check && jlpm prettier:check && jlpm eslint:check",
         "prettier": "jlpm prettier:base --write --list-different",
         "prettier:base": "prettier \"**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}\"",
         "prettier:check": "jlpm prettier:base --check",
-        "setup:dev": "jupyter labextension develop . --overwrite && jupyter server extension enable jupyter_ai_dalle",
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

### Comparing `jupyter_ai_dalle-0.4.0/tsconfig.json` & `jupyter_ai_dalle-0.5.0/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyter_ai_dalle-0.4.0/jupyter_ai_dalle/engine.py` & `jupyter_ai_dalle-0.5.0/jupyter_ai_dalle/engine.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai_dalle-0.4.0/jupyter_ai_dalle/tasks.py` & `jupyter_ai_dalle-0.5.0/jupyter_ai_dalle/tasks.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai_dalle-0.4.0/jupyter_ai_dalle/labextension/package.json` & `jupyter_ai_dalle-0.5.0/jupyter_ai_dalle/labextension/package.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.970959595959596%*

 * *Differences: {"'devDependencies'": "{'@jupyter-ai/core': '^0.5.0'}",*

 * * "'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.5f267942fa0b6ca3ba8e.js'}}",*

 * * "'scripts'": "{'dev-install': 'pip install -e . && jupyter labextension develop . --overwrite && "*

 * *              "jupyter server extension enable jupyter_ai', 'dev-uninstall': 'pip uninstall "*

 * *              "jupyter_ai_dalle -y', delete: ['setup:dev']}",*

 * * "'version'": "'0.5.0'"}*

```diff
@@ -10,15 +10,15 @@
     "dependencies": {
         "@jupyterlab/application": "^3.1.0"
     },
     "description": "A JupyterLab extension that adds a DALL-E model engine and image insertion modes.",
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
-            "load": "static/remoteEntry.2a61b3d6ed7e5b7aa159.js",
+            "load": "static/remoteEntry.5f267942fa0b6ca3ba8e.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "jupyter_ai_dalle/labextension"
     },
     "keywords": [
         "jupyter",
@@ -71,32 +71,33 @@
         "build:lib": "tsc",
         "build:prod": "jlpm clean && jlpm build:lib && jlpm build:labextension",
         "clean": "jlpm clean:lib",
         "clean:all": "jlpm clean:lib && jlpm clean:labextension && jlpm clean:lintcache",
         "clean:labextension": "rimraf jupyter_ai_dalle/labextension jupyter_ai_dalle/_version.py",
         "clean:lib": "rimraf lib tsconfig.tsbuildinfo",
         "clean:lintcache": "rimraf .eslintcache .stylelintcache",
+        "dev-install": "pip install -e . && jupyter labextension develop . --overwrite && jupyter server extension enable jupyter_ai",
+        "dev-uninstall": "pip uninstall jupyter_ai_dalle -y",
         "eslint": "jlpm eslint:check --fix",
         "eslint:check": "eslint . --cache --ext .ts,.tsx",
         "install:extension": "jlpm build",
         "lint": "jlpm stylelint && jlpm prettier && jlpm eslint",
         "lint:check": "jlpm stylelint:check && jlpm prettier:check && jlpm eslint:check",
         "prettier": "jlpm prettier:base --write --list-different",
         "prettier:base": "prettier \"**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}\"",
         "prettier:check": "jlpm prettier:base --check",
-        "setup:dev": "jupyter labextension develop . --overwrite && jupyter server extension enable jupyter_ai_dalle",
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

### Comparing `jupyter_ai_dalle-0.4.0/jupyter_ai_dalle/labextension/static/568.360c80aecf15fb74bd5d.js` & `jupyter_ai_dalle-0.5.0/jupyter_ai_dalle/labextension/static/568.360c80aecf15fb74bd5d.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai_dalle-0.4.0/jupyter_ai_dalle/labextension/static/643.9e0e6dc147127c5f5b07.js` & `jupyter_ai_dalle-0.5.0/jupyter_ai_dalle/labextension/static/643.9e0e6dc147127c5f5b07.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai_dalle-0.4.0/jupyter_ai_dalle/labextension/static/remoteEntry.2a61b3d6ed7e5b7aa159.js` & `jupyter_ai_dalle-0.5.0/jupyter_ai_dalle/labextension/static/remoteEntry.5f267942fa0b6ca3ba8e.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -106,15 +106,15 @@
                     var o = a[e] = a[e] || {},
                         u = o[r];
                     (!u || !u.loaded && (1 != !u.eager ? n : i > u.from)) && (o[r] = {
                         get: () => b.e(568).then((() => () => b(568))),
                         from: i,
                         eager: !1
                     })
-                })("@jupyter-ai/dalle", "0.4.0"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                })("@jupyter-ai/dalle", "0.5.0"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         b.g.importScripts && (e = b.g.location + "");
         var r = b.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
```

### Comparing `jupyter_ai_dalle-0.4.0/jupyter_ai_dalle/labextension/static/third-party-licenses.json` & `jupyter_ai_dalle-0.5.0/jupyter_ai_dalle/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyter_ai_dalle-0.4.0/src/index.ts` & `jupyter_ai_dalle-0.5.0/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyter_ai_dalle-0.4.0/ui-tests/README.md` & `jupyter_ai_dalle-0.5.0/ui-tests/README.md`

 * *Files identical despite different names*

### Comparing `jupyter_ai_dalle-0.4.0/ui-tests/jupyter_server_test_config.py` & `jupyter_ai_dalle-0.5.0/ui-tests/jupyter_server_test_config.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai_dalle-0.4.0/ui-tests/tests/jupyter_ai_dalle.spec.ts` & `jupyter_ai_dalle-0.5.0/ui-tests/tests/jupyter_ai_dalle.spec.ts`

 * *Files identical despite different names*

### Comparing `jupyter_ai_dalle-0.4.0/.gitignore` & `jupyter_ai_dalle-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyter_ai_dalle-0.4.0/LICENSE` & `jupyter_ai_dalle-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_ai_dalle-0.4.0/README.md` & `jupyter_ai_dalle-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `jupyter_ai_dalle-0.4.0/pyproject.toml` & `jupyter_ai_dalle-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyter_ai_dalle-0.4.0/PKG-INFO` & `jupyter_ai_dalle-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter_ai_dalle
-Version: 0.4.0
+Version: 0.5.0
 Summary: A JupyterLab extension that adds a DALL-E model engine and image insertion modes.
 Project-URL: Homepage, https://github.com/jupyterlab/jupyter-ai
 Project-URL: Bug Tracker, https://github.com/jupyterlab/jupyter-ai/issues
 Project-URL: Repository, https://github.com/jupyterlab/jupyter-ai.git
 Author-email: Project Jupyter <jupyter@googlegroups.com>
 License: BSD 3-Clause License
```

