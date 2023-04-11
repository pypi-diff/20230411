# Comparing `tmp/c7n_left-0.1.5-py3-none-any.whl.zip` & `tmp/c7n_left-0.1.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,17 @@
-Zip file size: 15281 bytes, number of entries: 14
--rw-r--r--  2.0 unx     2173 b- defN 80-Jan-01 00:00 c7n_left/cli.py
--rw-r--r--  2.0 unx    11131 b- defN 80-Jan-01 00:00 c7n_left/core.py
+Zip file size: 19616 bytes, number of entries: 15
+-rw-r--r--  2.0 unx     2977 b- defN 80-Jan-01 00:00 c7n_left/cli.py
+-rw-r--r--  2.0 unx    11560 b- defN 80-Jan-01 00:00 c7n_left/core.py
 -rw-r--r--  2.0 unx      142 b- defN 80-Jan-01 00:00 c7n_left/entry.py
 -rw-r--r--  2.0 unx     4315 b- defN 80-Jan-01 00:00 c7n_left/filters.py
--rw-r--r--  2.0 unx    12016 b- defN 80-Jan-01 00:00 c7n_left/output.py
+-rw-r--r--  2.0 unx    11802 b- defN 80-Jan-01 00:00 c7n_left/output.py
 -rw-r--r--  2.0 unx      121 b- defN 80-Jan-01 00:00 c7n_left/providers/terraform/__init__.py
 -rw-r--r--  2.0 unx     3282 b- defN 80-Jan-01 00:00 c7n_left/providers/terraform/graph.py
--rw-r--r--  2.0 unx     1508 b- defN 80-Jan-01 00:00 c7n_left/providers/terraform/provider.py
+-rw-r--r--  2.0 unx     1552 b- defN 80-Jan-01 00:00 c7n_left/providers/terraform/provider.py
 -rw-r--r--  2.0 unx      945 b- defN 80-Jan-01 00:00 c7n_left/providers/terraform/resource.py
--rw-r--r--  2.0 unx      717 b- defN 80-Jan-01 00:00 c7n_left/utils.py
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 c7n_left-0.1.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       45 b- defN 80-Jan-01 00:00 c7n_left-0.1.5.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     4244 b- defN 16-Jan-01 00:00 c7n_left-0.1.5.dist-info/METADATA
-?rw-------  2.0 unx     1132 b- defN 23-Mar-16 06:02 c7n_left-0.1.5.dist-info/RECORD
-14 files, 41859 bytes uncompressed, 13407 bytes compressed:  68.0%
+-rw-r--r--  2.0 unx     7208 b- defN 80-Jan-01 00:00 c7n_left/test.py
+-rw-r--r--  2.0 unx      732 b- defN 80-Jan-01 00:00 c7n_left/utils.py
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 c7n_left-0.1.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       45 b- defN 80-Jan-01 00:00 c7n_left-0.1.6.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx    12065 b- defN 16-Jan-01 00:00 c7n_left-0.1.6.dist-info/METADATA
+?rw-------  2.0 unx     1206 b- defN 23-Apr-11 08:33 c7n_left-0.1.6.dist-info/RECORD
+15 files, 58040 bytes uncompressed, 17634 bytes compressed:  69.6%
```

## zipnote {}

```diff
@@ -21,23 +21,26 @@
 
 Filename: c7n_left/providers/terraform/provider.py
 Comment: 
 
 Filename: c7n_left/providers/terraform/resource.py
 Comment: 
 
+Filename: c7n_left/test.py
+Comment: 
+
 Filename: c7n_left/utils.py
 Comment: 
 
-Filename: c7n_left-0.1.5.dist-info/WHEEL
+Filename: c7n_left-0.1.6.dist-info/WHEEL
 Comment: 
 
-Filename: c7n_left-0.1.5.dist-info/entry_points.txt
+Filename: c7n_left-0.1.6.dist-info/entry_points.txt
 Comment: 
 
-Filename: c7n_left-0.1.5.dist-info/METADATA
+Filename: c7n_left-0.1.6.dist-info/METADATA
 Comment: 
 
-Filename: c7n_left-0.1.5.dist-info/RECORD
+Filename: c7n_left-0.1.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## c7n_left/cli.py

