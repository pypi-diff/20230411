# Comparing `tmp/revizor_fuzzer-1.2.2.tar.gz` & `tmp/revizor_fuzzer-1.2.3.tar.gz`

## Comparing `revizor_fuzzer-1.2.2.tar` & `revizor_fuzzer-1.2.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.2/.editorconfig
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.2/.gitmodules
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.2/.sync-exclude.lst
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.2/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     3598 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.2/CONTRIBUTING.md
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.2/Makefile
--rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.2/SECURITY.md
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.2/mkdocs.yml
--rwxr-xr-x   0        0        0      297 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.2/revizor.py
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.2/revizor/__init__.py
--rw-r--r--   0        0        0     4045 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.2/revizor/analyser.py
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.2/revizor/bigfuzz.yaml
--rwxr-xr-x   0        0        0     8189 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.2/revizor/cli.py
--rw-r--r--   0        0        0    10877 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.2/revizor/config.py
--rw-r--r--   0        0        0    10630 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.2/revizor/coverage.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.2/revizor/executor.py
--rw-r--r--   0        0        0     5968 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.2/revizor/factory.py
--rw-r--r--   0        0        0    15383 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.2/revizor/fuzzer.py
--rw-r--r--   0        0        0    24567 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.2/revizor/generator.py
--rw-r--r--   0        0        0     4625 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.2/revizor/input_generator.py
--rw-r--r--   0        0        0    26042 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.2/revizor/interfaces.py
--rw-r--r--   0        0        0     6249 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.2/revizor/isa_loader.py
--rw-r--r--   0        0        0    35874 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.2/revizor/model.py
--rw-r--r--   0        0        0     6271 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.2/revizor/postprocessor.py
--rw-r--r--   0        0        0    40667 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.2/revizor/unicorn.pyi
--rw-r--r--   0        0        0    13933 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.2/revizor/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.2/revizor/x86/__init__.py
--rwxr-xr-x   0        0        0    10643 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.2/revizor/x86/get_spec.py
--rw-r--r--   0        0        0     3725 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.2/revizor/x86/x86_config.py
--rw-r--r--   0        0        0     6504 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.2/revizor/x86/x86_executor.py
--rw-r--r--   0        0        0     5542 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.2/revizor/x86/x86_fuzzer.py
--rw-r--r--   0        0        0    37228 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.2/revizor/x86/x86_generator.py
--rw-r--r--   0        0        0    32893 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.2/revizor/x86/x86_model.py
--rw-r--r--   0        0        0     7072 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.2/revizor/x86/x86_target_desc.py
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.2/.gitignore
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.2/AUTHORS
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.2/LICENSE
--rw-r--r--   0        0        0     9196 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.2/README.md
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.2/pyproject.toml
--rw-r--r--   0        0        0    10063 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.3/.editorconfig
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.3/.gitmodules
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.3/.sync-exclude.lst
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     3598 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.3/CONTRIBUTING.md
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.3/Makefile
+-rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.3/SECURITY.md
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.3/mkdocs.yml
+-rwxr-xr-x   0        0        0      235 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.3/revizor.py
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.3/revizor/__init__.py
+-rw-r--r--   0        0        0     4045 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.3/revizor/analyser.py
+-rwxr-xr-x   0        0        0     8150 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.3/revizor/cli.py
+-rw-r--r--   0        0        0    10812 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.3/revizor/config.py
+-rw-r--r--   0        0        0    10630 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.3/revizor/coverage.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.3/revizor/executor.py
+-rw-r--r--   0        0        0     5968 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.3/revizor/factory.py
+-rw-r--r--   0        0        0    15571 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.3/revizor/fuzzer.py
+-rw-r--r--   0        0        0    24707 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.3/revizor/generator.py
+-rw-r--r--   0        0        0     4726 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.3/revizor/input_generator.py
+-rw-r--r--   0        0        0    26042 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.3/revizor/interfaces.py
+-rw-r--r--   0        0        0     6249 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.3/revizor/isa_loader.py
+-rw-r--r--   0        0        0    35965 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.3/revizor/model.py
+-rw-r--r--   0        0        0     6271 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.3/revizor/postprocessor.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.3/revizor/py.typed
+-rw-r--r--   0        0        0    40667 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.3/revizor/unicorn.pyi
+-rw-r--r--   0        0        0    14277 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.3/revizor/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.3/revizor/x86/__init__.py
+-rwxr-xr-x   0        0        0    10643 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.3/revizor/x86/get_spec.py
+-rw-r--r--   0        0        0     3725 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.3/revizor/x86/x86_config.py
+-rw-r--r--   0        0        0     6564 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.3/revizor/x86/x86_executor.py
+-rw-r--r--   0        0        0     5542 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.3/revizor/x86/x86_fuzzer.py
+-rw-r--r--   0        0        0    37970 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.3/revizor/x86/x86_generator.py
+-rw-r--r--   0        0        0    32893 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.3/revizor/x86/x86_model.py
+-rw-r--r--   0        0        0     7072 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.3/revizor/x86/x86_target_desc.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.3/.gitignore
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.3/AUTHORS
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.3/LICENSE
+-rw-r--r--   0        0        0     9564 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.3/README.md
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0    10431 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.3/PKG-INFO
```

### Comparing `revizor_fuzzer-1.2.2/.editorconfig` & `revizor_fuzzer-1.2.3/.editorconfig`

 * *Files identical despite different names*

### Comparing `revizor_fuzzer-1.2.2/CONTRIBUTING.md` & `revizor_fuzzer-1.2.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `revizor_fuzzer-1.2.2/SECURITY.md` & `revizor_fuzzer-1.2.3/SECURITY.md`

 * *Files identical despite different names*

### Comparing `revizor_fuzzer-1.2.2/mkdocs.yml` & `revizor_fuzzer-1.2.3/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `revizor_fuzzer-1.2.2/revizor/analyser.py` & `revizor_fuzzer-1.2.3/revizor/analyser.py`

 * *Files identical despite different names*

