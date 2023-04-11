# Comparing `tmp/iga-0.0.4.tar.gz` & `tmp/iga-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iga-0.0.4.tar", last modified: Sat Apr  8 03:28:16 2023, max compression
+gzip compressed data, was "iga-0.0.5.tar", last modified: Tue Apr 11 00:15:28 2023, max compression
```

## Comparing `iga-0.0.4.tar` & `iga-0.0.5.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-04-08 03:28:16.709047 iga-0.0.4/
--rw-r--r--   0 mhucka     (503) staff       (20)     1527 2023-03-16 00:12:10.000000 iga-0.0.4/LICENSE
--rw-r--r--   0 mhucka     (503) staff       (20)    25734 2023-04-08 03:28:16.709125 iga-0.0.4/PKG-INFO
--rw-r--r--   0 mhucka     (503) staff       (20)    24828 2023-04-06 20:04:04.000000 iga-0.0.4/README.md
-drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-04-08 03:28:16.706339 iga-0.0.4/iga/
--rw-r--r--   0 mhucka     (503) staff       (20)     1458 2023-04-08 03:19:45.000000 iga-0.0.4/iga/__init__.py
--rw-r--r--   0 mhucka     (503) staff       (20)      905 2023-03-16 00:12:36.000000 iga-0.0.4/iga/__main__.py
--rw-r--r--   0 mhucka     (503) staff       (20)    31136 2023-04-08 02:46:54.000000 iga-0.0.4/iga/cli.py
--rw-r--r--   0 mhucka     (503) staff       (20)     3317 2023-03-27 20:05:34.000000 iga-0.0.4/iga/data_utils.py
--rw-r--r--   0 mhucka     (503) staff       (20)     2867 2023-04-08 02:43:47.000000 iga-0.0.4/iga/doi.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1069 2023-04-07 18:13:39.000000 iga-0.0.4/iga/exceptions.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1447 2023-03-28 00:40:16.000000 iga-0.0.4/iga/exit_codes.py
--rw-r--r--   0 mhucka     (503) staff       (20)    12807 2023-04-08 02:43:51.000000 iga-0.0.4/iga/github.py
--rw-r--r--   0 mhucka     (503) staff       (20)     3192 2023-03-28 22:54:00.000000 iga-0.0.4/iga/id_utils.py
--rw-r--r--   0 mhucka     (503) staff       (20)    14944 2023-04-08 02:43:56.000000 iga-0.0.4/iga/invenio.py
--rw-r--r--   0 mhucka     (503) staff       (20)     2054 2023-04-08 02:43:59.000000 iga-0.0.4/iga/json_utils.py
--rw-r--r--   0 mhucka     (503) staff       (20)   242887 2023-03-08 23:12:16.000000 iga-0.0.4/iga/licenses.py
--rw-r--r--   0 mhucka     (503) staff       (20)    67896 2023-04-08 02:44:10.000000 iga-0.0.4/iga/metadata.py
--rw-r--r--   0 mhucka     (503) staff       (20)    13434 2023-04-08 03:10:23.000000 iga-0.0.4/iga/name_utils.py
--rw-r--r--   0 mhucka     (503) staff       (20)     5273 2023-04-08 02:44:39.000000 iga-0.0.4/iga/orcid.py
--rw-r--r--   0 mhucka     (503) staff       (20)     5147 2023-04-08 02:44:39.000000 iga-0.0.4/iga/reference.py
--rw-r--r--   0 mhucka     (503) staff       (20)     3969 2023-04-08 02:44:39.000000 iga-0.0.4/iga/ror.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1624 2023-04-08 02:44:39.000000 iga-0.0.4/iga/text_utils.py
-drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-04-08 03:28:16.707095 iga-0.0.4/iga.egg-info/
--rw-r--r--   0 mhucka     (503) staff       (20)    25734 2023-04-08 03:28:16.000000 iga-0.0.4/iga.egg-info/PKG-INFO
--rw-r--r--   0 mhucka     (503) staff       (20)      904 2023-04-08 03:28:16.000000 iga-0.0.4/iga.egg-info/SOURCES.txt
--rw-r--r--   0 mhucka     (503) staff       (20)        1 2023-04-08 03:28:16.000000 iga-0.0.4/iga.egg-info/dependency_links.txt
--rw-r--r--   0 mhucka     (503) staff       (20)       58 2023-04-08 03:28:16.000000 iga-0.0.4/iga.egg-info/entry_points.txt
--rw-r--r--   0 mhucka     (503) staff       (20)        1 2023-04-08 03:28:03.000000 iga-0.0.4/iga.egg-info/not-zip-safe
--rw-r--r--   0 mhucka     (503) staff       (20)      657 2023-04-08 03:28:16.000000 iga-0.0.4/iga.egg-info/requires.txt
--rw-r--r--   0 mhucka     (503) staff       (20)        4 2023-04-08 03:28:16.000000 iga-0.0.4/iga.egg-info/top_level.txt
--rw-r--r--   0 mhucka     (503) staff       (20)     1095 2023-04-08 03:28:16.709479 iga-0.0.4/setup.cfg
--rwxr-xr-x   0 mhucka     (503) staff       (20)     1708 2023-04-08 01:05:22.000000 iga-0.0.4/setup.py
-drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-04-08 03:28:16.708948 iga-0.0.4/tests/
--rw-r--r--   0 mhucka     (503) staff       (20)     5701 2023-04-08 01:24:41.000000 iga-0.0.4/tests/test_cli.py
--rw-r--r--   0 mhucka     (503) staff       (20)     4481 2023-03-27 19:38:15.000000 iga-0.0.4/tests/test_data_utils.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1417 2023-03-17 23:21:28.000000 iga-0.0.4/tests/test_doi.py
--rw-r--r--   0 mhucka     (503) staff       (20)      686 2023-03-02 15:36:12.000000 iga-0.0.4/tests/test_exceptions.py
--rw-r--r--   0 mhucka     (503) staff       (20)      177 2023-01-13 03:19:50.000000 iga-0.0.4/tests/test_exit_codes.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1446 2023-04-07 01:26:59.000000 iga-0.0.4/tests/test_github.py
--rw-r--r--   0 mhucka     (503) staff       (20)     3015 2023-04-07 01:20:36.000000 iga-0.0.4/tests/test_github_mocks.py
--rw-r--r--   0 mhucka     (503) staff       (20)     2149 2023-03-02 15:19:42.000000 iga-0.0.4/tests/test_id_utils.py
--rw-r--r--   0 mhucka     (503) staff       (20)      641 2022-12-08 00:11:08.000000 iga-0.0.4/tests/test_init.py
--rw-r--r--   0 mhucka     (503) staff       (20)      912 2023-03-02 15:16:32.000000 iga-0.0.4/tests/test_licenses.py
--rw-r--r--   0 mhucka     (503) staff       (20)    51703 2023-04-07 00:07:41.000000 iga-0.0.4/tests/test_name_parsing.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1821 2023-03-02 23:15:31.000000 iga-0.0.4/tests/test_name_utils.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1054 2023-03-18 00:09:09.000000 iga-0.0.4/tests/test_orcid.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1935 2023-04-08 01:31:14.000000 iga-0.0.4/tests/test_record_from_codemeta.py
--rw-r--r--   0 mhucka     (503) staff       (20)     6026 2023-03-02 23:04:18.000000 iga-0.0.4/tests/test_reference.py
--rw-r--r--   0 mhucka     (503) staff       (20)      947 2023-03-18 00:05:51.000000 iga-0.0.4/tests/test_ror.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1375 2023-04-06 22:54:59.000000 iga-0.0.4/tests/test_text_utils.py
+drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-04-11 00:15:28.032966 iga-0.0.5/
+-rw-r--r--   0 mhucka     (503) staff       (20)     1527 2023-03-16 00:12:10.000000 iga-0.0.5/LICENSE
+-rw-r--r--   0 mhucka     (503) staff       (20)    25734 2023-04-11 00:15:28.033045 iga-0.0.5/PKG-INFO
+-rw-r--r--   0 mhucka     (503) staff       (20)    24828 2023-04-06 20:04:04.000000 iga-0.0.5/README.md
+drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-04-11 00:15:28.030262 iga-0.0.5/iga/
+-rw-r--r--   0 mhucka     (503) staff       (20)     1458 2023-04-11 00:11:34.000000 iga-0.0.5/iga/__init__.py
+-rw-r--r--   0 mhucka     (503) staff       (20)      905 2023-03-16 00:12:36.000000 iga-0.0.5/iga/__main__.py
+-rw-r--r--   0 mhucka     (503) staff       (20)    31130 2023-04-10 21:10:55.000000 iga-0.0.5/iga/cli.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     3317 2023-03-27 20:05:34.000000 iga-0.0.5/iga/data_utils.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     2859 2023-04-10 21:11:51.000000 iga-0.0.5/iga/doi.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1069 2023-04-07 18:13:39.000000 iga-0.0.5/iga/exceptions.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1447 2023-03-28 00:40:16.000000 iga-0.0.5/iga/exit_codes.py
+-rw-r--r--   0 mhucka     (503) staff       (20)    12795 2023-04-10 21:12:02.000000 iga-0.0.5/iga/github.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     3192 2023-03-28 22:54:00.000000 iga-0.0.5/iga/id_utils.py
+-rw-r--r--   0 mhucka     (503) staff       (20)    14934 2023-04-10 21:13:20.000000 iga-0.0.5/iga/invenio.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     2054 2023-04-08 02:43:59.000000 iga-0.0.5/iga/json_utils.py
+-rw-r--r--   0 mhucka     (503) staff       (20)   242887 2023-03-08 23:12:16.000000 iga-0.0.5/iga/licenses.py
+-rw-r--r--   0 mhucka     (503) staff       (20)    68275 2023-04-10 23:14:29.000000 iga-0.0.5/iga/metadata.py
+-rw-r--r--   0 mhucka     (503) staff       (20)    13434 2023-04-08 03:10:23.000000 iga-0.0.5/iga/name_utils.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     5273 2023-04-08 02:44:39.000000 iga-0.0.5/iga/orcid.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     5147 2023-04-08 02:44:39.000000 iga-0.0.5/iga/reference.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     3969 2023-04-08 02:44:39.000000 iga-0.0.5/iga/ror.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1624 2023-04-08 02:44:39.000000 iga-0.0.5/iga/text_utils.py
+drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-04-11 00:15:28.031036 iga-0.0.5/iga.egg-info/
+-rw-r--r--   0 mhucka     (503) staff       (20)    25734 2023-04-11 00:15:27.000000 iga-0.0.5/iga.egg-info/PKG-INFO
+-rw-r--r--   0 mhucka     (503) staff       (20)      904 2023-04-11 00:15:28.000000 iga-0.0.5/iga.egg-info/SOURCES.txt
+-rw-r--r--   0 mhucka     (503) staff       (20)        1 2023-04-11 00:15:27.000000 iga-0.0.5/iga.egg-info/dependency_links.txt
+-rw-r--r--   0 mhucka     (503) staff       (20)       58 2023-04-11 00:15:27.000000 iga-0.0.5/iga.egg-info/entry_points.txt
+-rw-r--r--   0 mhucka     (503) staff       (20)        1 2023-04-11 00:15:27.000000 iga-0.0.5/iga.egg-info/not-zip-safe
+-rw-r--r--   0 mhucka     (503) staff       (20)      657 2023-04-11 00:15:27.000000 iga-0.0.5/iga.egg-info/requires.txt
+-rw-r--r--   0 mhucka     (503) staff       (20)        4 2023-04-11 00:15:28.000000 iga-0.0.5/iga.egg-info/top_level.txt
+-rw-r--r--   0 mhucka     (503) staff       (20)     1095 2023-04-11 00:15:28.033381 iga-0.0.5/setup.cfg
+-rwxr-xr-x   0 mhucka     (503) staff       (20)     1708 2023-04-08 01:05:22.000000 iga-0.0.5/setup.py
+drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-04-11 00:15:28.032872 iga-0.0.5/tests/
+-rw-r--r--   0 mhucka     (503) staff       (20)     5701 2023-04-08 01:24:41.000000 iga-0.0.5/tests/test_cli.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     4481 2023-03-27 19:38:15.000000 iga-0.0.5/tests/test_data_utils.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1417 2023-03-17 23:21:28.000000 iga-0.0.5/tests/test_doi.py
+-rw-r--r--   0 mhucka     (503) staff       (20)      686 2023-03-02 15:36:12.000000 iga-0.0.5/tests/test_exceptions.py
+-rw-r--r--   0 mhucka     (503) staff       (20)      177 2023-01-13 03:19:50.000000 iga-0.0.5/tests/test_exit_codes.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1446 2023-04-07 01:26:59.000000 iga-0.0.5/tests/test_github.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     3015 2023-04-07 01:20:36.000000 iga-0.0.5/tests/test_github_mocks.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     2149 2023-03-02 15:19:42.000000 iga-0.0.5/tests/test_id_utils.py
+-rw-r--r--   0 mhucka     (503) staff       (20)      641 2022-12-08 00:11:08.000000 iga-0.0.5/tests/test_init.py
+-rw-r--r--   0 mhucka     (503) staff       (20)      912 2023-03-02 15:16:32.000000 iga-0.0.5/tests/test_licenses.py
+-rw-r--r--   0 mhucka     (503) staff       (20)    51703 2023-04-07 00:07:41.000000 iga-0.0.5/tests/test_name_parsing.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1821 2023-03-02 23:15:31.000000 iga-0.0.5/tests/test_name_utils.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1054 2023-03-18 00:09:09.000000 iga-0.0.5/tests/test_orcid.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1935 2023-04-08 01:31:14.000000 iga-0.0.5/tests/test_record_from_codemeta.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     6026 2023-03-02 23:04:18.000000 iga-0.0.5/tests/test_reference.py
+-rw-r--r--   0 mhucka     (503) staff       (20)      947 2023-03-18 00:05:51.000000 iga-0.0.5/tests/test_ror.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1375 2023-04-06 22:54:59.000000 iga-0.0.5/tests/test_text_utils.py
```

### Comparing `iga-0.0.4/LICENSE` & `iga-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `iga-0.0.4/PKG-INFO` & `iga-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iga
-Version: 0.0.4
+Version: 0.0.5
 Summary: InvenioRDM GitHub Archiver
 Home-page: https://github.com/caltechlibrary/iga
 Author: Michael Hucka
 Author-email: helpdesk@library.caltech.edu
 License: https://github.com/caltechlibrary/iga/blob/main/LICENSE
 Project-URL: Source Code, https://github.com/caltechlibrary/iga
 Project-URL: Bug Tracker, https://github.com/caltechlibrary/iga/issues
```

