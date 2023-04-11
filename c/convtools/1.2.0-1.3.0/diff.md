# Comparing `tmp/convtools-1.2.0.tar.gz` & `tmp/convtools-1.3.0.tar.gz`

## Comparing `convtools-1.2.0.tar` & `convtools-1.3.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 convtools-1.2.0/convtools/__init__.py
--rw-r--r--   0        0        0    51224 2020-02-02 00:00:00.000000 convtools-1.2.0/convtools/_aggregations.py
--rw-r--r--   0        0        0   107382 2020-02-02 00:00:00.000000 convtools-1.2.0/convtools/_base.py
--rw-r--r--   0        0        0     7609 2020-02-02 00:00:00.000000 convtools-1.2.0/convtools/_chunks.py
--rw-r--r--   0        0        0     5696 2020-02-02 00:00:00.000000 convtools-1.2.0/convtools/_columns.py
--rw-r--r--   0        0        0     5405 2020-02-02 00:00:00.000000 convtools-1.2.0/convtools/_conversion.py
--rw-r--r--   0        0        0     3207 2020-02-02 00:00:00.000000 convtools-1.2.0/convtools/_cumulative.py
--rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 convtools-1.2.0/convtools/_debug.py
--rw-r--r--   0        0        0    20223 2020-02-02 00:00:00.000000 convtools-1.2.0/convtools/_dt.py
--rw-r--r--   0        0        0     3134 2020-02-02 00:00:00.000000 convtools-1.2.0/convtools/_heuristics.py
--rw-r--r--   0        0        0    17783 2020-02-02 00:00:00.000000 convtools-1.2.0/convtools/_joins.py
--rw-r--r--   0        0        0     5693 2020-02-02 00:00:00.000000 convtools-1.2.0/convtools/_mutations.py
--rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 convtools-1.2.0/convtools/_unique.py
--rw-r--r--   0        0        0     8584 2020-02-02 00:00:00.000000 convtools-1.2.0/convtools/_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 convtools-1.2.0/convtools/contrib/__init__.py
--rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 convtools-1.2.0/convtools/contrib/fs.py
--rw-r--r--   0        0        0    34670 2020-02-02 00:00:00.000000 convtools-1.2.0/convtools/contrib/tables.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 convtools-1.2.0/.gitignore
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 convtools-1.2.0/LICENSE.txt
--rw-r--r--   0        0        0     4067 2020-02-02 00:00:00.000000 convtools-1.2.0/README.md
--rw-r--r--   0        0        0     2473 2020-02-02 00:00:00.000000 convtools-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     7634 2020-02-02 00:00:00.000000 convtools-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 convtools-1.3.0/convtools/__init__.py
+-rw-r--r--   0        0        0    51224 2020-02-02 00:00:00.000000 convtools-1.3.0/convtools/_aggregations.py
+-rw-r--r--   0        0        0   108078 2020-02-02 00:00:00.000000 convtools-1.3.0/convtools/_base.py
+-rw-r--r--   0        0        0     7609 2020-02-02 00:00:00.000000 convtools-1.3.0/convtools/_chunks.py
+-rw-r--r--   0        0        0     5696 2020-02-02 00:00:00.000000 convtools-1.3.0/convtools/_columns.py
+-rw-r--r--   0        0        0     5538 2020-02-02 00:00:00.000000 convtools-1.3.0/convtools/_conversion.py
+-rw-r--r--   0        0        0     3207 2020-02-02 00:00:00.000000 convtools-1.3.0/convtools/_cumulative.py
+-rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 convtools-1.3.0/convtools/_debug.py
+-rw-r--r--   0        0        0    20223 2020-02-02 00:00:00.000000 convtools-1.3.0/convtools/_dt.py
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 convtools-1.3.0/convtools/_expect.py
+-rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 convtools-1.3.0/convtools/_heuristics.py
+-rw-r--r--   0        0        0    17783 2020-02-02 00:00:00.000000 convtools-1.3.0/convtools/_joins.py
+-rw-r--r--   0        0        0     5693 2020-02-02 00:00:00.000000 convtools-1.3.0/convtools/_mutations.py
+-rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 convtools-1.3.0/convtools/_unique.py
+-rw-r--r--   0        0        0     8584 2020-02-02 00:00:00.000000 convtools-1.3.0/convtools/_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 convtools-1.3.0/convtools/contrib/__init__.py
+-rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 convtools-1.3.0/convtools/contrib/fs.py
+-rw-r--r--   0        0        0    34670 2020-02-02 00:00:00.000000 convtools-1.3.0/convtools/contrib/tables.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 convtools-1.3.0/.gitignore
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 convtools-1.3.0/LICENSE.txt
+-rw-r--r--   0        0        0     4067 2020-02-02 00:00:00.000000 convtools-1.3.0/README.md
+-rw-r--r--   0        0        0     2473 2020-02-02 00:00:00.000000 convtools-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     7634 2020-02-02 00:00:00.000000 convtools-1.3.0/PKG-INFO
```

### Comparing `convtools-1.2.0/convtools/_aggregations.py` & `convtools-1.3.0/convtools/_aggregations.py`

 * *Files identical despite different names*

### Comparing `convtools-1.2.0/convtools/_base.py` & `convtools-1.3.0/convtools/_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 )
 
 
 convtools_cumulative = LazyModule("convtools._cumulative")
 convtools_debug = LazyModule("convtools._debug")
 convtools_mutations = LazyModule("convtools._mutations")
 convtools_unique = LazyModule("convtools._unique")