### Comparing `revizor_fuzzer-1.2.2/revizor/cli.py` & `revizor_fuzzer-1.2.3/revizor/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """
 File: Function definitions for using Revizor as command-line tool
 (Note: the actual CLI is accessed via revizor.py)
 
 Copyright (C) Microsoft Corporation
 SPDX-License-Identifier: MIT
 """
+
 import os
 import yaml
 from typing import Dict
 from argparse import ArgumentParser
 from .factory import get_minimizer, get_fuzzer, get_downloader
 from .fuzzer import Fuzzer
 from .config import CONF
-from .util import LOGGER
 
 
 def main() -> int:
     parser = ArgumentParser(description='', add_help=False)
     subparsers = parser.add_subparsers(dest='subparser_name')
     subparsers.required = True
 
@@ -221,15 +221,14 @@
     # Update configuration
     if getattr(args, 'config', None):
         CONF.config_path = args.config
         with open(args.config, "r") as f:
             config_update: Dict = yaml.safe_load(f)
         for var, value in config_update.items():
             setattr(CONF, var, value)
-    LOGGER.set_logging_modes()
 
     # Fuzzing
     if args.subparser_name == 'fuzz':
         # Make sure we're ready for fuzzing
         if args.working_directory and not os.path.isdir(args.working_directory):
             SystemExit("The working directory does not exist")
 
@@ -268,15 +267,15 @@
     # Test case minimisation
     if args.subparser_name == "minimize":
         minimizer = get_minimizer(args.instruction_set)
         minimizer.minimize(args.infile, args.outfile, args.num_inputs, args.add_fences)
         return 0
 
     if args.subparser_name == "download_spec":
-        get_downloader(args.architecture, args.extensions, args.outfile).run()
+        get_downloader(args.architecture, args.extensions, args.outfile).run()  # type: ignore
         return 0
 
     raise Exception("Unreachable")
 
 
 if __name__ == '__main__':
     print("[ERROR]", "This file is not meant to be run directly. Use `revizor.py` instead.")
```

### Comparing `revizor_fuzzer-1.2.2/revizor/config.py` & `revizor_fuzzer-1.2.3/revizor/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -148,24 +148,22 @@
     """ multiline_output: """
     logging_modes: List[str] = ["info", "stat"]
     """ logging_modes: """
     color: bool = False
 
     # ==============================================================================================
     # Internal
-    _instance = None
+    _borg_shared_state: Dict = {}
     _no_generation: bool = False
     _option_values: Dict[str, List] = {}  # set by ISA-specific config.py
     _default_instruction_blocklist: List[str] = []
 
-    # Implementation of singleton
-    def __new__(cls, *args, **kwargs):
-        if not isinstance(cls._instance, cls):
-            cls._instance = object.__new__(cls, *args, **kwargs)
-        return cls._instance
+    # Implementation of Borg pattern
+    def __init__(self) -> None:
+        self.setattr_internal("__dict__", self._borg_shared_state)
 
     def __setattr__(self, name, value):
         # print(f"CONF: setting {name} to {value}")
 
         # Sanity checks
         if name[0] == "_":
             raise ConfigException(
```

### Comparing `revizor_fuzzer-1.2.2/revizor/coverage.py` & `revizor_fuzzer-1.2.3/revizor/coverage.py`

 * *Files identical despite different names*

### Comparing `revizor_fuzzer-1.2.2/revizor/factory.py` & `revizor_fuzzer-1.2.3/revizor/factory.py`

 * *Files identical despite different names*

### Comparing `revizor_fuzzer-1.2.2/revizor/fuzzer.py` & `revizor_fuzzer-1.2.3/revizor/fuzzer.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,40 +11,43 @@
 import copy
 
 from . import factory
 from .interfaces import CTrace, HTrace, Input, InputTaint, EquivalenceClass, TestCase, Generator, \
     InputGenerator, Model, Executor, Analyser, Coverage, InputID, Measurement
 from .isa_loader import InstructionSet
 from .config import CONF
-from .util import STAT, LOGGER, TWOS_COMPLEMENT_MASK_64, bit_count
+from .util import Logger, STAT, TWOS_COMPLEMENT_MASK_64, bit_count, pretty_trace
 
 
 class Fuzzer:
     instruction_set: InstructionSet
     existing_test_case: str
     input_paths: List[str]
 
     generator: Generator
     input_gen: InputGenerator
     executor: Executor
     model: Model
     analyser: Analyser
     coverage: Coverage
 
+    LOG: Logger  # name capitalized to make logging easily distinguishable from the main logic
+
     def __init__(self,
                  instruction_set_spec: str,
                  work_dir: str,
                  existing_test_case: str = "",
                  inputs: List[str] = []):
         self._adjust_config(existing_test_case)
         self.existing_test_case = existing_test_case
         self.input_paths = inputs
 
         self.instruction_set = InstructionSet(instruction_set_spec, CONF.instruction_categories)
         self.work_dir = work_dir
+        self.LOG = Logger()
 
     def _adjust_config(self, existing_test_case):
         if existing_test_case:
             CONF.setattr_internal("_no_generation", True)
             CONF.setattr_internal("_default_instruction_blocklist", [])
             CONF.register_blocklist = []
         # more adjustments could be implemented by subclasses!
@@ -62,28 +65,28 @@
 
     def start(self,
               num_test_cases: int,
               num_inputs: int,
               timeout: int,
               nonstop: bool = False) -> bool:
         start_time = datetime.today()
-        LOGGER.fuzzer_start(num_test_cases, start_time)
+        self.LOG.fuzzer_start(num_test_cases, start_time)
 
         # create all main modules
         self.initialize_modules()
 
         for i in range(num_test_cases):
-            LOGGER.fuzzer_start_round(i)
-            LOGGER.dbg_report_coverage(i, self.coverage.get_brief())
+            self.LOG.fuzzer_start_round(i)
+            self.LOG.dbg_report_coverage(i, self.coverage.get_brief())
 
             # terminate the fuzzer if the timeout has expired
             if timeout:
                 now = datetime.today()
                 if (now - start_time).total_seconds() > timeout:
-                    LOGGER.fuzzer_timeout()
+                    self.LOG.fuzzer_timeout()
                     break
 
             # Generate a test case
             test_case: TestCase
             if self.existing_test_case:
                 test_case = self.generator.load(self.existing_test_case)
             else:
@@ -105,21 +108,21 @@
             if self.filter(test_case, inputs):
                 continue
 
             # Fuzz the test case
             violation = self.fuzzing_round(test_case, inputs)
 
             if violation:
-                LOGGER.fuzzer_report_violations(violation, self.model)
+                self.LOG.fuzzer_report_violations(violation, self.model)
                 self.store_test_case(test_case, violation)
                 STAT.violations += 1
                 if not nonstop:
                     break
 
-        LOGGER.fuzzer_finish()
+        self.LOG.fuzzer_finish()
         return STAT.violations > 0
 
     def filter(self, test_case, inputs):
         return False  # implemented by architecture-specific subclasses
 
     def fuzzing_round(self, test_case: TestCase, inputs: List[Input]) -> Optional[EquivalenceClass]:
         self.model.load_test_case(test_case)
@@ -134,23 +137,23 @@
         # so that we can detect contract violations (note that it wasn't necessary
         # up to this point because we weren't testing against a contract)
         boosted_inputs: List[Input] = self.boost_inputs(inputs, 1)
 
         # check for violations
         ctraces = self.model.trace_test_case(boosted_inputs, 1)
         htraces = self.executor.trace_test_case(boosted_inputs, CONF.executor_repetitions)
-        LOGGER.trc_fuzzer_dump_traces(self.model, boosted_inputs, htraces, ctraces,
-                                      self.executor.get_last_feedback())
+        self.LOG.trc_fuzzer_dump_traces(self.model, boosted_inputs, htraces, ctraces,
+                                        self.executor.get_last_feedback())
         violations = self.analyser.filter_violations(boosted_inputs, ctraces, htraces, True)
         if not violations:  # nothing detected? -> we are done here, move to next test case
             return None
 
         # 2. Repeat with with max nesting
         if 'seq' not in CONF.contract_execution_clause:
-            LOGGER.fuzzer_nesting_increased()
+            self.LOG.fuzzer_nesting_increased()
             boosted_inputs = self.boost_inputs(inputs, CONF.model_max_nesting)
             ctraces = self.model.trace_test_case(boosted_inputs, CONF.model_max_nesting)
             htraces = self.executor.trace_test_case(boosted_inputs, CONF.executor_repetitions)
             violations = self.analyser.filter_violations(boosted_inputs, ctraces, htraces, True)
             if not violations:
                 return None
 
@@ -163,15 +166,15 @@
         # 4. Check if the violation survives priming
         if not CONF.enable_priming:
             return violations[-1]
         STAT.required_priming += 1
 
         violation_stack = list(violations)  # make a copy
         while violation_stack:
-            LOGGER.fuzzer_priming(len(violation_stack))
+            self.LOG.fuzzer_priming(len(violation_stack))
             violation: EquivalenceClass = violation_stack.pop()
             if self.priming(violation, boosted_inputs):
                 break
         else:
             # All violations were cleared by priming.
             return None
 
@@ -207,21 +210,21 @@
         with open(f"{self.work_dir}/report-{timestamp}.txt", "w") as f:
             f.write("# Violation Report\n\n")
             f.write(f"Detected: {datetime.today().strftime('%d.%m.%y at %H:%M:%S')}\n\n")
             f.write("## Counterexample Inputs\n")
             for m in violation.measurements:
                 f.write(f"\nInput #{m.input_id}\n")
                 f.write(f"* Contract trace hash: {m.ctrace}\n")
-                f.write(f"* Hardware trace: {LOGGER.pretty_bitmap(m.htrace)}\n")
+                f.write(f"* Hardware trace: {pretty_trace(m.htrace)}\n")
 
     # ==============================================================================================
     # Single-stage interfaces
     def generate_test_batch(self, program_generator_seed: int, num_test_cases: int, num_inputs: int,
                             permit_overwrite: bool):
-        LOGGER.fuzzer_start(0, datetime.today())
+        self.LOG.fuzzer_start(0, datetime.today())
 
         # prepare for generation
         STAT.test_cases = num_test_cases
         CONF.program_generator_seed = program_generator_seed
         program_gen = factory.get_program_generator(self.instruction_set,
                                                     CONF.program_generator_seed)
         input_gen = factory.get_input_generator(CONF.input_gen_seed)
@@ -229,28 +232,29 @@
         # generate test cases
         Path(self.work_dir).mkdir(exist_ok=True)
         for i in range(0, num_test_cases):
             test_case_dir = self.work_dir + "/tc" + str(i)
             try:
                 Path(test_case_dir).mkdir(exist_ok=permit_overwrite)
             except FileExistsError:
-                LOGGER.error(f"Directory '{test_case_dir}' already exists\n"
-                             "       Use --permit-overwrite to overwrite the test case")
+                self.LOG.error(f"Directory '{test_case_dir}' already exists\n"
+                               "       Use --permit-overwrite to overwrite the test case")
 
             program_gen.create_test_case(test_case_dir + "/" + "program.asm", True)
             inputs = input_gen.generate(num_inputs)
             for j, input_ in enumerate(inputs):
                 input_.save(f"{test_case_dir}/input{j}.bin")
 
-        LOGGER.fuzzer_finish()
+        self.LOG.fuzzer_finish()
 
     @staticmethod
     def analyse_traces_from_files(ctrace_file: str, htrace_file: str):
-        LOGGER.dbg_violation = False  # make sure we don't try to call the model
-        LOGGER.fuzzer_start(0, datetime.today())
+        logger = Logger()
+        logger.dbg_violation = False  # make sure we don't try to call the model
+        logger.fuzzer_start(0, datetime.today())
         STAT.test_cases = 1
 
         # read traces
         ctraces: List[CTrace] = []
         htraces: List[HTrace] = []
 
         with open(ctrace_file, 'r') as f:
@@ -267,17 +271,17 @@
 
         # check for violations
         analyser = factory.get_analyser()
         violations = analyser.filter_violations(dummy_inputs, ctraces, htraces, True)
 
         # print results
         if violations:
-            LOGGER.fuzzer_report_violations(violations[0], None)
+            logger.fuzzer_report_violations(violations[0], None)
 
-        LOGGER.fuzzer_finish()
+        logger.fuzzer_finish()
 
     # ==============================================================================================
     # Priming and reproducibility
     def check_if_reproducible(self, violations: List[EquivalenceClass], inputs: List[Input],
                               org_htraces: List[HTrace]) -> bool:
         # re-collect htraces
         htraces: List[HTrace] = self.executor.trace_test_case(inputs, CONF.executor_repetitions)
@@ -339,19 +343,19 @@
     """
 
     def __init__(self,
                  instruction_set_spec: str,
                  work_dir: str,
                  existing_test_case: str = "",
                  inputs: List[str] = []):
