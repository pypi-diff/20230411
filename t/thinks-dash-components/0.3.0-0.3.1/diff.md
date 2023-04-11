# Comparing `tmp/thinks_dash_components-0.3.0.tar.gz` & `tmp/thinks_dash_components-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thinks_dash_components-0.3.0.tar", last modified: Fri Apr  7 03:20:04 2023, max compression
+gzip compressed data, was "thinks_dash_components-0.3.1.tar", last modified: Tue Apr 11 02:30:53 2023, max compression
```

## Comparing `thinks_dash_components-0.3.0.tar` & `thinks_dash_components-0.3.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-04-07 03:20:04.326775 thinks_dash_components-0.3.0/
--rw-rw-rw-   0        0        0        0 2023-02-22 05:17:07.000000 thinks_dash_components-0.3.0/LICENSE
--rw-rw-rw-   0        0        0      464 2023-02-22 05:17:07.000000 thinks_dash_components-0.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4087 2023-04-07 03:20:04.325778 thinks_dash_components-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     3802 2023-02-22 05:17:07.000000 thinks_dash_components-0.3.0/README.md
--rw-rw-rw-   0        0        0     2320 2023-04-07 03:17:49.000000 thinks_dash_components-0.3.0/package.json
--rw-rw-rw-   0        0        0       42 2023-04-07 03:20:04.326775 thinks_dash_components-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0      737 2023-02-22 05:19:29.000000 thinks_dash_components-0.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-07 03:20:04.313810 thinks_dash_components-0.3.0/thinks_dash_components/
--rw-rw-rw-   0        0        0     1857 2023-04-07 03:19:42.000000 thinks_dash_components-0.3.0/thinks_dash_components/Alert.py
--rw-rw-rw-   0        0        0     1700 2023-04-07 03:19:42.000000 thinks_dash_components-0.3.0/thinks_dash_components/DesignableRadioItems.py
--rw-rw-rw-   0        0        0     2183 2023-04-07 03:19:42.000000 thinks_dash_components-0.3.0/thinks_dash_components/IndexedDB.py
--rw-rw-rw-   0        0        0     1088 2023-04-07 03:19:42.000000 thinks_dash_components-0.3.0/thinks_dash_components/InputNumber.py
--rw-rw-rw-   0        0        0     1092 2023-04-07 03:19:42.000000 thinks_dash_components-0.3.0/thinks_dash_components/IosScrollWrapper.py
--rw-rw-rw-   0        0        0     1913 2023-04-07 03:19:42.000000 thinks_dash_components-0.3.0/thinks_dash_components/LoadingWrapper.py
--rw-rw-rw-   0        0        0     1374 2023-04-07 03:19:42.000000 thinks_dash_components-0.3.0/thinks_dash_components/MobileDropdown.py
--rw-rw-rw-   0        0        0     2192 2023-04-07 03:19:42.000000 thinks_dash_components-0.3.0/thinks_dash_components/Notice.py
--rw-rw-rw-   0        0        0     1352 2023-04-07 03:19:42.000000 thinks_dash_components-0.3.0/thinks_dash_components/OperationObserver.py
--rw-rw-rw-   0        0        0     1388 2023-04-07 03:19:42.000000 thinks_dash_components-0.3.0/thinks_dash_components/Rotate.py
--rw-rw-rw-   0        0        0     1613 2023-04-07 03:19:42.000000 thinks_dash_components-0.3.0/thinks_dash_components/SelectableBox.py
--rw-rw-rw-   0        0        0     1343 2023-04-06 01:49:20.000000 thinks_dash_components-0.3.0/thinks_dash_components/StorageObserver.py
--rw-rw-rw-   0        0        0     1878 2023-04-07 03:19:42.000000 thinks_dash_components-0.3.0/thinks_dash_components/TouchableComponent.py
--rw-rw-rw-   0        0        0      999 2023-04-07 03:19:42.000000 thinks_dash_components-0.3.0/thinks_dash_components/UrlObserver.py
--rw-rw-rw-   0        0        0     1598 2023-04-07 03:19:42.000000 thinks_dash_components-0.3.0/thinks_dash_components/_ComponentTemplate.py
--rw-rw-rw-   0        0        0     2360 2023-02-22 05:17:07.000000 thinks_dash_components-0.3.0/thinks_dash_components/__init__.py
--rw-rw-rw-   0        0        0      899 2023-04-07 03:19:42.000000 thinks_dash_components-0.3.0/thinks_dash_components/_imports_.py
--rw-rw-rw-   0        0        0    44064 2023-04-07 03:19:42.000000 thinks_dash_components-0.3.0/thinks_dash_components/metadata.json
--rw-rw-rw-   0        0        0     2320 2023-04-07 03:19:41.000000 thinks_dash_components-0.3.0/thinks_dash_components/package-info.json
--rw-rw-rw-   0        0        0   124007 2023-04-07 03:19:40.000000 thinks_dash_components-0.3.0/thinks_dash_components/thinks_dash_components.min.js
--rw-rw-rw-   0        0        0      106 2023-04-07 03:19:40.000000 thinks_dash_components-0.3.0/thinks_dash_components/thinks_dash_components.min.js.map
-drwxrwxrwx   0        0        0        0 2023-04-07 03:20:04.324781 thinks_dash_components-0.3.0/thinks_dash_components.egg-info/
--rw-rw-rw-   0        0        0     4087 2023-04-07 03:20:04.000000 thinks_dash_components-0.3.0/thinks_dash_components.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1092 2023-04-07 03:20:04.000000 thinks_dash_components-0.3.0/thinks_dash_components.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-07 03:20:04.000000 thinks_dash_components-0.3.0/thinks_dash_components.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-04-07 03:20:04.000000 thinks_dash_components-0.3.0/thinks_dash_components.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-11 02:30:53.080063 thinks_dash_components-0.3.1/
+-rw-rw-rw-   0        0        0        0 2023-02-22 05:17:07.000000 thinks_dash_components-0.3.1/LICENSE
+-rw-rw-rw-   0        0        0      464 2023-02-22 05:17:07.000000 thinks_dash_components-0.3.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     4087 2023-04-11 02:30:53.080063 thinks_dash_components-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3802 2023-02-22 05:17:07.000000 thinks_dash_components-0.3.1/README.md
+-rw-rw-rw-   0        0        0     2320 2023-04-11 02:30:30.000000 thinks_dash_components-0.3.1/package.json
+-rw-rw-rw-   0        0        0       42 2023-04-11 02:30:53.081060 thinks_dash_components-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      737 2023-02-22 05:19:29.000000 thinks_dash_components-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 02:30:53.075076 thinks_dash_components-0.3.1/thinks_dash_components/
+-rw-rw-rw-   0        0        0     1857 2023-04-11 02:30:43.000000 thinks_dash_components-0.3.1/thinks_dash_components/Alert.py
+-rw-rw-rw-   0        0        0     1700 2023-04-11 02:30:43.000000 thinks_dash_components-0.3.1/thinks_dash_components/DesignableRadioItems.py
+-rw-rw-rw-   0        0        0     2183 2023-04-11 02:30:43.000000 thinks_dash_components-0.3.1/thinks_dash_components/IndexedDB.py
+-rw-rw-rw-   0        0        0     1088 2023-04-11 02:30:43.000000 thinks_dash_components-0.3.1/thinks_dash_components/InputNumber.py
+-rw-rw-rw-   0        0        0     1092 2023-04-11 02:30:43.000000 thinks_dash_components-0.3.1/thinks_dash_components/IosScrollWrapper.py
+-rw-rw-rw-   0        0        0     1913 2023-04-11 02:30:43.000000 thinks_dash_components-0.3.1/thinks_dash_components/LoadingWrapper.py
+-rw-rw-rw-   0        0        0     1374 2023-04-11 02:30:43.000000 thinks_dash_components-0.3.1/thinks_dash_components/MobileDropdown.py
+-rw-rw-rw-   0        0        0     2192 2023-04-11 02:30:43.000000 thinks_dash_components-0.3.1/thinks_dash_components/Notice.py
+-rw-rw-rw-   0        0        0     1352 2023-04-11 02:30:43.000000 thinks_dash_components-0.3.1/thinks_dash_components/OperationObserver.py
+-rw-rw-rw-   0        0        0     1388 2023-04-11 02:30:43.000000 thinks_dash_components-0.3.1/thinks_dash_components/Rotate.py
+-rw-rw-rw-   0        0        0     1613 2023-04-11 02:30:43.000000 thinks_dash_components-0.3.1/thinks_dash_components/SelectableBox.py
+-rw-rw-rw-   0        0        0     1343 2023-04-06 01:49:20.000000 thinks_dash_components-0.3.1/thinks_dash_components/StorageObserver.py
+-rw-rw-rw-   0        0        0     1878 2023-04-11 02:30:43.000000 thinks_dash_components-0.3.1/thinks_dash_components/TouchableComponent.py
+-rw-rw-rw-   0        0        0      999 2023-04-11 02:30:43.000000 thinks_dash_components-0.3.1/thinks_dash_components/UrlObserver.py
+-rw-rw-rw-   0        0        0     1598 2023-04-11 02:30:43.000000 thinks_dash_components-0.3.1/thinks_dash_components/_ComponentTemplate.py
+-rw-rw-rw-   0        0        0     2360 2023-02-22 05:17:07.000000 thinks_dash_components-0.3.1/thinks_dash_components/__init__.py
+-rw-rw-rw-   0        0        0      899 2023-04-11 02:30:43.000000 thinks_dash_components-0.3.1/thinks_dash_components/_imports_.py
+-rw-rw-rw-   0        0        0    44064 2023-04-11 02:30:43.000000 thinks_dash_components-0.3.1/thinks_dash_components/metadata.json
+-rw-rw-rw-   0        0        0     2320 2023-04-11 02:30:42.000000 thinks_dash_components-0.3.1/thinks_dash_components/package-info.json
+-rw-rw-rw-   0        0        0   124007 2023-04-11 02:30:40.000000 thinks_dash_components-0.3.1/thinks_dash_components/thinks_dash_components.min.js
+-rw-rw-rw-   0        0        0      106 2023-04-11 02:30:40.000000 thinks_dash_components-0.3.1/thinks_dash_components/thinks_dash_components.min.js.map
+drwxrwxrwx   0        0        0        0 2023-04-11 02:30:53.079066 thinks_dash_components-0.3.1/thinks_dash_components.egg-info/
+-rw-rw-rw-   0        0        0     4087 2023-04-11 02:30:52.000000 thinks_dash_components-0.3.1/thinks_dash_components.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1092 2023-04-11 02:30:52.000000 thinks_dash_components-0.3.1/thinks_dash_components.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 02:30:52.000000 thinks_dash_components-0.3.1/thinks_dash_components.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-04-11 02:30:52.000000 thinks_dash_components-0.3.1/thinks_dash_components.egg-info/top_level.txt
```

### Comparing `thinks_dash_components-0.3.0/PKG-INFO` & `thinks_dash_components-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thinks_dash_components
-Version: 0.3.0
+Version: 0.3.1
 Summary: Dash Extension Components for Smartphones
 Author: thinkup-sol <s_matsumoto@thinkup-sol.co.jp>
 License: MIT
 Classifier: Framework :: Dash
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `thinks_dash_components-0.3.0/README.md` & `thinks_dash_components-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.0/package.json` & `thinks_dash_components-0.3.1/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'version'": "'0.3.1'"}*

```diff
@@ -54,9 +54,9 @@
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:py_and_r)",
         "build:js": "webpack --mode production",
         "prepublishOnly": "npm run validate-init",
         "pug": "pug --out ./doc/reference --watch ./doc/reference/src --pretty",
         "start": "webpack-serve --host localhost --config ./webpack.serve.config.js --open",
         "validate-init": "python _validate_init.py"
     },
