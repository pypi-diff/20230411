# Comparing `tmp/jsonbourne-0.8.1.tar.gz` & `tmp/jsonbourne-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonbourne-0.8.1.tar", last modified: Sat Sep 26 01:03:59 2020, max compression
+gzip compressed data, was "jsonbourne-0.9.0.tar", last modified: Tue Sep 29 20:21:53 2020, max compression
```

## Comparing `jsonbourne-0.8.1.tar` & `jsonbourne-0.9.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      995 2020-09-25 15:41:22.000000 jsonbourne-0.8.1/JSON.py
--rw-r--r--   0        0        0     1056 2020-09-25 15:41:22.000000 jsonbourne-0.8.1/LICENSE
--rw-r--r--   0        0        0       79 2020-09-25 15:41:22.000000 jsonbourne-0.8.1/david_webb.py
--rw-r--r--   0        0        0      820 2020-09-25 15:41:22.000000 jsonbourne-0.8.1/jsonbourne/__init__.py
--rw-r--r--   0        0        0     1321 2020-09-25 15:41:22.000000 jsonbourne-0.8.1/jsonbourne/_import.py
--rw-r--r--   0        0        0      340 2020-09-26 01:03:05.000000 jsonbourne-0.8.1/jsonbourne/_version.py
--rw-r--r--   0        0        0    28754 2020-09-26 00:21:13.000000 jsonbourne-0.8.1/jsonbourne/core.py
--rw-r--r--   0        0        0      459 2020-09-25 15:41:22.000000 jsonbourne-0.8.1/jsonbourne/fastapi.py
--rw-r--r--   0        0        0      151 2020-09-25 15:41:22.000000 jsonbourne-0.8.1/jsonbourne/json.py
--rw-r--r--   0        0        0       50 2020-09-25 15:41:22.000000 jsonbourne-0.8.1/jsonbourne/jsonlib/__init__.py
--rw-r--r--   0        0        0     1354 2020-09-25 15:41:22.000000 jsonbourne-0.8.1/jsonbourne/jsonlib/_json_stdlib.py
--rw-r--r--   0        0        0     1333 2020-09-25 15:41:22.000000 jsonbourne-0.8.1/jsonbourne/jsonlib/_orjson.py
--rw-r--r--   0        0        0     1466 2020-09-25 15:41:22.000000 jsonbourne-0.8.1/jsonbourne/jsonlib/_rapidjson.py
--rw-r--r--   0        0        0     1617 2020-09-25 15:41:22.000000 jsonbourne-0.8.1/jsonbourne/jsonlib/base.py
--rw-r--r--   0        0        0        0 2020-09-25 15:41:22.000000 jsonbourne-0.8.1/jsonbourne/py.typed
--rw-r--r--   0        0        0     7607 2020-09-26 00:56:18.000000 jsonbourne-0.8.1/jsonbourne/pydantic.py
--rw-r--r--   0        0        0      577 2020-09-25 15:41:22.000000 jsonbourne-0.8.1/jsonbourne/types.py
--rw-r--r--   0        0        0     2695 2020-09-26 01:02:55.000000 jsonbourne-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     1105 2020-09-26 01:03:59.388385 jsonbourne-0.8.1/setup.py
--rw-r--r--   0        0        0     1259 2020-09-26 01:03:59.388693 jsonbourne-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0       79 2020-09-04 20:39:05.770407 jsonbourne-0.9.0/david_webb.py
+-rw-r--r--   0        0        0      995 2020-09-04 20:39:05.742405 jsonbourne-0.9.0/JSON.py
+-rw-r--r--   0        0        0      820 2020-09-04 20:39:05.776407 jsonbourne-0.9.0/jsonbourne/__init__.py
+-rw-r--r--   0        0        0     1321 2020-09-04 20:39:05.782406 jsonbourne-0.9.0/jsonbourne/_import.py
+-rw-r--r--   0        0        0      340 2020-09-29 20:21:21.471696 jsonbourne-0.9.0/jsonbourne/_version.py
+-rw-r--r--   0        0        0    29033 2020-09-29 20:20:50.718432 jsonbourne-0.9.0/jsonbourne/core.py
+-rw-r--r--   0        0        0      459 2020-09-28 23:39:58.588407 jsonbourne-0.9.0/jsonbourne/fastapi.py
+-rw-r--r--   0        0        0      151 2020-09-04 20:39:05.806406 jsonbourne-0.9.0/jsonbourne/json.py
+-rw-r--r--   0        0        0       50 2020-09-04 20:39:05.813406 jsonbourne-0.9.0/jsonbourne/jsonlib/__init__.py
+-rw-r--r--   0        0        0     1354 2020-09-04 20:39:05.816405 jsonbourne-0.9.0/jsonbourne/jsonlib/_json_stdlib.py
+-rw-r--r--   0        0        0     1333 2020-09-04 20:39:05.823409 jsonbourne-0.9.0/jsonbourne/jsonlib/_orjson.py
+-rw-r--r--   0        0        0     1466 2020-09-29 20:18:25.374296 jsonbourne-0.9.0/jsonbourne/jsonlib/_rapidjson.py
+-rw-r--r--   0        0        0     1617 2020-09-29 20:18:31.307855 jsonbourne-0.9.0/jsonbourne/jsonlib/base.py
+-rw-r--r--   0        0        0        0 2020-09-04 20:39:05.837406 jsonbourne-0.9.0/jsonbourne/py.typed
+-rw-r--r--   0        0        0     7667 2020-09-29 20:06:00.869569 jsonbourne-0.9.0/jsonbourne/pydantic.py
+-rw-r--r--   0        0        0      577 2020-09-04 20:39:05.847406 jsonbourne-0.9.0/jsonbourne/types.py
+-rw-r--r--   0        0        0     1056 2020-09-04 20:39:05.745406 jsonbourne-0.9.0/LICENSE
+-rw-r--r--   0        0        0     2776 2020-09-29 20:21:07.086043 jsonbourne-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     1105 2020-09-29 20:21:53.787511 jsonbourne-0.9.0/setup.py
+-rw-r--r--   0        0        0     1259 2020-09-29 20:21:53.787511 jsonbourne-0.9.0/PKG-INFO
```

### Comparing `jsonbourne-0.8.1/JSON.py` & `jsonbourne-0.9.0/JSON.py`

 * *Files identical despite different names*

### Comparing `jsonbourne-0.8.1/LICENSE` & `jsonbourne-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonbourne-0.8.1/jsonbourne/__init__.py` & `jsonbourne-0.9.0/jsonbourne/__init__.py`

 * *Files identical despite different names*

### Comparing `jsonbourne-0.8.1/jsonbourne/_import.py` & `jsonbourne-0.9.0/jsonbourne/_import.py`

 * *Files identical despite different names*

### Comparing `jsonbourne-0.8.1/jsonbourne/core.py` & `jsonbourne-0.9.0/jsonbourne/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -142,14 +142,16 @@
         >>> 'not_in_d' in d
         False
         >>> d
         JsonObj(**{'uno': 'ONE', 'dos': 2, 'tres': 3})
         >>> del d['dos']
         >>> d
         JsonObj(**{'uno': 'ONE', 'tres': 3})
