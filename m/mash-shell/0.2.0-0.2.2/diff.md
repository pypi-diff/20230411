# Comparing `tmp/mash-shell-0.2.0.tar.gz` & `tmp/mash-shell-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mash-shell-0.2.0.tar", last modified: Sat Mar 18 14:39:11 2023, max compression
+gzip compressed data, was "mash-shell-0.2.2.tar", last modified: Tue Apr 11 19:58:05 2023, max compression
```

## Comparing `mash-shell-0.2.0.tar` & `mash-shell-0.2.2.tar`

### file list

```diff
@@ -1,70 +1,73 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-03-18 14:39:11.174103 mash-shell-0.2.0/
--rw-r--r--   0 mark       (501) staff       (20)    35149 2022-11-28 19:29:51.000000 mash-shell-0.2.0/LICENSE
--rw-r--r--   0 mark       (501) staff       (20)     3486 2023-03-18 14:39:11.173488 mash-shell-0.2.0/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)     2918 2023-03-18 14:38:35.000000 mash-shell-0.2.0/README.md
--rw-r--r--   0 mark       (501) staff       (20)      736 2023-03-18 14:37:39.000000 mash-shell-0.2.0/pyproject.toml
--rw-r--r--   0 mark       (501) staff       (20)      161 2023-03-18 10:23:14.000000 mash-shell-0.2.0/requirements.txt
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-03-18 14:39:11.174228 mash-shell-0.2.0/setup.cfg
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-03-18 14:39:11.136265 mash-shell-0.2.0/src/
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-03-18 14:39:11.142008 mash-shell-0.2.0/src/examples/
--rw-r--r--   0 mark       (501) staff       (20)       91 2023-03-18 13:42:50.000000 mash-shell-0.2.0/src/examples/_extend_path.py
--rwxr-xr-x   0 mark       (501) staff       (20)     2059 2023-03-18 13:42:50.000000 mash-shell-0.2.0/src/examples/discoverable.py
--rwxr-xr-x   0 mark       (501) staff       (20)      965 2023-03-18 13:42:50.000000 mash-shell-0.2.0/src/examples/discoverable_api.py
--rw-r--r--   0 mark       (501) staff       (20)     1000 2023-03-18 13:42:50.000000 mash-shell-0.2.0/src/examples/discoverable_with_oas.py
--rwxr-xr-x   0 mark       (501) staff       (20)      785 2023-03-18 13:42:50.000000 mash-shell-0.2.0/src/examples/filesystem.py
--rwxr-xr-x   0 mark       (501) staff       (20)     3477 2023-03-18 13:42:50.000000 mash-shell-0.2.0/src/examples/object_parser.py
--rwxr-xr-x   0 mark       (501) staff       (20)     1381 2023-03-18 14:32:23.000000 mash-shell-0.2.0/src/examples/shell_example.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-03-18 14:39:11.152288 mash-shell-0.2.0/src/mash/
--rw-r--r--   0 mark       (501) staff       (20)       43 2023-03-18 13:42:50.000000 mash-shell-0.2.0/src/mash/__main__.py
--rwxr-xr-x   0 mark       (501) staff       (20)     2209 2023-03-18 14:32:23.000000 mash-shell-0.2.0/src/mash/cli.py
--rw-r--r--   0 mark       (501) staff       (20)     2186 2023-03-18 13:42:50.000000 mash-shell-0.2.0/src/mash/doc_inference.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-03-18 14:39:11.155500 mash-shell-0.2.0/src/mash/filesystem/
--rw-r--r--   0 mark       (501) staff       (20)      121 2023-03-18 13:42:50.000000 mash-shell-0.2.0/src/mash/filesystem/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)     6916 2023-03-18 13:42:50.000000 mash-shell-0.2.0/src/mash/filesystem/discoverable.py
--rw-r--r--   0 mark       (501) staff       (20)    10629 2023-03-18 13:42:50.000000 mash-shell-0.2.0/src/mash/filesystem/filesystem.py
--rw-r--r--   0 mark       (501) staff       (20)     3252 2023-03-18 14:32:23.000000 mash-shell-0.2.0/src/mash/filesystem/scope.py
--rw-r--r--   0 mark       (501) staff       (20)     4432 2023-03-18 13:42:50.000000 mash-shell-0.2.0/src/mash/filesystem/view.py
--rw-r--r--   0 mark       (501) staff       (20)     3455 2023-03-18 13:42:50.000000 mash-shell-0.2.0/src/mash/html_table.py
--rw-r--r--   0 mark       (501) staff       (20)     2048 2023-03-18 13:42:50.000000 mash-shell-0.2.0/src/mash/html_table_data.py
--rw-r--r--   0 mark       (501) staff       (20)     5075 2023-03-18 13:42:50.000000 mash-shell-0.2.0/src/mash/io_util.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-03-18 14:39:11.159289 mash-shell-0.2.0/src/mash/object_parser/
--rw-r--r--   0 mark       (501) staff       (20)      733 2023-03-18 13:42:50.000000 mash-shell-0.2.0/src/mash/object_parser/errors.py
--rw-r--r--   0 mark       (501) staff       (20)     8289 2023-03-18 13:42:50.000000 mash-shell-0.2.0/src/mash/object_parser/factory.py
--rw-r--r--   0 mark       (501) staff       (20)     4505 2023-03-18 13:42:50.000000 mash-shell-0.2.0/src/mash/object_parser/oas.py
--rw-r--r--   0 mark       (501) staff       (20)     1727 2023-03-18 14:24:14.000000 mash-shell-0.2.0/src/mash/object_parser/object_parser.py
--rw-r--r--   0 mark       (501) staff       (20)     1129 2023-03-18 13:42:50.000000 mash-shell-0.2.0/src/mash/object_parser/object_parser_standards.py
--rw-r--r--   0 mark       (501) staff       (20)     4322 2023-03-18 13:42:50.000000 mash-shell-0.2.0/src/mash/object_parser/spec.py
--rwxr-xr-x   0 mark       (501) staff       (20)      574 2023-03-18 13:42:50.000000 mash-shell-0.2.0/src/mash/object_parser_server.py
--rw-r--r--   0 mark       (501) staff       (20)     8032 2023-03-18 13:42:50.000000 mash-shell-0.2.0/src/mash/parallel.py
--rw-r--r--   0 mark       (501) staff       (20)     4176 2023-03-18 13:42:50.000000 mash-shell-0.2.0/src/mash/parallel_requests.py
--rw-r--r--   0 mark       (501) staff       (20)     9208 2023-03-18 13:42:50.000000 mash-shell-0.2.0/src/mash/pipeline.py
--rw-r--r--   0 mark       (501) staff       (20)     2761 2023-03-18 13:42:50.000000 mash-shell-0.2.0/src/mash/server.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-03-18 14:39:11.166395 mash-shell-0.2.0/src/mash/shell/
--rw-r--r--   0 mark       (501) staff       (20)      213 2023-03-18 14:32:23.000000 mash-shell-0.2.0/src/mash/shell/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)    39491 2023-03-18 14:32:23.000000 mash-shell-0.2.0/src/mash/shell/base.py
--rw-r--r--   0 mark       (501) staff       (20)     1035 2023-03-18 14:32:23.000000 mash-shell-0.2.0/src/mash/shell/delimiters.py
--rw-r--r--   0 mark       (501) staff       (20)      136 2023-03-18 14:32:23.000000 mash-shell-0.2.0/src/mash/shell/errors.py
--rw-r--r--   0 mark       (501) staff       (20)     1986 2023-03-18 14:32:23.000000 mash-shell-0.2.0/src/mash/shell/function.py
--rw-r--r--   0 mark       (501) staff       (20)     2274 2023-03-18 14:32:23.000000 mash-shell-0.2.0/src/mash/shell/if_statement.py
--rw-r--r--   0 mark       (501) staff       (20)    13353 2023-03-18 14:32:23.000000 mash-shell-0.2.0/src/mash/shell/lex_parser.py
--rw-r--r--   0 mark       (501) staff       (20)    24135 2023-03-18 13:42:50.000000 mash-shell-0.2.0/src/mash/shell/parsetab.py
--rw-r--r--   0 mark       (501) staff       (20)     4476 2023-03-18 14:32:23.000000 mash-shell-0.2.0/src/mash/shell/parsing.py
--rw-r--r--   0 mark       (501) staff       (20)      230 2023-03-18 13:42:50.000000 mash-shell-0.2.0/src/mash/shell/progress_bar.py
--rwxr-xr-x   0 mark       (501) staff       (20)    12164 2023-03-18 14:32:23.000000 mash-shell-0.2.0/src/mash/shell/shell.py
--rw-r--r--   0 mark       (501) staff       (20)     5368 2023-03-18 13:42:50.000000 mash-shell-0.2.0/src/mash/shell/with_filesystem.py
--rw-r--r--   0 mark       (501) staff       (20)     3229 2023-03-18 13:42:50.000000 mash-shell-0.2.0/src/mash/subshell.py
--rw-r--r--   0 mark       (501) staff       (20)    18187 2023-03-18 14:32:23.000000 mash-shell-0.2.0/src/mash/util.py
--rw-r--r--   0 mark       (501) staff       (20)     4024 2023-03-18 13:42:50.000000 mash-shell-0.2.0/src/mash/verify_server.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-03-18 14:39:11.169272 mash-shell-0.2.0/src/mash_shell.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)     3486 2023-03-18 14:39:11.000000 mash-shell-0.2.0/src/mash_shell.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)     1619 2023-03-18 14:39:11.000000 mash-shell-0.2.0/src/mash_shell.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-03-18 14:39:11.000000 mash-shell-0.2.0/src/mash_shell.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)      161 2023-03-18 14:39:11.000000 mash-shell-0.2.0/src/mash_shell.egg-info/requires.txt
--rw-r--r--   0 mark       (501) staff       (20)       18 2023-03-18 14:39:11.000000 mash-shell-0.2.0/src/mash_shell.egg-info/top_level.txt
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-03-18 14:39:11.172654 mash-shell-0.2.0/test/
--rw-r--r--   0 mark       (501) staff       (20)      822 2022-12-04 19:37:35.000000 mash-shell-0.2.0/test/test_html_table.py
--rw-r--r--   0 mark       (501) staff       (20)     1106 2023-03-18 14:17:38.000000 mash-shell-0.2.0/test/test_parallel.py
--rw-r--r--   0 mark       (501) staff       (20)    10304 2023-03-18 14:16:22.000000 mash-shell-0.2.0/test/test_pipeline.py
--rw-r--r--   0 mark       (501) staff       (20)     4054 2023-03-18 14:32:23.000000 mash-shell-0.2.0/test/test_server.py
--rw-r--r--   0 mark       (501) staff       (20)     8153 2022-12-11 09:47:43.000000 mash-shell-0.2.0/test/test_util.py
--rw-r--r--   0 mark       (501) staff       (20)     2500 2022-12-04 19:39:10.000000 mash-shell-0.2.0/test/test_verify_server.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-11 19:58:05.767710 mash-shell-0.2.2/
+-rw-r--r--   0 mark       (501) staff       (20)    35149 2022-11-28 19:29:51.000000 mash-shell-0.2.2/LICENSE
+-rw-r--r--   0 mark       (501) staff       (20)     8174 2023-04-11 19:58:05.767215 mash-shell-0.2.2/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)     7606 2023-04-11 19:57:54.000000 mash-shell-0.2.2/README.md
+-rw-r--r--   0 mark       (501) staff       (20)      736 2023-04-11 19:57:54.000000 mash-shell-0.2.2/pyproject.toml
+-rw-r--r--   0 mark       (501) staff       (20)      161 2023-03-18 10:23:14.000000 mash-shell-0.2.2/requirements.txt
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-04-11 19:58:05.767826 mash-shell-0.2.2/setup.cfg
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-11 19:58:05.722658 mash-shell-0.2.2/src/
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-11 19:58:05.732631 mash-shell-0.2.2/src/examples/
+-rw-r--r--   0 mark       (501) staff       (20)       91 2023-03-18 13:42:50.000000 mash-shell-0.2.2/src/examples/_extend_path.py
+-rwxr-xr-x   0 mark       (501) staff       (20)     2059 2023-03-18 13:42:50.000000 mash-shell-0.2.2/src/examples/discoverable.py
+-rwxr-xr-x   0 mark       (501) staff       (20)      965 2023-03-22 06:58:11.000000 mash-shell-0.2.2/src/examples/discoverable_api.py
+-rw-r--r--   0 mark       (501) staff       (20)     1004 2023-04-08 06:46:34.000000 mash-shell-0.2.2/src/examples/discoverable_with_oas.py
+-rwxr-xr-x   0 mark       (501) staff       (20)      785 2023-03-18 13:42:50.000000 mash-shell-0.2.2/src/examples/filesystem.py
+-rw-r--r--   0 mark       (501) staff       (20)     1126 2023-03-24 06:51:08.000000 mash-shell-0.2.2/src/examples/ms_graph_api.py
+-rwxr-xr-x   0 mark       (501) staff       (20)     3477 2023-03-18 13:42:50.000000 mash-shell-0.2.2/src/examples/object_parser.py
+-rwxr-xr-x   0 mark       (501) staff       (20)     1324 2023-04-11 19:57:54.000000 mash-shell-0.2.2/src/examples/shell_example.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-11 19:58:05.743519 mash-shell-0.2.2/src/mash/
+-rw-r--r--   0 mark       (501) staff       (20)       43 2023-03-18 13:42:50.000000 mash-shell-0.2.2/src/mash/__main__.py
+-rwxr-xr-x   0 mark       (501) staff       (20)     2209 2023-03-18 14:32:23.000000 mash-shell-0.2.2/src/mash/cli.py
+-rw-r--r--   0 mark       (501) staff       (20)     2479 2023-04-11 19:57:54.000000 mash-shell-0.2.2/src/mash/doc_inference.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-11 19:58:05.746314 mash-shell-0.2.2/src/mash/filesystem/
+-rw-r--r--   0 mark       (501) staff       (20)      121 2023-03-18 13:42:50.000000 mash-shell-0.2.2/src/mash/filesystem/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)     6953 2023-04-11 19:57:54.000000 mash-shell-0.2.2/src/mash/filesystem/discoverable.py
+-rw-r--r--   0 mark       (501) staff       (20)    10629 2023-04-10 07:54:42.000000 mash-shell-0.2.2/src/mash/filesystem/filesystem.py
+-rw-r--r--   0 mark       (501) staff       (20)     3252 2023-03-18 14:32:23.000000 mash-shell-0.2.2/src/mash/filesystem/scope.py
+-rw-r--r--   0 mark       (501) staff       (20)     4627 2023-03-24 08:15:55.000000 mash-shell-0.2.2/src/mash/filesystem/view.py
+-rw-r--r--   0 mark       (501) staff       (20)     3455 2023-03-18 13:42:50.000000 mash-shell-0.2.2/src/mash/html_table.py
+-rw-r--r--   0 mark       (501) staff       (20)     2048 2023-03-18 13:42:50.000000 mash-shell-0.2.2/src/mash/html_table_data.py
+-rw-r--r--   0 mark       (501) staff       (20)     5161 2023-03-24 07:32:34.000000 mash-shell-0.2.2/src/mash/io_util.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-11 19:58:05.750594 mash-shell-0.2.2/src/mash/object_parser/
+-rw-r--r--   0 mark       (501) staff       (20)      733 2023-03-18 13:42:50.000000 mash-shell-0.2.2/src/mash/object_parser/errors.py
+-rw-r--r--   0 mark       (501) staff       (20)     8289 2023-03-18 13:42:50.000000 mash-shell-0.2.2/src/mash/object_parser/factory.py
+-rw-r--r--   0 mark       (501) staff       (20)     4505 2023-03-18 13:42:50.000000 mash-shell-0.2.2/src/mash/object_parser/oas.py
+-rw-r--r--   0 mark       (501) staff       (20)     1727 2023-03-18 14:24:14.000000 mash-shell-0.2.2/src/mash/object_parser/object_parser.py
+-rw-r--r--   0 mark       (501) staff       (20)     1129 2023-03-18 13:42:50.000000 mash-shell-0.2.2/src/mash/object_parser/object_parser_standards.py
+-rw-r--r--   0 mark       (501) staff       (20)     4322 2023-03-18 13:42:50.000000 mash-shell-0.2.2/src/mash/object_parser/spec.py
+-rwxr-xr-x   0 mark       (501) staff       (20)      574 2023-03-18 13:42:50.000000 mash-shell-0.2.2/src/mash/object_parser_server.py
+-rw-r--r--   0 mark       (501) staff       (20)     8032 2023-03-18 13:42:50.000000 mash-shell-0.2.2/src/mash/parallel.py
+-rw-r--r--   0 mark       (501) staff       (20)     4176 2023-03-18 13:42:50.000000 mash-shell-0.2.2/src/mash/parallel_requests.py
+-rw-r--r--   0 mark       (501) staff       (20)     9208 2023-03-18 13:42:50.000000 mash-shell-0.2.2/src/mash/pipeline.py
+-rw-r--r--   0 mark       (501) staff       (20)     2761 2023-03-18 13:42:50.000000 mash-shell-0.2.2/src/mash/server.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-11 19:58:05.760913 mash-shell-0.2.2/src/mash/shell/
+-rw-r--r--   0 mark       (501) staff       (20)      215 2023-04-11 19:57:54.000000 mash-shell-0.2.2/src/mash/shell/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)    11161 2023-04-11 19:57:54.000000 mash-shell-0.2.2/src/mash/shell/base.py
+-rw-r--r--   0 mark       (501) staff       (20)     6357 2023-04-11 19:57:54.000000 mash-shell-0.2.2/src/mash/shell/cmd2.py
+-rw-r--r--   0 mark       (501) staff       (20)     1035 2023-04-11 19:57:54.000000 mash-shell-0.2.2/src/mash/shell/delimiters.py
+-rw-r--r--   0 mark       (501) staff       (20)      136 2023-03-18 14:32:23.000000 mash-shell-0.2.2/src/mash/shell/errors.py
+-rw-r--r--   0 mark       (501) staff       (20)     2140 2023-04-11 19:57:54.000000 mash-shell-0.2.2/src/mash/shell/function.py
+-rw-r--r--   0 mark       (501) staff       (20)     2310 2023-04-11 19:57:54.000000 mash-shell-0.2.2/src/mash/shell/if_statement.py
+-rw-r--r--   0 mark       (501) staff       (20)    13323 2023-04-11 19:57:54.000000 mash-shell-0.2.2/src/mash/shell/lex_parser.py
+-rw-r--r--   0 mark       (501) staff       (20)    25476 2023-04-11 19:57:54.000000 mash-shell-0.2.2/src/mash/shell/model.py
+-rw-r--r--   0 mark       (501) staff       (20)    24815 2023-04-10 18:49:45.000000 mash-shell-0.2.2/src/mash/shell/parsetab.py
+-rw-r--r--   0 mark       (501) staff       (20)     4083 2023-04-11 19:57:54.000000 mash-shell-0.2.2/src/mash/shell/parsing.py
+-rw-r--r--   0 mark       (501) staff       (20)      230 2023-03-18 13:42:50.000000 mash-shell-0.2.2/src/mash/shell/progress_bar.py
+-rwxr-xr-x   0 mark       (501) staff       (20)    11434 2023-04-11 19:57:54.000000 mash-shell-0.2.2/src/mash/shell/shell.py
+-rw-r--r--   0 mark       (501) staff       (20)     6367 2023-04-11 19:57:54.000000 mash-shell-0.2.2/src/mash/shell/with_filesystem.py
+-rw-r--r--   0 mark       (501) staff       (20)     3229 2023-03-18 13:42:50.000000 mash-shell-0.2.2/src/mash/subshell.py
+-rw-r--r--   0 mark       (501) staff       (20)    18188 2023-04-11 18:51:45.000000 mash-shell-0.2.2/src/mash/util.py
+-rw-r--r--   0 mark       (501) staff       (20)     4024 2023-03-18 13:42:50.000000 mash-shell-0.2.2/src/mash/verify_server.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-11 19:58:05.763275 mash-shell-0.2.2/src/mash_shell.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)     8174 2023-04-11 19:58:05.000000 mash-shell-0.2.2/src/mash_shell.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)     1695 2023-04-11 19:58:05.000000 mash-shell-0.2.2/src/mash_shell.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-04-11 19:58:05.000000 mash-shell-0.2.2/src/mash_shell.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)      161 2023-04-11 19:58:05.000000 mash-shell-0.2.2/src/mash_shell.egg-info/requires.txt
+-rw-r--r--   0 mark       (501) staff       (20)       18 2023-04-11 19:58:05.000000 mash-shell-0.2.2/src/mash_shell.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-11 19:58:05.766685 mash-shell-0.2.2/test/
+-rw-r--r--   0 mark       (501) staff       (20)      822 2022-12-04 19:37:35.000000 mash-shell-0.2.2/test/test_html_table.py
+-rw-r--r--   0 mark       (501) staff       (20)     1106 2023-03-18 14:17:38.000000 mash-shell-0.2.2/test/test_parallel.py
+-rw-r--r--   0 mark       (501) staff       (20)    10304 2023-03-18 14:16:22.000000 mash-shell-0.2.2/test/test_pipeline.py
+-rw-r--r--   0 mark       (501) staff       (20)     4054 2023-03-18 14:32:23.000000 mash-shell-0.2.2/test/test_server.py
+-rw-r--r--   0 mark       (501) staff       (20)     8153 2022-12-11 09:47:43.000000 mash-shell-0.2.2/test/test_util.py
+-rw-r--r--   0 mark       (501) staff       (20)     2500 2022-12-04 19:39:10.000000 mash-shell-0.2.2/test/test_verify_server.py
```

### Comparing `mash-shell-0.2.0/LICENSE` & `mash-shell-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.0/pyproject.toml` & `mash-shell-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mash-shell"
-version = "0.2.0"
+version = "0.2.2"
 authors = [
   { name="voschezang", email="mark.voschezang@student.uva.nl" },
 ]
 description = "A shell and other utils"
 dynamic = ["dependencies"]
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `mash-shell-0.2.0/src/examples/discoverable.py` & `mash-shell-0.2.2/src/examples/discoverable.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.0/src/examples/discoverable_api.py` & `mash-shell-0.2.2/src/examples/discoverable_api.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.0/src/examples/discoverable_with_oas.py` & `mash-shell-0.2.2/src/examples/discoverable_with_oas.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,16 +19,16 @@
     obj.init_home(['repository'])
 
     path = []
     result = 'departments'
 
     # for i in range(7):
     for i in range(7):
-        k = result.split('\n')[-1]
-        path.append(k)
+        key = result.split('\n')[-1]
+        path.append(key)
         result = obj.ll(*path)
 
     json = JSONFactory(Organization).build(obj['repository'])
     oas = OAS()
     oas.extend(json)
     oas['servers'] = [{'url': 'http://localhost:5000/v1'}]
     oas['paths']['/organizations'] = path_create('Organization')
```