-    "version": "0.3.0"
+    "version": "0.3.1"
 }
```

### Comparing `thinks_dash_components-0.3.0/setup.py` & `thinks_dash_components-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.0/thinks_dash_components/Alert.py` & `thinks_dash_components-0.3.1/thinks_dash_components/Alert.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.0/thinks_dash_components/DesignableRadioItems.py` & `thinks_dash_components-0.3.1/thinks_dash_components/DesignableRadioItems.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.0/thinks_dash_components/IndexedDB.py` & `thinks_dash_components-0.3.1/thinks_dash_components/IndexedDB.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.0/thinks_dash_components/InputNumber.py` & `thinks_dash_components-0.3.1/thinks_dash_components/InputNumber.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.0/thinks_dash_components/IosScrollWrapper.py` & `thinks_dash_components-0.3.1/thinks_dash_components/IosScrollWrapper.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.0/thinks_dash_components/LoadingWrapper.py` & `thinks_dash_components-0.3.1/thinks_dash_components/LoadingWrapper.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.0/thinks_dash_components/MobileDropdown.py` & `thinks_dash_components-0.3.1/thinks_dash_components/MobileDropdown.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.0/thinks_dash_components/Notice.py` & `thinks_dash_components-0.3.1/thinks_dash_components/Notice.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.0/thinks_dash_components/OperationObserver.py` & `thinks_dash_components-0.3.1/thinks_dash_components/OperationObserver.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.0/thinks_dash_components/Rotate.py` & `thinks_dash_components-0.3.1/thinks_dash_components/Rotate.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.0/thinks_dash_components/SelectableBox.py` & `thinks_dash_components-0.3.1/thinks_dash_components/SelectableBox.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.0/thinks_dash_components/StorageObserver.py` & `thinks_dash_components-0.3.1/thinks_dash_components/StorageObserver.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.0/thinks_dash_components/TouchableComponent.py` & `thinks_dash_components-0.3.1/thinks_dash_components/TouchableComponent.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.0/thinks_dash_components/UrlObserver.py` & `thinks_dash_components-0.3.1/thinks_dash_components/UrlObserver.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.0/thinks_dash_components/_ComponentTemplate.py` & `thinks_dash_components-0.3.1/thinks_dash_components/_ComponentTemplate.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.0/thinks_dash_components/__init__.py` & `thinks_dash_components-0.3.1/thinks_dash_components/__init__.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.0/thinks_dash_components/_imports_.py` & `thinks_dash_components-0.3.1/thinks_dash_components/_imports_.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.0/thinks_dash_components/metadata.json` & `thinks_dash_components-0.3.1/thinks_dash_components/metadata.json`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.0/thinks_dash_components/package-info.json` & `thinks_dash_components-0.3.1/thinks_dash_components/package-info.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'version'": "'0.3.1'"}*

```diff
@@ -54,9 +54,9 @@
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:py_and_r)",
         "build:js": "webpack --mode production",
         "prepublishOnly": "npm run validate-init",
         "pug": "pug --out ./doc/reference --watch ./doc/reference/src --pretty",
         "start": "webpack-serve --host localhost --config ./webpack.serve.config.js --open",
         "validate-init": "python _validate_init.py"
     },