+        >>> d.tres
+        3
         >>> del d.tres
         >>> d
         JsonObj(**{'uno': 'ONE'})
         >>> d = {"uno": 1, "dos": 2, "tres": {"a": 1, "b": [3, 4, 5, 6]}}
         >>> d = JsonObj(d)
         >>> d
         JsonObj(**{'uno': 1, 'dos': 2, 'tres': {'a': 1, 'b': [3, 4, 5, 6]}})
@@ -171,29 +173,32 @@
         >>> jd.alist[0]
         JsonObj(**{'sub': 123})
         >>> jd.eject()
         {'a': 1, 'b': 'herm', 'alist': [{'sub': 123}]}
 
     """
 
+    _data: Dict[str, Any]
+
     def __init__(self, *args: Any, **kwargs: Any) -> None:
         """Use the object dict"""
-        self.__dict__.update(*args, **kwargs)
+        _data = dict(*args, **kwargs)
+        super().__setattr__('_data', _data)
         try:
-            assert all(isinstance(k, str) for k in self.__dict__)
+            assert all(isinstance(k, str) for k in self._data)
         except AssertionError:
-            d = {k: v for k, v in self.__dict__.items() if not isinstance(k, str)}
+            d = {k: v for k, v in self._data.items() if not isinstance(k, str)}
             raise ValueError(
                 "JsonObj keys MUST be strings! Bad key values: {}".format(str(d))
             )
         self.recurse()
 
     def recurse(self) -> None:
         """Recusively convert all sub dictionaries to JsonObj objects"""
-        self.__dict__.update({k: jsonify(v) for k, v in self.__dict__.items()})
+        self._data.update({k: jsonify(v) for k, v in self._data.items()})
 
     def __attrs_post_init__(self) -> None:
         self.recurse()
 
     def __contains__(self, key: str) -> bool:  # type: ignore
         """Check if a key or dot-key is contained within the JsonObj object
 