-        LOGGER.warning("fuzzer", "Running in architectural mode. "
-                       "Contract violations can't be detected!")
         CONF.setattr_internal('executor_mode', "GPR")
         CONF.contract_observation_clause = 'gpr'
         super().__init__(instruction_set_spec, work_dir, existing_test_case, inputs)
+        self.LOG.warning("fuzzer", "Running in architectural mode. "
+                         "Contract violations can't be detected!")
 
     def fuzzing_round(self, test_case: TestCase, inputs: List[Input]) -> Optional[EquivalenceClass]:
         self.model.load_test_case(test_case)
         self.executor.load_test_case(test_case)
         self.coverage.load_test_case(test_case)
 
         # collect architectural hardware traces
```

### Comparing `revizor_fuzzer-1.2.2/revizor/generator.py` & `revizor_fuzzer-1.2.3/revizor/generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from subprocess import CalledProcessError, run
 from collections import OrderedDict
 
 from .isa_loader import InstructionSet
 from .interfaces import Generator, TestCase, Operand, RegisterOperand, FlagsOperand, \
     MemoryOperand, ImmediateOperand, AgenOperand, LabelOperand, OT, Instruction, BasicBlock, \
     Function, OperandSpec, InstructionSpec, CondOperand, TargetDesc
-from .util import NotSupportedException, LOGGER
+from .util import NotSupportedException, Logger
 from .config import CONF
 
 
 # Helpers
 class GeneratorException(Exception):
     pass
 