```diff
@@ -4,17 +4,18 @@
 import logging
 from pathlib import Path
 import sys
 
 import click
 from c7n.config import Config
 
+from .core import CollectionRunner, ExecutionFilter
 from .entry import initialize_iac
 from .output import get_reporter, report_outputs, summary_options
-from .core import CollectionRunner, ExecutionFilter
+from .test import TestReporter, TestRunner
 from .utils import load_policies
 
 
 log = logging.getLogger("c7n.iac")
 
 
 @click.group()
@@ -61,14 +62,39 @@
         log.warning("no policies found")
         sys.exit(1)
     reporter = get_reporter(config)
     runner = CollectionRunner(policies, config, reporter)
     sys.exit(int(runner.run()))
 
 
+@cli.command()
+@click.option("-p", "--policy-dir", type=click.Path(), required=True)
+@click.option(
+    "--filters", help="filter policies or resources as k=v pairs with globbing"
+)
+def test(policy_dir, filters):
+    """Run policy tests."""
+    policy_dir = Path(policy_dir)
+    source_dir = policy_dir / "tests"
+
+    config = Config.empty(
+        source_dir=source_dir,
+        policy_dir=policy_dir,
+        output_file=sys.stdout,
+        filters=filters,
+    )
+
+    reporter = TestReporter(None, config)
+    exec_filter = ExecutionFilter.parse(config)
+    config["exec_filter"] = exec_filter
+    policies = exec_filter.filter_policies(load_policies(policy_dir, config))
+    runner = TestRunner(policies, config, reporter)
+    sys.exit(int(runner.run()))
+
+
 if __name__ == "__main__":  # pragma: no cover
     try:
         cli()
     except Exception:
         import pdb, traceback
 
         traceback.print_exc()
```

## c7n_left/core.py

```diff
@@ -259,17 +259,21 @@
     def get_event(self):
         return {"config": self.options}
 
     @staticmethod
     def match_type(rtype, p):
         if isinstance(p.resource_type, str):
             return fnmatch.fnmatch(rtype, p.resource_type.split(".", 1)[-1])
+        found = False
         if isinstance(p.resource_type, list):
             for pr in p.resource_type:
-                return fnmatch.fnmatch(rtype, pr.split(".", 1)[-1])
+                if fnmatch.fnmatch(rtype, pr.split(".", 1)[-1]):
+                    found = True
+                    break
+        return found
 
 
 class IACSourceMode(PolicyExecutionMode):
     @property
     def manager(self):
         return self.policy.resource_manager
 
@@ -290,14 +294,23 @@
 
 
 class PolicyResourceResult:
     def __init__(self, resource, policy):
         self.resource = resource
         self.policy = policy
 
+    def as_dict(self):
+        return {
+            "policy": dict(self.policy.data),
+            "resource": dict(self.resource),
+            "file_path": str(self.resource.src_dir / self.resource.filename),
+            "file_line_start": self.resource.line_start,
+            "file_line_end": self.resource.line_end,
+        }
+
 
 class IACResourceManager(ResourceManager):
     filter_registry = FilterRegistry("iac.filters")
     action_registry = ActionRegistry("iac.actions")
     log = log
 
     def __init__(self, ctx, data):
```

## c7n_left/output.py

```diff
@@ -369,15 +369,10 @@
         lines = resource.get_source_lines()
         line_pairs = []
         index = resource.line_start
         for l in lines:
             line_pairs.append((index, l))
             index += 1
 
-        return {
-            "policy": dict(result.policy.data),
-            "resource": dict(resource),
-            "file_path": str(resource.src_dir / resource.filename),
-            "file_line_start": resource.line_start,
-            "file_line_end": resource.line_end,
-            "code_block": line_pairs,
-        }
+        formatted = result.as_dict()
+        formatted["code_block"] = line_pairs
+        return formatted
```

## c7n_left/providers/terraform/provider.py

```diff
@@ -39,15 +39,17 @@
 
     def initialize_policies(self, policies, options):
         for p in policies:
             p.data["mode"] = {"type": "terraform-source"}
         return policies
 
     def parse(self, source_dir):
-        graph = TerraformGraph(load_from_path(source_dir), source_dir)
+        graph = TerraformGraph(
+            load_from_path(source_dir, allow_downloads=True), source_dir
+        )
         graph.build()
         log.debug("Loaded %d %s resources", len(graph), self.type)
         return graph
 
     def match_dir(self, source_dir):
         files = list(source_dir.glob("*.tf"))
         files += list(source_dir.glob("*.tf.json"))
```

## c7n_left/utils.py