@@ -216,25 +221,25 @@
             True
             >>> 'sub.d.a' in d
             False
 
         """
         if "." in key:
             first_key, _, rest = key.partition(".")
-            val = self.__dict__.get(first_key)
+            val = self._data.get(first_key)
             return isinstance(val, MutableMapping) and val.__contains__(rest)
-        return key in self.__dict__
+        return key in self._data
 
-    def __setattr__(self, attr, value):
+    def __setattr__(self, attr: str, value: Any) -> None:
         if attr in self._cls_protected_attrs():
             raise ValueError(
                 f"Cannot set protected attribute ('{str(attr)}'),"
                 f" must use brackets/setitem syntax: json_obj['{str(attr)}']"
             )
-        super(JsonObj, self).__setattr__(attr, value)
+        return self.__setitem__(attr, value)
 
     def __setitem__(self, key: str, value: Any) -> None:
         """Set JsonObj item with 'key' to 'value'
 
         Args:
             key (str): Key/item to set
             value: Value to set
@@ -256,21 +261,21 @@
             JsonObj(**{'a': 123, 'b': 321, '123': 'a'})
             >>> d['456'] = 'a'
             >>> d
             JsonObj(**{'a': 123, 'b': 321, '123': 'a', '456': 'a'})
 
         """
         if is_int(key):
-            self.__dict__[str(key)] = value
+            self._data[str(key)] = value
             return None
         if not is_identifier(key):
             raise ValueError(
                 f"Invalid key: ({key}).\n" f"Key(s) is not a valid python identifier"
             )
-        self.__dict__[key] = value
+        self._data[key] = value
 
     def __getattr__(self, item: str) -> Any:
         """Return an attr
 
         Examples:
             >>> d = {
             ...     'falsey_dict': {},
@@ -290,59 +295,65 @@
             ...     }
             ...
             >>> d = JsonObj(d)
             >>> d.__getattr__('b')
             2
 
         """
-        if item in _JsonObjMutableMapping_attrs:
-            return object.__getattribute__(self, item)
-        if item in self._cls_protected_attrs():
+        if item == '_data':
+            try:
+                return object.__getattribute__(self, '_data')
+            except AttributeError:
+                return self.__dict__
+        if item in _JsonObjMutableMapping_attrs or item in self._cls_protected_attrs():
             return object.__getattribute__(self, item)
         try:
-            return self.__getitem__(str(item))
+            return jsonify(self.__getitem__(str(item)))
         except KeyError:
             pass
         return object.__getattribute__(self, item)
 
     def __object_getattribute__(self, item: str) -> Any:
         return object.__getattribute__(self, item)
 
     def __getitem__(self, key: str) -> Any:
         if "." in key:
             return self.dot_lookup(key)
         try:
-            return jsonify(self.__dict__[key])
+            return jsonify(self._data[key])
         except KeyError:
             pass
         try:
             return jsonify(self.__object_getattribute__(key))
         except AttributeError:
             raise KeyError(str(key))
 
     def __delitem__(self, key: str) -> None:
-        del self.__dict__[key]
+        return self._data.__delitem__(key)
+
+    def __delattr__(self, item: str) -> None:
+        return self.__delitem__(item)
 
     def __iter__(self) -> Iterator[Any]:
-        return iter(self.__dict__)
+        return iter(self._data)
 
     def __len__(self) -> int:
-        return len(self.__dict__)
+        return len(self._data)
 
     def items(self) -> ItemsView[str, Any]:
         """Return an items view of the JsonObj object"""
-        return self.__dict__.items()
+        return self._data.items()
 
     def entries(self) -> ItemsView[str, Any]:
         """Alias for items"""
         return self.items()
 
     def keys(self) -> KeysView[str]:
         """Return the keys view of the JsonObj object"""
-        return self.__dict__.keys()
+        return self._data.keys()
 
     def filter_none(self, recursive: bool = False) -> "JsonObj":
         """Filter key-values where the value is `None` but not false-y
 
         Args:
             recursive (bool): Recursively filter out None values
 