-    "version": "0.3.0"
+    "version": "0.3.1"
 }
```

### Comparing `thinks_dash_components-0.3.0/thinks_dash_components/thinks_dash_components.min.js` & `thinks_dash_components-0.3.1/thinks_dash_components/thinks_dash_components.min.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -64,15 +64,15 @@
             var t = function(e) {
                     return /\/_dash-component-suites\//.test(e.src)
                 }(o()),
                 r = i(e);
             if (!t) return r;
             var n = r.split("/"),
                 a = n.slice(-1)[0].split(".");
-            return a.splice(1, 0, "v0_3_0m1680837578"), n.splice(-1, 1, a.join(".")), n.join("/")
+            return a.splice(1, 0, "v0_3_1m1681180238"), n.splice(-1, 1, a.join(".")), n.join("/")
         }
     }
     return r(r.s = 13)
 }([function(e, t) {
     e.exports = window.PropTypes
 }, function(e, t) {
     e.exports = window.React
@@ -3473,15 +3473,15 @@
             value: function() {
                 var e = this.props,
                     t = e.id,
                     r = e.className,
                     n = e.children;
                 return h.a.createElement("div", {
                     id: t,
-                    className: "loading_wrapper " + r + " loading_" + this.state.isLoading,
+                    className: "loading-wrapper " + r + " loading-" + this.state.isLoading,
                     ref: this.ref
                 }, n)
             }
         }]) && we(t.prototype, r), n && we(t, n), Object.defineProperty(t, "prototype", {
             writable: !1
         }), i
     }(d.Component);