+convtools_expect = LazyModule("convtools._expect")
 
 
 black: "t.Optional[t.Any]" = None
 try:
     import black as black_  # pragma: no cover
 
     black = black_  # pragma: no cover
@@ -843,14 +844,24 @@
     def __mul__(self, b) -> "InlineExpr":
         return (
             InlineExpr("{0} * {1}", Weights.MATH_SIMPLE)
             .pass_args(self, b)
             .add_hint(self.OutputHints.NOT_NONE)
         )
 
+    def pow(self, b) -> "InlineExpr":
+        return self**b
+
+    def __pow__(self, b) -> "InlineExpr":
+        return (
+            InlineExpr("{0} ** {1}", Weights.MATH_SIMPLE)
+            .pass_args(self, b)
+            .add_hint(self.OutputHints.NOT_NONE)
+        )
+
     def sub(self, b) -> "InlineExpr":
         return self - b
 
     def __sub__(self, b) -> "InlineExpr":
         return (
             InlineExpr("{0} - {1}", Weights.MATH_SIMPLE)
             .pass_args(self, b)
@@ -1177,14 +1188,20 @@
             datetime_trunc_to_microsecond,
             self,
             step.to_us(),
             0 if offset is None else offset.to_us(),
             mode,
         )
 
+    def expect(self, condition, error_msg=None):
+        """Checks condition and return the input as is. If condition is not
+        met, raises ExpectException with error_msg (can be conversion too) as
+        param"""
+        return convtools_expect.Expect(self, condition, error_msg)
+
 
 class BaseMutation(BaseConversion):
     used_in_narrow_context = True
     weight = Weights.FUNCTION_CALL
 
 
 class BaseMethodConversion(BaseConversion):
@@ -3090,14 +3107,16 @@
     __le__ = delegate_simple_1_arg("__le__")
     lte = delegate_simple_1_arg("lte")
     __lt__ = delegate_simple_1_arg("__lt__")
     lt = delegate_simple_1_arg("lt")
     __mod__ = delegate_simple_1_arg("__mod__")
     mod = delegate_simple_1_arg("mod")
     __mul__ = delegate_simple_1_arg("__mul__")
+    pow = delegate_simple_1_arg("pow")
+    __pow__ = delegate_simple_1_arg("__pow__")
     mul = delegate_simple_1_arg("mul")
     __ne__ = delegate_simple_1_arg("__ne__")
     not_eq = delegate_simple_1_arg("not_eq")
     __or__ = delegate_simple_1_arg("__or__")
     __sub__ = delegate_simple_1_arg("__sub__")
     sub = delegate_simple_1_arg("sub")
     __truediv__ = delegate_simple_1_arg("__truediv__")