@@ -63,17 +63,20 @@
     """
     instruction_set: InstructionSet
     test_case: TestCase
     passes: List[Pass]  # set by subclasses
     printer: Printer  # set by subclasses
     target_desc: TargetDesc  # set by subclasses
 
+    LOG: Logger  # name capitalized to make logging easily distinguishable from the main logic
+
     def __init__(self, instruction_set: InstructionSet, seed: int):
         super().__init__(instruction_set, seed)
-        LOGGER.dbg_gen_instructions(instruction_set.instructions)
+        self.LOG = Logger()
+        self.LOG.dbg_gen_instructions(instruction_set.instructions)
         self.control_flow_instructions = \
             [i for i in self.instruction_set.instructions if i.control_flow]
         assert self.control_flow_instructions or CONF.max_bb_per_function <= 1, \
                "The instruction set is insufficient to generate a test case"
 
         self.non_control_flow_instructions = \
             [i for i in self.instruction_set.instructions if not i.control_flow]
@@ -98,16 +101,16 @@
 
     def create_test_case(self, asm_file: str, disable_assembler: bool = False) -> TestCase:
         self.test_case = TestCase(self._state)
 
         # set seeds
         if self._state == 0:
             self._state = random.randint(1, 1000000)
-            LOGGER.inform("prog_gen",
-                          f"Setting program_generator_seed to random value: {self._state}")
+            self.LOG.inform("prog_gen",
+                            f"Setting program_generator_seed to random value: {self._state}")
         random.seed(self._state)
         self._state += 1
 
         # create the main function
         func = self.generate_function(".function_main")
 
         # fill the function with instructions
@@ -155,22 +158,23 @@
                     msg += f"\n  Line {line}\n    (the line was parsed as {parsed})"
             return msg
 
         try:
             out = run(f"as {asm_file} -o {bin_file}", shell=True, check=True, capture_output=True)
         except CalledProcessError as e:
             error_msg = e.stderr.decode()
-            if "Assembler messages:" not in error_msg:
+            if "Assembler messages:" in error_msg:
+                print(pretty_error_msg(error_msg))
+            else:
                 print(error_msg)
-                raise e
-            LOGGER.error(pretty_error_msg(error_msg))
+            raise e
 
         output = out.stderr.decode()
         if "Assembler messages:" in output:
-            LOGGER.warning("generator", pretty_error_msg(output))
+            print("WARNING: [generator]" + pretty_error_msg(output))
 
         run(f"strip --remove-section=.note.gnu.property {bin_file}", shell=True, check=True)
         run(f"objcopy {bin_file} -O binary {bin_file}", shell=True, check=True)
 
     def load(self, asm_file: str) -> TestCase:
         test_case = TestCase(0)
         test_case.asm_path = asm_file
```

### Comparing `revizor_fuzzer-1.2.2/revizor/input_generator.py` & `revizor_fuzzer-1.2.3/revizor/input_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,30 +7,34 @@
 import os
 import random
 import numpy as np
 from abc import abstractmethod
 from typing import List
 from .interfaces import Input, InputTaint, InputGenerator
 from .config import CONF
-from .util import LOGGER
+from .util import Logger
 
 POW32 = pow(2, 32)
 
 
 class InputGeneratorCommon(InputGenerator):
 
+    def __init__(self, seed: int):
+        super().__init__(seed)
+        self.LOG = Logger()
+
     @abstractmethod
     def _generate_one(self) -> Input:
         pass
 
     def generate(self, count: int) -> List[Input]:
         # if it's the first invocation and the seed is zero - use random seed
         if self._state == 0:
             self._state = random.randint(0, pow(2, 32) - 1)
-            LOGGER.inform("input_gen", f"Setting input seed to: {self._state}")
+            self.LOG.inform("input_gen", f"Setting input seed to: {self._state}")
 
         generated_inputs = []
         for _ in range(count):
             input_ = self._generate_one()
             generated_inputs.append(input_)
         return generated_inputs
 
@@ -64,16 +68,16 @@
         inputs = []
         for input_path in input_paths:
             input_ = Input()
 
             # check that the file is not corrupted
             size = os.path.getsize(input_path)
             if size != len(input_) * 8:
-                LOGGER.error(f"Incorrect size of input `{input_path}` "
-                             f"({size} B, expected {len(input_) * 8} B)")
+                self.LOG.error(f"Incorrect size of input `{input_path}` "
+                               f"({size} B, expected {len(input_) * 8} B)")
 
             input_.load(input_path)
             inputs.append(input_)
         return inputs
 
 
 class LegacyRandomInputGenerator(InputGeneratorCommon):
```

### Comparing `revizor_fuzzer-1.2.2/revizor/interfaces.py` & `revizor_fuzzer-1.2.3/revizor/interfaces.py`

 * *Files identical despite different names*

### Comparing `revizor_fuzzer-1.2.2/revizor/isa_loader.py` & `revizor_fuzzer-1.2.3/revizor/isa_loader.py`

 * *Files identical despite different names*

### Comparing `revizor_fuzzer-1.2.2/revizor/model.py` & `revizor_fuzzer-1.2.3/revizor/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from unicorn import Uc, UcError, UC_MEM_WRITE, UC_MEM_READ, UC_SECOND_SCALE, UC_HOOK_MEM_READ, \
     UC_HOOK_MEM_WRITE, UC_HOOK_CODE, UC_HOOK_MEM_UNMAPPED
 
 from .interfaces import CTrace, TestCase, Model, InputTaint, Instruction, ExecutionTrace, \
     TracedInstruction, TracedMemAccess, Input, Tracer, \
     RegisterOperand, FlagsOperand, MemoryOperand, TaintTrackerInterface, TargetDesc
 from .config import CONF
-from .util import LOGGER, NotSupportedException
+from .util import Logger, NotSupportedException
 
 
 # ==================================================================================================
 # Abstract Interfaces
 # ==================================================================================================
 class UnicornTargetDesc(ABC):
     registers: List[int]
@@ -40,14 +40,15 @@
     trace: List[int]
     execution_trace: ExecutionTrace
     instruction_id: int
 
     def __init__(self):
         super().__init__()
         self.trace = []
+        self.LOG = Logger()
 
     def init_trace(self, emulator, target_desc: UnicornTargetDesc) -> None:
         self.trace = []
         self.execution_trace = []
 
     def get_contract_trace(self, model: Model) -> CTrace:
         # make the trace reproducible by normalizing the addresses
@@ -76,43 +77,45 @@
         self.trace.append(address)
         model.taint_tracker.taint_pc()
 
     def observe_mem_access(self, access, address: int, size: int, value: int,
                            model: UnicornModel) -> None:
         normalized_address = address - model.sandbox_base
         is_store = (access != UC_MEM_READ)
-        LOGGER.dbg_model_mem_access(normalized_address, value, address, size, is_store, model)
+        self.LOG.dbg_model_mem_access(normalized_address, value, address, size, is_store, model)
 
         if model.in_speculation:
             return
 
         if model.execution_tracing_enabled:
             val = value if is_store else int.from_bytes(
                 model.emulator.mem_read(address, size), byteorder='little')
             traced_instruction = self.execution_trace[self.instruction_id]
             traced_instruction.accesses.append(TracedMemAccess(normalized_address, val, is_store))
 
     def observe_instruction(self, address: int, size: int, model) -> None:
         normalized_address = address - model.code_start
         if normalized_address in model.test_case.address_map:
-            LOGGER.dbg_model_instruction(normalized_address, model)
+            self.LOG.dbg_model_instruction(normalized_address, model)
 
         if model.in_speculation:
             return
 
         if model.execution_tracing_enabled:
             self.execution_trace.append(TracedInstruction(normalized_address, []))
             self.instruction_id = len(self.execution_trace) - 1
 
 
 class UnicornModel(Model, ABC):
     """
     Base class for all Unicorn-based models.
     Serves as an adapter between Unicorn and our fuzzer.
     """
+    LOG: Logger
+
     CODE_SIZE = 4 * 1024
     MAIN_REGION_SIZE = CONF.input_main_region_size
     FAULTY_REGION_SIZE = CONF.input_faulty_region_size
     OVERFLOW_REGION_SIZE = 4096
 
     emulator: Uc
     target_desc: UnicornTargetDesc
@@ -147,14 +150,16 @@
 
     # set by subclasses
     architecture: Tuple[int, int]
     flags_id: int
 
     def __init__(self, sandbox_base, code_start):
         super().__init__(sandbox_base, code_start)
+        self.LOG = Logger()
+
         self.code_start = code_start
         self.sandbox_base = sandbox_base
 
         self.lower_overflow_base = self.sandbox_base - self.OVERFLOW_REGION_SIZE
         self.upper_overflow_base = \
             self.sandbox_base + self.MAIN_REGION_SIZE + self.FAULTY_REGION_SIZE
         self.main_region = self.sandbox_base
@@ -227,15 +232,15 @@
             emulator.hook_add(UC_HOOK_MEM_READ | UC_HOOK_MEM_WRITE, self.trace_mem_access, self)
             emulator.hook_add(UC_HOOK_MEM_UNMAPPED, self.trace_mem_access, self)
             emulator.hook_add(UC_HOOK_CODE, self.instruction_hook, self)
 
             self.emulator = emulator
 
         except UcError as e:
-            LOGGER.error("[UnicornModel:load_test_case] %s" % e)
+            self.LOG.error("[UnicornModel:load_test_case] %s" % e)
 
     @abstractmethod
     def _load_input(self, input_: Input):
         """
         Load registers with given input: this is architecture specific
         """
         pass
@@ -247,15 +252,15 @@
         self.nesting = nesting
 
         contract_traces: List[CTrace] = []
         execution_traces: List[ExecutionTrace] = []
         taints = []
 
         for index, input_ in enumerate(inputs):
-            LOGGER.dbg_model_header(index)
+            self.LOG.dbg_model_header(index)
 
             self._load_input(input_)
             self.reset_model()
             start_address = self.code_start
             while True:
                 self.pending_fault_id = 0
 
@@ -415,15 +420,15 @@
 
         # an expected fault - terminate execution
         if errno in self.handled_faults:
             return self.code_end
 
         # unexpected fault - throw an error
         self.print_state()
-        LOGGER.error(f"[UnicornModel:trace_test_case] {errno} {self.errno_to_str(errno)}")
+        self.LOG.error(f"Unexpected exception {errno} {self.errno_to_str(errno)}", print_tb=True)
 
     @staticmethod
     @abstractmethod
     def trace_instruction(emulator: Uc, address: int, size: int, model: UnicornModel) -> None:
         pass
 
     @staticmethod
@@ -645,15 +650,15 @@
 
     def rollback(self) -> int:
         # restore register values
         state, next_instr, flags, spec_window = self.checkpoints.pop()
         if not self.checkpoints:
             self.in_speculation = False
 
-        LOGGER.dbg_model_rollback(next_instr, self.code_start)
+        self.LOG.dbg_model_rollback(next_instr, self.code_start)
         self.latest_rollback_address = next_instr
 
         # restore the speculation state
         self.emulator.context_restore(state)
         self.speculation_window = spec_window
 
         # rollback memory changes
```

### Comparing `revizor_fuzzer-1.2.2/revizor/postprocessor.py` & `revizor_fuzzer-1.2.3/revizor/postprocessor.py`

 * *Files identical despite different names*

### Comparing `revizor_fuzzer-1.2.2/revizor/unicorn.pyi` & `revizor_fuzzer-1.2.3/revizor/unicorn.pyi`

 * *Files identical despite different names*

### Comparing `revizor_fuzzer-1.2.2/revizor/util.py` & `revizor_fuzzer-1.2.3/revizor/util.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,37 +2,44 @@
 File: Global classes that provide service to all Revizor modules
 
 Copyright (C) Microsoft Corporation
 SPDX-License-Identifier: MIT
 """
 
 from datetime import datetime
