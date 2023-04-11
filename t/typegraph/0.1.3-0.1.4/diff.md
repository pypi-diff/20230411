# Comparing `tmp/typegraph-0.1.3.tar.gz` & `tmp/typegraph-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typegraph-0.1.3.tar", max compression
+gzip compressed data, was "typegraph-0.1.4.tar", max compression
```

## Comparing `typegraph-0.1.3.tar` & `typegraph-0.1.4.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     5252 2023-04-06 07:53:02.371676 typegraph-0.1.3/LICENSE.md
--rw-r--r--   0        0        0     1318 2023-04-06 07:53:02.371676 typegraph-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      225 2023-04-06 07:53:02.375676 typegraph-0.1.3/typegraph/__init__.py
--rw-r--r--   0        0        0      904 2023-04-06 07:53:02.375676 typegraph-0.1.3/typegraph/effects.py
--rw-r--r--   0        0        0     3323 2023-04-06 07:53:02.375676 typegraph-0.1.3/typegraph/graph/auth/__init__.py
--rw-r--r--   0        0        0      377 2023-04-06 07:53:02.375676 typegraph-0.1.3/typegraph/graph/auth/oauth2.py
--rw-r--r--   0        0        0     1868 2023-04-06 07:53:02.375676 typegraph-0.1.3/typegraph/graph/builder.py
--rw-r--r--   0        0        0     3066 2023-04-06 07:53:02.375676 typegraph-0.1.3/typegraph/graph/models.py
--rw-r--r--   0        0        0     1947 2023-04-06 07:53:02.375676 typegraph-0.1.3/typegraph/graph/nodes.py
--rw-r--r--   0        0        0     5774 2023-04-06 07:53:02.375676 typegraph-0.1.3/typegraph/graph/typegraph.py
--rw-r--r--   0        0        0     7955 2023-04-06 07:53:02.375676 typegraph-0.1.3/typegraph/importers/base/importer.py
--rw-r--r--   0        0        0     3667 2023-04-06 07:53:02.375676 typegraph-0.1.3/typegraph/importers/base/typify.py
--rw-r--r--   0        0        0     7499 2023-04-06 07:53:02.375676 typegraph-0.1.3/typegraph/importers/google_discovery.py
--rw-r--r--   0        0        0     4236 2023-04-06 07:53:02.375676 typegraph-0.1.3/typegraph/importers/graphql.py
--rw-r--r--   0        0        0     8909 2023-04-06 07:53:02.375676 typegraph-0.1.3/typegraph/importers/openapi.py
--rw-r--r--   0        0        0     4078 2023-04-06 07:53:02.375676 typegraph-0.1.3/typegraph/policies.py
--rw-r--r--   0        0        0     1675 2023-04-06 07:53:02.375676 typegraph-0.1.3/typegraph/providers/aws/runtimes/s3.py
--rw-r--r--   0        0        0    28490 2023-04-06 07:53:02.375676 typegraph-0.1.3/typegraph/providers/prisma/relations.py
--rw-r--r--   0        0        0    21779 2023-04-06 07:53:02.375676 typegraph-0.1.3/typegraph/providers/prisma/runtimes/prisma.py
--rw-r--r--   0        0        0     6601 2023-04-06 07:53:02.375676 typegraph-0.1.3/typegraph/providers/prisma/schema.py
--rw-r--r--   0        0        0    13927 2023-04-06 07:53:02.375676 typegraph-0.1.3/typegraph/providers/prisma/type_generator.py
--rw-r--r--   0        0        0     2373 2023-04-06 07:53:02.375676 typegraph-0.1.3/typegraph/providers/prisma/utils.py
--rw-r--r--   0        0        0     2209 2023-04-06 07:53:02.375676 typegraph-0.1.3/typegraph/providers/temporal/runtimes/temporal.py
--rw-r--r--   0        0        0     1351 2023-04-06 07:53:02.375676 typegraph-0.1.3/typegraph/runtimes/base.py
--rw-r--r--   0        0        0     4713 2023-04-06 07:53:02.375676 typegraph-0.1.3/typegraph/runtimes/deno.py
--rw-r--r--   0        0        0     1403 2023-04-06 07:53:02.375676 typegraph-0.1.3/typegraph/runtimes/graphql.py
--rw-r--r--   0        0        0     2789 2023-04-06 07:53:02.375676 typegraph-0.1.3/typegraph/runtimes/http.py
--rw-r--r--   0        0        0     1352 2023-04-06 07:53:02.375676 typegraph-0.1.3/typegraph/runtimes/python_wasi.py
--rw-r--r--   0        0        0     2880 2023-04-06 07:53:02.375676 typegraph-0.1.3/typegraph/runtimes/random.py
--rw-r--r--   0        0        0     2053 2023-04-06 07:53:02.375676 typegraph-0.1.3/typegraph/runtimes/typegate.py
--rw-r--r--   0        0        0     1169 2023-04-06 07:53:02.375676 typegraph-0.1.3/typegraph/runtimes/wasmedge.py
--rw-r--r--   0        0        0    20216 2023-04-06 07:53:02.375676 typegraph-0.1.3/typegraph/types.py
--rw-r--r--   0        0        0      487 2023-04-06 07:53:02.375676 typegraph-0.1.3/typegraph/utils/__init__.py
--rw-r--r--   0        0        0      644 2023-04-06 07:53:02.375676 typegraph-0.1.3/typegraph/utils/attrs.py
--rw-r--r--   0        0        0     1977 2023-04-06 07:53:02.375676 typegraph-0.1.3/typegraph/utils/jsonschema.py
--rw-r--r--   0        0        0     2159 2023-04-06 07:53:02.375676 typegraph-0.1.3/typegraph/utils/loaders.py
--rw-r--r--   0        0        0      185 2023-04-06 07:53:02.375676 typegraph-0.1.3/typegraph/utils/sanitizers.py
--rw-r--r--   0        0        0     1361 1970-01-01 00:00:00.000000 typegraph-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     5252 2023-04-11 08:10:14.940361 typegraph-0.1.4/LICENSE.md
+-rw-r--r--   0        0        0     1427 2023-04-11 08:10:14.940361 typegraph-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      225 2023-04-11 08:10:14.944361 typegraph-0.1.4/typegraph/__init__.py
+-rw-r--r--   0        0        0      904 2023-04-11 08:10:14.944361 typegraph-0.1.4/typegraph/effects.py
+-rw-r--r--   0        0        0     3323 2023-04-11 08:10:14.944361 typegraph-0.1.4/typegraph/graph/auth/__init__.py
+-rw-r--r--   0        0        0      377 2023-04-11 08:10:14.944361 typegraph-0.1.4/typegraph/graph/auth/oauth2.py
+-rw-r--r--   0        0        0     1868 2023-04-11 08:10:14.944361 typegraph-0.1.4/typegraph/graph/builder.py
+-rw-r--r--   0        0        0     3066 2023-04-11 08:10:14.944361 typegraph-0.1.4/typegraph/graph/models.py
+-rw-r--r--   0        0        0     1947 2023-04-11 08:10:14.944361 typegraph-0.1.4/typegraph/graph/nodes.py
+-rw-r--r--   0        0        0     5774 2023-04-11 08:10:14.944361 typegraph-0.1.4/typegraph/graph/typegraph.py
+-rw-r--r--   0        0        0     7955 2023-04-11 08:10:14.944361 typegraph-0.1.4/typegraph/importers/base/importer.py
+-rw-r--r--   0        0        0     3667 2023-04-11 08:10:14.944361 typegraph-0.1.4/typegraph/importers/base/typify.py
+-rw-r--r--   0        0        0     7499 2023-04-11 08:10:14.944361 typegraph-0.1.4/typegraph/importers/google_discovery.py
+-rw-r--r--   0        0        0     4236 2023-04-11 08:10:14.944361 typegraph-0.1.4/typegraph/importers/graphql.py
+-rw-r--r--   0        0        0     8909 2023-04-11 08:10:14.944361 typegraph-0.1.4/typegraph/importers/openapi.py
+-rw-r--r--   0        0        0     4078 2023-04-11 08:10:14.944361 typegraph-0.1.4/typegraph/policies.py
+-rw-r--r--   0        0        0     1675 2023-04-11 08:10:14.944361 typegraph-0.1.4/typegraph/providers/aws/runtimes/s3.py
+-rw-r--r--   0        0        0    28490 2023-04-11 08:10:14.944361 typegraph-0.1.4/typegraph/providers/prisma/relations.py
+-rw-r--r--   0        0        0    21779 2023-04-11 08:10:14.944361 typegraph-0.1.4/typegraph/providers/prisma/runtimes/prisma.py
+-rw-r--r--   0        0        0     6601 2023-04-11 08:10:14.944361 typegraph-0.1.4/typegraph/providers/prisma/schema.py
+-rw-r--r--   0        0        0    13927 2023-04-11 08:10:14.944361 typegraph-0.1.4/typegraph/providers/prisma/type_generator.py
+-rw-r--r--   0        0        0     2373 2023-04-11 08:10:14.944361 typegraph-0.1.4/typegraph/providers/prisma/utils.py
+-rw-r--r--   0        0        0     2209 2023-04-11 08:10:14.944361 typegraph-0.1.4/typegraph/providers/temporal/runtimes/temporal.py
+-rw-r--r--   0        0        0     1351 2023-04-11 08:10:14.944361 typegraph-0.1.4/typegraph/runtimes/base.py
+-rw-r--r--   0        0        0     5234 2023-04-11 08:10:14.944361 typegraph-0.1.4/typegraph/runtimes/deno.py
+-rw-r--r--   0        0        0     1403 2023-04-11 08:10:14.944361 typegraph-0.1.4/typegraph/runtimes/graphql.py
+-rw-r--r--   0        0        0     2789 2023-04-11 08:10:14.944361 typegraph-0.1.4/typegraph/runtimes/http.py
+-rw-r--r--   0        0        0     1352 2023-04-11 08:10:14.944361 typegraph-0.1.4/typegraph/runtimes/python_wasi.py
+-rw-r--r--   0        0        0     2880 2023-04-11 08:10:14.944361 typegraph-0.1.4/typegraph/runtimes/random.py
+-rw-r--r--   0        0        0     2053 2023-04-11 08:10:14.944361 typegraph-0.1.4/typegraph/runtimes/typegate.py
+-rw-r--r--   0        0        0     1169 2023-04-11 08:10:14.944361 typegraph-0.1.4/typegraph/runtimes/wasmedge.py
+-rw-r--r--   0        0        0    20231 2023-04-11 08:10:14.944361 typegraph-0.1.4/typegraph/types.py
+-rw-r--r--   0        0        0      487 2023-04-11 08:10:14.944361 typegraph-0.1.4/typegraph/utils/__init__.py
+-rw-r--r--   0        0        0      644 2023-04-11 08:10:14.944361 typegraph-0.1.4/typegraph/utils/attrs.py
+-rw-r--r--   0        0        0     1977 2023-04-11 08:10:14.944361 typegraph-0.1.4/typegraph/utils/jsonschema.py
+-rw-r--r--   0        0        0     2159 2023-04-11 08:10:14.944361 typegraph-0.1.4/typegraph/utils/loaders.py
+-rw-r--r--   0        0        0      185 2023-04-11 08:10:14.944361 typegraph-0.1.4/typegraph/utils/sanitizers.py
+-rw-r--r--   0        0        0     1470 1970-01-01 00:00:00.000000 typegraph-0.1.4/PKG-INFO
```

### Comparing `typegraph-0.1.3/LICENSE.md` & `typegraph-0.1.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.3/pyproject.toml` & `typegraph-0.1.4/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "typegraph"
-version = "0.1.3"
-description = "Free and open ecosystem for API composition."
+version = "0.1.4"
+description = "Compose your data, anywhere, and build iterative API blocks with zero-trust and serverless deployment, no matter where and how your (legacy) systems are."
 authors = ["Metatype Contributors <support@metatype.dev>"]
 license = "ELv2"
 homepage = "https://metatype.dev"
 repository = "https://github.com/metatypedev/metatype"
 include = ["typegraph/**/*", "LICENSE.md"]
 keywords = ["api", "composition", "typesystem", "graphql", "ecosystem"]
 classifiers = [
```

### Comparing `typegraph-0.1.3/typegraph/effects.py` & `typegraph-0.1.4/typegraph/effects.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.3/typegraph/graph/auth/__init__.py` & `typegraph-0.1.4/typegraph/graph/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.3/typegraph/graph/builder.py` & `typegraph-0.1.4/typegraph/graph/builder.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.3/typegraph/graph/models.py` & `typegraph-0.1.4/typegraph/graph/models.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.3/typegraph/graph/nodes.py` & `typegraph-0.1.4/typegraph/graph/nodes.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.3/typegraph/graph/typegraph.py` & `typegraph-0.1.4/typegraph/graph/typegraph.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.3/typegraph/importers/base/importer.py` & `typegraph-0.1.4/typegraph/importers/base/importer.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.3/typegraph/importers/base/typify.py` & `typegraph-0.1.4/typegraph/importers/base/typify.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.3/typegraph/importers/google_discovery.py` & `typegraph-0.1.4/typegraph/importers/google_discovery.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.3/typegraph/importers/graphql.py` & `typegraph-0.1.4/typegraph/importers/graphql.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.3/typegraph/importers/openapi.py` & `typegraph-0.1.4/typegraph/importers/openapi.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.3/typegraph/policies.py` & `typegraph-0.1.4/typegraph/policies.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.3/typegraph/providers/aws/runtimes/s3.py` & `typegraph-0.1.4/typegraph/providers/aws/runtimes/s3.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.3/typegraph/providers/prisma/relations.py` & `typegraph-0.1.4/typegraph/providers/prisma/relations.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.3/typegraph/providers/prisma/runtimes/prisma.py` & `typegraph-0.1.4/typegraph/providers/prisma/runtimes/prisma.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.3/typegraph/providers/prisma/schema.py` & `typegraph-0.1.4/typegraph/providers/prisma/schema.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.3/typegraph/providers/prisma/type_generator.py` & `typegraph-0.1.4/typegraph/providers/prisma/type_generator.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.3/typegraph/providers/prisma/utils.py` & `typegraph-0.1.4/typegraph/providers/prisma/utils.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.3/typegraph/providers/temporal/runtimes/temporal.py` & `typegraph-0.1.4/typegraph/providers/temporal/runtimes/temporal.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.3/typegraph/runtimes/base.py` & `typegraph-0.1.4/typegraph/runtimes/base.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.3/typegraph/runtimes/deno.py` & `typegraph-0.1.4/typegraph/runtimes/deno.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import os
 from typing import Any, Dict, List, Optional, Tuple
 
 from attrs import field, frozen
 from frozendict import frozendict
 
 from typegraph import effects
+from typegraph import types as t
 from typegraph.effects import Effect
 from typegraph.graph.builder import Collector
 from typegraph.graph.nodes import Node
 from typegraph.runtimes.base import Materializer, Runtime
 from typegraph.utils.attrs import SKIP, always
 
 
@@ -19,14 +20,25 @@
     worker: str = field(kw_only=True, default="default")
     allow_net: Tuple[str, ...] = field(
         kw_only=True, factory=tuple, metadata={SKIP: True}
     )
     permissions: Dict[str, Any] = field(factory=frozendict, init=False)
     runtime_name: str = always("deno")
 
+    @classmethod
+    def static(cls, out: t.Type, value: Any) -> "StaticMat":
+        def prepare(x):
+            if isinstance(x, dict):
+                return frozendict({k: prepare(v) for k, v in x.items()})
+            if isinstance(x, list):
+                return tuple(prepare(v) for v in x)
+            return x
+
+        return t.func(t.struct({}), out, StaticMat(prepare(value)))
+
     def __attrs_post_init__(self):
         permissions = {}
         if len(self.allow_net) > 0:
             if "*" in self.allow_net:
                 permissions["net"] = True
             else:
                 permissions["net"] = self.allow_net
@@ -130,10 +142,12 @@
             secrets=self.secrets,
             effect=effect,
             **kwargs,
         )
 
 
 @frozen