@@ -558,15 +569,15 @@
             The result of the dot-notation key look up
 
         Raises:
             KeyError: Raised if the dot-key is not in in the object
 
         """
         parts = dot_key.split(".")
-        root_val: Any = self.__dict__.get(parts[0])
+        root_val: Any = self._data.get(parts[0])
         cur_val = root_val
         for ix, part in enumerate(parts[1:], start=1):
             try:
                 cur_val = cur_val[part]
             except TypeError:
                 reached = ".".join(parts[:ix])
                 raise KeyError(
@@ -704,15 +715,15 @@
             >>> type(plain_ol_dict)
             <class 'dict'>
 
         """
         return {
             k: unjsonify(v)
             # if not isinstance(v, JsonObj) else v.eject()
-            for k, v in self.__dict__.items()
+            for k, v in self._data.items()
         }
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the JsonObj object (and children) as a python dictionary"""
         return self.eject()
 
     def asdict(self) -> Dict[str, Any]:
@@ -834,15 +845,15 @@
 
     return value
 
 
 def unjsonify(value: Any) -> Any:
     """Recursively eject a JsonDit object"""
     if isinstance(value, JsonObj):
-        return {k: unjsonify(v) for k, v in value.__dict__.items()}
+        return {k: unjsonify(v) for k, v in value._data.items()}
     if isinstance(value, list):
         return [unjsonify(el) for el in value]
     if isinstance(value, tuple):
         return tuple([unjsonify(el) for el in value])
     return value
 
 
@@ -941,14 +952,14 @@
     @staticmethod
     def __call__(value: Any):  # type: ignore
         """Jsonify a value"""
         return jsonify(value)
 
 
 @lru_cache(maxsize=None)
-def _cls_protected_attrs(cls) -> Set[str]:
+def _cls_protected_attrs(cls: Any) -> Set[str]:
     """Return attrs-attribute names for an object decorated with attrs"""
     return set(dir(cls))
 
 
 stringify = JSON.stringify
 parse = JSON.parse
```

### Comparing `jsonbourne-0.8.1/jsonbourne/jsonlib/_json_stdlib.py` & `jsonbourne-0.9.0/jsonbourne/jsonlib/_json_stdlib.py`

 * *Files identical despite different names*

### Comparing `jsonbourne-0.8.1/jsonbourne/jsonlib/_orjson.py` & `jsonbourne-0.9.0/jsonbourne/jsonlib/_orjson.py`

 * *Files identical despite different names*

### Comparing `jsonbourne-0.8.1/jsonbourne/jsonlib/_rapidjson.py` & `jsonbourne-0.9.0/jsonbourne/jsonlib/_rapidjson.py`

 * *Files identical despite different names*

### Comparing `jsonbourne-0.8.1/jsonbourne/jsonlib/base.py` & `jsonbourne-0.9.0/jsonbourne/jsonlib/base.py`

 * *Files identical despite different names*

### Comparing `jsonbourne-0.8.1/jsonbourne/pydantic.py` & `jsonbourne-0.9.0/jsonbourne/pydantic.py`

 * *Files 5% similar despite different names*

```diff
@@ -84,15 +84,15 @@
             Thing(a=1, b='herm', c=None)
             >>> t.to_dict_filter_none()
             {'a': 1, 'b': 'herm'}
             >>> t.to_json_obj_filter_none()
             JsonObj(**{'a': 1, 'b': 'herm'})
 
         """