### Comparing `mash-shell-0.2.0/src/examples/filesystem.py` & `mash-shell-0.2.2/src/examples/filesystem.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.0/src/examples/object_parser.py` & `mash-shell-0.2.2/src/examples/object_parser.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.0/src/examples/shell_example.py` & `mash-shell-0.2.2/src/examples/shell_example.py`

 * *Files 13% similar despite different names*

```diff
@@ -42,15 +42,14 @@
     'another_function': f,
     'f': f,
     'g': g,
     'h': h,
     'example': example,
     'inspect': inspect,
     'ls': Function(sh_to_py('ls'), args={'-latr': 'flags', '[file]': ''}),
-    'cat': Function(sh_to_py('cat'), args={'file': ''}),
     'vi': Function(sh_to_py('vi'), args={'[file]': ''})}
 
 if __name__ == '__main__':
     # setting cli args is a requirement for shell.has_input
     set_cli_args()
 
     if has_output(sys.stdin) or has_input():
```

### Comparing `mash-shell-0.2.0/src/mash/cli.py` & `mash-shell-0.2.2/src/mash/cli.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.0/src/mash/doc_inference.py` & `mash-shell-0.2.2/src/mash/doc_inference.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 from typing import Dict
 
+from mash.util import removeprefix
+
 
 def infer_default_and_non_default_args(func):
-    args = list(func.__code__.co_varnames)
+    try:
+        args = list(func.__code__.co_varnames)
+    except AttributeError:
+        raise NotImplementedError()
+
     n_default_args = len(func.__defaults__) if func.__defaults__ else 0
     n_non_default_args = len(args) - n_default_args
     non_default_args = args[:n_non_default_args]
     default_args = args[n_non_default_args:]
     return non_default_args, default_args
 
 
@@ -14,15 +20,22 @@
     non_default_args, default_args = infer_default_and_non_default_args(func)
     return non_default_args + [f'[{a}]' for a in default_args]
 
 
 def infer_synopsis(func, variables=[]) -> str:
     if not variables:
         variables = infer_args(func)
-    return ' '.join([func.__name__] + variables)
+
+        # rm arg: self
+        if variables and variables[0] == 'self':
+            variables = variables[1:]
+
+    # rm prefix: do_
+    func_name = removeprefix(func.__name__, 'do_')
+    return ' '.join([func_name] + variables)
 
 
 def infer_signature(func) -> dict:
     _, default_args = infer_default_and_non_default_args(func)
 
     def format(k):
         key = k
```

### Comparing `mash-shell-0.2.0/src/mash/filesystem/discoverable.py` & `mash-shell-0.2.2/src/mash/filesystem/discoverable.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,14 +92,16 @@
         cwd.set(k, observed_value)
 
         initial_values_key = infer_initial_value_key(k, cwd)
         if initial_values_key not in self.initial_values:
             self.initial_values[initial_values_key] = initial_value
 
     def show(self, *path: str):
+        """Show contents
+        """
         # TODO keys in path are not autocompleted
         if path == ((),):
             path = self.full_path[1:]
         else:
             path = self.full_path[1:] + list(path)
 
         data = self.observe_child_fields(path)
```

### Comparing `mash-shell-0.2.0/src/mash/filesystem/filesystem.py` & `mash-shell-0.2.2/src/mash/filesystem/filesystem.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.0/src/mash/filesystem/scope.py` & `mash-shell-0.2.2/src/mash/filesystem/scope.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.0/src/mash/filesystem/view.py` & `mash-shell-0.2.2/src/mash/filesystem/view.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,15 +58,21 @@
     def set(self, k: Key, value):
         self.tree[k] = value
 
     def ls(self) -> Iterable[Key]:
         try:
             return self.tree.keys()
         except AttributeError:
-            return range(len(self.tree))
+            if isinstance(self.tree, list):
+                try:
+                    return [item[NAME] for item in self.tree]
+                except (TypeError, KeyError):
+                    pass
+
+        return range(len(self.tree))
 
     def cp(self, *references: Key):
         *sources, dst = references
 
         if not sources:
             raise ValueError(
                 f'At least two arguments are required, but got {references}')
```

### Comparing `mash-shell-0.2.0/src/mash/html_table.py` & `mash-shell-0.2.2/src/mash/html_table.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.0/src/mash/html_table_data.py` & `mash-shell-0.2.2/src/mash/html_table_data.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.0/src/mash/io_util.py` & `mash-shell-0.2.2/src/mash/io_util.py`

 * *Files 4% similar despite different names*

```diff
@@ -211,8 +211,13 @@
 
     msg = result.stdout.decode(), result.stderr.decode()
     assert result.returncode == 0, msg
 
     return result.stdout.decode().rstrip('\n')
 
 
+@functools.lru_cache(maxsize=64)
+def log_once(*msgs: str):
+    logging.debug(*msgs)
+
+
 set_verbosity()
```

### Comparing `mash-shell-0.2.0/src/mash/object_parser/errors.py` & `mash-shell-0.2.2/src/mash/object_parser/errors.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.0/src/mash/object_parser/factory.py` & `mash-shell-0.2.2/src/mash/object_parser/factory.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.0/src/mash/object_parser/oas.py` & `mash-shell-0.2.2/src/mash/object_parser/oas.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.0/src/mash/object_parser/object_parser.py` & `mash-shell-0.2.2/src/mash/object_parser/object_parser.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.0/src/mash/object_parser/object_parser_standards.py` & `mash-shell-0.2.2/src/mash/object_parser/object_parser_standards.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.0/src/mash/object_parser/spec.py` & `mash-shell-0.2.2/src/mash/object_parser/spec.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.0/src/mash/object_parser_server.py` & `mash-shell-0.2.2/src/mash/object_parser_server.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.0/src/mash/parallel.py` & `mash-shell-0.2.2/src/mash/parallel.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.0/src/mash/parallel_requests.py` & `mash-shell-0.2.2/src/mash/parallel_requests.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.0/src/mash/pipeline.py` & `mash-shell-0.2.2/src/mash/pipeline.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.0/src/mash/server.py` & `mash-shell-0.2.2/src/mash/server.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.0/src/mash/shell/delimiters.py` & `mash-shell-0.2.2/src/mash/shell/delimiters.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.0/src/mash/shell/function.py` & `mash-shell-0.2.2/src/mash/shell/function.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,43 @@
+from collections import defaultdict
 from copy import deepcopy
 from dataclasses import dataclass, field
 from types import TracebackType
 from typing import Dict, List
-import logging
 import sys
 
 from mash.doc_inference import generate_docs
-from mash.io_util import log
+from mash.io_util import log, log_once
 from mash import util
 
 # this data is impacts by both the classes Function and Shell, hence it should be global
 exception_hint = '(run `E` for details)'
 
 # global cache: sys.last_value and sys.last_traceback don't store exceptions raised in cmd.Cmd
 last_exception: Exception = None
 last_traceback: TracebackType = None
 
 
+LAST_RESULTS = '_last_results'
+LAST_RESULTS_INDEX = '_last_results_index'
+
+
 class ShellFunction:
     def __init__(self, func, func_name=None, synopsis: str = None, args: Dict[str, str] = None, doc: str = None) -> None:
         try:
             self.help = generate_docs(func, synopsis, args, doc)
         except NotImplementedError:
             self.help = func.__doc__
 
         try:
             # copy to prevent side-effects
             func = deepcopy(func)
         except TypeError as e:
             name = getattr(func, '__name__', 'func')
-            logging.debug(f'Cannot deepcopy `{name}`: {e.args[0]}')
+            log_once(f'Cannot deepcopy `{name}`: {e.args[0]}')
 
         self.func = func
 
         if func_name is not None:
             util.rename(self.func, func_name)
 
     def __call__(self, args: str = ''):
@@ -61,7 +65,11 @@
 class InlineFunction:
     command: str
     args: List[str]
     func_name: str
     multiline: bool = False
     line_indent: str = None
     inner: List[str] = field(default_factory=list)
+
+
+def scope() -> dict:
+    return defaultdict(dict)
```

### Comparing `mash-shell-0.2.0/src/mash/shell/if_statement.py` & `mash-shell-0.2.2/src/mash/shell/if_statement.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from operator import contains
 from typing import Tuple
 from mash.shell.delimiters import ELSE, IF, INLINE_THEN, THEN
 from mash.shell.errors import ShellError
 
 LINE_INDENT = 'line_indent'
+RAW_LINE_INDENT = 'raw_line_indent'
 
 
 class Abort(RuntimeError):
     pass
 
 
 def State(self, value, branch=None) -> dict:
```

### Comparing `mash-shell-0.2.0/src/mash/shell/lex_parser.py` & `mash-shell-0.2.2/src/mash/shell/lex_parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from collections import UserString
 from logging import getLogger
 import ply.lex as lex
 import ply.yacc as yacc
+from mash.shell.model import Assign, BashPipe, BinaryExpression, Else, ElseIf, ElseIfThen, FunctionDefinition, If, IfThen, IfThenElse, Indent, InlineFunctionDefinition, Lines, LogicExpression, Map, Math, Method, Pipe, Quoted, Return, Shell, Terms, Then, Variable, Word
 from mash.shell.parsing import indent_width
 from mash.shell.errors import ShellSyntaxError
 
 lexer = None
 
 tokens = (
     'BASH',  # | >>
@@ -36,14 +36,15 @@
     'WORD',
     'WORD_WITH_DOT',
     'NUMBER_WITH_DOT',
 
     'WILDCARD',
     'WILDCARD_RANGE',
     'NUMBER',  # 0123456789
+    'LONG_SYMBOL',
     'SYMBOL',
 )
 reserved = {
     'if': 'IF',
     'then': 'THEN',
     'else': 'ELSE',
     'return': 'RETURN',
@@ -51,20 +52,14 @@
     'and': 'AND',
     'or': 'OR',
     'math': 'MATH',
 }
 tokens += tuple(reserved.values())
 
 
-class Term(UserString):
-    def __init__(self, value, string_type='term'):
-        self.data = value
-        self.type = string_type
-
-
 def init_lex():
     """
     Token regexes are defined with the prefix `t_`.
     From ply docs:
     - functions are matched in order of specification
     - strings are sorted by regular expression length
     """
@@ -98,17 +93,14 @@
         # semicolon_with_whitespace = r'((\;)+[ \t]*)'
         # newlines = r'(\n+)'
 
         # TOOD if not ;
         t.lexer.lineno += len(t.value)
         return t
 
-    # def t_COMMENT(t):
-    #     r'\#.*'
-
     def t_INDENT(t):
         r'\ {2,}|\t+'
         return t
 
     def t_DOUBLE_QUOTED_STRING(t):
         r'"((\\\")|[^\""])*"'
         t.type = reserved.get(t.value, 'DOUBLE_QUOTED_STRING')
@@ -152,14 +144,18 @@
         return t
 
     def t_NUMBER_WITH_DOT(t):
         r'-?(\d+\.\d*)|(\d*\.\d+)'
         # match *. or .* or *.*
         return t
 
+    def t_LONG_SYMBOL(t):
+        r'\+\+|::|=>|~>|\|->'
+        return t
+
     def t_MAP(t):
         r'>>='
         return t
 
     def t_PIPE(t):
         r'\|>'
         return t
@@ -181,27 +177,27 @@
         return t
 
     def t_INFIX_OPERATOR(t):
         r'!=|<=|>=|<|>'
         return t
 
     def t_WORD(t):
-        r'[\w\d\-%&\~]+'
+        r'[\w\d\-%&\~/]+'
         return t
 
     def t_NUMBER(t):
         r'-?\d+'
         return t
 
     def t_SHELL(t):
         r'\!'
         return t
 
     def t_SYMBOL(t):