@@ -3894,30 +3894,30 @@
                     }, h.a.createElement("span", null, i || "No results found")));
                     return h.a.createElement("div", {
                         id: r,
                         style: {
                             width: "100%",
                             position: "relative"
                         },
-                        className: "mobile_dropdown " + n + (this.state.open ? " open" : "")
+                        className: "mobile-dropdown " + n + (this.state.open ? " open" : "")
                     }, h.a.createElement(lt, {
-                        className: "mobile_dropdown_bg",
+                        className: "mobile-dropdown_bg",
                         style: {
                             display: this.state.open ? "block" : "none"
                         },
                         onTouchEnd: this.close
                     }), h.a.createElement(st, {
                         id: this.id + "-value",
-                        className: "mobile_dropdown-value",
+                        className: "mobile-dropdown-value",
                         onTouchEnd: this.toggle
                     }, h.a.createElement(ct, null, e), a ? h.a.createElement(ut, {
                         onTouchEnd: this.clear,
-                        className: "mobile_dropdown-clear"
+                        className: "mobile-dropdown-clear"
                     }, h.a.createElement($e, null)) : null), h.a.createElement(ot, {
-                        className: "mobile_dropdown-list",
+                        className: "mobile-dropdown-list",
                         style: this.state.listStyle,
                         ref: this.wrapRef,
                         onScroll: this.scroll,
                         onTouchStart: this.touchStart,
                         onTouchEnd: this.touchEnd
                     }, h.a.createElement(it, {
                         id: this.id + "-list",
@@ -4799,21 +4799,21 @@
                     a = [],
                     s = function(t) {
                         a.push(h.a.createElement("div", {
                             key: o[t],
                             onClick: function() {
                                 return e.updateValue(o[t])
                             },
-                            className: "selectable_box_item " + (e.state.value === o[t] ? "selected" : "")
+                            className: "selectable-box-item " + (e.state.value === o[t] ? "selected" : "")
                         }, n[t]))
                     };
                 for (var c in n) s(c);
                 return h.a.createElement("div", {
                     id: r,
-                    className: "selectable_box_list " + i
+                    className: "selectable-box-list " + i
                 }, a)
             }
         }]) && Zt(t.prototype, r), n && Zt(t, n), Object.defineProperty(t, "prototype", {
             writable: !1
         }), i
     }(d.Component);
 