### Comparing `iga-0.0.4/README.md` & `iga-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `iga-0.0.4/iga/__init__.py` & `iga-0.0.5/iga/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # .............................................................................
 #
 #  ╭────────────────────── Notice ── Notice ── Notice ─────────────────────╮
 #  |    The following values are automatically updated at every release    |
 #  |    by the Makefile. Manual changes to these values will be lost.      |
 #  ╰────────────────────── Notice ── Notice ── Notice ─────────────────────╯
 
-__version__     = '0.0.4'
+__version__     = '0.0.5'
 __description__ = 'InvenioRDM GitHub Archiver'
 __url__         = 'https://github.com/caltechlibrary/iga'
 __author__      = 'Michael Hucka'
 __email__       = 'helpdesk@library.caltech.edu'
 __license__     = 'https://github.com/caltechlibrary/iga/blob/main/LICENSE'
```

### Comparing `iga-0.0.4/iga/__main__.py` & `iga-0.0.5/iga/__main__.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.4/iga/cli.py` & `iga-0.0.5/iga/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,15 +101,15 @@
     If CLI argument value is None, the environment variable env_var is checked
     and if it has a value, it's returned; otherwise, this function prints an
     error message and exits with a status code signifying "bad argument".
 
     If the value is "help", this function prints help text and causes the
     program to exit.
     '''
-    if ctx.params.get('url_or_tag', None) == 'help':
+    if ctx.params.get('url_or_tag') == 'help':
         _print_help_and_exit(ctx)
     elif value:
         log(f'using CLI option "--{param.name} {value}" for the {thing}')
         os.environ[env_var] = str(value).strip()
     elif env_var in os.environ:
         log(f"using value of environment variable {env_var} as the {thing}")
     elif required:
```

### Comparing `iga-0.0.4/iga/data_utils.py` & `iga-0.0.5/iga/data_utils.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.4/iga/doi.py` & `iga-0.0.5/iga/doi.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,17 +53,17 @@
     log(f'looking up DOI for {scheme} {pub_id} using NCBI idconv')
     url = f'https://www.ncbi.nlm.nih.gov/pmc/utils/idconv/v1.0/?format=json&ids={pub_id}'
     try:
         data = network('get', url).json()
         if os.environ.get('IGA_RUN_MODE') == 'debug':
             log(f'data received for {scheme} "{pub_id}" from NCBI:\n{str(data)}')
         with suppress(KeyError, IndexError):
-            if doi := data['records'][0].get('doi', ''):
+            if doi := data['records'][0].get('doi'):
                 return doi
-            elif errmsg := data['records'][0].get('errmsg', ''):
+            elif errmsg := data['records'][0].get('errmsg'):
                 log(f'NCBI returned an error for {pub_id}: ' + errmsg)
             else:
                 log(f'did not get a DOI or error message for {pub_id} from NCBI')
     except KeyboardInterrupt:
         raise
     except commonpy.exceptions.NoContent:
         log(f'NBCI returned no result for "{pub_id}"')
```

### Comparing `iga-0.0.4/iga/exceptions.py` & `iga-0.0.5/iga/exceptions.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.4/iga/exit_codes.py` & `iga-0.0.5/iga/exit_codes.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.4/iga/github.py` & `iga-0.0.5/iga/github.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,17 +55,17 @@
     the files in the default branch of the repository.'''
 
     def __init__(self, repo_dict):
         super().__init__(**repo_dict)
         if os.environ.get('IGA_RUN_MODE') == 'debug':
             log('GitHub repo data: ' + json.dumps(repo_dict, indent=2))
         self.owner = GitHubAccount(repo_dict['owner'])