-        r'[\~\+\*\-%&.?]+'
+        r'[\~\+\*\-%&.]+'
         return t
 
     def t_error(t):
         print(f'Illegal character: `{t.value[0]}`')
         t.lexer.skip(1)
         raise ShellSyntaxError(f'Illegal character: `{t.value[0]}`')
 
@@ -239,57 +235,56 @@
 
     def p_lines_empty(p):
         """lines : BREAK
                  | INDENT BREAK
         """
         'lines : BREAK'
         # TODO handle `indent expr ; expr`
-        p[0] = ('lines', [])
+        p[0] = Lines([])
 
     def p_lines_suffix(p):
         """lines : line
                  | line BREAK
         """
-        p[0] = ('lines', [p[1]])
+        p[0] = Lines([p[1]])
 
     def p_lines_infix(p):
         'lines : line BREAK lines'
-        _, lines = p[3]
-        p[0] = ('lines', [p[1]] + lines)
+        p[0] = Lines([p[1]]) + p[3]
 
     def p_lines_prefix(p):
         'lines : BREAK lines'
         p[0] = p[2]
 
     def p_line_indented(p):
         'line : INDENT statement'
         n = indent_width(p[1])
-        p[0] = ('indent', n, p[2])
+        p[0] = Indent(p[2], n)
 
     def p_line(p):
         'line : statement'
         p[0] = p[1]
 
     def p_line_indent_empty(p):
         'line : INDENT'
         n = indent_width(p[1])
-        p[0] = ('indent', n, None)
+        p[0] = Indent(None, n)
 
     def p_statement(p):
         """statement : assignment
                      | conditional
                      | definition
                      | inner_statement
                      | return_statement
         """
         p[0] = p[1]
 
     def p_statement_return(p):
         'return_statement : RETURN inner_statement'
-        p[0] = ('return', p[2])
+        p[0] = Return(p[2])
 
     def p_inner_statement(p):
         """inner_statement : conjunction
                            | full_conditional
         """
         p[0] = p[1]
 
@@ -297,141 +292,141 @@
         """final_statement : conjunction
                            | return_statement
         """
         p[0] = p[1]
 
     def p_assign(p):
         'assignment : terms ASSIGN inner_statement'
-        p[0] = ('assign', p[2], p[1], p[3])
+        p[0] = Assign(p[1], p[3], p[2])
 
     def p_assign_right(p):
         'assignment : inner_statement ASSIGN_RIGHT terms'
-        p[0] = ('assign', p[2], p[1], p[3])
+        p[0] = Assign(p[3], p[1], p[2])
 
     def p_def_inline_function(p):
         'definition : METHOD LPAREN terms RPAREN DEFINE_FUNCTION inner_statement'
-        p[0] = ('define-inline-function', p[1], p[3], p[6])
+        p[0] = InlineFunctionDefinition(p[1], p[3], body=p[6])
 
     def p_def_inline_function_constant(p):
         'definition : METHOD LPAREN RPAREN DEFINE_FUNCTION inner_statement'
-        p[0] = ('define-inline-function', p[1], '', p[5])
+        p[0] = InlineFunctionDefinition(p[1], body=p[5])
 
     def p_def_function(p):
         'definition : METHOD LPAREN terms RPAREN DEFINE_FUNCTION'
-        p[0] = ('define-function', p[1], p[3])
+        p[0] = FunctionDefinition(p[1], p[3])
 
     def p_def_function_constant(p):
         'definition : METHOD LPAREN RPAREN DEFINE_FUNCTION'
-        p[0] = ('define-function', p[1], p[3])
+        p[0] = FunctionDefinition(p[1])
 
     def p_scope(p):
         'scope : LPAREN inner_statement RPAREN'
         q = p[2]
         p[0] = ('scope', q)
 
     def p_if(p):
         'conditional : IF conjunction'
-        p[0] = ('if', p[2])
+        p[0] = If(p[2])
 
     def p_full_conditional(p):
         'full_conditional : IF conjunction THEN conjunction ELSE conjunction'
         _, _if, cond, _then, true, _else, false = p
-        p[0] = ('if-then-else', cond, true, false)
+        p[0] = IfThenElse(cond, true, false)
 
     def p_if_then_inline(p):
         'full_conditional : IF conjunction THEN conjunction'
         _, _if, cond, _then, true = p
-        p[0] = ('if-then', cond, true)
+        p[0] = IfThen(cond, true)
 
     def p_if_then_else(p):
         'conditional : IF conjunction THEN conjunction ELSE'
         _, _if, cond, _then, true, _else = p
         p[0] = ('if-then-else', cond, true, None)
 
     def p_if_then(p):
         'conditional : IF conjunction THEN'
-        p[0] = ('if-then', p[2], None)
+        p[0] = IfThen(p[2])
 
     def p_if_then_inline_final(p):
         'conditional : IF conjunction THEN return_statement'
         _, _if, cond, _then, true = p
-        p[0] = ('if-then', cond, true)
+        p[0] = IfThen(cond, true)
 
     def p_then(p):
         """conditional : THEN final_statement
                        | THEN
         """
         if len(p) == 2:
-            p[0] = ('then', None)
+            p[0] = Then()
         else:
-            p[0] = ('then', p[2])
+            p[0] = Then(p[2])
 
     def p_else_if_then(p):
         """conditional : ELSE IF conjunction THEN final_statement
                       | ELSE IF conjunction THEN
         """
         if len(p) == 6:
-            p[0] = ('else-if-then', p[3], p[5])
+            p[0] = ElseIfThen(p[3], p[5])
         else:
-            p[0] = ('else-if-then', p[3], None)
+            p[0] = ElseIfThen(p[3])
 
     def p_else_if(p):
         'conditional : ELSE IF conjunction'
-        p[0] = ('else-if', p[3])
+        p[0] = ElseIf(p[3])
 
     def p_else(p):
         """conditional : ELSE final_statement
                        | ELSE
         """
         if len(p) == 2:
-            p[0] = ('else', None)
+            p[0] = Else()
         else:
-            p[0] = ('else', p[2])
+            p[0] = Else(p[2])
 
     def p_conditional(p):
         """conditional : conjunction
                        | full_conditional
         """
         p[0] = p[1]
 
     def p_pipe_py(p):
         'conjunction : expression PIPE conjunction'
-        p[0] = ('pipe', p[1], p[3])
+        p[0] = Pipe(p[1], p[3], p[2])
 
     def p_conjunction(p):
         'conjunction : expression'
         p[0] = p[1]
 
     def p_pipe_bash(p):
         'expression : expression BASH expression'
-        p[0] = ('bash', p[2], p[1], p[3])
+        p[0] = BashPipe(p[1], p[3], p[2])
 
     def p_pipe_map(p):
         'expression : expression MAP expression'
-        p[0] = ('map', p[1], p[3])
+        p[0] = Map(p[1], p[3])
 
     def p_expression_full_conditional(p):
         'expression : full_conditional'
         p[0] = p[1]
 
     def p_expression(p):
         'expression : basic_expression'
         p[0] = p[1]
 
     def p_shell(p):
         'expression : SHELL expression'
-        p[0] = ('!', p[2])
+        p[0] = Shell(p[2])
 
     def p_shell_empty(p):
         'expression : SHELL'
-        p[0] = ('!', '')
+        p[0] = Shell()
 
     def p_math(p):
         'expression : MATH expression'
-        p[0] = ('math', p[2])
+        p[0] = Math(p[2])
 
     def p_basic_expression(p):
         """basic_expression : join
                             | logic_expression
                             | terms
         """
         p[0] = p[1]
@@ -439,94 +434,96 @@
     def p_logic_binary(p):
         """join : logic_expression AND join
                 | logic_expression AND logic_expression
                 | logic_expression OR join
                 | logic_expression OR logic_expression
         """
         # TODO use flat tree any/all (or, a, b, c) = any : e OR any  | e OR e
-        p[0] = ('logic', p[2], p[1], p[3])
+        p[0] = LogicExpression(p[1], p[3], p[2])
 
     def p_logic_expression_infix(p):
         'logic_expression : terms INFIX_OPERATOR logic_expression'
-        p[0] = ('binary-expression', p[2], p[1], p[3])
+        p[0] = BinaryExpression(p[1], p[3], p[2])
 
     def p_logic_expression_infix_equals(p):
         'logic_expression : logic_expression EQUALS logic_expression'
-        p[0] = ('binary-expression', p[2], p[1], p[3])
+        p[0] = BinaryExpression(p[1], p[3], p[2])
 
     def p_logic_negation(p):
         'logic_expression : NOT terms'
+        # TODO
         p[0] = ('not', p[2])
 
     def p_logic(p):
         'logic_expression : terms'
         p[0] = p[1]
 
     def p_terms_pair(p):
         'terms : term term'
-        p[0] = ('terms', [p[1], p[2]])
+        p[0] = Terms([p[1], p[2]])
 
     def p_terms_head_tail(p):
         'terms : term terms'
-        key, tail = p[2]
-        p[0] = ('terms', [p[1]] + tail)
+        p[0] = Terms([p[1]] + p[2].values)
 
     def p_terms_singleton(p):
         'terms : term'
         p[0] = p[1]
 
     def p_term(p):
         """term : SPECIAL
                 | WORD
                 | WORD_WITH_DOT
         """
-        p[0] = Term(p[1])
+        p[0] = Word(p[1], 'term')
 
     def p_term_value(p):
         """term : value
                 | method
                 | scope
         """
         p[0] = p[1]
 
     def p_value_wildcard(p):
         'value : WILDCARD'
-        p[0] = Term(p[1], 'wildcard')
+        p[0] = Word(p[1], 'wildcard')
 
     def p_value_wildcard_range(p):
         'value : WILDCARD_RANGE'
-        p[0] = Term(p[1], 'range')
+        p[0] = Word(p[1], 'range')
 
     def p_value_number_int(p):
         'value : NUMBER'
-        p[0] = Term(p[1], 'number')
+        p[0] = Word(p[1], 'number')
 
     def p_value_number_float(p):
         'value : NUMBER_WITH_DOT'
-        p[0] = Term(p[1], 'number')
+        p[0] = Word(p[1], 'number')
 
     def p_value_method(p):
         'method : METHOD'
-        p[0] = Term(p[1], 'method')
+        p[0] = Method(p[1])
 
     def p_value_variable(p):
         'value : VARIABLE'
-        p[0] = Term(p[1], 'variable')
+        p[0] = Variable(p[1])
 
     def p_value_symbol(p):
-        'value : SYMBOL'
-        p[0] = Term(p[1], 'symbol')
+        """value : SYMBOL
+                 | LONG_SYMBOL
+        """
+        p[0] = Word(p[1], 'symbol')
 
     def p_value_literal_string(p):
         'value : SINGLE_QUOTED_STRING'
-        p[0] = Term(p[1], 'literal string')
+        p[0] = Word(p[1], 'literal string')
 
     def p_value_string(p):
         'value : DOUBLE_QUOTED_STRING'
