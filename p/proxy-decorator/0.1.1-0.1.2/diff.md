# Comparing `tmp/proxy-decorator-0.1.1.tar.gz` & `tmp/proxy-decorator-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proxy-decorator-0.1.1.tar", last modified: Tue Apr 11 08:08:30 2023, max compression
+gzip compressed data, was "proxy-decorator-0.1.2.tar", last modified: Tue Apr 11 08:52:56 2023, max compression
```

## Comparing `proxy-decorator-0.1.1.tar` & `proxy-decorator-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 08:08:30.939415 proxy-decorator-0.1.1/
--rw-rw-rw-   0        0        0      352 2023-04-11 08:08:30.937420 proxy-decorator-0.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-11 08:08:30.935414 proxy-decorator-0.1.1/proxy_decorator.egg-info/
--rw-rw-rw-   0        0        0      352 2023-04-11 08:08:30.000000 proxy-decorator-0.1.1/proxy_decorator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2023-04-11 08:08:30.000000 proxy-decorator-0.1.1/proxy_decorator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 08:08:30.000000 proxy-decorator-0.1.1/proxy_decorator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-04-11 08:08:30.000000 proxy-decorator-0.1.1/proxy_decorator.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 08:08:30.000000 proxy-decorator-0.1.1/proxy_decorator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 08:08:30.939415 proxy-decorator-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      538 2023-04-11 08:08:25.000000 proxy-decorator-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 08:52:56.216230 proxy-decorator-0.1.2/
+-rw-rw-rw-   0        0        0     1010 2023-04-11 08:52:56.214229 proxy-decorator-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      572 2023-04-11 08:50:37.000000 proxy-decorator-0.1.2/README.md
+-rw-rw-rw-   0        0        0      440 2023-04-11 08:43:52.000000 proxy-decorator-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-11 08:52:56.217233 proxy-decorator-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-11 08:52:56.180230 proxy-decorator-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-11 08:52:56.194230 proxy-decorator-0.1.2/src/proxy_decorator/
+-rw-rw-rw-   0        0        0        0 2023-04-11 08:31:33.000000 proxy-decorator-0.1.2/src/proxy_decorator/__init__.py
+-rw-rw-rw-   0        0        0     2011 2023-04-11 07:27:44.000000 proxy-decorator-0.1.2/src/proxy_decorator/proxy_decorator.py
+drwxrwxrwx   0        0        0        0 2023-04-11 08:52:56.210228 proxy-decorator-0.1.2/src/proxy_decorator.egg-info/
+-rw-rw-rw-   0        0        0     1010 2023-04-11 08:52:56.000000 proxy-decorator-0.1.2/src/proxy_decorator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      267 2023-04-11 08:52:56.000000 proxy-decorator-0.1.2/src/proxy_decorator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 08:52:56.000000 proxy-decorator-0.1.2/src/proxy_decorator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-04-11 08:52:56.000000 proxy-decorator-0.1.2/src/proxy_decorator.egg-info/top_level.txt
```