-from typing import NoReturn
+from typing import NoReturn, Dict
 from pprint import pformat
+from traceback import print_stack
 from .interfaces import EquivalenceClass
 from .config import CONF
 
 MASK_64BIT = pow(2, 64)
 POW2_64 = pow(2, 64)
 TWOS_COMPLEMENT_MASK_64 = pow(2, 64) - 1
 
 
 class StatisticsCls:
-    test_cases = 0
-    num_inputs = 0
-    eff_classes = 0
-    single_entry_classes = 0
-    required_priming = 0
-    flaky_violations = 0
-    violations = 0
-    coverage = 0
+    _borg_shared_state: Dict = {}
+
+    test_cases: int = 0
+    num_inputs: int = 0
+    eff_classes: int = 0
+    single_entry_classes: int = 0
+    required_priming: int = 0
+    flaky_violations: int = 0
+    violations: int = 0
+    coverage: int = 0
     analysed_test_cases: int = 0
     spec_filter: int = 0
     observ_filter: int = 0
 
+    # Implementation of Borg pattern
+    def __init__(self) -> None:
+        self.__dict__ = self._borg_shared_state
+
     def __str__(self):
         total_clss = self.eff_classes + self.single_entry_classes
         effectiveness = self.eff_classes / total_clss if total_clss else 0
         total_clss_per_test_case = total_clss / self.analysed_test_cases \
             if self.analysed_test_cases else 0
         effective_clss = self.eff_classes / self.analysed_test_cases \
             if self.analysed_test_cases else 0