-        p[0] = Term(p[1], 'quoted string')
+        p[0] = Quoted(p[1])
 
     def p_illegal_if_then(p):
         """conditional : IF THEN
                        | IF INDENT THEN
                        | IF ELSE
                        | IF INDENT ELSE
                        | ELSE THEN
@@ -548,20 +545,16 @@
     log = getLogger()
     parser = yacc.yacc(debug=log)
 
     # add a newline to allow empty strings to be matched
     return parser.parse('\n' + text)
 
 
-def Terms(args):
-    return ('terms', args)
-
-
 if __name__ == '__main__':
     data = """
 
     echo x
     if 1 = 3 then 2 else 3
     """
 
-    result = parse(data)
-    print('out', result)
+    prev_result = parse(data)
+    print('out', prev_result)
```

### Comparing `mash-shell-0.2.0/src/mash/shell/parsetab.py` & `mash-shell-0.2.2/src/mash/shell/parsetab.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,114 +2,115 @@
 # parsetab.py
 # This file is automatically generated. Do not edit.
 # pylint: disable=W,C,R
 _tabversion = '3.10'
 
 _lr_method = 'LALR'
 
-_lr_signature = 'leftBREAKleftINDENTleftASSIGNleftPIPEBASHleftMATHleftINFIX_OPERATORleftEQUALSleftORleftANDleftNOTAND ASSIGN ASSIGN_RIGHT BASH BREAK DEFINE_FUNCTION DOUBLE_QUOTED_STRING ELSE EQUALS IF INDENT INFIX_OPERATOR LPAREN MAP MATH METHOD NOT NUMBER NUMBER_WITH_DOT OR PIPE RETURN RPAREN SHELL SINGLE_QUOTED_STRING SPACE SPECIAL SYMBOL THEN VARIABLE WILDCARD WILDCARD_RANGE WORD WORD_WITH_DOTlines : BREAK\n                 | INDENT BREAK\n        lines : line\n                 | line BREAK\n        lines : line BREAK lineslines : BREAK linesline : INDENT statementline : statementline : INDENTstatement : assignment\n                     | conditional\n                     | definition\n                     | inner_statement\n                     | return_statement\n        return_statement : RETURN inner_statementinner_statement : conjunction\n                           | full_conditional\n        final_statement : conjunction\n                           | return_statement\n        assignment : terms ASSIGN inner_statementassignment : inner_statement ASSIGN_RIGHT termsdefinition : METHOD LPAREN terms RPAREN DEFINE_FUNCTION inner_statementdefinition : METHOD LPAREN RPAREN DEFINE_FUNCTION inner_statementdefinition : METHOD LPAREN terms RPAREN DEFINE_FUNCTIONdefinition : METHOD LPAREN RPAREN DEFINE_FUNCTIONscope : LPAREN inner_statement RPARENconditional : IF conjunctionfull_conditional : IF conjunction THEN conjunction ELSE conjunctionfull_conditional : IF conjunction THEN conjunctionconditional : IF conjunction THEN conjunction ELSEconditional : IF conjunction THENconditional : IF conjunction THEN return_statementconditional : THEN final_statement\n                       | THEN\n        conditional : ELSE IF conjunction THEN final_statement\n                      | ELSE IF conjunction THEN\n        conditional : ELSE IF conjunctionconditional : ELSE final_statement\n                       | ELSE\n        conditional : conjunction\n                       | full_conditional\n        conjunction : expression PIPE conjunctionconjunction : expressionexpression : expression BASH expressionexpression : expression MAP expressionexpression : full_conditionalexpression : basic_expressionexpression : SHELL expressionexpression : SHELLexpression : MATH expressionbasic_expression : join\n                            | logic_expression\n                            | terms\n        join : logic_expression AND join\n                | logic_expression AND logic_expression\n                | logic_expression OR join\n                | logic_expression OR logic_expression\n        logic_expression : terms INFIX_OPERATOR logic_expressionlogic_expression : logic_expression EQUALS logic_expressionlogic_expression : NOT termslogic_expression : termsterms : term termterms : term termsterms : termterm : SPECIAL\n                | WORD\n                | WORD_WITH_DOT\n        term : value\n                | method\n                | scope\n        value : WILDCARDvalue : WILDCARD_RANGEvalue : NUMBERvalue : NUMBER_WITH_DOTmethod : METHODvalue : VARIABLEvalue : SYMBOLvalue : SINGLE_QUOTED_STRINGvalue : DOUBLE_QUOTED_STRINGconditional : IF THEN\n                       | IF INDENT THEN\n                       | IF ELSE\n                       | IF INDENT ELSE\n                       | ELSE THEN\n                       | ELSE INDENT THEN\n        '
+_lr_signature = 'leftBREAKleftINDENTleftASSIGNleftPIPEBASHleftMATHleftINFIX_OPERATORleftEQUALSleftORleftANDleftNOTAND ASSIGN ASSIGN_RIGHT BASH BREAK DEFINE_FUNCTION DOUBLE_QUOTED_STRING ELSE EQUALS IF INDENT INFIX_OPERATOR LONG_SYMBOL LPAREN MAP MATH METHOD NOT NUMBER NUMBER_WITH_DOT OR PIPE RETURN RPAREN SHELL SINGLE_QUOTED_STRING SPACE SPECIAL SYMBOL THEN VARIABLE WILDCARD WILDCARD_RANGE WORD WORD_WITH_DOTlines : BREAK\n                 | INDENT BREAK\n        lines : line\n                 | line BREAK\n        lines : line BREAK lineslines : BREAK linesline : INDENT statementline : statementline : INDENTstatement : assignment\n                     | conditional\n                     | definition\n                     | inner_statement\n                     | return_statement\n        return_statement : RETURN inner_statementinner_statement : conjunction\n                           | full_conditional\n        final_statement : conjunction\n                           | return_statement\n        assignment : terms ASSIGN inner_statementassignment : inner_statement ASSIGN_RIGHT termsdefinition : METHOD LPAREN terms RPAREN DEFINE_FUNCTION inner_statementdefinition : METHOD LPAREN RPAREN DEFINE_FUNCTION inner_statementdefinition : METHOD LPAREN terms RPAREN DEFINE_FUNCTIONdefinition : METHOD LPAREN RPAREN DEFINE_FUNCTIONscope : LPAREN inner_statement RPARENconditional : IF conjunctionfull_conditional : IF conjunction THEN conjunction ELSE conjunctionfull_conditional : IF conjunction THEN conjunctionconditional : IF conjunction THEN conjunction ELSEconditional : IF conjunction THENconditional : IF conjunction THEN return_statementconditional : THEN final_statement\n                       | THEN\n        conditional : ELSE IF conjunction THEN final_statement\n                      | ELSE IF conjunction THEN\n        conditional : ELSE IF conjunctionconditional : ELSE final_statement\n                       | ELSE\n        conditional : conjunction\n                       | full_conditional\n        conjunction : expression PIPE conjunctionconjunction : expressionexpression : expression BASH expressionexpression : expression MAP expressionexpression : full_conditionalexpression : basic_expressionexpression : SHELL expressionexpression : SHELLexpression : MATH expressionbasic_expression : join\n                            | logic_expression\n                            | terms\n        join : logic_expression AND join\n                | logic_expression AND logic_expression\n                | logic_expression OR join\n                | logic_expression OR logic_expression\n        logic_expression : terms INFIX_OPERATOR logic_expressionlogic_expression : logic_expression EQUALS logic_expressionlogic_expression : NOT termslogic_expression : termsterms : term termterms : term termsterms : termterm : SPECIAL\n                | WORD\n                | WORD_WITH_DOT\n        term : value\n                | method\n                | scope\n        value : WILDCARDvalue : WILDCARD_RANGEvalue : NUMBERvalue : NUMBER_WITH_DOTmethod : METHODvalue : VARIABLEvalue : SYMBOL\n                 | LONG_SYMBOL\n        value : SINGLE_QUOTED_STRINGvalue : DOUBLE_QUOTED_STRINGconditional : IF THEN\n                       | IF INDENT THEN\n                       | IF ELSE\n                       | IF INDENT ELSE\n                       | ELSE THEN\n                       | ELSE INDENT THEN\n        '
     
-_lr_action_items = {'BREAK':([0,2,3,4,5,6,7,8,9,10,11,13,14,15,16,17,20,21,22,23,24,25,26,27,28,29,31,32,33,34,35,36,37,38,39,40,44,45,50,51,52,54,55,56,57,58,59,61,62,66,67,68,69,70,74,75,79,81,82,83,84,86,87,88,89,90,93,94,95,96,97,98,99,100,101,103,104,105,107,108,109,110,111,112,113,115,116,],[2,2,-9,45,-8,-10,-11,-12,-13,-14,-53,-16,-34,-39,-17,-75,-64,-43,-65,-66,-67,-68,-69,-70,-47,-49,-71,-72,-73,-74,-76,-77,-78,-79,-51,-52,-7,2,-27,-80,-82,-46,-53,-75,-33,-18,-19,-84,-38,-16,-17,-15,-62,-63,-48,-50,-60,-21,-20,-61,-58,-31,-81,-83,-37,-85,-26,-42,-44,-45,-55,-54,-57,-56,-59,-29,-32,-36,-25,-29,-30,-18,-35,-24,-23,-28,-22,]),'INDENT':([0,2,12,15,45,],[3,3,53,63,3,]),'IF':([0,2,3,12,14,15,18,19,29,30,45,47,49,60,71,72,73,86,102,105,107,109,112,114,],[12,12,12,49,49,60,49,49,49,49,12,49,49,49,49,49,49,49,49,49,49,49,49,49,]),'THEN':([0,2,3,12,15,20,21,22,23,24,25,26,27,28,29,31,32,33,34,35,36,37,38,39,40,45,50,53,54,55,56,63,69,70,74,75,79,83,84,85,89,93,94,95,96,97,98,99,100,101,108,115,],[14,14,14,51,61,-64,-43,-65,-66,-67,-68,-69,-70,-47,-49,-71,-72,-73,-74,-76,-77,-78,-79,-51,-52,14,86,87,-46,-53,-75,90,-62,-63,-48,-50,-60,-61,-58,102,105,-26,-42,-44,-45,-55,-54,-57,-56,-59,-29,-28,]),'ELSE':([0,2,3,12,20,21,22,23,24,25,26,27,28,29,31,32,33,34,35,36,37,38,39,40,45,53,54,55,56,69,70,74,75,79,83,84,93,94,95,96,97,98,99,100,101,103,108,110,115,],[15,15,15,52,-64,-43,-65,-66,-67,-68,-69,-70,-47,-49,-71,-72,-73,-74,-76,-77,-78,-79,-51,-52,15,88,-46,-53,-75,-62,-63,-48,-50,-60,-61,-58,-26,-42,-44,-45,-55,-54,-57,-56,-59,109,114,114,-28,]),'METHOD':([0,2,3,12,14,15,17,18,19,20,22,23,24,25,26,27,29,30,31,32,33,34,35,36,37,38,41,45,46,47,48,49,56,60,64,69,71,72,73,76,77,78,86,93,102,105,107,109,112,114,],[17,17,17,56,56,56,-75,56,56,56,-65,-66,-67,-68,-69,-70,56,56,-71,-72,-73,-74,-76,-77,-78,-79,56,17,56,56,56,56,-75,56,56,56,56,56,56,56,56,56,56,-26,56,56,56,56,56,56,]),'RETURN':([0,2,3,14,15,45,86,105,],[19,19,19,19,19,19,19,19,]),'SPECIAL':([0,2,3,12,14,15,17,18,19,20,22,23,24,25,26,27,29,30,31,32,33,34,35,36,37,38,41,45,46,47,48,49,56,60,64,69,71,72,73,76,77,78,86,93,102,105,107,109,112,114,],[22,22,22,22,22,22,-75,22,22,22,-65,-66,-67,-68,-69,-70,22,22,-71,-72,-73,-74,-76,-77,-78,-79,22,22,22,22,22,22,-75,22,22,22,22,22,22,22,22,22,22,-26,22,22,22,22,22,22,]),'WORD':([0,2,3,12,14,15,17,18,19,20,22,23,24,25,26,27,29,30,31,32,33,34,35,36,37,38,41,45,46,47,48,49,56,60,64,69,71,72,73,76,77,78,86,93,102,105,107,109,112,114,],[23,23,23,23,23,23,-75,23,23,23,-65,-66,-67,-68,-69,-70,23,23,-71,-72,-73,-74,-76,-77,-78,-79,23,23,23,23,23,23,-75,23,23,23,23,23,23,23,23,23,23,-26,23,23,23,23,23,23,]),'WORD_WITH_DOT':([0,2,3,12,14,15,17,18,19,20,22,23,24,25,26,27,29,30,31,32,33,34,35,36,37,38,41,45,46,47,48,49,56,60,64,69,71,72,73,76,77,78,86,93,102,105,107,109,112,114,],[24,24,24,24,24,24,-75,24,24,24,-65,-66,-67,-68,-69,-70,24,24,-71,-72,-73,-74,-76,-77,-78,-79,24,24,24,24,24,24,-75,24,24,24,24,24,24,24,24,24,24,-26,24,24,24,24,24,24,]),'SHELL':([0,2,3,12,14,15,18,19,29,30,45,47,49,60,71,72,73,86,102,105,107,109,112,114,],[29,29,29,29,29,29,29,29,29,29,29,29,29,29,29,29,29,29,29,29,29,29,29,29,]),'MATH':([0,2,3,12,14,15,18,19,29,30,45,47,49,60,71,72,73,86,102,105,107,109,112,114,],[30,30,30,30,30,30,30,30,30,30,30,30,30,30,30,30,30,30,30,30,30,30,30,30,]),'WILDCARD':([0,2,3,12,14,15,17,18,19,20,22,23,24,25,26,27,29,30,31,32,33,34,35,36,37,38,41,45,46,47,48,49,56,60,64,69,71,72,73,76,77,78,86,93,102,105,107,109,112,114,],[31,31,31,31,31,31,-75,31,31,31,-65,-66,-67,-68,-69,-70,31,31,-71,-72,-73,-74,-76,-77,-78,-79,31,31,31,31,31,31,-75,31,31,31,31,31,31,31,31,31,31,-26,31,31,31,31,31,31,]),'WILDCARD_RANGE':([0,2,3,12,14,15,17,18,19,20,22,23,24,25,26,27,29,30,31,32,33,34,35,36,37,38,41,45,46,47,48,49,56,60,64,69,71,72,73,76,77,78,86,93,102,105,107,109,112,114,],[32,32,32,32,32,32,-75,32,32,32,-65,-66,-67,-68,-69,-70,32,32,-71,-72,-73,-74,-76,-77,-78,-79,32,32,32,32,32,32,-75,32,32,32,32,32,32,32,32,32,32,-26,32,32,32,32,32,32,]),'NUMBER':([0,2,3,12,14,15,17,18,19,20,22,23,24,25,26,27,29,30,31,32,33,34,35,36,37,38,41,45,46,47,48,49,56,60,64,69,71,72,73,76,77,78,86,93,102,105,107,109,112,114,],[33,33,33,33,33,33,-75,33,33,33,-65,-66,-67,-68,-69,-70,33,33,-71,-72,-73,-74,-76,-77,-78,-79,33,33,33,33,33,33,-75,33,33,33,33,33,33,33,33,33,33,-26,33,33,33,33,33,33,]),'NUMBER_WITH_DOT':([0,2,3,12,14,15,17,18,19,20,22,23,24,25,26,27,29,30,31,32,33,34,35,36,37,38,41,45,46,47,48,49,56,60,64,69,71,72,73,76,77,78,86,93,102,105,107,109,112,114,],[34,34,34,34,34,34,-75,34,34,34,-65,-66,-67,-68,-69,-70,34,34,-71,-72,-73,-74,-76,-77,-78,-79,34,34,34,34,34,34,-75,34,34,34,34,34,34,34,34,34,34,-26,34,34,34,34,34,34,]),'VARIABLE':([0,2,3,12,14,15,17,18,19,20,22,23,24,25,26,27,29,30,31,32,33,34,35,36,37,38,41,45,46,47,48,49,56,60,64,69,71,72,73,76,77,78,86,93,102,105,107,109,112,114,],[35,35,35,35,35,35,-75,35,35,35,-65,-66,-67,-68,-69,-70,35,35,-71,-72,-73,-74,-76,-77,-78,-79,35,35,35,35,35,35,-75,35,35,35,35,35,35,35,35,35,35,-26,35,35,35,35,35,35,]),'SYMBOL':([0,2,3,12,14,15,17,18,19,20,22,23,24,25,26,27,29,30,31,32,33,34,35,36,37,38,41,45,46,47,48,49,56,60,64,69,71,72,73,76,77,78,86,93,102,105,107,109,112,114,],[36,36,36,36,36,36,-75,36,36,36,-65,-66,-67,-68,-69,-70,36,36,-71,-72,-73,-74,-76,-77,-78,-79,36,36,36,36,36,36,-75,36,36,36,36,36,36,36,36,36,36,-26,36,36,36,36,36,36,]),'SINGLE_QUOTED_STRING':([0,2,3,12,14,15,17,18,19,20,22,23,24,25,26,27,29,30,31,32,33,34,35,36,37,38,41,45,46,47,48,49,56,60,64,69,71,72,73,76,77,78,86,93,102,105,107,109,112,114,],[37,37,37,37,37,37,-75,37,37,37,-65,-66,-67,-68,-69,-70,37,37,-71,-72,-73,-74,-76,-77,-78,-79,37,37,37,37,37,37,-75,37,37,37,37,37,37,37,37,37,37,-26,37,37,37,37,37,37,]),'DOUBLE_QUOTED_STRING':([0,2,3,12,14,15,17,18,19,20,22,23,24,25,26,27,29,30,31,32,33,34,35,36,37,38,41,45,46,47,48,49,56,60,64,69,71,72,73,76,77,78,86,93,102,105,107,109,112,114,],[38,38,38,38,38,38,-75,38,38,38,-65,-66,-67,-68,-69,-70,38,38,-71,-72,-73,-74,-76,-77,-78,-79,38,38,38,38,38,38,-75,38,38,38,38,38,38,38,38,38,38,-26,38,38,38,38,38,38,]),'LPAREN':([0,2,3,12,14,15,17,18,19,20,22,23,24,25,26,27,29,30,31,32,33,34,35,36,37,38,41,45,46,47,48,49,56,60,64,69,71,72,73,76,77,78,86,93,102,105,107,109,112,114,],[18,18,18,18,18,18,64,18,18,18,-65,-66,-67,-68,-69,-70,18,18,-71,-72,-73,-74,-76,-77,-78,-79,18,18,18,18,18,18,-75,18,18,18,18,18,18,18,18,18,18,-26,18,18,18,18,18,18,]),'NOT':([0,2,3,12,14,15,18,19,29,30,45,47,48,49,60,71,72,73,76,77,78,86,102,105,107,109,112,114,],[41,41,41,41,41,41,41,41,41,41,41,41,41,41,41,41,41,41,41,41,41,41,41,41,41,41,41,41,]),'$end':([1,2,3,4,5,6,7,8,9,10,11,13,14,15,16,17,20,21,22,23,24,25,26,27,28,29,31,32,33,34,35,36,37,38,39,40,42,43,44,45,50,51,52,54,55,56,57,58,59,61,62,66,67,68,69,70,74,75,79,80,81,82,83,84,86,87,88,89,90,93,94,95,96,97,98,99,100,101,103,104,105,107,108,109,110,111,112,113,115,116,],[0,-1,-9,-3,-8,-10,-11,-12,-13,-14,-53,-16,-34,-39,-17,-75,-64,-43,-65,-66,-67,-68,-69,-70,-47,-49,-71,-72,-73,-74,-76,-77,-78,-79,-51,-52,-6,-2,-7,-4,-27,-80,-82,-46,-53,-75,-33,-18,-19,-84,-38,-16,-17,-15,-62,-63,-48,-50,-60,-5,-21,-20,-61,-58,-31,-81,-83,-37,-85,-26,-42,-44,-45,-55,-54,-57,-56,-59,-29,-32,-36,-25,-29,-30,-18,-35,-24,-23,-28,-22,]),'ASSIGN_RIGHT':([9,11,13,16,17,20,21,22,23,24,25,26,27,28,29,31,32,33,34,35,36,37,38,39,40,54,55,56,69,70,74,75,79,83,84,93,94,95,96,97,98,99,100,101,103,108,115,],[46,-53,-16,-17,-75,-64,-43,-65,-66,-67,-68,-69,-70,-47,-49,-71,-72,-73,-74,-76,-77,-78,-79,-51,-52,-46,-53,-75,-62,-63,-48,-50,-60,-61,-58,-26,-42,-44,-45,-55,-54,-57,-56,-59,-29,-29,-28,]),'ASSIGN':([11,17,20,22,23,24,25,26,27,31,32,33,34,35,36,37,38,56,69,70,93,],[47,-75,-64,-65,-66,-67,-68,-69,-70,-71,-72,-73,-74,-76,-77,-78,-79,-75,-62,-63,-26,]),'PIPE':([11,16,17,20,21,22,23,24,25,26,27,28,29,31,32,33,34,35,36,37,38,39,40,54,55,56,67,69,70,74,75,79,83,84,93,94,95,96,97,98,99,100,101,103,108,110,115,],[-53,-46,-75,-64,71,-65,-66,-67,-68,-69,-70,-47,-49,-71,-72,-73,-74,-76,-77,-78,-79,-51,-52,-46,-53,-75,-46,-62,-63,-48,-50,-60,-61,-58,-26,-42,-44,-45,-55,-54,-57,-56,-59,-29,-29,-29,-28,]),'BASH':([11,16,17,20,21,22,23,24,25,26,27,28,29,31,32,33,34,35,36,37,38,39,40,54,55,56,67,69,70,74,75,79,83,84,93,94,95,96,97,98,99,100,101,103,108,110,115,],[-53,-46,-75,-64,72,-65,-66,-67,-68,-69,-70,-47,-49,-71,-72,-73,-74,-76,-77,-78,-79,-51,-52,-46,-53,-75,-46,-62,-63,72,-50,-60,-61,-58,-26,-42,-44,72,-55,-54,-57,-56,-59,-29,-29,-29,-28,]),'MAP':([11,16,17,20,21,22,23,24,25,26,27,28,29,31,32,33,34,35,36,37,38,39,40,54,55,56,67,69,70,74,75,79,83,84,93,94,95,96,97,98,99,100,101,103,108,110,115,],[-53,-46,-75,-64,73,-65,-66,-67,-68,-69,-70,-47,-49,-71,-72,-73,-74,-76,-77,-78,-79,-51,-52,-46,-53,-75,-46,-62,-63,73,-50,-60,-61,-58,-26,-42,-44,73,-55,-54,-57,-56,-59,-29,-29,-29,-28,]),'INFIX_OPERATOR':([11,17,20,22,23,24,25,26,27,31,32,33,34,35,36,37,38,55,56,69,70,83,93,],[48,-75,-64,-65,-66,-67,-68,-69,-70,-71,-72,-73,-74,-76,-77,-78,-79,48,-75,-62,-63,48,-26,]),'AND':([11,17,20,22,23,24,25,26,27,31,32,33,34,35,36,37,38,40,55,56,69,70,79,83,84,93,97,99,101,],[-61,-75,-64,-65,-66,-67,-68,-69,-70,-71,-72,-73,-74,-76,-77,-78,-79,76,-61,-75,-62,-63,-60,-61,-58,-26,76,76,-59,]),'OR':([11,17,20,22,23,24,25,26,27,31,32,33,34,35,36,37,38,40,55,56,69,70,79,83,84,93,97,99,101,],[-61,-75,-64,-65,-66,-67,-68,-69,-70,-71,-72,-73,-74,-76,-77,-78,-79,77,-61,-75,-62,-63,-60,-61,-58,-26,77,77,-59,]),'EQUALS':([11,17,20,22,23,24,25,26,27,31,32,33,34,35,36,37,38,40,55,56,69,70,79,83,84,93,97,99,101,],[-61,-75,-64,-65,-66,-67,-68,-69,-70,-71,-72,-73,-74,-76,-77,-78,-79,78,-61,-75,-62,-63,-60,-61,78,-26,78,78,-59,]),'RPAREN':([20,21,22,23,24,25,26,27,28,29,31,32,33,34,35,36,37,38,39,40,54,55,56,64,65,66,67,69,70,74,75,79,83,84,91,93,94,95,96,97,98,99,100,101,108,115,],[-64,-43,-65,-66,-67,-68,-69,-70,-47,-49,-71,-72,-73,-74,-76,-77,-78,-79,-51,-52,-46,-53,-75,92,93,-16,-17,-62,-63,-48,-50,-60,-61,-58,106,-26,-42,-44,-45,-55,-54,-57,-56,-59,-29,-28,]),'DEFINE_FUNCTION':([92,106,],[107,112,]),}
+_lr_action_items = {'BREAK':([0,2,3,4,5,6,7,8,9,10,11,13,14,15,16,17,20,21,22,23,24,25,26,27,28,29,31,32,33,34,35,36,37,38,39,40,41,45,46,51,52,53,55,56,57,58,59,60,62,63,67,68,69,70,71,75,76,80,82,83,84,85,87,88,89,90,91,94,95,96,97,98,99,100,101,102,104,105,106,108,109,110,111,112,113,114,116,117,],[2,2,-9,46,-8,-10,-11,-12,-13,-14,-53,-16,-34,-39,-17,-75,-64,-43,-65,-66,-67,-68,-69,-70,-47,-49,-71,-72,-73,-74,-76,-77,-78,-79,-80,-51,-52,-7,2,-27,-81,-83,-46,-53,-75,-33,-18,-19,-85,-38,-16,-17,-15,-62,-63,-48,-50,-60,-21,-20,-61,-58,-31,-82,-84,-37,-86,-26,-42,-44,-45,-55,-54,-57,-56,-59,-29,-32,-36,-25,-29,-30,-18,-35,-24,-23,-28,-22,]),'INDENT':([0,2,12,15,46,],[3,3,54,64,3,]),'IF':([0,2,3,12,14,15,18,19,29,30,46,48,50,61,72,73,74,87,103,106,108,110,113,115,],[12,12,12,50,50,61,50,50,50,50,12,50,50,50,50,50,50,50,50,50,50,50,50,50,]),'THEN':([0,2,3,12,15,20,21,22,23,24,25,26,27,28,29,31,32,33,34,35,36,37,38,39,40,41,46,51,54,55,56,57,64,70,71,75,76,80,84,85,86,90,94,95,96,97,98,99,100,101,102,109,116,],[14,14,14,52,62,-64,-43,-65,-66,-67,-68,-69,-70,-47,-49,-71,-72,-73,-74,-76,-77,-78,-79,-80,-51,-52,14,87,88,-46,-53,-75,91,-62,-63,-48,-50,-60,-61,-58,103,106,-26,-42,-44,-45,-55,-54,-57,-56,-59,-29,-28,]),'ELSE':([0,2,3,12,20,21,22,23,24,25,26,27,28,29,31,32,33,34,35,36,37,38,39,40,41,46,54,55,56,57,70,71,75,76,80,84,85,94,95,96,97,98,99,100,101,102,104,109,111,116,],[15,15,15,53,-64,-43,-65,-66,-67,-68,-69,-70,-47,-49,-71,-72,-73,-74,-76,-77,-78,-79,-80,-51,-52,15,89,-46,-53,-75,-62,-63,-48,-50,-60,-61,-58,-26,-42,-44,-45,-55,-54,-57,-56,-59,110,115,115,-28,]),'METHOD':([0,2,3,12,14,15,17,18,19,20,22,23,24,25,26,27,29,30,31,32,33,34,35,36,37,38,39,42,46,47,48,49,50,57,61,65,70,72,73,74,77,78,79,87,94,103,106,108,110,113,115,],[17,17,17,57,57,57,-75,57,57,57,-65,-66,-67,-68,-69,-70,57,57,-71,-72,-73,-74,-76,-77,-78,-79,-80,57,17,57,57,57,57,-75,57,57,57,57,57,57,57,57,57,57,-26,57,57,57,57,57,57,]),'RETURN':([0,2,3,14,15,46,87,106,],[19,19,19,19,19,19,19,19,]),'SPECIAL':([0,2,3,12,14,15,17,18,19,20,22,23,24,25,26,27,29,30,31,32,33,34,35,36,37,38,39,42,46,47,48,49,50,57,61,65,70,72,73,74,77,78,79,87,94,103,106,108,110,113,115,],[22,22,22,22,22,22,-75,22,22,22,-65,-66,-67,-68,-69,-70,22,22,-71,-72,-73,-74,-76,-77,-78,-79,-80,22,22,22,22,22,22,-75,22,22,22,22,22,22,22,22,22,22,-26,22,22,22,22,22,22,]),'WORD':([0,2,3,12,14,15,17,18,19,20,22,23,24,25,26,27,29,30,31,32,33,34,35,36,37,38,39,42,46,47,48,49,50,57,61,65,70,72,73,74,77,78,79,87,94,103,106,108,110,113,115,],[23,23,23,23,23,23,-75,23,23,23,-65,-66,-67,-68,-69,-70,23,23,-71,-72,-73,-74,-76,-77,-78,-79,-80,23,23,23,23,23,23,-75,23,23,23,23,23,23,23,23,23,23,-26,23,23,23,23,23,23,]),'WORD_WITH_DOT':([0,2,3,12,14,15,17,18,19,20,22,23,24,25,26,27,29,30,31,32,33,34,35,36,37,38,39,42,46,47,48,49,50,57,61,65,70,72,73,74,77,78,79,87,94,103,106,108,110,113,115,],[24,24,24,24,24,24,-75,24,24,24,-65,-66,-67,-68,-69,-70,24,24,-71,-72,-73,-74,-76,-77,-78,-79,-80,24,24,24,24,24,24,-75,24,24,24,24,24,24,24,24,24,24,-26,24,24,24,24,24,24,]),'SHELL':([0,2,3,12,14,15,18,19,29,30,46,48,50,61,72,73,74,87,103,106,108,110,113,115,],[29,29,29,29,29,29,29,29,29,29,29,29,29,29,29,29,29,29,29,29,29,29,29,29,]),'MATH':([0,2,3,12,14,15,18,19,29,30,46,48,50,61,72,73,74,87,103,106,108,110,113,115,],[30,30,30,30,30,30,30,30,30,30,30,30,30,30,30,30,30,30,30,30,30,30,30,30,]),'WILDCARD':([0,2,3,12,14,15,17,18,19,20,22,23,24,25,26,27,29,30,31,32,33,34,35,36,37,38,39,42,46,47,48,49,50,57,61,65,70,72,73,74,77,78,79,87,94,103,106,108,110,113,115,],[31,31,31,31,31,31,-75,31,31,31,-65,-66,-67,-68,-69,-70,31,31,-71,-72,-73,-74,-76,-77,-78,-79,-80,31,31,31,31,31,31,-75,31,31,31,31,31,31,31,31,31,31,-26,31,31,31,31,31,31,]),'WILDCARD_RANGE':([0,2,3,12,14,15,17,18,19,20,22,23,24,25,26,27,29,30,31,32,33,34,35,36,37,38,39,42,46,47,48,49,50,57,61,65,70,72,73,74,77,78,79,87,94,103,106,108,110,113,115,],[32,32,32,32,32,32,-75,32,32,32,-65,-66,-67,-68,-69,-70,32,32,-71,-72,-73,-74,-76,-77,-78,-79,-80,32,32,32,32,32,32,-75,32,32,32,32,32,32,32,32,32,32,-26,32,32,32,32,32,32,]),'NUMBER':([0,2,3,12,14,15,17,18,19,20,22,23,24,25,26,27,29,30,31,32,33,34,35,36,37,38,39,42,46,47,48,49,50,57,61,65,70,72,73,74,77,78,79,87,94,103,106,108,110,113,115,],[33,33,33,33,33,33,-75,33,33,33,-65,-66,-67,-68,-69,-70,33,33,-71,-72,-73,-74,-76,-77,-78,-79,-80,33,33,33,33,33,33,-75,33,33,33,33,33,33,33,33,33,33,-26,33,33,33,33,33,33,]),'NUMBER_WITH_DOT':([0,2,3,12,14,15,17,18,19,20,22,23,24,25,26,27,29,30,31,32,33,34,35,36,37,38,39,42,46,47,48,49,50,57,61,65,70,72,73,74,77,78,79,87,94,103,106,108,110,113,115,],[34,34,34,34,34,34,-75,34,34,34,-65,-66,-67,-68,-69,-70,34,34,-71,-72,-73,-74,-76,-77,-78,-79,-80,34,34,34,34,34,34,-75,34,34,34,34,34,34,34,34,34,34,-26,34,34,34,34,34,34,]),'VARIABLE':([0,2,3,12,14,15,17,18,19,20,22,23,24,25,26,27,29,30,31,32,33,34,35,36,37,38,39,42,46,47,48,49,50,57,61,65,70,72,73,74,77,78,79,87,94,103,106,108,110,113,115,],[35,35,35,35,35,35,-75,35,35,35,-65,-66,-67,-68,-69,-70,35,35,-71,-72,-73,-74,-76,-77,-78,-79,-80,35,35,35,35,35,35,-75,35,35,35,35,35,35,35,35,35,35,-26,35,35,35,35,35,35,]),'SYMBOL':([0,2,3,12,14,15,17,18,19,20,22,23,24,25,26,27,29,30,31,32,33,34,35,36,37,38,39,42,46,47,48,49,50,57,61,65,70,72,73,74,77,78,79,87,94,103,106,108,110,113,115,],[36,36,36,36,36,36,-75,36,36,36,-65,-66,-67,-68,-69,-70,36,36,-71,-72,-73,-74,-76,-77,-78,-79,-80,36,36,36,36,36,36,-75,36,36,36,36,36,36,36,36,36,36,-26,36,36,36,36,36,36,]),'LONG_SYMBOL':([0,2,3,12,14,15,17,18,19,20,22,23,24,25,26,27,29,30,31,32,33,34,35,36,37,38,39,42,46,47,48,49,50,57,61,65,70,72,73,74,77,78,79,87,94,103,106,108,110,113,115,],[37,37,37,37,37,37,-75,37,37,37,-65,-66,-67,-68,-69,-70,37,37,-71,-72,-73,-74,-76,-77,-78,-79,-80,37,37,37,37,37,37,-75,37,37,37,37,37,37,37,37,37,37,-26,37,37,37,37,37,37,]),'SINGLE_QUOTED_STRING':([0,2,3,12,14,15,17,18,19,20,22,23,24,25,26,27,29,30,31,32,33,34,35,36,37,38,39,42,46,47,48,49,50,57,61,65,70,72,73,74,77,78,79,87,94,103,106,108,110,113,115,],[38,38,38,38,38,38,-75,38,38,38,-65,-66,-67,-68,-69,-70,38,38,-71,-72,-73,-74,-76,-77,-78,-79,-80,38,38,38,38,38,38,-75,38,38,38,38,38,38,38,38,38,38,-26,38,38,38,38,38,38,]),'DOUBLE_QUOTED_STRING':([0,2,3,12,14,15,17,18,19,20,22,23,24,25,26,27,29,30,31,32,33,34,35,36,37,38,39,42,46,47,48,49,50,57,61,65,70,72,73,74,77,78,79,87,94,103,106,108,110,113,115,],[39,39,39,39,39,39,-75,39,39,39,-65,-66,-67,-68,-69,-70,39,39,-71,-72,-73,-74,-76,-77,-78,-79,-80,39,39,39,39,39,39,-75,39,39,39,39,39,39,39,39,39,39,-26,39,39,39,39,39,39,]),'LPAREN':([0,2,3,12,14,15,17,18,19,20,22,23,24,25,26,27,29,30,31,32,33,34,35,36,37,38,39,42,46,47,48,49,50,57,61,65,70,72,73,74,77,78,79,87,94,103,106,108,110,113,115,],[18,18,18,18,18,18,65,18,18,18,-65,-66,-67,-68,-69,-70,18,18,-71,-72,-73,-74,-76,-77,-78,-79,-80,18,18,18,18,18,18,-75,18,18,18,18,18,18,18,18,18,18,-26,18,18,18,18,18,18,]),'NOT':([0,2,3,12,14,15,18,19,29,30,46,48,49,50,61,72,73,74,77,78,79,87,103,106,108,110,113,115,],[42,42,42,42,42,42,42,42,42,42,42,42,42,42,42,42,42,42,42,42,42,42,42,42,42,42,42,42,]),'$end':([1,2,3,4,5,6,7,8,9,10,11,13,14,15,16,17,20,21,22,23,24,25,26,27,28,29,31,32,33,34,35,36,37,38,39,40,41,43,44,45,46,51,52,53,55,56,57,58,59,60,62,63,67,68,69,70,71,75,76,80,81,82,83,84,85,87,88,89,90,91,94,95,96,97,98,99,100,101,102,104,105,106,108,109,110,111,112,113,114,116,117,],[0,-1,-9,-3,-8,-10,-11,-12,-13,-14,-53,-16,-34,-39,-17,-75,-64,-43,-65,-66,-67,-68,-69,-70,-47,-49,-71,-72,-73,-74,-76,-77,-78,-79,-80,-51,-52,-6,-2,-7,-4,-27,-81,-83,-46,-53,-75,-33,-18,-19,-85,-38,-16,-17,-15,-62,-63,-48,-50,-60,-5,-21,-20,-61,-58,-31,-82,-84,-37,-86,-26,-42,-44,-45,-55,-54,-57,-56,-59,-29,-32,-36,-25,-29,-30,-18,-35,-24,-23,-28,-22,]),'ASSIGN_RIGHT':([9,11,13,16,17,20,21,22,23,24,25,26,27,28,29,31,32,33,34,35,36,37,38,39,40,41,55,56,57,70,71,75,76,80,84,85,94,95,96,97,98,99,100,101,102,104,109,116,],[47,-53,-16,-17,-75,-64,-43,-65,-66,-67,-68,-69,-70,-47,-49,-71,-72,-73,-74,-76,-77,-78,-79,-80,-51,-52,-46,-53,-75,-62,-63,-48,-50,-60,-61,-58,-26,-42,-44,-45,-55,-54,-57,-56,-59,-29,-29,-28,]),'ASSIGN':([11,17,20,22,23,24,25,26,27,31,32,33,34,35,36,37,38,39,57,70,71,94,],[48,-75,-64,-65,-66,-67,-68,-69,-70,-71,-72,-73,-74,-76,-77,-78,-79,-80,-75,-62,-63,-26,]),'PIPE':([11,16,17,20,21,22,23,24,25,26,27,28,29,31,32,33,34,35,36,37,38,39,40,41,55,56,57,68,70,71,75,76,80,84,85,94,95,96,97,98,99,100,101,102,104,109,111,116,],[-53,-46,-75,-64,72,-65,-66,-67,-68,-69,-70,-47,-49,-71,-72,-73,-74,-76,-77,-78,-79,-80,-51,-52,-46,-53,-75,-46,-62,-63,-48,-50,-60,-61,-58,-26,-42,-44,-45,-55,-54,-57,-56,-59,-29,-29,-29,-28,]),'BASH':([11,16,17,20,21,22,23,24,25,26,27,28,29,31,32,33,34,35,36,37,38,39,40,41,55,56,57,68,70,71,75,76,80,84,85,94,95,96,97,98,99,100,101,102,104,109,111,116,],[-53,-46,-75,-64,73,-65,-66,-67,-68,-69,-70,-47,-49,-71,-72,-73,-74,-76,-77,-78,-79,-80,-51,-52,-46,-53,-75,-46,-62,-63,73,-50,-60,-61,-58,-26,-42,-44,73,-55,-54,-57,-56,-59,-29,-29,-29,-28,]),'MAP':([11,16,17,20,21,22,23,24,25,26,27,28,29,31,32,33,34,35,36,37,38,39,40,41,55,56,57,68,70,71,75,76,80,84,85,94,95,96,97,98,99,100,101,102,104,109,111,116,],[-53,-46,-75,-64,74,-65,-66,-67,-68,-69,-70,-47,-49,-71,-72,-73,-74,-76,-77,-78,-79,-80,-51,-52,-46,-53,-75,-46,-62,-63,74,-50,-60,-61,-58,-26,-42,-44,74,-55,-54,-57,-56,-59,-29,-29,-29,-28,]),'INFIX_OPERATOR':([11,17,20,22,23,24,25,26,27,31,32,33,34,35,36,37,38,39,56,57,70,71,84,94,],[49,-75,-64,-65,-66,-67,-68,-69,-70,-71,-72,-73,-74,-76,-77,-78,-79,-80,49,-75,-62,-63,49,-26,]),'AND':([11,17,20,22,23,24,25,26,27,31,32,33,34,35,36,37,38,39,41,56,57,70,71,80,84,85,94,98,100,102,],[-61,-75,-64,-65,-66,-67,-68,-69,-70,-71,-72,-73,-74,-76,-77,-78,-79,-80,77,-61,-75,-62,-63,-60,-61,-58,-26,77,77,-59,]),'OR':([11,17,20,22,23,24,25,26,27,31,32,33,34,35,36,37,38,39,41,56,57,70,71,80,84,85,94,98,100,102,],[-61,-75,-64,-65,-66,-67,-68,-69,-70,-71,-72,-73,-74,-76,-77,-78,-79,-80,78,-61,-75,-62,-63,-60,-61,-58,-26,78,78,-59,]),'EQUALS':([11,17,20,22,23,24,25,26,27,31,32,33,34,35,36,37,38,39,41,56,57,70,71,80,84,85,94,98,100,102,],[-61,-75,-64,-65,-66,-67,-68,-69,-70,-71,-72,-73,-74,-76,-77,-78,-79,-80,79,-61,-75,-62,-63,-60,-61,79,-26,79,79,-59,]),'RPAREN':([20,21,22,23,24,25,26,27,28,29,31,32,33,34,35,36,37,38,39,40,41,55,56,57,65,66,67,68,70,71,75,76,80,84,85,92,94,95,96,97,98,99,100,101,102,109,116,],[-64,-43,-65,-66,-67,-68,-69,-70,-47,-49,-71,-72,-73,-74,-76,-77,-78,-79,-80,-51,-52,-46,-53,-75,93,94,-16,-17,-62,-63,-48,-50,-60,-61,-58,107,-26,-42,-44,-45,-55,-54,-57,-56,-59,-29,-28,]),'DEFINE_FUNCTION':([93,107,],[108,113,]),}
 
 _lr_action = {}
 for _k, _v in _lr_action_items.items():
    for _x,_y in zip(_v[0],_v[1]):
       if not _x in _lr_action:  _lr_action[_x] = {}
       _lr_action[_x][_k] = _y
 del _lr_action_items
 
-_lr_goto_items = {'lines':([0,2,45,],[1,42,80,]),'line':([0,2,45,],[4,4,4,]),'statement':([0,2,3,45,],[5,5,44,5,]),'assignment':([0,2,3,45,],[6,6,6,6,]),'conditional':([0,2,3,45,],[7,7,7,7,]),'definition':([0,2,3,45,],[8,8,8,8,]),'inner_statement':([0,2,3,18,19,45,47,107,112,],[9,9,9,65,68,9,82,113,116,]),'return_statement':([0,2,3,14,15,45,86,105,],[10,10,10,59,59,10,104,59,]),'terms':([0,2,3,12,14,15,18,19,20,29,30,41,45,46,47,48,49,60,64,69,71,72,73,76,77,78,86,102,105,107,109,112,114,],[11,11,11,55,55,55,55,55,70,55,55,79,11,81,55,83,55,55,91,70,55,55,55,83,83,83,55,55,55,55,55,55,55,]),'conjunction':([0,2,3,12,14,15,18,19,45,47,49,60,71,86,102,105,107,109,112,114,],[13,13,13,50,58,58,66,66,13,66,85,89,94,103,108,110,66,115,66,115,]),'full_conditional':([0,2,3,12,14,15,18,19,29,30,45,47,49,60,71,72,73,86,102,105,107,109,112,114,],[16,16,16,54,54,54,67,67,54,54,16,67,54,54,54,54,54,54,54,54,67,54,67,54,]),'term':([0,2,3,12,14,15,18,19,20,29,30,41,45,46,47,48,49,60,64,69,71,72,73,76,77,78,86,102,105,107,109,112,114,],[20,20,20,20,20,20,20,20,69,20,20,20,20,20,20,20,20,20,20,69,20,20,20,20,20,20,20,20,20,20,20,20,20,]),'expression':([0,2,3,12,14,15,18,19,29,30,45,47,49,60,71,72,73,86,102,105,107,109,112,114,],[21,21,21,21,21,21,21,21,74,75,21,21,21,21,21,95,96,21,21,21,21,21,21,21,]),'value':([0,2,3,12,14,15,18,19,20,29,30,41,45,46,47,48,49,60,64,69,71,72,73,76,77,78,86,102,105,107,109,112,114,],[25,25,25,25,25,25,25,25,25,25,25,25,25,25,25,25,25,25,25,25,25,25,25,25,25,25,25,25,25,25,25,25,25,]),'method':([0,2,3,12,14,15,18,19,20,29,30,41,45,46,47,48,49,60,64,69,71,72,73,76,77,78,86,102,105,107,109,112,114,],[26,26,26,26,26,26,26,26,26,26,26,26,26,26,26,26,26,26,26,26,26,26,26,26,26,26,26,26,26,26,26,26,26,]),'scope':([0,2,3,12,14,15,18,19,20,29,30,41,45,46,47,48,49,60,64,69,71,72,73,76,77,78,86,102,105,107,109,112,114,],[27,27,27,27,27,27,27,27,27,27,27,27,27,27,27,27,27,27,27,27,27,27,27,27,27,27,27,27,27,27,27,27,27,]),'basic_expression':([0,2,3,12,14,15,18,19,29,30,45,47,49,60,71,72,73,86,102,105,107,109,112,114,],[28,28,28,28,28,28,28,28,28,28,28,28,28,28,28,28,28,28,28,28,28,28,28,28,]),'join':([0,2,3,12,14,15,18,19,29,30,45,47,49,60,71,72,73,76,77,86,102,105,107,109,112,114,],[39,39,39,39,39,39,39,39,39,39,39,39,39,39,39,39,39,98,100,39,39,39,39,39,39,39,]),'logic_expression':([0,2,3,12,14,15,18,19,29,30,45,47,48,49,60,71,72,73,76,77,78,86,102,105,107,109,112,114,],[40,40,40,40,40,40,40,40,40,40,40,40,84,40,40,40,40,40,97,99,101,40,40,40,40,40,40,40,]),'final_statement':([14,15,105,],[57,62,111,]),}
+_lr_goto_items = {'lines':([0,2,46,],[1,43,81,]),'line':([0,2,46,],[4,4,4,]),'statement':([0,2,3,46,],[5,5,45,5,]),'assignment':([0,2,3,46,],[6,6,6,6,]),'conditional':([0,2,3,46,],[7,7,7,7,]),'definition':([0,2,3,46,],[8,8,8,8,]),'inner_statement':([0,2,3,18,19,46,48,108,113,],[9,9,9,66,69,9,83,114,117,]),'return_statement':([0,2,3,14,15,46,87,106,],[10,10,10,60,60,10,105,60,]),'terms':([0,2,3,12,14,15,18,19,20,29,30,42,46,47,48,49,50,61,65,70,72,73,74,77,78,79,87,103,106,108,110,113,115,],[11,11,11,56,56,56,56,56,71,56,56,80,11,82,56,84,56,56,92,71,56,56,56,84,84,84,56,56,56,56,56,56,56,]),'conjunction':([0,2,3,12,14,15,18,19,46,48,50,61,72,87,103,106,108,110,113,115,],[13,13,13,51,59,59,67,67,13,67,86,90,95,104,109,111,67,116,67,116,]),'full_conditional':([0,2,3,12,14,15,18,19,29,30,46,48,50,61,72,73,74,87,103,106,108,110,113,115,],[16,16,16,55,55,55,68,68,55,55,16,68,55,55,55,55,55,55,55,55,68,55,68,55,]),'term':([0,2,3,12,14,15,18,19,20,29,30,42,46,47,48,49,50,61,65,70,72,73,74,77,78,79,87,103,106,108,110,113,115,],[20,20,20,20,20,20,20,20,70,20,20,20,20,20,20,20,20,20,20,70,20,20,20,20,20,20,20,20,20,20,20,20,20,]),'expression':([0,2,3,12,14,15,18,19,29,30,46,48,50,61,72,73,74,87,103,106,108,110,113,115,],[21,21,21,21,21,21,21,21,75,76,21,21,21,21,21,96,97,21,21,21,21,21,21,21,]),'value':([0,2,3,12,14,15,18,19,20,29,30,42,46,47,48,49,50,61,65,70,72,73,74,77,78,79,87,103,106,108,110,113,115,],[25,25,25,25,25,25,25,25,25,25,25,25,25,25,25,25,25,25,25,25,25,25,25,25,25,25,25,25,25,25,25,25,25,]),'method':([0,2,3,12,14,15,18,19,20,29,30,42,46,47,48,49,50,61,65,70,72,73,74,77,78,79,87,103,106,108,110,113,115,],[26,26,26,26,26,26,26,26,26,26,26,26,26,26,26,26,26,26,26,26,26,26,26,26,26,26,26,26,26,26,26,26,26,]),'scope':([0,2,3,12,14,15,18,19,20,29,30,42,46,47,48,49,50,61,65,70,72,73,74,77,78,79,87,103,106,108,110,113,115,],[27,27,27,27,27,27,27,27,27,27,27,27,27,27,27,27,27,27,27,27,27,27,27,27,27,27,27,27,27,27,27,27,27,]),'basic_expression':([0,2,3,12,14,15,18,19,29,30,46,48,50,61,72,73,74,87,103,106,108,110,113,115,],[28,28,28,28,28,28,28,28,28,28,28,28,28,28,28,28,28,28,28,28,28,28,28,28,]),'join':([0,2,3,12,14,15,18,19,29,30,46,48,50,61,72,73,74,77,78,87,103,106,108,110,113,115,],[40,40,40,40,40,40,40,40,40,40,40,40,40,40,40,40,40,99,101,40,40,40,40,40,40,40,]),'logic_expression':([0,2,3,12,14,15,18,19,29,30,46,48,49,50,61,72,73,74,77,78,79,87,103,106,108,110,113,115,],[41,41,41,41,41,41,41,41,41,41,41,41,85,41,41,41,41,41,98,100,102,41,41,41,41,41,41,41,]),'final_statement':([14,15,106,],[58,63,112,]),}
 
 _lr_goto = {}
 for _k, _v in _lr_goto_items.items():
    for _x, _y in zip(_v[0], _v[1]):
        if not _x in _lr_goto: _lr_goto[_x] = {}
        _lr_goto[_x][_k] = _y
 del _lr_goto_items
 _lr_productions = [
   ("S' -> lines","S'",1,None,None,None),
-  ('lines -> BREAK','lines',1,'p_lines_empty','lex_parser.py',242),
-  ('lines -> INDENT BREAK','lines',2,'p_lines_empty','lex_parser.py',243),
-  ('lines -> line','lines',1,'p_lines_suffix','lex_parser.py',250),
-  ('lines -> line BREAK','lines',2,'p_lines_suffix','lex_parser.py',251),
-  ('lines -> line BREAK lines','lines',3,'p_lines_infix','lex_parser.py',256),
-  ('lines -> BREAK lines','lines',2,'p_lines_prefix','lex_parser.py',261),
-  ('line -> INDENT statement','line',2,'p_line_indented','lex_parser.py',265),
-  ('line -> statement','line',1,'p_line','lex_parser.py',270),
-  ('line -> INDENT','line',1,'p_line_indent_empty','lex_parser.py',274),
-  ('statement -> assignment','statement',1,'p_statement','lex_parser.py',279),
-  ('statement -> conditional','statement',1,'p_statement','lex_parser.py',280),
-  ('statement -> definition','statement',1,'p_statement','lex_parser.py',281),
-  ('statement -> inner_statement','statement',1,'p_statement','lex_parser.py',282),
-  ('statement -> return_statement','statement',1,'p_statement','lex_parser.py',283),
-  ('return_statement -> RETURN inner_statement','return_statement',2,'p_statement_return','lex_parser.py',288),
-  ('inner_statement -> conjunction','inner_statement',1,'p_inner_statement','lex_parser.py',292),
-  ('inner_statement -> full_conditional','inner_statement',1,'p_inner_statement','lex_parser.py',293),
-  ('final_statement -> conjunction','final_statement',1,'p_final_statement','lex_parser.py',298),
-  ('final_statement -> return_statement','final_statement',1,'p_final_statement','lex_parser.py',299),
-  ('assignment -> terms ASSIGN inner_statement','assignment',3,'p_assign','lex_parser.py',304),
-  ('assignment -> inner_statement ASSIGN_RIGHT terms','assignment',3,'p_assign_right','lex_parser.py',308),
-  ('definition -> METHOD LPAREN terms RPAREN DEFINE_FUNCTION inner_statement','definition',6,'p_def_inline_function','lex_parser.py',312),
-  ('definition -> METHOD LPAREN RPAREN DEFINE_FUNCTION inner_statement','definition',5,'p_def_inline_function_constant','lex_parser.py',316),
-  ('definition -> METHOD LPAREN terms RPAREN DEFINE_FUNCTION','definition',5,'p_def_function','lex_parser.py',320),
-  ('definition -> METHOD LPAREN RPAREN DEFINE_FUNCTION','definition',4,'p_def_function_constant','lex_parser.py',324),
-  ('scope -> LPAREN inner_statement RPAREN','scope',3,'p_scope','lex_parser.py',328),
-  ('conditional -> IF conjunction','conditional',2,'p_if','lex_parser.py',333),
-  ('full_conditional -> IF conjunction THEN conjunction ELSE conjunction','full_conditional',6,'p_full_conditional','lex_parser.py',337),
-  ('full_conditional -> IF conjunction THEN conjunction','full_conditional',4,'p_if_then_inline','lex_parser.py',342),
-  ('conditional -> IF conjunction THEN conjunction ELSE','conditional',5,'p_if_then_else','lex_parser.py',347),
-  ('conditional -> IF conjunction THEN','conditional',3,'p_if_then','lex_parser.py',352),
-  ('conditional -> IF conjunction THEN return_statement','conditional',4,'p_if_then_inline_final','lex_parser.py',356),
-  ('conditional -> THEN final_statement','conditional',2,'p_then','lex_parser.py',361),
-  ('conditional -> THEN','conditional',1,'p_then','lex_parser.py',362),
-  ('conditional -> ELSE IF conjunction THEN final_statement','conditional',5,'p_else_if_then','lex_parser.py',370),
-  ('conditional -> ELSE IF conjunction THEN','conditional',4,'p_else_if_then','lex_parser.py',371),
-  ('conditional -> ELSE IF conjunction','conditional',3,'p_else_if','lex_parser.py',379),
-  ('conditional -> ELSE final_statement','conditional',2,'p_else','lex_parser.py',383),
-  ('conditional -> ELSE','conditional',1,'p_else','lex_parser.py',384),
-  ('conditional -> conjunction','conditional',1,'p_conditional','lex_parser.py',392),
-  ('conditional -> full_conditional','conditional',1,'p_conditional','lex_parser.py',393),
-  ('conjunction -> expression PIPE conjunction','conjunction',3,'p_pipe_py','lex_parser.py',398),
-  ('conjunction -> expression','conjunction',1,'p_conjunction','lex_parser.py',402),
-  ('expression -> expression BASH expression','expression',3,'p_pipe_bash','lex_parser.py',406),
-  ('expression -> expression MAP expression','expression',3,'p_pipe_map','lex_parser.py',410),
-  ('expression -> full_conditional','expression',1,'p_expression_full_conditional','lex_parser.py',414),
-  ('expression -> basic_expression','expression',1,'p_expression','lex_parser.py',418),
-  ('expression -> SHELL expression','expression',2,'p_shell','lex_parser.py',422),
-  ('expression -> SHELL','expression',1,'p_shell_empty','lex_parser.py',426),
-  ('expression -> MATH expression','expression',2,'p_math','lex_parser.py',430),
-  ('basic_expression -> join','basic_expression',1,'p_basic_expression','lex_parser.py',434),
-  ('basic_expression -> logic_expression','basic_expression',1,'p_basic_expression','lex_parser.py',435),
-  ('basic_expression -> terms','basic_expression',1,'p_basic_expression','lex_parser.py',436),
-  ('join -> logic_expression AND join','join',3,'p_logic_binary','lex_parser.py',441),
-  ('join -> logic_expression AND logic_expression','join',3,'p_logic_binary','lex_parser.py',442),
-  ('join -> logic_expression OR join','join',3,'p_logic_binary','lex_parser.py',443),
-  ('join -> logic_expression OR logic_expression','join',3,'p_logic_binary','lex_parser.py',444),
-  ('logic_expression -> terms INFIX_OPERATOR logic_expression','logic_expression',3,'p_logic_expression_infix','lex_parser.py',450),
-  ('logic_expression -> logic_expression EQUALS logic_expression','logic_expression',3,'p_logic_expression_infix_equals','lex_parser.py',454),
-  ('logic_expression -> NOT terms','logic_expression',2,'p_logic_negation','lex_parser.py',458),
-  ('logic_expression -> terms','logic_expression',1,'p_logic','lex_parser.py',462),
-  ('terms -> term term','terms',2,'p_terms_pair','lex_parser.py',466),
-  ('terms -> term terms','terms',2,'p_terms_head_tail','lex_parser.py',470),
-  ('terms -> term','terms',1,'p_terms_singleton','lex_parser.py',475),
-  ('term -> SPECIAL','term',1,'p_term','lex_parser.py',479),
-  ('term -> WORD','term',1,'p_term','lex_parser.py',480),
-  ('term -> WORD_WITH_DOT','term',1,'p_term','lex_parser.py',481),
-  ('term -> value','term',1,'p_term_value','lex_parser.py',486),
-  ('term -> method','term',1,'p_term_value','lex_parser.py',487),
-  ('term -> scope','term',1,'p_term_value','lex_parser.py',488),
-  ('value -> WILDCARD','value',1,'p_value_wildcard','lex_parser.py',493),
-  ('value -> WILDCARD_RANGE','value',1,'p_value_wildcard_range','lex_parser.py',497),
-  ('value -> NUMBER','value',1,'p_value_number_int','lex_parser.py',501),
-  ('value -> NUMBER_WITH_DOT','value',1,'p_value_number_float','lex_parser.py',505),
-  ('method -> METHOD','method',1,'p_value_method','lex_parser.py',509),
-  ('value -> VARIABLE','value',1,'p_value_variable','lex_parser.py',513),
-  ('value -> SYMBOL','value',1,'p_value_symbol','lex_parser.py',517),
-  ('value -> SINGLE_QUOTED_STRING','value',1,'p_value_literal_string','lex_parser.py',521),
-  ('value -> DOUBLE_QUOTED_STRING','value',1,'p_value_string','lex_parser.py',525),
-  ('conditional -> IF THEN','conditional',2,'p_illegal_if_then','lex_parser.py',529),
-  ('conditional -> IF INDENT THEN','conditional',3,'p_illegal_if_then','lex_parser.py',530),
-  ('conditional -> IF ELSE','conditional',2,'p_illegal_if_then','lex_parser.py',531),
-  ('conditional -> IF INDENT ELSE','conditional',3,'p_illegal_if_then','lex_parser.py',532),
-  ('conditional -> ELSE THEN','conditional',2,'p_illegal_if_then','lex_parser.py',533),
-  ('conditional -> ELSE INDENT THEN','conditional',3,'p_illegal_if_then','lex_parser.py',534),
+  ('lines -> BREAK','lines',1,'p_lines_empty','lex_parser.py',237),
+  ('lines -> INDENT BREAK','lines',2,'p_lines_empty','lex_parser.py',238),
+  ('lines -> line','lines',1,'p_lines_suffix','lex_parser.py',245),
+  ('lines -> line BREAK','lines',2,'p_lines_suffix','lex_parser.py',246),
+  ('lines -> line BREAK lines','lines',3,'p_lines_infix','lex_parser.py',251),
+  ('lines -> BREAK lines','lines',2,'p_lines_prefix','lex_parser.py',255),
+  ('line -> INDENT statement','line',2,'p_line_indented','lex_parser.py',259),
+  ('line -> statement','line',1,'p_line','lex_parser.py',264),
+  ('line -> INDENT','line',1,'p_line_indent_empty','lex_parser.py',268),
+  ('statement -> assignment','statement',1,'p_statement','lex_parser.py',273),
+  ('statement -> conditional','statement',1,'p_statement','lex_parser.py',274),
+  ('statement -> definition','statement',1,'p_statement','lex_parser.py',275),
+  ('statement -> inner_statement','statement',1,'p_statement','lex_parser.py',276),
+  ('statement -> return_statement','statement',1,'p_statement','lex_parser.py',277),
+  ('return_statement -> RETURN inner_statement','return_statement',2,'p_statement_return','lex_parser.py',282),
+  ('inner_statement -> conjunction','inner_statement',1,'p_inner_statement','lex_parser.py',286),
+  ('inner_statement -> full_conditional','inner_statement',1,'p_inner_statement','lex_parser.py',287),
+  ('final_statement -> conjunction','final_statement',1,'p_final_statement','lex_parser.py',292),
+  ('final_statement -> return_statement','final_statement',1,'p_final_statement','lex_parser.py',293),
+  ('assignment -> terms ASSIGN inner_statement','assignment',3,'p_assign','lex_parser.py',298),
+  ('assignment -> inner_statement ASSIGN_RIGHT terms','assignment',3,'p_assign_right','lex_parser.py',302),
+  ('definition -> METHOD LPAREN terms RPAREN DEFINE_FUNCTION inner_statement','definition',6,'p_def_inline_function','lex_parser.py',306),
+  ('definition -> METHOD LPAREN RPAREN DEFINE_FUNCTION inner_statement','definition',5,'p_def_inline_function_constant','lex_parser.py',310),
+  ('definition -> METHOD LPAREN terms RPAREN DEFINE_FUNCTION','definition',5,'p_def_function','lex_parser.py',314),
+  ('definition -> METHOD LPAREN RPAREN DEFINE_FUNCTION','definition',4,'p_def_function_constant','lex_parser.py',318),
+  ('scope -> LPAREN inner_statement RPAREN','scope',3,'p_scope','lex_parser.py',322),
+  ('conditional -> IF conjunction','conditional',2,'p_if','lex_parser.py',327),
+  ('full_conditional -> IF conjunction THEN conjunction ELSE conjunction','full_conditional',6,'p_full_conditional','lex_parser.py',331),
+  ('full_conditional -> IF conjunction THEN conjunction','full_conditional',4,'p_if_then_inline','lex_parser.py',336),
+  ('conditional -> IF conjunction THEN conjunction ELSE','conditional',5,'p_if_then_else','lex_parser.py',341),
+  ('conditional -> IF conjunction THEN','conditional',3,'p_if_then','lex_parser.py',346),
+  ('conditional -> IF conjunction THEN return_statement','conditional',4,'p_if_then_inline_final','lex_parser.py',350),
+  ('conditional -> THEN final_statement','conditional',2,'p_then','lex_parser.py',355),
+  ('conditional -> THEN','conditional',1,'p_then','lex_parser.py',356),
+  ('conditional -> ELSE IF conjunction THEN final_statement','conditional',5,'p_else_if_then','lex_parser.py',364),
+  ('conditional -> ELSE IF conjunction THEN','conditional',4,'p_else_if_then','lex_parser.py',365),
+  ('conditional -> ELSE IF conjunction','conditional',3,'p_else_if','lex_parser.py',373),
+  ('conditional -> ELSE final_statement','conditional',2,'p_else','lex_parser.py',377),
+  ('conditional -> ELSE','conditional',1,'p_else','lex_parser.py',378),
+  ('conditional -> conjunction','conditional',1,'p_conditional','lex_parser.py',386),
+  ('conditional -> full_conditional','conditional',1,'p_conditional','lex_parser.py',387),
+  ('conjunction -> expression PIPE conjunction','conjunction',3,'p_pipe_py','lex_parser.py',392),
+  ('conjunction -> expression','conjunction',1,'p_conjunction','lex_parser.py',396),
+  ('expression -> expression BASH expression','expression',3,'p_pipe_bash','lex_parser.py',400),
+  ('expression -> expression MAP expression','expression',3,'p_pipe_map','lex_parser.py',404),
+  ('expression -> full_conditional','expression',1,'p_expression_full_conditional','lex_parser.py',408),
+  ('expression -> basic_expression','expression',1,'p_expression','lex_parser.py',412),
+  ('expression -> SHELL expression','expression',2,'p_shell','lex_parser.py',416),
+  ('expression -> SHELL','expression',1,'p_shell_empty','lex_parser.py',420),
+  ('expression -> MATH expression','expression',2,'p_math','lex_parser.py',424),
+  ('basic_expression -> join','basic_expression',1,'p_basic_expression','lex_parser.py',428),
+  ('basic_expression -> logic_expression','basic_expression',1,'p_basic_expression','lex_parser.py',429),
+  ('basic_expression -> terms','basic_expression',1,'p_basic_expression','lex_parser.py',430),
+  ('join -> logic_expression AND join','join',3,'p_logic_binary','lex_parser.py',435),
+  ('join -> logic_expression AND logic_expression','join',3,'p_logic_binary','lex_parser.py',436),
+  ('join -> logic_expression OR join','join',3,'p_logic_binary','lex_parser.py',437),
+  ('join -> logic_expression OR logic_expression','join',3,'p_logic_binary','lex_parser.py',438),
+  ('logic_expression -> terms INFIX_OPERATOR logic_expression','logic_expression',3,'p_logic_expression_infix','lex_parser.py',444),
+  ('logic_expression -> logic_expression EQUALS logic_expression','logic_expression',3,'p_logic_expression_infix_equals','lex_parser.py',448),
+  ('logic_expression -> NOT terms','logic_expression',2,'p_logic_negation','lex_parser.py',452),
+  ('logic_expression -> terms','logic_expression',1,'p_logic','lex_parser.py',457),
+  ('terms -> term term','terms',2,'p_terms_pair','lex_parser.py',461),
+  ('terms -> term terms','terms',2,'p_terms_head_tail','lex_parser.py',465),
+  ('terms -> term','terms',1,'p_terms_singleton','lex_parser.py',469),
+  ('term -> SPECIAL','term',1,'p_term','lex_parser.py',473),
+  ('term -> WORD','term',1,'p_term','lex_parser.py',474),
+  ('term -> WORD_WITH_DOT','term',1,'p_term','lex_parser.py',475),
+  ('term -> value','term',1,'p_term_value','lex_parser.py',480),
+  ('term -> method','term',1,'p_term_value','lex_parser.py',481),
+  ('term -> scope','term',1,'p_term_value','lex_parser.py',482),
+  ('value -> WILDCARD','value',1,'p_value_wildcard','lex_parser.py',487),
+  ('value -> WILDCARD_RANGE','value',1,'p_value_wildcard_range','lex_parser.py',491),
+  ('value -> NUMBER','value',1,'p_value_number_int','lex_parser.py',495),
+  ('value -> NUMBER_WITH_DOT','value',1,'p_value_number_float','lex_parser.py',499),
+  ('method -> METHOD','method',1,'p_value_method','lex_parser.py',503),
+  ('value -> VARIABLE','value',1,'p_value_variable','lex_parser.py',507),
+  ('value -> SYMBOL','value',1,'p_value_symbol','lex_parser.py',511),
+  ('value -> LONG_SYMBOL','value',1,'p_value_symbol','lex_parser.py',512),
+  ('value -> SINGLE_QUOTED_STRING','value',1,'p_value_literal_string','lex_parser.py',517),
+  ('value -> DOUBLE_QUOTED_STRING','value',1,'p_value_string','lex_parser.py',521),
+  ('conditional -> IF THEN','conditional',2,'p_illegal_if_then','lex_parser.py',525),
+  ('conditional -> IF INDENT THEN','conditional',3,'p_illegal_if_then','lex_parser.py',526),
+  ('conditional -> IF ELSE','conditional',2,'p_illegal_if_then','lex_parser.py',527),
+  ('conditional -> IF INDENT ELSE','conditional',3,'p_illegal_if_then','lex_parser.py',528),
+  ('conditional -> ELSE THEN','conditional',2,'p_illegal_if_then','lex_parser.py',529),
+  ('conditional -> ELSE INDENT THEN','conditional',3,'p_illegal_if_then','lex_parser.py',530),
 ]
```

### Comparing `mash-shell-0.2.0/src/mash/shell/parsing.py` & `mash-shell-0.2.2/src/mash/shell/parsing.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,36 +5,14 @@
 from mash.io_util import log
 from mash.shell import delimiters
 from mash.shell.delimiters import FALSE, TRUE
 from mash.shell.errors import ShellError
 from mash.util import is_globbable, is_valid_method_name, match_words, quote, quote_all, removeprefix, glob
 
 
-def infer_infix_args(op: str, *args: str) -> Tuple[Tuple[str], Tuple[str]]:
-    if args[1] == op:
-        lhs, _, *rhs = args
-        lhs = (lhs,)
-    else:
-        i = args.index(op)
-        lhs = args[:i]
-        rhs = args[i+1:]
-    return lhs, rhs
-
-
-
-
-
-def unquote_delimiters(terms: List[str], delimiters: List[str]) -> List[str]:
-    for i, term in enumerate(terms):
-        if term.startswith('\\'):
-            suffix = removeprefix(term, '\\')
-            if suffix in delimiters:
-                terms[i] = suffix
-
-
 def expand_variables(terms: List[str], env: dict,
                      completenames_options: List[str],
                      ignore_invalid_syntax: bool,
                      wildcard_value='$',
                      escape=False) -> Iterable[str]:
     """Replace variables with their values.
     E.g.