-        if repo_dict.get('organization', None):
+        if repo_dict.get('organization'):
             self.organization = GitHubAccount(repo_dict['organization'])
-        if repo_dict.get('license', None):
+        if repo_dict.get('license'):
             self.license = GitHubLicense(repo_dict['license'])
         # Save the original data for debugging purposes.
         self._json_dict = repo_dict
 
 
 class GitHubAccount(SimpleNamespace):
     '''Simple data structure corresponding to a GitHub user or org account.'''
```

### Comparing `iga-0.0.4/iga/id_utils.py` & `iga-0.0.5/iga/id_utils.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.4/iga/invenio.py` & `iga-0.0.5/iga/invenio.py`

 * *Files 1% similar despite different names*

```diff
@@ -227,15 +227,15 @@
     '''
     log(f'asking InvenioRDM server for vocabulary "{vocab}"')
     # At the time of this writing (2023-03-08), the "languages" vocabulary has
     # 7847 entries. We currently don't use the languages vocab in IGA, but in
     # case we ever do in the future, this code tries to get everything at once.
     endpoint = '/api/vocabularies/' + vocab + '?size=10000'
     result = _invenio('get', endpoint=endpoint, msg=f'get vocabulary {vocab}')
-    if hits := result.get('hits', {}):
+    if hits := result.get('hits'):
         # This is not a mistake; it really is a nested 'hits' dictionary.
         num_items = len(hits['hits'])
         log(f'received {num_items} items for vocabulary "{vocab}"')
         if num_items < hits['total']:
             log(f'warning: server actually has {hits["total"]} values available')
         return hits['hits']
     else:
@@ -328,15 +328,15 @@
 
     This uses the value in the environment variable IGA_NETWORK_TIMEOUT, if
     given. If no explicit timeout value has been given, this calculates an
     adaptive timeout value based on the size of the data, using a custom
     heuristic invented by the author based on his experiences with a
     slowish network.
     '''