@@ -94,44 +101,53 @@
     msg: str = ""
     line_ending: str = ""
     redraw_mode: bool = True
 
     # info modes
     info: bool = False
     stat: bool = False
+    debug: bool = False
 
-    # debugging
+    # debugging specific modules
     dbg_timestamp: bool = False
     dbg_violation: bool = False
     dbg_traces: bool = False
     dbg_model: bool = False
     dbg_coverage: bool = False
     dbg_generator: bool = False
 
     def __init__(self) -> None:
-        pass
+        self.update_logging_modes()
 
-    def set_logging_modes(self):
+    def update_logging_modes(self):
         for mode in CONF.logging_modes:
             if not mode:
                 continue
             if getattr(self, mode, None) is None:
                 self.error(f"Unknown value '{mode}' of config variable 'logging_modes'")
             setattr(self, mode, True)
+            if "dbg" in mode:  # enable debug mode if any debug mode is enabled
+                self.debug = True
 
         if not __debug__:
             if self.dbg_timestamp or self.dbg_model or self.dbg_coverage or self.dbg_traces\
                or self.dbg_generator:
                 self.warning(
                     "", "Current value of `logging_modes` requires debugging mode!\n"
                     "Remove '-O' from python arguments")
 
-    def error(self, msg) -> NoReturn:
+    def error(self, msg: str, print_tb: bool = False) -> NoReturn:
         if self.redraw_mode:
             print("")
+
+        if print_tb:
+            print("Encountered an unrecoverable error\nTraceback:")
+            print_stack()
+            print("\n")
+
         print(f"ERROR: {msg}")
         exit(1)
 
     def warning(self, src, msg) -> None:
         if self.redraw_mode:
             print("")
         print(f"WARNING: [{src}] {msg}")
@@ -139,17 +155,18 @@
     def inform(self, src, msg, end="\n") -> None:
         if self.info:
             if self.redraw_mode:
                 print("")
             print(f"INFO: [{src}] {msg}", end=end, flush=True)
 
     def dbg(self, src, msg) -> None:
-        if self.redraw_mode:
-            print("")
-        print(f"DBG: [{src}] {msg}")
+        if self.debug:
+            if self.redraw_mode:
+                print("")
+            print(f"DBG: [{src}] {msg}")
 
     # ==============================================================================================
     # Generator
     def dbg_gen_instructions(self, instructions):
         if not __debug__:
             return
 
@@ -234,32 +251,30 @@
                 if CONF.contract_observation_clause == 'l1d':
                     for i in range(len(htraces)):
                         if i > 100:
                             self.warning("fuzzer", "Trace output is limited to 100 traces")
                             break
                         ctrace = ctraces[i]
                         print("    ")
-                        print(
-                            f"CTr{i:<2} {self.pretty_bitmap(ctrace, ctrace > pow(2, 64), '      ')}"
-                        )
-                        print(f"HTr{i:<2} {self.pretty_bitmap(htraces[i])}")
+                        print(f"CTr{i:<2} {pretty_trace(ctrace, ctrace > pow(2, 64), '      ')}")
+                        print(f"HTr{i:<2} {pretty_trace(htraces[i])}")
                         print(f"Feedback{i}: {hw_feedback[i]}")
 
                     return
 
                 org_debug_state = self.dbg_model
                 self.dbg_model = False
                 for i in range(len(htraces)):
                     if i > 100:
                         self.warning("fuzzer", "Trace output is limited to 100 traces")
                         break
                     ctrace_full = model.dbg_get_trace_detailed(inputs[i], 1)
                     print("    ")
                     print(f"CTr{i}: {ctrace_full}")
-                    print(f"HTr{i}: {self.pretty_bitmap(htraces[i])}")
+                    print(f"HTr{i}: {pretty_trace(htraces[i])}")
                     print(f"Feedback{i}: {hw_feedback[i]}")
                 self.dbg_model = org_debug_state
 
     def fuzzer_report_violations(self, violation: EquivalenceClass, model):
         print("\n\n================================ Violations detected ==========================")
         print("Contract trace:")
         if CONF.contract_observation_clause != 'l1d':
@@ -273,15 +288,15 @@
         print("Hardware traces:")
         for htrace, measurements in violation.htrace_map.items():
             inputs = [m.input_id for m in measurements]
             if len(inputs) < 4:
                 print(f" Inputs {inputs}:")
             else:
                 print(f" Inputs {inputs[:4]} (+ {len(inputs) - 4} ):")
