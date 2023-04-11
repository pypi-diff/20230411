# Comparing `tmp/noteyXMLParser-0.2.3.tar.gz` & `tmp/noteyXMLParser-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/noteyXMLParser-0.2.3.tar", last modified: Tue Apr  4 01:47:09 2023, max compression
+gzip compressed data, was "dist/noteyXMLParser-0.2.4.tar", last modified: Tue Apr 11 05:45:58 2023, max compression
```

## Comparing `noteyXMLParser-0.2.3.tar` & `noteyXMLParser-0.2.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
-drwxr-xr-x   0 aminmahjoub   (501) staff       (20)        0 2023-04-04 01:47:09.076678 noteyXMLParser-0.2.3/
--rw-r--r--   0 aminmahjoub   (501) staff       (20)      443 2023-04-04 01:47:09.076331 noteyXMLParser-0.2.3/PKG-INFO
--rw-r--r--   0 aminmahjoub   (501) staff       (20)       10 2023-04-03 05:02:31.000000 noteyXMLParser-0.2.3/README.md
--rw-r--r--   0 aminmahjoub   (501) staff       (20)       38 2023-04-04 01:47:09.076830 noteyXMLParser-0.2.3/setup.cfg
--rw-r--r--   0 aminmahjoub   (501) staff       (20)      689 2023-04-04 01:31:10.000000 noteyXMLParser-0.2.3/setup.py
+drwxr-xr-x   0 aminmahjoub   (501) staff       (20)        0 2023-04-11 05:45:58.507878 noteyXMLParser-0.2.4/
+-rw-r--r--   0 aminmahjoub   (501) staff       (20)      772 2023-04-11 05:45:58.507543 noteyXMLParser-0.2.4/PKG-INFO
+-rw-r--r--   0 aminmahjoub   (501) staff       (20)      251 2023-04-10 22:52:02.000000 noteyXMLParser-0.2.4/README.md
+-rw-r--r--   0 aminmahjoub   (501) staff       (20)       38 2023-04-11 05:45:58.508013 noteyXMLParser-0.2.4/setup.cfg
+-rw-r--r--   0 aminmahjoub   (501) staff       (20)      689 2023-04-11 05:45:53.000000 noteyXMLParser-0.2.4/setup.py
```

### Comparing `noteyXMLParser-0.2.3/setup.py` & `noteyXMLParser-0.2.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
      name='noteyXMLParser',  
-     version='0.2.3',
+     version='0.2.4',
      author="Amin Mahjoub",
      author_email="mahjoub@usc.edu",
      description="Music XML Parser",
      long_description=long_description,
      package_dir={"":"/Users/aminmahjoub/NoteyXMLParser/xmlParser/src"},
      url="https://github.com/mmahjoub5/NoteyXMLParser",
    long_description_content_type="text/markdown",
```