@@ -88,35 +66,42 @@
 
         if escape and matches:
             yield quote(v, ignore=list('*$<>'))
         else:
             yield v
 
 
-def to_string(value: Any) -> str:
-    """Convert a variable to a string.
-    """
-    if isinstance(value, bool):
-        value = TRUE if value else FALSE
-    return str(value)
-
-
 def expand_variables_inline(line: str, env: dict,
                             completenames_options: List[str],
                             ignore_invalid_syntax: bool) -> str:
     """Expand $variables in `line`.
     """
     terms = line.split(' ')
     expanded_terms = expand_variables(terms, env,
                                       completenames_options,
                                       ignore_invalid_syntax)
     line = ' '.join(expanded_terms)
     return line
 
 
+def to_string(value: Any) -> str:
+    """Convert a variable to a string.
+    """
+    if isinstance(value, bool):
+        value = TRUE if value else FALSE
+    return str(value)
+
+
+def to_bool(line: str) -> bool:
+    if isinstance(line, bool):
+        return line
+
+    return line != FALSE and line is not None
+
+
 def filter_comments(terms: List[str]) -> List[str]:
     if '#' in terms:
         i = terms.index('#')
         terms = terms[:i]
     return terms
```

### Comparing `mash-shell-0.2.0/src/mash/shell/shell.py` & `mash-shell-0.2.2/src/mash/shell/shell.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,59 +1,55 @@
 from argparse import ArgumentParser
 from cmd import Cmd