```

### Comparing `convtools-1.2.0/convtools/_chunks.py` & `convtools-1.3.0/convtools/_chunks.py`

 * *Files identical despite different names*

### Comparing `convtools-1.2.0/convtools/_columns.py` & `convtools-1.3.0/convtools/_columns.py`

 * *Files identical despite different names*

### Comparing `convtools-1.2.0/convtools/_conversion.py` & `convtools-1.3.0/convtools/_conversion.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,14 +46,15 @@
     Tuple,
     TupleComp,
     ensure_conversion,
 )
 from ._chunks import ChunkBy, ChunkByCondition
 from ._columns import ColumnRef
 from ._cumulative import Cumulative
+from ._expect import ExpectException
 from ._joins import JoinConversion, _JoinConditions
 from ._mutations import Mutations
 
 
 __all__ = ["conversion", "Conversion"]
 
 _none = BaseConversion._none
@@ -74,14 +75,15 @@
     >>>     {"name": "Bob", "value": 7},
     >>>     {"name": "Ron", "value": 3},
     >>> ]) == {'Bob': 17, 'Ron': 3}
 
     """
 
     ConversionException = ConversionException  # pylint: disable=invalid-name
+    ExpectException = ExpectException  # pylint: disable=invalid-name
     BaseConversion = BaseConversion  # pylint: disable=invalid-name
     OptionsCtx = ConverterOptionsCtx  # pylint: disable=invalid-name
     CodeGenerationOptionsCtx = (  # pylint: disable=invalid-name
         CodeGenerationOptionsCtx
     )
 
     ReduceFuncs = ReduceFuncs  # pylint: disable=invalid-name
@@ -148,14 +150,16 @@
     chunk_by_condition = ChunkByCondition
     CHUNK = ChunkByCondition.CHUNK
 
     breakpoint = This.breakpoint
     date_trunc = This.date_trunc
     datetime_trunc = This.datetime_trunc
 
+    expect = This.expect
+
     PREV = Cumulative.PREV
     cumulative = This.cumulative
     cumulative_reset = This.cumulative_reset
 
     date_parse = This.date_parse
     datetime_parse = This.datetime_parse
```

### Comparing `convtools-1.2.0/convtools/_cumulative.py` & `convtools-1.3.0/convtools/_cumulative.py`

 * *Files identical despite different names*

### Comparing `convtools-1.2.0/convtools/_debug.py` & `convtools-1.3.0/convtools/_debug.py`

 * *Files identical despite different names*

### Comparing `convtools-1.2.0/convtools/_dt.py` & `convtools-1.3.0/convtools/_dt.py`

 * *Files identical despite different names*

### Comparing `convtools-1.2.0/convtools/_heuristics.py` & `convtools-1.3.0/convtools/_heuristics.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,99 +7,115 @@
 
 # generated by "python benchmarks/build_heuristics.py"
 
 PY_VERSION = sys.version_info[0:2]
 if PY_VERSION <= (3, 6):
     # 3.6.15
     class Weights:  # type: ignore # pragma: no cover # pylint: disable=missing-class-docstring # noqa: F811
-        # base_time: 4.0568550033715e-11
+        # base_time: 9.447378699587717e-11
         STEP = 100
-        LOGICAL = 251
-        DICT_LOOKUP = 327
-        MATH_SIMPLE = 377
-        ATTR_LOOKUP = 342
-        TUPLE_INIT = 538
-        LIST_INIT = 675
-        SET_INIT = 1711
-        DICT_INIT = 1667
+        LOGICAL = 107
+        DICT_LOOKUP = 139
+        MATH_SIMPLE = 161
+        ATTR_LOOKUP = 146
+        TUPLE_INIT = 231
+        LIST_INIT = 289
+        SET_INIT = 731
+        DICT_INIT = 724
         FUNCTION_CALL = DICT_LOOKUP * 4
-        UNPREDICTABLE = 171100
+        UNPREDICTABLE = 73100
 
 elif PY_VERSION <= (3, 7):  # pragma: no cover
     # 3.7.16
     class Weights:  # type: ignore # pragma: no cover # pylint: disable=missing-class-docstring # noqa: F811
-        # base_time: 4.08321829275715e-11
+        # base_time: 9.359483375e-11
         STEP = 100
-        LOGICAL = 236
-        DICT_LOOKUP = 337
-        MATH_SIMPLE = 365
-        ATTR_LOOKUP = 319
-        TUPLE_INIT = 525
-        LIST_INIT = 655
-        SET_INIT = 1643
-        DICT_INIT = 1685
+        LOGICAL = 103
+        DICT_LOOKUP = 147
+        MATH_SIMPLE = 159
+        ATTR_LOOKUP = 139
+        TUPLE_INIT = 230
+        LIST_INIT = 286
+        SET_INIT = 730
+        DICT_INIT = 725
         FUNCTION_CALL = DICT_LOOKUP * 4
-        UNPREDICTABLE = 168500
+        UNPREDICTABLE = 73000
 
 elif PY_VERSION == (3, 8):  # pragma: no cover
     # 3.8.16
     class Weights:  # type: ignore # pragma: no cover # pylint: disable=missing-class-docstring # noqa: F811
-        # base_time: 4.144752377655609e-11
+        # base_time: 9.942295274999998e-11
         STEP = 100
-        LOGICAL = 226
-        DICT_LOOKUP = 319
-        MATH_SIMPLE = 368
-        ATTR_LOOKUP = 309
-        TUPLE_INIT = 532
-        LIST_INIT = 675
-        SET_INIT = 1677
-        DICT_INIT = 1758
+        LOGICAL = 94
+        DICT_LOOKUP = 132
+        MATH_SIMPLE = 153
+        ATTR_LOOKUP = 129
+        TUPLE_INIT = 221
+        LIST_INIT = 281
+        SET_INIT = 692
+        DICT_INIT = 749
         FUNCTION_CALL = DICT_LOOKUP * 4
-        UNPREDICTABLE = 175800
+        UNPREDICTABLE = 74900
 
 elif PY_VERSION == (3, 9):  # pragma: no cover
     # 3.9.12
     class Weights:  # type: ignore # pragma: no cover # pylint: disable=missing-class-docstring # noqa: F811
-        # base_time: 4.01792780282291e-11
+        # base_time: 1.0032663587500003e-10
         STEP = 100
-        LOGICAL = 241
-        DICT_LOOKUP = 345
-        MATH_SIMPLE = 409
-        ATTR_LOOKUP = 328
-        TUPLE_INIT = 610
-        LIST_INIT = 775
-        SET_INIT = 1422
-        DICT_INIT = 1912
+        LOGICAL = 96
+        DICT_LOOKUP = 138
+        MATH_SIMPLE = 164
+        ATTR_LOOKUP = 131
+        TUPLE_INIT = 244
+        LIST_INIT = 311
+        SET_INIT = 569
+        DICT_INIT = 767
         FUNCTION_CALL = DICT_LOOKUP * 4
-        UNPREDICTABLE = 191200
+        UNPREDICTABLE = 76700
 
 elif PY_VERSION == (3, 10):  # pragma: no cover
     # 3.10.9
     class Weights:  # type: ignore # pragma: no cover # pylint: disable=missing-class-docstring # noqa: F811
-        # base_time: 4.1176799481692785e-11
+        # base_time: 9.785650500089106e-11
         STEP = 100
-        LOGICAL = 206
-        DICT_LOOKUP = 306
-        MATH_SIMPLE = 365
-        ATTR_LOOKUP = 301
-        TUPLE_INIT = 565
-        LIST_INIT = 668
-        SET_INIT = 1431
-        DICT_INIT = 1798
+        LOGICAL = 86
+        DICT_LOOKUP = 129
+        MATH_SIMPLE = 154
+        ATTR_LOOKUP = 126
+        TUPLE_INIT = 238
+        LIST_INIT = 283
+        SET_INIT = 602
+        DICT_INIT = 800
         FUNCTION_CALL = DICT_LOOKUP * 4
-        UNPREDICTABLE = 179800
+        UNPREDICTABLE = 80000
 
-else:
+elif PY_VERSION == (3, 11):  # pragma: no cover
     # 3.11.1
     class Weights:  # type: ignore # pragma: no cover # pylint: disable=missing-class-docstring # noqa: F811
-        # base_time: 4.285590663856272e-11
+        # base_time: 9.514307286917756e-11
+        STEP = 100
+        LOGICAL = 80
+        DICT_LOOKUP = 140
+        MATH_SIMPLE = 153
+        ATTR_LOOKUP = 128
+        TUPLE_INIT = 239
+        LIST_INIT = 293
+        SET_INIT = 623
+        DICT_INIT = 888
+        FUNCTION_CALL = DICT_LOOKUP * 4
+        UNPREDICTABLE = 88800
+
+else:
+    # 3.12.0a7
+    class Weights:  # type: ignore # pragma: no cover # pylint: disable=missing-class-docstring # noqa: F811
+        # base_time: 9.114620300169917e-11
         STEP = 100
-        LOGICAL = 178
-        DICT_LOOKUP = 313
-        MATH_SIMPLE = 343
-        ATTR_LOOKUP = 282
-        TUPLE_INIT = 530
-        LIST_INIT = 647
-        SET_INIT = 1379
-        DICT_INIT = 1958
+        LOGICAL = 109
+        DICT_LOOKUP = 148
+        MATH_SIMPLE = 173
+        ATTR_LOOKUP = 68
+        TUPLE_INIT = 232
+        LIST_INIT = 307
+        SET_INIT = 634
+        DICT_INIT = 997
         FUNCTION_CALL = DICT_LOOKUP * 4
-        UNPREDICTABLE = 195800
+        UNPREDICTABLE = 99700
```

### Comparing `convtools-1.2.0/convtools/_joins.py` & `convtools-1.3.0/convtools/_joins.py`

 * *Files identical despite different names*

### Comparing `convtools-1.2.0/convtools/_mutations.py` & `convtools-1.3.0/convtools/_mutations.py`

 * *Files identical despite different names*

### Comparing `convtools-1.2.0/convtools/_unique.py` & `convtools-1.3.0/convtools/_unique.py`

 * *Files identical despite different names*

### Comparing `convtools-1.2.0/convtools/_utils.py` & `convtools-1.3.0/convtools/_utils.py`

 * *Files identical despite different names*

### Comparing `convtools-1.2.0/convtools/contrib/fs.py` & `convtools-1.3.0/convtools/contrib/fs.py`

 * *Files identical despite different names*

### Comparing `convtools-1.2.0/convtools/contrib/tables.py` & `convtools-1.3.0/convtools/contrib/tables.py`

 * *Files identical despite different names*

### Comparing `convtools-1.2.0/.gitignore` & `convtools-1.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `convtools-1.2.0/LICENSE.txt` & `convtools-1.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `convtools-1.2.0/README.md` & `convtools-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `convtools-1.2.0/pyproject.toml` & `convtools-1.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 [tool.hatch.build.targets.sdist]
 include = ["/src"]
 
 
 [project]
 name = "convtools"
-version = "1.2.0"
+version = "1.3.0"
 description = "dynamic, declarative data transformations with automatic code generation"
 
 readme = "README.md"
 requires-python = ">=3.6"
 license = {file = "LICENSE.txt"}
 keywords = ["etl", "converters", "codegen", "convtools"]
 authors = [
```

### Comparing `convtools-1.2.0/PKG-INFO` & `convtools-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: convtools
-Version: 1.2.0
+Version: 1.3.0
 Summary: dynamic, declarative data transformations with automatic code generation
 Project-URL: homepage, https://github.com/westandskif/convtools
 Project-URL: documentation, https://convtools.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/westandskif/convtools
 Project-URL: changelog, https://github.com/westandskif/convtools/blob/master/docs/CHANGELOG.md
 Author-email: Nikita Almakov <nikita.almakov@gmail.com>
 Maintainer-email: Nikita Almakov <nikita.almakov@gmail.com>
```

