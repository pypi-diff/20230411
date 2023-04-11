# Comparing `tmp/pytest-embedded-idf-1.2.4.tar.gz` & `tmp/pytest-embedded-idf-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pytest-embedded-idf-1.2.4.tar", last modified: Fri Mar 10 07:12:29 2023, max compression
+gzip compressed data, was "dist/pytest-embedded-idf-1.2.5.tar", last modified: Tue Apr 11 05:40:51 2023, max compression
```

## Comparing `pytest-embedded-idf-1.2.4.tar` & `pytest-embedded-idf-1.2.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 07:12:29.000000 pytest-embedded-idf-1.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-03-10 07:12:29.000000 pytest-embedded-idf-1.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-03-10 07:12:19.000000 pytest-embedded-idf-1.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 07:12:29.000000 pytest-embedded-idf-1.2.4/pytest_embedded_idf/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-03-10 07:12:19.000000 pytest-embedded-idf-1.2.4/pytest_embedded_idf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-03-10 07:12:19.000000 pytest-embedded-idf-1.2.4/pytest_embedded_idf/app.py
--rw-r--r--   0 runner    (1001) docker     (123)    21936 2023-03-10 07:12:19.000000 pytest-embedded-idf-1.2.4/pytest_embedded_idf/dut.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-03-10 07:12:19.000000 pytest-embedded-idf-1.2.4/pytest_embedded_idf/linux.py
--rw-r--r--   0 runner    (1001) docker     (123)     9588 2023-03-10 07:12:19.000000 pytest-embedded-idf-1.2.4/pytest_embedded_idf/serial.py
--rw-r--r--   0 runner    (1001) docker     (123)    11939 2023-03-10 07:12:19.000000 pytest-embedded-idf-1.2.4/pytest_embedded_idf/unity_tester.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 07:12:29.000000 pytest-embedded-idf-1.2.4/pytest_embedded_idf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-03-10 07:12:29.000000 pytest-embedded-idf-1.2.4/pytest_embedded_idf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-03-10 07:12:29.000000 pytest-embedded-idf-1.2.4/pytest_embedded_idf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-10 07:12:29.000000 pytest-embedded-idf-1.2.4/pytest_embedded_idf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-03-10 07:12:29.000000 pytest-embedded-idf-1.2.4/pytest_embedded_idf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-10 07:12:29.000000 pytest-embedded-idf-1.2.4/pytest_embedded_idf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-10 07:12:29.000000 pytest-embedded-idf-1.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-03-10 07:12:19.000000 pytest-embedded-idf-1.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 05:40:51.000000 pytest-embedded-idf-1.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-11 05:40:51.000000 pytest-embedded-idf-1.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-11 05:40:39.000000 pytest-embedded-idf-1.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 05:40:51.000000 pytest-embedded-idf-1.2.5/pytest_embedded_idf/
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-11 05:40:39.000000 pytest-embedded-idf-1.2.5/pytest_embedded_idf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8278 2023-04-11 05:40:39.000000 pytest-embedded-idf-1.2.5/pytest_embedded_idf/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22131 2023-04-11 05:40:39.000000 pytest-embedded-idf-1.2.5/pytest_embedded_idf/dut.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-11 05:40:39.000000 pytest-embedded-idf-1.2.5/pytest_embedded_idf/linux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9584 2023-04-11 05:40:39.000000 pytest-embedded-idf-1.2.5/pytest_embedded_idf/serial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11939 2023-04-11 05:40:39.000000 pytest-embedded-idf-1.2.5/pytest_embedded_idf/unity_tester.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 05:40:51.000000 pytest-embedded-idf-1.2.5/pytest_embedded_idf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-11 05:40:51.000000 pytest-embedded-idf-1.2.5/pytest_embedded_idf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-11 05:40:51.000000 pytest-embedded-idf-1.2.5/pytest_embedded_idf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 05:40:51.000000 pytest-embedded-idf-1.2.5/pytest_embedded_idf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-11 05:40:51.000000 pytest-embedded-idf-1.2.5/pytest_embedded_idf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-11 05:40:51.000000 pytest-embedded-idf-1.2.5/pytest_embedded_idf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 05:40:51.000000 pytest-embedded-idf-1.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-11 05:40:39.000000 pytest-embedded-idf-1.2.5/setup.py
```

### Comparing `pytest-embedded-idf-1.2.4/PKG-INFO` & `pytest-embedded-idf-1.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-embedded-idf
-Version: 1.2.4
+Version: 1.2.5
 Summary: pytest embedded plugin for esp-idf project
 Home-page: https://docs.espressif.com/projects/pytest-embedded/en/latest/
 Author: Fu Hanxi
 Author-email: fuhanxi@espressif.com
 License: MIT
 Description: ### pytest-embedded-idf
```

### Comparing `pytest-embedded-idf-1.2.4/pytest_embedded_idf/app.py` & `pytest-embedded-idf-1.2.5/pytest_embedded_idf/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -207,15 +207,15 @@
                         return entry['encrypted'] == 'true'
                 except (TypeError, KeyError):
                     continue
 
             return False
 
         flash_files = []