-from collections import defaultdict
 from copy import deepcopy
-from pathlib import Path
-import re
-from typing import Callable, Dict, List, Tuple
+import subprocess
+from typing import Callable, Dict, Iterable, List, Tuple
 import logging
 import os
 import sys
-import traceback
 
 from mash import io_util
-from mash.io_util import ArgparseWrapper, bold, has_argument, has_output, log, read_file
-from mash.util import has_method, is_valid_method_name, translate_items
-
-from mash.shell.function import ShellFunction as Function
-import mash.shell.function as func
-from mash.shell.base import FALSE, TRUE, BaseShell, filter_private_keys
+from mash.io_util import ArgparseWrapper, bold, has_argument, has_output, log, log_once
+from mash.shell.model import LAST_RESULTS, ElseCondition, Indent, Lines, Map, Math, Node, Term, Terms
+from mash.shell.base import BaseShell
+from mash.shell.cmd2 import default_prompt, run
+from mash.shell.delimiters import DEFINE_FUNCTION
+from mash.shell.errors import ShellError, ShellPipeError, ShellSyntaxError
 from mash.shell.errors import ShellSyntaxError
+from mash.shell.function import ShellFunction as Function
+from mash.shell.if_statement import Abort, handle_prev_then_else_statements
+from mash.shell.lex_parser import parse
+from mash.util import has_method, is_valid_method_name
 
 description = 'If no positional arguments are given then an interactive subshell is started.'
 epilog = f"""
 --------------------------------------------------------------------------------
 {bold('Default Commands')}
 Run shell commands by prefixing them with `!`.
 E.g.
     ./shell.py !echo abc; echo def # Bash
 
 Run multiple Python commands by separating each command with colons or newlines.
 E.g.
     ./shell.py 'print abc; print def \n print ghi'
 
 {bold('Variables')}
-Assignment constants or evaluate expressiosn:
+Assign constants or evaluate expressiosn:
 ```
 a = 100
 b <- print $a
 echo $a $b
 ```
 
-Store expression results:
-```
-echo 100 -> a
-echo $a
-```
-
 {bold('Interopability')}
 Interopability with Bash can be done with pipes:
     `|>` for Python.
     `|`  for Bash
-    `>`  for Bash (write to file)
+    `>-`  for Bash (write to file)
+    `>>`  for Bash (append to file)
 
 1. To stdin and stdout
 E.g.
     echo abc | ./shell.py print
     ./shell.py print abc | echo
 
 2. Within the dsl
@@ -63,193 +59,176 @@
     ./shell.py 'print abc |> print'
 """
 
 
 class Shell(BaseShell):
     """Extend BaseShell(Cmd) with helper functions.
     """