-            print(f"  {self.pretty_bitmap(htrace)}")
+            print(f"  {pretty_trace(htrace)}")
         print("")
 
         if not __debug__:
             return
 
         if self.dbg_violation:
             # print details
@@ -343,45 +358,41 @@
     # ==============================================================================================
     # Coverage
     def dbg_report_coverage(self, round_id, msg):
         if __debug__:
             if self.dbg_coverage and round_id and round_id % 100 == 0:
                 print(f"\nDBG: [coverage] {msg}")
 
-    # ==============================================================================================
-    # Helpers
-    def pretty_bitmap(self, bits: int, merged=False, offset: str = ""):
-        if not merged:
-            s = f"{bits:064b}"
-        else:
-            s = f"{bits % MASK_64BIT:064b} [ns]\n" \
-                f"{offset}{(bits >> 64) % MASK_64BIT:064b} [s]"
-        s = s.replace("0", ".").replace("1", "^")
-        if CONF.color:
-            s = '\033[33;34m' + s[0:8] + '\033[33;32m' + s[8:16] \
-                + '\033[33;34m' + s[16:24] + '\033[33;32m' + s[24:32] \
-                + '\033[33;34m' + s[32:40] + '\033[33;32m' + s[40:48] \
-                + '\033[33;34m' + s[48:56] + '\033[33;32m' + s[56:64] \
-                + "\033[0m" + s[64:]
-        return s
-
-
-LOGGER = Logger()
-
 
 # ==================================================================================================
 # Small helper functions
 # ==================================================================================================
 def bit_count(n):
     count = 0
     while n:
         count += n & 1
         n >>= 1
     return count
 
 
+def pretty_trace(bits: int, merged=False, offset: str = ""):
+    if not merged:
+        s = f"{bits:064b}"
+    else:
+        s = f"{bits % MASK_64BIT:064b} [ns]\n" \
+            f"{offset}{(bits >> 64) % MASK_64BIT:064b} [s]"
+    s = s.replace("0", ".").replace("1", "^")
+    if CONF.color:
+        s = '\033[33;34m' + s[0:8] + '\033[33;32m' + s[8:16] \
+            + '\033[33;34m' + s[16:24] + '\033[33;32m' + s[24:32] \
+            + '\033[33;34m' + s[32:40] + '\033[33;32m' + s[40:48] \
+            + '\033[33;34m' + s[48:56] + '\033[33;32m' + s[56:64] \
+            + "\033[0m" + s[64:]
+    return s
+
+
 class NotSupportedException(Exception):
     pass
 
 
 class UnreachableCode(Exception):
     pass
```

### Comparing `revizor_fuzzer-1.2.2/revizor/x86/get_spec.py` & `revizor_fuzzer-1.2.3/revizor/x86/get_spec.py`

 * *Files identical despite different names*

### Comparing `revizor_fuzzer-1.2.2/revizor/x86/x86_config.py` & `revizor_fuzzer-1.2.3/revizor/x86/x86_config.py`

 * *Files identical despite different names*

### Comparing `revizor_fuzzer-1.2.2/revizor/x86/x86_executor.py` & `revizor_fuzzer-1.2.3/revizor/x86/x86_executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import csv
 import numpy as np
 from collections import Counter
 from typing import List
 
 from ..interfaces import CombinedHTrace, Input, TestCase, Executor
 from ..config import CONF
-from ..util import LOGGER
+from ..util import Logger
 
 
 def write_to_sysfs_file(value, path: str) -> None:
     subprocess.run(f"sudo bash -c 'echo -n {value} > {path}'", shell=True, check=True)
 
 
 def write_to_sysfs_file_bytes(value: bytes, path: str) -> None:
@@ -24,37 +24,39 @@
 
 class X86IntelExecutor(Executor):
     previous_num_inputs: int = 0
     feedback: List[int]
 
     def __init__(self):
         super().__init__()
+        self.LOG = Logger()
+
         # check the execution environment: is SMT disabled?
         smt_on = None
         try:
             out = subprocess.run("lscpu", shell=True, check=True, capture_output=True)
         except subprocess.CalledProcessError:
-            LOGGER.error("Could not check if hyperthreading is enabled.\n"
-                         "       Is lscpu installed?")
+            self.LOG.error("Could not check if hyperthreading is enabled.\n"
+                           "       Is lscpu installed?")
         for line in out.stdout.decode().split("\n"):
             if line.startswith("Thread(s) per core:"):
                 if line[-1] == "1":
                     smt_on = False
                 else:
                     smt_on = True
         if smt_on is None:
-            LOGGER.warning("executor", "Could not check if SMT is on.")
+            self.LOG.warning("executor", "Could not check if SMT is on.")
         if smt_on:
-            LOGGER.warning("executor", "SMT is on! You may experience false positives.")
+            self.LOG.warning("executor", "SMT is on! You may experience false positives.")
 
         # is kernel module ready?
         if not os.path.isfile("/sys/x86_executor/trace"):
-            LOGGER.error("x86 executor: kernel module not installed\n\n"
-                         "Go to https://microsoft.github.io/sca-fuzzer/quick-start/ for "
-                         "installation instructions.")
+            self.LOG.error("x86 executor: kernel module not installed\n\n"
+                           "Go to https://microsoft.github.io/sca-fuzzer/quick-start/ for "
+                           "installation instructions.")
 
         # initialize the kernel module
         write_to_sysfs_file(CONF.executor_warmups, '/sys/x86_executor/warmups')
         write_to_sysfs_file("1" if CONF.x86_executor_enable_ssbp_patch else "0",
                             "/sys/x86_executor/enable_ssbp_patch")
         write_to_sysfs_file("1" if CONF.x86_executor_enable_prefetcher else "0",
                             "/sys/x86_executor/enable_prefetcher")
@@ -88,15 +90,15 @@
         # 1) Announce the number of inputs
         write_to_sysfs_file(str(len(inputs)), "/sys/x86_executor/n_inputs")
         # 2) Load the inputs
         write_to_sysfs_file_bytes(byte_inputs_merged, "/sys/x86_executor/inputs")
         # 3) Check that the load was successful
         with open('/sys/x86_executor/inputs', 'r') as f:
             if f.readline() != '1\n':
-                LOGGER.error("Failure loading inputs!")
+                self.LOG.error("Failure loading inputs!", print_tb=True)
 
         # run experiments and load the results
         all_results: np.ndarray = np.ndarray(
             shape=(len(inputs), repetitions, TRACE_NUM_ELEMENTS), dtype=np.uint64)
         for rep in range(repetitions):
             # executor prints results in reverse, so we begin from the end
             input_id = len(inputs) - 1