-    if given_timeout := os.environ.get('IGA_NETWORK_TIMEOUT', None):
+    if given_timeout := os.environ.get('IGA_NETWORK_TIMEOUT'):
         # Assume that the main cli() has done sanity-checking on the value.
         timeout = int(given_timeout)
     else:
         # Calculate a value based on these principles:
         #  - Scale by the size of the data at roughly 1 min per 5 MB
         #  - Don't exceed 30 minutes (1800 sec)
         timeout = min(1800, 60*max(1, len(data)//2_000_000))
```

### Comparing `iga-0.0.4/iga/json_utils.py` & `iga-0.0.5/iga/json_utils.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.4/iga/licenses.py` & `iga-0.0.5/iga/licenses.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.4/iga/metadata.py` & `iga-0.0.5/iga/metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -242,15 +242,15 @@
         metadata = json5.loads(content)
     except KeyboardInterrupt:
         raise
     except Exception as ex:             # noqa PIE786
         log(f'problem trying to read metadata from {str(file)}: ' + str(ex))
         return False
 
-    if not metadata.get('metadata', {}):
+    if 'metadata' not in metadata:
         log('record lacks a "metadata" field')
         return None
 
     for field in REQUIRED_FIELDS:
         if field not in metadata.get('metadata', {}):
             log(f'metadata structure lacks required field "{field}"')
             return None
@@ -733,15 +733,15 @@
             # particular sort of identifier. Try to extract the identifier.
             value = detected_id(value) or value
         if kind in CV['identifier-types'].values():
             identifiers.append({'identifier': value,
                                 'scheme': kind})
         else:
             log(f'skipping due to unsupported identifier type: {value}')
-    return identifiers
+    return deduplicated(identifiers)
 
 
 def languages(repo, release, include_all):
     '''Return InvenioRDM "languages".
     https://inveniordm.docs.cern.ch/reference/metadata/#languages-0-n
     '''
     # GitHub doesn't provide a way to deal with any other human language.
@@ -876,15 +876,15 @@
     # in InvenioRDM, it is not "same as"; rather it's closer to "a version of".
     # There's no equivalent in CFF or the GitHub repo data structure.
     if sameas_url := repo.codemeta.get('sameAs', ''):
         log('adding CodeMeta "sameAs" to "related_identifiers"')
         identifiers.append(id_dict(sameas_url, 'isversionof', 'software'))
 
     # CodeMeta softwareHelp type is CreativeWork but sometimes people use URLs.
-    for help in listified(repo.codemeta.get('softwareHelp', '')):
+    for help in listified(repo.codemeta.get('softwareHelp', '')):  # noqa A001
         if isinstance(help, str) and validators.url(help):
             url = help
         elif isinstance(help, dict):
             if help_url := help.get('url', ''):
                 url = normalized_url(help_url)
             elif validators.url(help.get('@id', '')):
                 url = normalized_url(help.get('@id'))
@@ -916,15 +916,15 @@
     # use a list. The nature of the relationship is more problematic. The
     # CodeMeta spec says this is "A link related to this object, e.g., related
     # web pages"; however, in the codemeta.json file, we get zero info about
     # what the links are meant to be. Worse, relatedLink has no direct
     # equivalent in the relations CV in InvenioRDM. Since the direction is
     # "this release" --> relatedLink --> "something", the closest relationship
     # term seems to be "references", as in "this release references this link".
-    if links := listified(repo.codemeta.get('relatedLink', None)):
+    if links := listified(repo.codemeta.get('relatedLink')):
         log('adding CodeMeta "relatedLink" URL value(s) to "related_identifiers"')
         for url in filter(lambda x: validators.url(x), links):
             url = normalized_url(url)
             # We don't add URLs we've already added (possibly as another type).
             # The list needs to be recreated in the loop b/c we're adding to it.
             added_urls = [item['identifier'] for item in identifiers]
             # We compare URLs loosely b/c people frequently put https in one
@@ -934,15 +934,15 @@
             # There's no good way to know what the resource type actually is.
             identifiers.append(id_dict(url, 'references', 'other'))
 
     # We add CodeMeta & CFF "references" values to InvenioRDM "references" but
     # formatted as references. Here, add the id's alone.
     if reference_ids := _codemeta_reference_ids(repo) | _cff_reference_ids(repo):
         log('adding id\'s of CodeMeta & CFF references to "related_identifiers"')
-    for id in reference_ids:
+    for id in reference_ids:            # noqa A001
         # Adding id's => must recreate the list in this test each iteration.
         if id not in [detected_id(item['identifier']) for item in identifiers]:
             identifiers.append({'identifier': id,
                                 'relation_type': {'id': 'isreferencedby'},
                                 'scheme': recognized_scheme(id)})
 
     # Final step: remove things that have urls not in our allowed list.
@@ -961,15 +961,15 @@
 
 def resource_type(repo, release, include_all):
     '''Return InvenioRDM "resource type".
     https://inveniordm.docs.cern.ch/reference/metadata/#resource-type-1
     '''
     # The only clear source of info about whether this is software or data is
     # the CFF file field "type", so if we can't use that, default to software.
-    if repo.cff.get('type', '') == 'dataset':
+    if repo.cff.get('type') == 'dataset':
         log('using CFF "type" as "resource_type" (and it is "dataset")')
         return {'id': 'dataset'}
     else:
         log('using default value "software" as "resource_type"')
         return {'id': 'software'}
 
 
@@ -1261,18 +1261,18 @@
     # subset anyway because there's no place in Invenio records to put the rest.
     person = {}
     org = {}
 
     type_ = data.get('@type', '') or data.get('type', '')
     if type_.lower().strip() == 'person':
         # Deal with field name differences between CodeMeta & CFF.
-        family  = data.get('family-names', '') or data.get('familyName', '')
-        given   = data.get('given-names', '') or data.get('givenName', '')
+        family = data.get('family-names', '') or data.get('familyName', '')
+        given  = data.get('given-names', '') or data.get('givenName', '')
 
-        id = detected_id(data.get('@id', ''))
+        id = detected_id(data.get('@id', ''))            # noqa A001
         id_type = recognized_scheme(id)
 
         if not (family or given) and id_type == 'orcid':
             # If we're lucky and the added an orcid, we can try to use that.
             log('no family & given name fields but have ORCID – trying orcid.org')
             from iga.orcid import name_from_orcid
             (given, family) = name_from_orcid(id)
@@ -1296,35 +1296,47 @@
                       'given_name': '',
                       'type': 'personal'}
 
         if id_type in ['orcid', 'isni', 'gnd']:
             person.update({'identifiers': [{'identifier': id,
                                             'scheme': id_type}]})
     else:
-        org = {'name': flattened_name(data.get('name', '')),
-               'type': 'organizational'}
+        org = _org_from_dict(data)
+        org['type'] = 'organizational'
 
     result = {}
     if person or org:
         result = {'person_or_org': person or org}
-        for affiliation in listified(data.get('affiliation', '')):
-            if isinstance(affiliation, str):
-                name = affiliation
-            elif isinstance(affiliation, dict):
-                # In CFF the field name is 'legalName'. In CodeMeta it's 'name'.
-                name = affiliation.get('legalName', '') or affiliation.get('name', '')
-            if name:
-                affiliations = result.get('affiliations', [])
-                affiliations.append({'name': flattened_name(name)})
-                result['affiliations'] = affiliations
-        if role:
-            result['role'] = {'id': role}
+    if person:
+        affiliations = []
+        for item in listified(data.get('affiliation', '')):
+            if isinstance(item, str):
+                affiliations.append({'name': flattened_name(item)})
+            elif isinstance(item, dict) and (aff := _org_from_dict(item)):
+                affiliations.append(aff)
+        if affiliations:
+            result['affiliations'] = affiliations
+    if role:
+        result['role'] = {'id': role}
     return result
 
 
+def _org_from_dict(data):
+    # Hopefully it has a name field or id. If it doesn't, we can't do anything
+    # more anyway, and will end up with an empty structure.
+    org = {}
+    id = detected_id(data.get('@id', ''))  # noqa A001
+    if recognized_scheme(id) == 'ror':
+        org = {'id': detected_id(data)}
+    elif name := (data.get('legalName', '') or data.get('name', '')):
+        # In CFF the field name is 'legalName'. In CodeMeta it's 'name'.
+        org = {'name': flattened_name(name)}
+    return org
+
+
 def _entity_match(first, second):
     # Match based on names only.
     p1 = first['person_or_org']
     p2 = second['person_or_org']
 
     p1_orcid = None
     p2_orcid = None
@@ -1453,15 +1465,15 @@
                 identifiers.add(detected_id(item))
             else:
                 log('unrecognized scheme in item: ' + str(item))
         elif isinstance(item, dict):
             for field in ['id', '@id', 'identifier', '@identifier']:
                 id_field = item.get(field, '')
                 if recognized_scheme(id_field):
-                    id = detected_id(id_field)
+                    id = detected_id(id_field)  # noqa A001
                     log(f'found id {id} in CodeMeta "referencePublication"')
                     identifiers.add(id)
                     break
             else:
                 log(f'cannot use {item} from CodeMeta "referencePublication"')
         else:
             log('unrecognized referencePublication format: ' + str(item))
```

### Comparing `iga-0.0.4/iga/name_utils.py` & `iga-0.0.5/iga/name_utils.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.4/iga/orcid.py` & `iga-0.0.5/iga/orcid.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.4/iga/reference.py` & `iga-0.0.5/iga/reference.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.4/iga/ror.py` & `iga-0.0.5/iga/ror.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.4/iga/text_utils.py` & `iga-0.0.5/iga/text_utils.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.4/iga.egg-info/PKG-INFO` & `iga-0.0.5/iga.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iga
-Version: 0.0.4
+Version: 0.0.5
 Summary: InvenioRDM GitHub Archiver
 Home-page: https://github.com/caltechlibrary/iga
 Author: Michael Hucka
 Author-email: helpdesk@library.caltech.edu
 License: https://github.com/caltechlibrary/iga/blob/main/LICENSE
 Project-URL: Source Code, https://github.com/caltechlibrary/iga
 Project-URL: Bug Tracker, https://github.com/caltechlibrary/iga/issues
```

### Comparing `iga-0.0.4/iga.egg-info/SOURCES.txt` & `iga-0.0.5/iga.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iga-0.0.4/iga.egg-info/requires.txt` & `iga-0.0.5/iga.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `iga-0.0.4/setup.cfg` & `iga-0.0.5/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = iga
-version = 0.0.4
+version = 0.0.5
 description = InvenioRDM GitHub Archiver
 author = Michael Hucka
 author_email = helpdesk@library.caltech.edu
 license = https://github.com/caltechlibrary/iga/blob/main/LICENSE
 license_files = LICENSE
 url = https://github.com/caltechlibrary/iga
 project_urls =
```

### Comparing `iga-0.0.4/setup.py` & `iga-0.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.4/tests/test_cli.py` & `iga-0.0.5/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.4/tests/test_data_utils.py` & `iga-0.0.5/tests/test_data_utils.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.4/tests/test_doi.py` & `iga-0.0.5/tests/test_doi.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.4/tests/test_exceptions.py` & `iga-0.0.5/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.4/tests/test_github.py` & `iga-0.0.5/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.4/tests/test_github_mocks.py` & `iga-0.0.5/tests/test_github_mocks.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.4/tests/test_id_utils.py` & `iga-0.0.5/tests/test_id_utils.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.4/tests/test_init.py` & `iga-0.0.5/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.4/tests/test_licenses.py` & `iga-0.0.5/tests/test_licenses.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.4/tests/test_name_parsing.py` & `iga-0.0.5/tests/test_name_parsing.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.4/tests/test_name_utils.py` & `iga-0.0.5/tests/test_name_utils.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.4/tests/test_orcid.py` & `iga-0.0.5/tests/test_orcid.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.4/tests/test_record_from_codemeta.py` & `iga-0.0.5/tests/test_record_from_codemeta.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.4/tests/test_reference.py` & `iga-0.0.5/tests/test_reference.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.4/tests/test_ror.py` & `iga-0.0.5/tests/test_ror.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.4/tests/test_text_utils.py` & `iga-0.0.5/tests/test_text_utils.py`

 * *Files identical despite different names*