```diff
@@ -7,15 +7,15 @@
 
 
 SEVERITY_LEVELS = {"critical": 0, "high": 10, "medium": 20, "low": 30, "unknown": 40}
 
 
 def load_policies(policy_dir, options):
     loader = DirectoryLoader(config=options)
-    policies = loader.load_directory(policy_dir)
+    policies = loader.load_directory(policy_dir, recurse=False)
     if not policies:
         return ()
 
     providers = {p.provider_name for p in policies}
     assert len(providers), "only a single provider per policy dir"
     provider_name = providers.pop()
     provider = clouds[provider_name]()
```

## Comparing `c7n_left-0.1.5.dist-info/RECORD` & `c7n_left-0.1.6.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-c7n_left/cli.py,sha256=YDrHwRhQSOYH16Ili4MPFASMmhGuB5N_uCi69znhNVg,2173
-c7n_left/core.py,sha256=d11IoVSR0XKKPIJjS8dimTWUAydxNiytMWS93D_cBjs,11131
+c7n_left/cli.py,sha256=Ve97mFA__pIr7cVh5KUHpGVpk7N9bS0AnMXYfjYrgEE,2977
+c7n_left/core.py,sha256=HYj2zIa4p9DYWkh78SqRhTOQj4qN_ezMalQu4CfrYG4,11560
 c7n_left/entry.py,sha256=qnxA1j66drB8YISyJQmRiv0DKG0lv5SOogIuL2IDE6M,142
 c7n_left/filters.py,sha256=8yYvVBBtiozDpi8_KWSfJWflbqm6Fp9BvtPrsN2fIQk,4315
-c7n_left/output.py,sha256=6M7CNEarGlNSpWK48LSVhioxM0tPIUdWzAHNg-E3Qsw,12016
+c7n_left/output.py,sha256=aeaPfPFzLhQyc3HRnXY5l88HXUtIkmxPloAleEK2qVM,11802
 c7n_left/providers/terraform/__init__.py,sha256=BPUsPHvPInkb9N5fqhYccTRt_dWnFsdSEkFSDwgAFlY,121
 c7n_left/providers/terraform/graph.py,sha256=b47aqwKM6QCjdfRwWwteciplflNER-WKw86JTB-F1Gc,3282
-c7n_left/providers/terraform/provider.py,sha256=N7DHjsE0nWzs5dq6ILcrIg0MtEfnLuwZIY58Moo2GNg,1508
+c7n_left/providers/terraform/provider.py,sha256=5etOLvG-3nssOsfw1Dfs08QPTmujiBb6RvfZ1v_7Ve4,1552
 c7n_left/providers/terraform/resource.py,sha256=6sZhzlHrZ8unJKJViHsQkalQAspCzUyMAL8mjzngR98,945
-c7n_left/utils.py,sha256=h9wnv34Wd-67_pdXrFpaTDP-dCyXFyab5dXwFYsZas4,717
-c7n_left-0.1.5.dist-info/WHEEL,sha256=kLuE8m1WYU0Ig0_YEGrXyTtiJvKPpLpDEiChiNyei5Y,88
-c7n_left-0.1.5.dist-info/entry_points.txt,sha256=BP7MM3oxRCtY3qaC9GsUqrYj3962epelsmHx4XkQ6pY,45
-c7n_left-0.1.5.dist-info/RECORD,,
-c7n_left-0.1.5.dist-info/METADATA,sha256=t5KxcKp9HJZZHawBIae2C0tvoyK2BNJVEcWhQDTwjBg,4244
+c7n_left/test.py,sha256=iOW7nQLjCk9Luk4LhjAqKfKBnoy_tJCUrMPO9qKW20I,7208
+c7n_left/utils.py,sha256=V8yRbNRjKmuz24ZrfYwtYSLdyLMlZ0MVIhAkZdMwFbQ,732
+c7n_left-0.1.6.dist-info/WHEEL,sha256=kLuE8m1WYU0Ig0_YEGrXyTtiJvKPpLpDEiChiNyei5Y,88
+c7n_left-0.1.6.dist-info/entry_points.txt,sha256=BP7MM3oxRCtY3qaC9GsUqrYj3962epelsmHx4XkQ6pY,45
+c7n_left-0.1.6.dist-info/RECORD,,
+c7n_left-0.1.6.dist-info/METADATA,sha256=Uz4LdIO9V--nSuTpor_06G4UyqgxxJ5_UQmpgN-7rTo,12065
```