```

### Comparing `revizor_fuzzer-1.2.2/revizor/x86/x86_fuzzer.py` & `revizor_fuzzer-1.2.3/revizor/x86/x86_fuzzer.py`

 * *Files identical despite different names*

### Comparing `revizor_fuzzer-1.2.2/revizor/x86/x86_generator.py` & `revizor_fuzzer-1.2.3/revizor/x86/x86_generator.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 Copyright (C) Microsoft Corporation
 SPDX-License-Identifier: MIT
 """
 import abc
 import math
 import re
 import random
+import copy
 from typing import List, Dict, Set, Optional, Tuple
 from subprocess import run
 
 from ..isa_loader import InstructionSet
 from ..interfaces import TestCase, Operand, RegisterOperand, FlagsOperand, MemoryOperand, \
     ImmediateOperand, AgenOperand, LabelOperand, OT, Instruction, BasicBlock, InstructionSpec, \
     PageTableModifier
@@ -714,32 +715,45 @@
                     patches = self.find_flags_patch(list(flags_to_set), flags_to_set)
                     for patch in patches:
                         bb.insert_before(bb.get_first(), patch)
                         patch.is_instrumentation = True
 
     def find_flags_patch(self, undef_flags, flags_to_set) -> List[Instruction]:
         """
-        Find an instruction that would overwrite the undefined flags
+        Find an instruction sequence that would overwrite a list of flags
+
+        :param undef_flags: list of undefined flags that have to be overwritten
+            by the patch instructions
+        :param flags_to_set: list of flags that will be read by one of the following instructions,
+            and thus should not be set to the undef state by the patch. This should be always
+            a superset of or the same as undef_flags.
+        :return: list of instructions that overwrite the undefined flags
         """
+        org_undef = copy.deepcopy(undef_flags)
         patches: List[Instruction] = []
         for instruction_spec in self.patch_candidates:
             patch = self.generator.generate_instruction(instruction_spec)
             patch_flags = patch.get_flags_operand()
             assert patch_flags
-            new_undef_flags = [i for i in patch_flags.get_undef_flags() if i in flags_to_set]
+            new_undef_flags = [
+                i for i in patch_flags.get_undef_flags()
+                if i not in undef_flags and i in flags_to_set
+            ]
             not_patched_flags = [i for i in undef_flags if i not in patch_flags.get_write_flags()]
 
             if not new_undef_flags and not_patched_flags != undef_flags:
                 patches.append(patch)
                 undef_flags = not_patched_flags
                 if not undef_flags:
                     break
 
         if undef_flags:
-            raise GeneratorException(f"Could not find an instruction to patch flags {undef_flags}")
+            raise GeneratorException("Could not find an instruction to patch flags.\n"
+                                     f"  Initial flags to be patched: {org_undef}\n"
+                                     f"  Flags for which a patch was not found: {undef_flags}")
 
         return patches
 
 
 class X86PatchUndefinedResultPass(Pass):
 
     def run_on_test_case(self, test_case: TestCase) -> None:
```

### Comparing `revizor_fuzzer-1.2.2/revizor/x86/x86_model.py` & `revizor_fuzzer-1.2.3/revizor/x86/x86_model.py`

 * *Files identical despite different names*

### Comparing `revizor_fuzzer-1.2.2/revizor/x86/x86_target_desc.py` & `revizor_fuzzer-1.2.3/revizor/x86/x86_target_desc.py`

 * *Files identical despite different names*

### Comparing `revizor_fuzzer-1.2.2/LICENSE` & `revizor_fuzzer-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `revizor_fuzzer-1.2.2/README.md` & `revizor_fuzzer-1.2.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -38,14 +38,23 @@
 
 Alternatively, install Revizor from sources:
 ```bash
 # run from the project root directory
 make install
 ```
 
+If the installation fails with `'revizor-fuzzer' requires a different Python:`, you'll have to install Python 3.9 and run Revizor from a virtual environment:
+```bash
+sudo apt install python3.9 python3.9-venv
+/usr/bin/python3.9 -m pip install virtualenv
+/usr/bin/python3.9 -m virtualenv ~/venv-revizor
+source ~/venv-revizor/bin/activate
+pip install revizor-fuzzer
+```
+
 ### 3. Install Revizor Executor (kernel module)
 
 Then build and install the kernel module:
 
 ```bash
 # building a kernel module require kernel headers
 sudo apt-get install linux-headers-$(uname -r)
```

### Comparing `revizor_fuzzer-1.2.2/pyproject.toml` & `revizor_fuzzer-1.2.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "revizor-fuzzer"
-version = "1.2.2"
+version = "1.2.3"
 description = "A fuzzer to search for microarchitectural leaks in CPUs"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "License :: OSI Approved :: MIT License",
```

### Comparing `revizor_fuzzer-1.2.2/PKG-INFO` & `revizor_fuzzer-1.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revizor-fuzzer
-Version: 1.2.2
+Version: 1.2.3
 Summary: A fuzzer to search for microarchitectural leaks in CPUs
 Project-URL: Homepage, https://microsoft.github.io/sca-fuzzer/
 Project-URL: Source code, https://github.com/microsoft/sca-fuzzer
 Project-URL: Bug Tracker, https://github.com/microsoft/sca-fuzzer/issues
 Project-URL: Changelog, https://github.com/microsoft/sca-fuzzer/releases
 Maintainer: Oleksii Oleksenko
 License-File: AUTHORS
@@ -61,14 +61,23 @@
 
 Alternatively, install Revizor from sources:
 ```bash
 # run from the project root directory
 make install
 ```
 
+If the installation fails with `'revizor-fuzzer' requires a different Python:`, you'll have to install Python 3.9 and run Revizor from a virtual environment:
+```bash
+sudo apt install python3.9 python3.9-venv
+/usr/bin/python3.9 -m pip install virtualenv
+/usr/bin/python3.9 -m virtualenv ~/venv-revizor
+source ~/venv-revizor/bin/activate
+pip install revizor-fuzzer
+```
+
 ### 3. Install Revizor Executor (kernel module)
 
 Then build and install the kernel module:
 
 ```bash
 # building a kernel module require kernel headers
 sudo apt-get install linux-headers-$(uname -r)
```