-        return {k: v for k, v in self.items() if v is not None}
+        return {k: v for k, v in self.dict().items() if v is not None}
 
     def to_dict_filter_defaults(self) -> Dict[str, Any]:
         """Eject object and filter key-values equal to (sub)class' default
 
         Examples:
             >>> class Thing(JsonBaseModel):
             ...     a: int = 1
@@ -111,15 +111,19 @@
             >>> t.to_dict_filter_defaults()
             {'a': 123}
             >>> t.to_json_obj_filter_defaults()
             JsonObj(**{'a': 123})
 
         """
         defaults = self.defaults_dict()
-        return {k: v for k, v in self.items() if k not in defaults or v != defaults[k]}
+        return {
+            k: v
+            for k, v in self.dict().items()
+            if k not in defaults or v != defaults[k]
+        }
 
     def to_json_obj_filter_defaults(self) -> JsonObj:
         """Eject to JsonObj and filter key-values equal to (sub)class' default"""
         return JsonObj(self.to_dict_filter_defaults())
 
     def to_json_obj_filter_none(self) -> JsonObj:
         """Eject to JsonObj and filter key-values where the value is None"""
```

### Comparing `jsonbourne-0.8.1/jsonbourne/types.py` & `jsonbourne-0.9.0/jsonbourne/types.py`

 * *Files identical despite different names*

### Comparing `jsonbourne-0.8.1/pyproject.toml` & `jsonbourne-0.9.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,81 +1,81 @@
-[tool.poetry]
-name = "jsonbourne"
-version = "0.8.1"
-description = "JSON not json"
-license = "MIT"
-authors = ["jesse <jesse@dgi.com>"]
-repository = "https://github.com/dynamic-graphics-inc/dgpy-libs"
-packages = [
-    { include = "jsonbourne", from = "." },
-    { include = "JSON.py", from = "." },
-    { include = "david_webb.py", from = "." },
-]
-classifiers = [
-    "Development Status :: 5 - Production/Stable",
-    "Intended Audience :: Developers",
-    "License :: OSI Approved :: MIT License",
-    "Programming Language :: Python",
-    "Programming Language :: Python :: 3.6",
-    "Programming Language :: Python :: 3.7",
-    "Programming Language :: Python :: 3.8",
-    "Typing :: Typed"
-]
-keywords = [
-    "json", "python", "jsonbourne", "pydantic", "orjson", "rapidjson",
-    "python-rapidjson", "mattdamon"
-]
-
-
-[tool.poetry.dependencies]
-python = "==3.*,>=3.6.1"
-pydantic = { version = "==1.*,>=1.5.0", optional = true }
-python-rapidjson = { version = "==0.*,>=0.9.1", optional = true }
-orjson = { version = "==3.*,>=3.0.0", optional = true }
-
-[tool.poetry.dev-dependencies]
-pytest = "==5.*,>=5.3.0"
-
-[tool.poetry.extras]
-rec = ["orjson"]
-rj = ["python-rapidjson"]
-oj = ["orjson"]
-rapidjson = ["python-rapidjson"]
-orjson = ["orjson"]
-pydantic = ["pydantic"]
-full = ["orjson", "pydantic", "python-rapidjson"]
-
-
-
-
-[tool.dephell.main]
-from = { format = "poetry", path = "pyproject.toml" }
-to = { format = "setuppy", path = "setup.py" }
-# explicitly specify your versioning scheme to let your users know what they can expect
-versioning = "semver"
-# git tag template for releases
-tag = "v"
-
-[tool.dephell.vendorized]
-from = { format = "poetry", path = "pyproject.toml" }
-to = { format = "wheel", path = "dist-vendored/" }
-envs = ["main"]
-
-# Make vendorized version of the project:
-# dephell vendor download --env=vendorized
-# dephell vendor import --env=vendorized
-[tool.dephell.vendorized.vendor]
-path = "dephell_vendor"
-exclude = ["jinja2", "tests", "setuptools", "pip"]
-
-[build-system]
-requires = ["poetry>=0.12"]
-build-backend = "poetry.masonry.api"
-
-# =============================================================================
-# /\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/
-# =============================================================================
-#  /\  /\  /\  /\  /\  /\  /\  /\  /\  /\  /\  /\  /\  /\  /\  /\  /\  /\  /\
-# /  \/  \/  \/  \/  \/  \/  \/  \/  \/  \/  \/  \/  \/  \/  \/  \/  \/  \/  \
-# =============================================================================
-# \/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\
-# =============================================================================
+[tool.poetry]
+name = "jsonbourne"
+version = "0.9.0"
+description = "JSON not json"
+license = "MIT"
+authors = ["jesse <jesse@dgi.com>"]
+repository = "https://github.com/dynamic-graphics-inc/dgpy-libs"
+packages = [
+    { include = "jsonbourne", from = "." },
+    { include = "JSON.py", from = "." },
+    { include = "david_webb.py", from = "." },
+]
+classifiers = [
+    "Development Status :: 5 - Production/Stable",
+    "Intended Audience :: Developers",
+    "License :: OSI Approved :: MIT License",
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3.6",
+    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
+    "Typing :: Typed"
+]
+keywords = [
+    "json", "python", "jsonbourne", "pydantic", "orjson", "rapidjson",
+    "python-rapidjson", "mattdamon"
+]
+
+
+[tool.poetry.dependencies]
+python = "==3.*,>=3.6.1"
+pydantic = { version = "==1.*,>=1.5.0", optional = true }
+python-rapidjson = { version = "==0.*,>=0.9.1", optional = true }
+orjson = { version = "==3.*,>=3.0.0", optional = true }
+
+[tool.poetry.dev-dependencies]
+pytest = "==5.*,>=5.3.0"
+
+[tool.poetry.extras]
+rec = ["orjson"]
+rj = ["python-rapidjson"]
+oj = ["orjson"]
+rapidjson = ["python-rapidjson"]
+orjson = ["orjson"]
+pydantic = ["pydantic"]
+full = ["orjson", "pydantic", "python-rapidjson"]
+
+
+
+
+[tool.dephell.main]
+from = { format = "poetry", path = "pyproject.toml" }
+to = { format = "setuppy", path = "setup.py" }
+# explicitly specify your versioning scheme to let your users know what they can expect
+versioning = "semver"
+# git tag template for releases
+tag = "v"
+
+[tool.dephell.vendorized]
+from = { format = "poetry", path = "pyproject.toml" }
+to = { format = "wheel", path = "dist-vendored/" }
+envs = ["main"]
+
+# Make vendorized version of the project:
+# dephell vendor download --env=vendorized
+# dephell vendor import --env=vendorized
+[tool.dephell.vendorized.vendor]
+path = "dephell_vendor"
+exclude = ["jinja2", "tests", "setuptools", "pip"]
+
+[build-system]
+requires = ["poetry>=0.12"]
+build-backend = "poetry.masonry.api"
+
+# =============================================================================
+# /\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/
+# =============================================================================
+#  /\  /\  /\  /\  /\  /\  /\  /\  /\  /\  /\  /\  /\  /\  /\  /\  /\  /\  /\
+# /  \/  \/  \/  \/  \/  \/  \/  \/  \/  \/  \/  \/  \/  \/  \/  \/  \/  \/  \
+# =============================================================================
+# \/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\
+# =============================================================================
```

### Comparing `jsonbourne-0.8.1/setup.py` & `jsonbourne-0.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
  'pydantic': ['pydantic>=1.5.0,<2.0.0'],
  'rapidjson': ['python-rapidjson>=0.9.1,<1.0.0'],
  'rec': ['orjson>=3.0.0,<4.0.0'],
  'rj': ['python-rapidjson>=0.9.1,<1.0.0']}
 
 setup_kwargs = {
     'name': 'jsonbourne',
-    'version': '0.8.1',
+    'version': '0.9.0',
     'description': 'JSON not json',
     'long_description': None,
     'author': 'jesse',
     'author_email': 'jesse@dgi.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/dynamic-graphics-inc/dgpy-libs',
```

### Comparing `jsonbourne-0.8.1/PKG-INFO` & `jsonbourne-0.9.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonbourne
-Version: 0.8.1
+Version: 0.9.0
 Summary: JSON not json
 Home-page: https://github.com/dynamic-graphics-inc/dgpy-libs
 License: MIT
 Keywords: json,python,jsonbourne,pydantic,orjson,rapidjson,python-rapidjson,mattdamon
 Author: jesse
 Author-email: jesse@dgi.com
 Requires-Python: >=3.6.1,<4.0.0
```