-class IdentityMat(PredefinedFunMat):
-    name: str = always("identity")
+class StaticMat(Materializer):
+    value: Any = field()
     effect: Effect = always(effects.none())
+    runtime: DenoRuntime = field(kw_only=True, factory=DenoRuntime)
+    materializer_name: str = always("static")
```

### Comparing `typegraph-0.1.3/typegraph/runtimes/graphql.py` & `typegraph-0.1.4/typegraph/runtimes/graphql.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.3/typegraph/runtimes/http.py` & `typegraph-0.1.4/typegraph/runtimes/http.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.3/typegraph/runtimes/python_wasi.py` & `typegraph-0.1.4/typegraph/runtimes/python_wasi.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.3/typegraph/runtimes/random.py` & `typegraph-0.1.4/typegraph/runtimes/random.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.3/typegraph/runtimes/typegate.py` & `typegraph-0.1.4/typegraph/runtimes/typegate.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.3/typegraph/runtimes/wasmedge.py` & `typegraph-0.1.4/typegraph/runtimes/wasmedge.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.3/typegraph/types.py` & `typegraph-0.1.4/typegraph/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -694,15 +694,15 @@
         if not isinstance(self.out, struct):
             raise Exception("Output required to be a struct.")
         return self.replace(out=self.out.compose(out))
 
     # def compose(self, other: "func") -> "func":
     #     assert self.out == other.inp
     #     # what if other == gen?
-    #     return func(self, other, IdentityMat())
+    #     return func(self, other, PredefinedFunMat("identity"))
 
     # def __mul__(self, other: "func") -> "func":
     #     return self.compose(other)
 
 
 def gen(out: typedef, mat: Materializer, **kwargs) -> func:
     return func(struct(), out, mat, **kwargs)
```

### Comparing `typegraph-0.1.3/typegraph/utils/attrs.py` & `typegraph-0.1.4/typegraph/utils/attrs.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.3/typegraph/utils/jsonschema.py` & `typegraph-0.1.4/typegraph/utils/jsonschema.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.3/typegraph/utils/loaders.py` & `typegraph-0.1.4/typegraph/utils/loaders.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.3/PKG-INFO` & `typegraph-0.1.4/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: typegraph
-Version: 0.1.3
-Summary: Free and open ecosystem for API composition.
+Version: 0.1.4
+Summary: Compose your data, anywhere, and build iterative API blocks with zero-trust and serverless deployment, no matter where and how your (legacy) systems are.
 Home-page: https://metatype.dev
 License: ELv2
 Keywords: api,composition,typesystem,graphql,ecosystem
 Author: Metatype Contributors
 Author-email: support@metatype.dev
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
```

