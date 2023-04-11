# Comparing `tmp/calldict-0.3.tar.gz` & `tmp/calldict-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\calldict-0.3.tar", last modified: Tue May 25 17:12:16 2021, max compression
+gzip compressed data, was "dist\calldict-0.4.tar", last modified: Tue Apr 11 17:13:51 2023, max compression
```

## Comparing `calldict-0.3.tar` & `calldict-0.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
-drwxrwxrwx   0        0        0        0 2021-05-25 17:12:16.000000 calldict-0.3/
--rw-rw-rw-   0        0        0      379 2021-05-25 17:12:16.000000 calldict-0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2021-05-25 17:12:16.000000 calldict-0.3/calldict/
--rw-rw-rw-   0        0        0     9184 2021-05-25 17:10:04.000000 calldict-0.3/calldict/__init__.py
--rw-rw-rw-   0        0        0      413 2021-05-25 17:08:59.000000 calldict-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 17:13:51.403276 calldict-0.4/
+-rw-rw-rw-   0        0        0      400 2023-04-11 17:13:51.404275 calldict-0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-11 17:13:51.399276 calldict-0.4/calldict/
+-rw-rw-rw-   0        0        0     6771 2023-04-11 17:12:17.052421 calldict-0.4/calldict/__init__.py
+-rw-rw-rw-   0        0        0      535 2023-04-11 11:53:12.349672 calldict-0.4/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