-        for (offset, file_path) in flash_args['flash_files'].items():
+        for offset, file_path in flash_args['flash_files'].items():
             flash_files.append(
                 FlashFile(
                     int(offset, 0),
                     os.path.join(self.binary_path, file_path),
                     _is_encrypted(flash_args, offset, file_path),
                 )
             )
```

### Comparing `pytest-embedded-idf-1.2.4/pytest_embedded_idf/dut.py` & `pytest-embedded-idf-1.2.5/pytest_embedded_idf/dut.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,24 +87,29 @@
             raise ValueError(
                 'Panic output decode script not found. Please use --panic-output-decode-script flag '
                 'to provide script or set IDF_PATH (Default: $IDF_PATH/tools/gdb_panic_server.py)'
             )
         return os.path.realpath(script_filepath)
 
     def _check_panic_decode_trigger(self):  # type: () -> None
+        if not self.app.elf_file:
+            logging.warning('No elf file found. Skipping decode panic output...')
+            return
+
         with open(self.logfile, 'rb') as output_file:
             output = output_file.read()
         # get the panic output by looking for the indexes
         # of the first occurrences of PANIC_START and PANIC_END patterns
         panic_output_idx_start = output.find(self.PANIC_START) - 10
         panic_output_idx_end = output.find(self.PANIC_END, output.find(self.PANIC_START) + 1) + 15
         panic_output_res = output[panic_output_idx_start:panic_output_idx_end]
         panic_output = panic_output_res if panic_output_res else None
         if panic_output is None:
             return
+
         with tempfile.NamedTemporaryFile(mode='wb', delete=False) as panic_output_file:
             panic_output_file.write(panic_output)
             panic_output_file.flush()
         try:
             cmd = [
                 f'{self.toolchain_prefix}-gdb',
                 '--command',
@@ -215,15 +220,15 @@
                 with redirect_stdout(fw):
                     coredump.info_corefile()
 
     def close(self) -> None:
         if not self.skip_check_coredump:
             try:
                 self._check_coredump()
-            except ValueError as e:
+            except Exception as e:
                 logging.debug(e)
         super().close()
 
     #####################
     # IDF-unity related #
     #####################
     def _parse_test_menu(
@@ -422,14 +427,17 @@
         else:
             warnings.warn('This function is for recording single unity test case only. Use the last matched one')
             attrs = {k: v for k, v in res[-1].groupdict().items() if v is not None}
 
         if additional_attrs:
             attrs.update(additional_attrs)
 
+        if log:
+            attrs.update({'stdout': log})
+
         testcase = TestCase(**attrs)
         self.testsuite.testcases.append(testcase)
         if testcase.result == 'FAIL':
             self.testsuite.attrs['failures'] += 1
         elif testcase.result == 'IGNORE':
             self.testsuite.attrs['skipped'] += 1
         else:
```

### Comparing `pytest-embedded-idf-1.2.4/pytest_embedded_idf/linux.py` & `pytest-embedded-idf-1.2.5/pytest_embedded_idf/linux.py`

 * *Files identical despite different names*

### Comparing `pytest-embedded-idf-1.2.4/pytest_embedded_idf/serial.py` & `pytest-embedded-idf-1.2.5/pytest_embedded_idf/serial.py`

 * *Files 0% similar despite different names*

```diff
@@ -167,17 +167,17 @@
         finally:
             if nvs_file:
                 nvs_file.close()
                 try:
                     os.remove(nvs_file.name)
                 except OSError:
                     pass
-            for (_, f) in flash_files:
+            for _, f in flash_files:
                 f.close()
-            for (_, f) in encrypt_files:
+            for _, f in encrypt_files:
                 f.close()
 
     @EspSerial.use_esptool()
     def dump_flash(
         self,
         partition: Optional[str] = None,
         address: Optional[str] = None,
```

### Comparing `pytest-embedded-idf-1.2.4/pytest_embedded_idf/unity_tester.py` & `pytest-embedded-idf-1.2.5/pytest_embedded_idf/unity_tester.py`

 * *Files identical despite different names*

### Comparing `pytest-embedded-idf-1.2.4/pytest_embedded_idf.egg-info/PKG-INFO` & `pytest-embedded-idf-1.2.5/pytest_embedded_idf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-embedded-idf
-Version: 1.2.4
+Version: 1.2.5
 Summary: pytest embedded plugin for esp-idf project
 Home-page: https://docs.espressif.com/projects/pytest-embedded/en/latest/
 Author: Fu Hanxi
 Author-email: fuhanxi@espressif.com
 License: MIT
 Description: ### pytest-embedded-idf
```

### Comparing `pytest-embedded-idf-1.2.4/setup.py` & `pytest-embedded-idf-1.2.5/setup.py`

 * *Files identical despite different names*