@@ -5094,15 +5094,15 @@
                     t = this.props,
                     r = t.children,
                     n = t.id,
                     o = t.className,
                     i = t.setProps;
                 return h.a.createElement("div", {
                     id: n,
-                    className: "touchable_component " + o + (this.state.active ? " active" : "") + (this.state.isLongTap ? " long_tap" : ""),
+                    className: "touchable-component " + o + (this.state.active ? " active" : "") + (this.state.isLongTap ? " long-tap" : ""),
                     onTouchStart: function(t) {
                         e.updateActive(!0), e.longTap(), e.swipeStart(t), i({
                             start_timestamp: Date.now(),
                             touches: e.touchData(t)
                         })
                     },
                     onTouchEnd: function(t) {
```

### Comparing `thinks_dash_components-0.3.0/thinks_dash_components.egg-info/PKG-INFO` & `thinks_dash_components-0.3.1/thinks_dash_components.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thinks-dash-components
-Version: 0.3.0
+Version: 0.3.1
 Summary: Dash Extension Components for Smartphones
 Author: thinkup-sol <s_matsumoto@thinkup-sol.co.jp>
 License: MIT
 Classifier: Framework :: Dash
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `thinks_dash_components-0.3.0/thinks_dash_components.egg-info/SOURCES.txt` & `thinks_dash_components-0.3.1/thinks_dash_components.egg-info/SOURCES.txt`

 * *Files identical despite different names*