-    default_function_group_key = '_'
-
-    def __init__(self, *args, **kwds):
-        super().__init__(*args, **kwds)
-        self.functions: Dict[str, List[str, Function]] = defaultdict(list)
-
-    def do_exit(self, args):
-        """exit [code]
-
-        Wrapper for sys.exit(code) with default code: 0
-        """
-        if not args:
-            args = 0
-
-        exit(int(args))
 
-    def do_cat(self, filename):
-        """Concatenate and print files
-        """
-        return ''.join((Path(f).read_text() for f in filename.split()))
+    def onecmd_inner(self, lines: str):
+        if not self.use_model:
+            return super().onecmd_inner(lines)
+
+        ast = parse(lines)
+        if ast is None:
+            raise ShellError('Invalid syntax: AST is empty')
 
-    def do_print(self, args):
-        """Mimic Python's print function.
-        """
-        logging.info(f'Cmd: print {args}')
-        return args
+        try:
+            self.run_commands(ast, '', run=True)
 
-    def do_println(self, args):
-        """Print each arg on a new line.
-        """
-        logging.info(f'Cmd: println {args}')
-        return self.do_flatten(args)
+        except ShellPipeError as e:
+            if self.ignore_invalid_syntax:
+                log(e)
+                return
 
-    def do_echo(self, args):
-        """Mimic Bash's print function.
-        """
-        logging.info(f'Cmd: echo {args}')
-        return args
+            raise ShellError(e)
 
-    def do_env(self, keys: str):
-        """Retrieve environment variables.
-        Return all variables if no key is given.
-        """
-        if not keys:
-            return filter_private_keys(self.env.asdict())
+        except subprocess.CalledProcessError as e:
+            returncode, stderr = e.args
+            log(f'Shell exited with {returncode}: {stderr}')
 
-        try:
-            return {k: self.env[k] for k in keys.split()}
-        except KeyError:
-            log('Invalid key')
+            if self.ignore_invalid_syntax:
+                return
 
-    def do_E(self, args):
-        """Show the last exception
-        """
-        traceback.print_exception(
-            type(func.last_exception), func.last_exception, func.last_traceback)
+            raise ShellError(str(e))
 
-    def do_save(self, _):
-        """Save the current session.
-        """
-        self.save_session()
+    def run_commands(self, ast: Node, prev_result='', run=False):
+        if isinstance(ast, Term):
+            return ast.run(prev_result, shell=self, lazy=not run)
 
-    def do_source(self, args: str):
-        files = args.split(' ')
-        for f in files:
-            run_command(read_file(f), self, strict=True)
+        elif isinstance(ast, str):
+            return self.run_commands(Term(ast), prev_result, run=run)
 
-    def do_reload(self, _):
-        """Reload the current session.
-        """
-        self.try_load_session()
+        done = self._handle_define_function(ast)
+        if done:
+            return
 
-    def do_undo(self, _):
-        """Undo the previous command
+        if not isinstance(ast, ElseCondition) and \
+                not isinstance(ast, Indent) and \
+                not isinstance(ast, Lines):
+            try:
+                handle_prev_then_else_statements(self)
+            except Abort:
+                return prev_result
+
+        if isinstance(ast, Node):
+            return ast.run(prev_result, shell=self, lazy=not run)
+        else:
+            raise NotImplementedError()
+
+    def _handle_define_function(self, ast: Node) -> bool:
+        if DEFINE_FUNCTION not in self.locals:
+            return False
+
+        # self._extend_inline_function_definition(line)
+        f = self.locals[DEFINE_FUNCTION]
+
+        if isinstance(ast, Indent):
+            # TODO compare indent width
+            width = ast.indent
+            if ast.data is None:
+                return True
+
+            if f.line_indent is None:
+                f.line_indent = width
+
+            if width >= f.line_indent:
+                self.locals[DEFINE_FUNCTION].inner.append(ast)
+                return True
+
+            self._finalize_define_function(f)
+
+        elif not isinstance(ast, Lines):
+            # TODO this will only be triggered after a non-Word command
+            self._finalize_define_function(f)
+
+        return False
+
+    def _finalize_define_function(self, f):
+        self.env[f.func_name] = f
+        self.locals.rm(DEFINE_FUNCTION)
+        self.prompt = default_prompt
+
+    def parse(self, results: str):
+        # TODO mv this function
+        # SMELL avoid circular import: base => model => lex_parser => model
+        return parse(results)
+
+    ############################################################################
+    # Commands: do_*
+    ############################################################################
+
+    def do_map(self, args=''):
+        """Apply a function to every line.
+        If `$` is present, then each line from stdin is inserted there.
+        Otherwise each line is appended.
+
+        Usage
+        -----
+        ```sh
+        println a b |> map echo
+        println a b |> map echo prefix $ suffix
+        ```
         """
-        if not self.lastcmd:
-            return
+        log('Expected arguments')
+        return ''
 
-        f = self.lastcmd.split()[0]
+    def _do_foreach(self, ast: tuple, prev_results: str) -> Iterable:
+        """Apply a function to every term or word.
 
-        method = f'undo_{f}'
-        if has_method(self, f'undo_{f}'):
-            return getattr(self, method)()
+        Usage
+        ```sh
+        echo a b |> foreach echo
+        echo a b |> foreach echo prefix $ suffix
+        ```
+        """
+        prev_results = '\n'.join(prev_results.split(' '))
+        return Map.map(ast, prev_results, self, delimiter=' ')
+
+    def foldr(self, commands: List[Term], prev_results: str, delimiter='\n'):
+        items = parse(prev_results).values
+        k, acc, *args = commands
+
+        for item in items:
+            command = Terms([k, acc] + args)
+            acc = self.run_commands(command, item, run=True)
+
+            if str(acc).strip() == '' and self._last_results:
+                acc = self._last_results[-1]
+                self.env[LAST_RESULTS] = []
 
-        raise NotImplementedError()
+        return acc
 
     def do_math(self, args: str) -> str:
-        operators = ['-', '\\+', '\\*', '%', '==', '!=', '<', '>']
-        delimiters = ['\\(', '\\)']
-        regex = '(' + '|'.join(operators + delimiters) + ')'
-        terms = re.split(regex, args)
-        return self._eval_terms(terms)
-
-    def do_range(self, args: str) -> str:
-        """range(start, stop, [step])
-        """
-        args = args.split(' ')
-        args = (int(a) for a in args)
-        return '\n'.join((str(i) for i in range(*args)))
-
-    def _eval_terms(self, terms=List[str]) -> str:
-        line = ''.join(translate_items(terms, self.env.asdict()))
-        log(line)
-
-        try:
-            result = eval(line)
-        except (NameError, SyntaxError, TypeError) as e:
-            raise ShellSyntaxError(f'eval failed: {line}') from e
-
-        # SMELL avoid side-effects on top of a return type
-        self._save_result(result)
+        result = Math.eval(args, self.env)
 
         if isinstance(result, bool):
-            result = TRUE if result else FALSE
+            self._save_result(result)
+            return ''
 
         return str(result)
 
-    def last_method(self):
-        """Find the method corresponding to the last command run in `shell`.
-        It has the form: do_{cmd}
-
-        Return a the last method if it exists and None otherwise.
-        """
-        # TODO integrate this into Shell and store the last succesful cmd
-
-        if not self.lastcmd:
-            return
-
-        cmd = self.lastcmd.split()[0]
-        return Shell.get_method(cmd)
-
-    @staticmethod
-    def get_method(method_suffix: str):
-        method_name = f'do_{method_suffix}'
-        if not has_method(Shell, method_name):
-            return
-
-        method = getattr(Shell, method_name)
-
-        if isinstance(method, Function):
-            return method.func
-
-        return method
-
-    def add_functions(self, functions: Dict[str, Function], group_key=None):
-        """Add commands to this instance of CMD.
-        These will be hidden from the help view, unlike shell.set_functions.
-        Use a key to select a group of functions
-        """
-        if group_key is None:
-            group_key = Shell.default_function_group_key
-
-        for key, func in functions.items():
-            set_functions({key: func}, self)
-            self.functions[group_key].append(key)
-
-    def remove_functions(self, group_key=None):
-        if group_key is None:
-            group_key = Shell.default_function_group_key
-
-        for key in self.functions[group_key]:
-            delattr(self, f'do_{key}')
-
-        del self.functions[group_key]
+################################################################################
+# Helpers
+################################################################################
 
 
 def all_commands(shell: Shell):
     for cmd in dir(shell):
         if cmd.startswith('do_') and has_method(shell, cmd):
             yield cmd.lstrip('do_')
 
 
 def set_functions(functions: Dict[str, Function], cls: Cmd = Shell) -> type:
     """Extend `cls` with a set of functions
     Note that this modifies the class Shell directly, rather than an instance.
     """
     for key, func in functions.items():
         if not is_valid_method_name(key):
-            logging.debug(f'Key: {key} is not a valid method name')
+            log_once(f'Key: {key} is not a valid method name')
 
         if not isinstance(func, Function):
             func = Function(func)
 
         setattr(cls, f'do_{key}', func)
         setattr(getattr(cls, f'do_{key}'), '__doc__', func.help)
 
@@ -266,14 +245,36 @@
         args = ' '.join(args)
         return os.system(''.join(cmd + ' ' + args))
 
     func.__name__ = cmd
     return func
 
 
+def run_command(command='', shell: Shell = None, strict=None):
+    """Run a newline-separated string of commands.
+
+    Parameters
+    ----------
+        strict : bool
+            Raise exceptions when encountering invalid syntax.
+    """
+    if shell is None:
+        shell = Shell()
+
+    if strict is not None:
+        shell.ignore_invalid_syntax = not strict
+
+    # TODO avoid splitines
+    # shell.onecmd(command)
+
+    for line in command.splitlines():
+        if line:
+            shell.onecmd(line)
+
+
 def add_cli_args(parser: ArgumentParser):
     if not has_argument(parser, 'cmd'):
         parser.add_argument('cmd', nargs='*',
                             help='A comma- or newline-separated list of commands')
     if not has_argument(parser, 'safe'):
         parser.add_argument('-s', '--safe', action='store_true',
                             help='Safe-mode. Ask for confirmation before executing commands.')
@@ -320,65 +321,14 @@
 
     except KeyboardInterrupt as e:
         print()
         logging.debug(e)
         exit(130)
 
 
-def run(shell, commands, filename, repl=True):
-    if commands or filename is not None:
-        # compile mode
-        if filename is not None:
-            run_commands_from_file(filename, shell)
-
-        if commands:
-            run_command(commands, shell, strict=True)
-
-    elif repl:
-        run_interactively(shell)
-
-
-def run_commands_from_file(filename: str, shell: Shell):
-    command = read_file(filename)
-    run_command(command, shell, strict=True)
-
-
-def run_command(command='', shell: Shell = None, strict=None):
-    """Run a single command in using `shell`.
-
-    Parameters
-    ----------
-        strict : bool
-            Raise exceptions when encountering invalid syntax.
-    """
-    if shell is None:
-        shell = Shell()
-
-    if strict is not None:
-        shell.ignore_invalid_syntax = not strict
-
-    # TODO skip splitlines
-    for line in command.splitlines():
-        if line:
-            shell.onecmd(line)
-
-
-def run_interactively(shell):
-    io_util.interactive = True
-    shell.auto_save = True
-    i = 0
-    while True:
-        i += 1
-        try:
-            shell.cmdloop()
-        except KeyboardInterrupt:
-            print('\nKeyboardInterrupt')
-            shell.intro = ''
-
-
 def build(functions: Dict[str, Function] = None, completions: Dict[str, Callable] = None, instantiate=True) -> Shell:
     """Extend the class Shell and create an instance of it.
     Note that `set_functions` must be called before instantiating Shell.
     """
     # copy class to avoid side-effects
     CustomShell = deepcopy(Shell)
```

### Comparing `mash-shell-0.2.0/src/mash/shell/with_filesystem.py` & `mash-shell-0.2.2/src/mash/shell/with_filesystem.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from functools import partial
+from logging import debug
 
 from mash.filesystem.filesystem import FileSystem, OPTIONS, Option
 from mash.filesystem.discoverable import Discoverable
 from mash.filesystem.view import Path
 from mash.shell.shell import build, set_completions, set_functions
-from mash.util import find_fuzzy_matches, has_method, partial_simple
+from mash.shell.function import ShellFunction as Function
+from mash.util import find_fuzzy_matches, hamming, has_method, is_digit, partial_simple
 
 cd_aliasses = 'cd_aliasses'
 path_delimiter = '/'
 
 
 class ShellWithFileSystem:
     def __init__(self, data={}, repository: FileSystem = None, **kwds):
@@ -23,16 +25,23 @@
 
     def init_shell(self, *build_args, **build_kwds):
         cls = build(*build_args, instantiate=False, **build_kwds)
         self._set_shell_functions(cls)
         self.set_shell_completions(cls)
 
         self.shell = cls(save_session_prehook=self.repository.snapshot,
-                         load_session_posthook=self.repository.load)
-        self.shell.set_do_char_method(self.repository.cd, OPTIONS)
+                         load_session_posthook=self.repository.load,
+                         completekey='tab'
+                         )
+
+        for option in OPTIONS:
+            func = partial_simple(self.repository.cd, option)
+            self.shell.add_special_function(option, func)
+
+        self.shell._default_method = self.default_method
 
     def _set_shell_functions(self, cls):
         # convert methods to functions
         cd = partial_simple(self.repository.cd)
         ls = partial_simple(self.repository.ll, delimiter=', ')
         ll = partial_simple(self.repository.ll)
         get = partial_simple(self.get)
@@ -63,20 +72,26 @@
                        'mv': mv,
                        'rm': rm,
                        'show': show,
                        'reset': reset,
                        }, cls)
 
     def pwd(self):
+        """Print the path to the current working directory
+        """
         return ' '.join(self.repository.full_path)
 
     def get(self, *path: str):
+        """Return the value of the file associated with `path`.
+        """
         return self.repository.get(path)
 
     def set(self, *args: str):
+        """Assign a value to the file k.
+        """
         k, *values = args
 
         if len(values) == 1:
             self.repository.set(k, values[0])
         elif len(values) > 1:
             self.repository.set(k, values)
 
@@ -113,16 +128,17 @@
         for dirname in dirs:
             method_name = f'do_{dirname}'
             if not has_method(self.shell, method_name):
                 self.add_cd_alias(dirname)
 
     def add_cd_alias(self, dirname: str):
         # create alias
-        cd_dirname = partial(self.repository.cd, dirname)
-        cd_dirname.__name__ = f'{self.repository.cd.__name__}({dirname})'
+        func = partial(self.repository.cd, dirname)
+        name = f'{self.repository.cd.__name__}({dirname})'
+        cd_dirname = Function(func, name, f'cd {dirname}')
 
         self.shell.add_functions({dirname: cd_dirname},
                                  group_key=cd_aliasses)
 
     def update_prompt(self):
         # TODO ensure that this method is run after an exception
         # e.g. after cd fails
@@ -152,7 +168,22 @@
         results = list(find_fuzzy_matches(text, candidates))
 
         if len(results) > 1:
             if results[0].startswith(text) and not results[1].startswith(text):
                 return results[:1]
 
         return results
+
+    def default_method(self, dirname: str):
+        candidates = self.complete_cd(dirname, None, None, None)
+        if candidates:
+            error = hamming(dirname, candidates[0])
+            if error < 0.9:
+                self.repository.cd(candidates[0])
+                return
+
+        if is_digit(dirname):
+            self.repository.cd(dirname)
+            return
+
+        debug('No matching directory found')
+        return dirname
```

### Comparing `mash-shell-0.2.0/src/mash/subshell.py` & `mash-shell-0.2.2/src/mash/subshell.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.0/src/mash/util.py` & `mash-shell-0.2.2/src/mash/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,14 +97,15 @@
 
 def crop(s: str, n=100, suffix='..') -> str:
     margin = len(suffix)
     if len(s) <= n + margin:
         return s
     return s[:n] + suffix
 
+
 ################################################################################
 # Operations for lists and sequences
 ################################################################################
 
 
 def append_list(a: list, b) -> list:
     a = a.copy()
```

### Comparing `mash-shell-0.2.0/src/mash/verify_server.py` & `mash-shell-0.2.2/src/mash/verify_server.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.0/src/mash_shell.egg-info/SOURCES.txt` & `mash-shell-0.2.2/src/mash_shell.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 pyproject.toml
 requirements.txt
 src/examples/_extend_path.py
 src/examples/discoverable.py
 src/examples/discoverable_api.py
 src/examples/discoverable_with_oas.py
 src/examples/filesystem.py
+src/examples/ms_graph_api.py
 src/examples/object_parser.py
 src/examples/shell_example.py
 src/mash/__main__.py
 src/mash/cli.py
 src/mash/doc_inference.py
 src/mash/html_table.py
 src/mash/html_table_data.py
@@ -32,19 +33,21 @@
 src/mash/object_parser/factory.py
 src/mash/object_parser/oas.py
 src/mash/object_parser/object_parser.py
 src/mash/object_parser/object_parser_standards.py
 src/mash/object_parser/spec.py
 src/mash/shell/__init__.py
 src/mash/shell/base.py
+src/mash/shell/cmd2.py
 src/mash/shell/delimiters.py
 src/mash/shell/errors.py
 src/mash/shell/function.py
 src/mash/shell/if_statement.py
 src/mash/shell/lex_parser.py
+src/mash/shell/model.py
 src/mash/shell/parsetab.py
 src/mash/shell/parsing.py
 src/mash/shell/progress_bar.py
 src/mash/shell/shell.py
 src/mash/shell/with_filesystem.py
 src/mash_shell.egg-info/PKG-INFO
 src/mash_shell.egg-info/SOURCES.txt
```

### Comparing `mash-shell-0.2.0/test/test_html_table.py` & `mash-shell-0.2.2/test/test_html_table.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.0/test/test_parallel.py` & `mash-shell-0.2.2/test/test_parallel.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.0/test/test_pipeline.py` & `mash-shell-0.2.2/test/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.0/test/test_server.py` & `mash-shell-0.2.2/test/test_server.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.0/test/test_util.py` & `mash-shell-0.2.2/test/test_util.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.0/test/test_verify_server.py` & `mash-shell-0.2.2/test/test_verify_server.py`

 * *Files identical despite different names*

