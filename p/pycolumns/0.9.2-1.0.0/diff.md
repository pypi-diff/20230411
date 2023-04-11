# Comparing `tmp/pycolumns-0.9.2.tar.gz` & `tmp/pycolumns-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycolumns-0.9.2.tar", last modified: Fri Apr  7 13:23:31 2023, max compression
+gzip compressed data, was "pycolumns-1.0.0.tar", last modified: Tue Apr 11 17:59:16 2023, max compression
```

## Comparing `pycolumns-0.9.2.tar` & `pycolumns-1.0.0.tar`

### file list

```diff
@@ -1,30 +1,29 @@
-drwxrwxr-x   0 esheldon  (1000) esheldon  (1000)        0 2023-04-07 13:23:31.534430 pycolumns-0.9.2/
-drwxrwxr-x   0 esheldon  (1000) esheldon  (1000)        0 2023-04-07 13:23:31.530430 pycolumns-0.9.2/.github/
-drwxrwxr-x   0 esheldon  (1000) esheldon  (1000)        0 2023-04-07 13:23:31.530430 pycolumns-0.9.2/.github/workflows/
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     1063 2023-04-07 12:59:58.000000 pycolumns-0.9.2/.github/workflows/test.yaml
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     1063 2023-04-07 13:14:36.000000 pycolumns-0.9.2/LICENSE
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     4648 2023-04-07 13:23:31.534430 pycolumns-0.9.2/PKG-INFO
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     4385 2023-04-01 14:58:59.000000 pycolumns-0.9.2/README.md
-drwxrwxr-x   0 esheldon  (1000) esheldon  (1000)        0 2023-04-07 13:23:31.530430 pycolumns-0.9.2/pycolumns/
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)      290 2023-04-07 12:59:58.000000 pycolumns-0.9.2/pycolumns/__init__.py
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    23944 2023-04-07 12:59:58.000000 pycolumns-0.9.2/pycolumns/column.py
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    25004 2023-04-07 12:59:58.000000 pycolumns-0.9.2/pycolumns/columns.py
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     2012 2023-04-07 12:59:58.000000 pycolumns-0.9.2/pycolumns/indices.py
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     6154 2023-04-07 12:59:58.000000 pycolumns-0.9.2/pycolumns/mergesort.py
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    17898 2023-04-07 12:59:58.000000 pycolumns-0.9.2/pycolumns/sfile.py
-drwxrwxr-x   0 esheldon  (1000) esheldon  (1000)        0 2023-04-07 13:23:31.534430 pycolumns-0.9.2/pycolumns/tests/
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)        0 2023-04-07 12:59:58.000000 pycolumns-0.9.2/pycolumns/tests/__init__.py
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     2416 2023-04-07 12:59:58.000000 pycolumns-0.9.2/pycolumns/tests/test_create.py
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)      897 2023-04-07 12:59:58.000000 pycolumns-0.9.2/pycolumns/tests/test_create_index.py
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     1347 2023-04-07 12:59:58.000000 pycolumns-0.9.2/pycolumns/tests/test_mergesort.py
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     2302 2023-04-07 12:59:58.000000 pycolumns-0.9.2/pycolumns/tests/test_query.py
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     2548 2023-04-07 12:59:58.000000 pycolumns-0.9.2/pycolumns/util.py
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)       22 2023-04-07 13:23:02.000000 pycolumns-0.9.2/pycolumns/version.py
-drwxrwxr-x   0 esheldon  (1000) esheldon  (1000)        0 2023-04-07 13:23:31.530430 pycolumns-0.9.2/pycolumns.egg-info/
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     4648 2023-04-07 13:23:31.000000 pycolumns-0.9.2/pycolumns.egg-info/PKG-INFO
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)      543 2023-04-07 13:23:31.000000 pycolumns-0.9.2/pycolumns.egg-info/SOURCES.txt
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)        1 2023-04-07 13:23:31.000000 pycolumns-0.9.2/pycolumns.egg-info/dependency_links.txt
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)        6 2023-04-07 13:23:31.000000 pycolumns-0.9.2/pycolumns.egg-info/requires.txt
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)       10 2023-04-07 13:23:31.000000 pycolumns-0.9.2/pycolumns.egg-info/top_level.txt
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)       38 2023-04-07 13:23:31.534430 pycolumns-0.9.2/setup.cfg
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)      705 2023-04-07 13:15:33.000000 pycolumns-0.9.2/setup.py
+drwxrwxr-x   0 esheldon  (1000) esheldon  (1000)        0 2023-04-11 17:59:16.038525 pycolumns-1.0.0/
+drwxrwxr-x   0 esheldon  (1000) esheldon  (1000)        0 2023-04-11 17:59:16.034525 pycolumns-1.0.0/.github/
+drwxrwxr-x   0 esheldon  (1000) esheldon  (1000)        0 2023-04-11 17:59:16.038525 pycolumns-1.0.0/.github/workflows/
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     1063 2023-04-07 12:59:58.000000 pycolumns-1.0.0/.github/workflows/test.yaml
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     1063 2023-04-07 13:14:36.000000 pycolumns-1.0.0/LICENSE
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     5545 2023-04-11 17:59:16.038525 pycolumns-1.0.0/PKG-INFO
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     5282 2023-04-11 17:57:49.000000 pycolumns-1.0.0/README.md
+drwxrwxr-x   0 esheldon  (1000) esheldon  (1000)        0 2023-04-11 17:59:16.038525 pycolumns-1.0.0/pycolumns/
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)      270 2023-04-11 17:57:49.000000 pycolumns-1.0.0/pycolumns/__init__.py
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    26520 2023-04-11 17:57:49.000000 pycolumns-1.0.0/pycolumns/column.py
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    20160 2023-04-11 17:57:49.000000 pycolumns-1.0.0/pycolumns/columns.py
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     2123 2023-04-11 17:57:49.000000 pycolumns-1.0.0/pycolumns/indices.py
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     5066 2023-04-11 17:57:49.000000 pycolumns-1.0.0/pycolumns/mergesort.py
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    17898 2023-04-11 13:40:40.000000 pycolumns-1.0.0/pycolumns/sfile.py
+drwxrwxr-x   0 esheldon  (1000) esheldon  (1000)        0 2023-04-11 17:59:16.038525 pycolumns-1.0.0/pycolumns/tests/
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)        0 2023-04-07 12:59:58.000000 pycolumns-1.0.0/pycolumns/tests/__init__.py
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     2538 2023-04-11 17:57:49.000000 pycolumns-1.0.0/pycolumns/tests/test_create.py
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     1833 2023-04-11 17:57:49.000000 pycolumns-1.0.0/pycolumns/tests/test_create_index.py
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     2302 2023-04-07 12:59:58.000000 pycolumns-1.0.0/pycolumns/tests/test_query.py
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     3408 2023-04-11 17:57:49.000000 pycolumns-1.0.0/pycolumns/util.py
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)       22 2023-04-11 17:57:49.000000 pycolumns-1.0.0/pycolumns/version.py
+drwxrwxr-x   0 esheldon  (1000) esheldon  (1000)        0 2023-04-11 17:59:16.038525 pycolumns-1.0.0/pycolumns.egg-info/
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     5545 2023-04-11 17:59:15.000000 pycolumns-1.0.0/pycolumns.egg-info/PKG-INFO
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)      509 2023-04-11 17:59:16.000000 pycolumns-1.0.0/pycolumns.egg-info/SOURCES.txt
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)        1 2023-04-11 17:59:15.000000 pycolumns-1.0.0/pycolumns.egg-info/dependency_links.txt
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)       13 2023-04-11 17:59:15.000000 pycolumns-1.0.0/pycolumns.egg-info/requires.txt
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)       10 2023-04-11 17:59:15.000000 pycolumns-1.0.0/pycolumns.egg-info/top_level.txt
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)       38 2023-04-11 17:59:16.038525 pycolumns-1.0.0/setup.cfg
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)      755 2023-04-11 17:57:49.000000 pycolumns-1.0.0/setup.py
```

### Comparing `pycolumns-0.9.2/.github/workflows/test.yaml` & `pycolumns-1.0.0/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `pycolumns-0.9.2/LICENSE` & `pycolumns-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pycolumns-0.9.2/PKG-INFO` & `pycolumns-1.0.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,171 +1,205 @@
 Metadata-Version: 2.1
 Name: pycolumns
-Version: 0.9.2
+Version: 1.0.0
 Summary: A simple, efficient, pythonic column data store
 Home-page: https://github.com/esheldon/pycolumns
 License: MIT
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENSE
 
 A simple, efficient column-oriented, pythonic data store.
 
 The focus is currently on efficiency of reading and writing.  The code is pure
-python but searching and reading data is fast due to the use of numpy memory
-maps and column indexing.  Basic consistency is ensured but the database is not
-fully ACID.
+python but searching and reading data is fast due to the use of the fitsio
+package for column data and index data.  Basic consistency is ensured for
+the columns in the table, but the database is not fully ACID.
 
 The storage is a simple directory with files on disk.
 
 Examples
 --------
 
 ```python
 >>> import pycolumns as pyc
 
 # instantiate a column database from the specified coldir
->>> c=pyc.Columns('/some/path/mycols.cols')
+>>> c = pyc.Columns('/some/path/mycols.cols')
 
 # display some info about the columns
 >>> c
-Column Directory:
+Columns Directory:
 
+  mydata
   dir: /some/path/mydata.cols
+  nrows: 64348146
   Columns:
-    name             type  dtype index  shape
-    --------------------------------------------------
-    ccd             array    <i2 True   (64348146,)
-    dec             array    <f8 False  (64348146,)
-    exposurename    array   |S20 True   (64348146,)
-    id              array    <i8 False  (64348146,)
-    imag            array    <f4 False  (64348146,)
-    ra              array    <f8 False  (64348146,)
-    x               array    <f4 False  (64348146,)
-    y               array    <f4 False  (64348146,)
-    g               array    <f8 False  (64348146, 2)
-    meta             dict
+    name             dtype index
+    -----------------------------
+    ccd                <i2 True
+    dec                <f8 False
+    exposurename      |S20 True
+    id                 <i8 True
+    imag               <f4 False
+    ra                 <f8 False
+    x                  <f4 False
+    y                  <f4 False
+    g                  <f8 False
 
+  Dictionaries
+    name
+    -----------------------------
+    meta
 
-  Sub-Column Directories:
+  Sub-Columns Directories:
     name
-    --------------------------------------------------
+    -----------------------------
     psfstars
 
 # display info about column 'id'
 >>> c['id']
 Column:
-  "id"
+  name: id
   filename: ./id.array
-  type: col
-  shape: (64348146,)
-  has index: False
+  type: array
   dtype: <i8
+  has index: False
+  nrows: 64348146
 
-# get the column names
->>> c.colnames
-['ccd', 'dec', 'exposurename', 'id', 'imag', 'ra', 'x', 'y', 'g', 'meta']
+# number of rows in table
+>>> c.nrows
 
-# reload all columns or specified column/column list
->>> c.reload(name=None)
+# read all columns into a single rec array.  By default the dict
+# columns are not loaded
 
-# read all data from array column 'id'
-# alternative syntaxes, including numpy style slicing
+>>> data = c.read()
+
+# using asdict=True puts the data into a dict.  The dict data
+# are also loaded in this case
+>>> data = c.read(asdict=True)
+
+# specify columns
+>>> data = c.read(columns=['id', 'flux'])
+
+# dict columns can be specified if asdict is True.  Dicts can also
+# be read as single columns, see below
+>>> data = c.read(columns=['id', 'flux', 'meta'], asdict=True)
+
+# specifying a set of rows as sequence/array or slice
+>>> data = c.read(columns=['id', 'flux'], rows=[3, 225, 1235])
+>>> data = c.read(columns=['id', 'flux'], rows=slice(10, 20))
+
+# read all data from column 'id' as an array rather than recarray
+# alternative syntaxes
 >>> ind = c['id'][:]
 >>> ind = c['id'].read()
 >>> ind = c.read_column('id')
 
-# dict columns are read as a dict. No slicing for dicts
->>> meta = c['meta'].read()
-
 # read a subset of rows
 # slicing
 >>> ind = c['id'][25:125]
 
 # specifying a set of rows
->>> rows=[3, 225, 1235]
+>>> rows = [3, 225, 1235]
 >>> ind = c['id'][rows]
 >>> ind = c.read_column('id', rows=rows)
 
-# read all columns into a single rec array.  By default the dict
-# columns are not loaded
-
->>> data = c.read()
-
-# using asdict=True puts the data into a dict.  The dict data
-# are loaded in this case
->>> data = c.read(asdict=True)
-
-# specify columns
->>> data = c.read(columns=['id', 'flux'], rows=rows)
-
-# dict columns can be specified if asdict is True
->>> data = c.read(columns=['id', 'flux', 'meta'], asdict=True)
+# reading a dictionary column
+>>> meta = c['meta'].read()
 
 # Create indexes for fast searching
 >>> c['id'].create_index()
 
-# get indices for some condition
+# get indices for some conditions
 >>> ind = c['id'] > 25
 >>> ind = c['id'].between(25, 35)
 >>> ind = c['id'] == 25
 
-# find all matches
->>> ind = c['id'].match([35, 77])
-
 # read the corresponding data
 >>> ccd = c['ccd'][ind]
 >>> data = c.read(columns=['ra', 'dec'], rows=ind)
 
 # composite searches over multiple columns
 >>> ind = (c['id'] == 25) & (col['ra'] < 15.23)
 >>> ind = c['id'].between(15, 25) | (c['id'] == 55)
 >>> ind = c['id'].between(15, 250) & (c['id'] != 66) & (c['ra'] < 100)
->>> ind = c['id'].between(15, 250) & c['id'].match([35, 99])
 
-# speed up reads by sorting indices
->>> ind.sort()
->>> data = c.read(columns=['ra', 'dec'], rows=ind)
+# write columns from the fields in a rec array names in the data correspond
+# to column names.  If this is the first time writing data, the columns are
+# created, and on subsequent writes, the columns must match
+
+>>> c.append(recdata)
+>>> c.append(new_data)
+
+# append data from the fields in a FITS file
+>>> c.from_fits(fitsfile_name)
 
-# you can check if the index is already sorted
->>> if not ind.is_sorted:
->>>    ind.sort()
+# add a dictionary column.
+>>> c.create_column('weather', 'dict')
+>>> c['weather'].write({'temp': 30.1, 'humid': 0.5})
+
+# overwrite dict column
+>>> c['weather'].write({'temp': 33.2, 'humid': 0.3, 'windspeed': 60.5})
+
+# you should not generally create array columns, since they
+# can get out of sync with existing columns.  This will by default
+# raise an exception, but you can send verify=False if you know
+# what you are doing.  In the future special support will be added for
+# adding new columns
+>>> c.create_column('test', 'array')
 
-# update values for a column
+# update values for an array column
 >>> c['id'][35] = 10
 >>> c['id'][35:35+3] = [8, 9, 10]
 >>> c['id'][rows] = idvalues
 
-# write multiple columns from the fields in a rec array
-# names in the data correspond to column names.
-# If columns are not present, they are created
-# but row count consistency must be maintained for all array
-# columns and this is checked.
+# get all names, including dictionary and sub Columns
+# same as list(c.keys())
+>>> c.names
+['ccd', 'dec', 'exposurename', 'id', 'imag', 'ra', 'x', 'y', 'g',
+ 'meta', 'psfstars']
+
+# only array column names
+>>> c.column_names
+['ccd', 'dec', 'exposurename', 'id', 'imag', 'ra', 'x', 'y', 'g']
+
+# only dict columns
+>>> c.dict_names
+['meta', 'weather']
+
+# only sub Columns directories
+>>> c.subcols_names
+['psfstars']
 
->>> c.append(recdata)
+# reload all columns or specified column/column list
+>>> c.reload()
 
-# append data from the fields in a FITS file
->>> c.from_fits(fitsfile_name)
+# delete all data.  This will ask for confirmation
+>>> c.delete()
+
+# delete column and its data
+>>> c.delete_column('ra')
 
-# add a dict column
->>> c.create_column('meta')
->>> c['meta'].write({'test': 'hello'})
->>> d = c['meta'].read()
-
-# heirarchical sets of columns are also supported
->>> c['psfstars']
-Column Directory:
+# to configure the amount of memory used during index creation, specify
+# cache_mem in gigabytes.  Default 1 gig
+>>> cols = pyc.Columns(fname, cache_mem=0.5)
 
+# columns can actually be another pycolumns directory
+>>> psfcols = cols['psfstars']
+>>> psfcols
   dir: /some/path/mydata.cols/psfstars.cols
   Columns:
     name             type  dtype index  shape
     --------------------------------------------------
-    ccd             array    <i2 True   (348146,)
-    exposurename    array   |S20 True   (348146,)
-    x               array    <f4 False  (348146,)
-    y               array    <f4 False  (348146,)
+    ccd             array    <i2 True   (64348146,)
+    id              array    <i8 True   (64348146,)
+    imag            array    <f4 False  (64348146,)
+    x               array    <f4 False  (64348146,)
+    y               array    <f4 False  (64348146,)
+    ...etc
 ```
 
 Dependencies
 ------------
 numpy
```

### Comparing `pycolumns-0.9.2/pycolumns/column.py` & `pycolumns-1.0.0/pycolumns/column.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,19 +2,17 @@
 TODO
 
     - allow appending without updating index, which we would do at the end
       of a series of appends
 
 """
 import os
-import bisect
 import numpy as np
 
 from . import util
-from .sfile import SimpleFile
 from .indices import Indices
 
 
 class ColumnBase(object):
     """
     Represent a column in a Columns database.  Facilitate opening, reading,
     writing of data.  This class can be instantiated alone, but is usually
@@ -266,53 +264,68 @@
         cache_mem=1,
     ):
         """
         initialize the meta data, and possibly load the mmap
         """
 
         self._type = 'array'
+        self._ext = 1
 
         self._cache_mem_gb = float(cache_mem)
 
         super()._do_init(
             filename=filename,
             name=name,
             dir=dir,
             verbose=verbose,
         )
 
-        if self.filename is None or not os.path.exists(self.filename):
+        # if self.filename is None or not os.path.exists(self.filename):
+        if self.filename is None:
             return
 
-        self._open_file('r+')
+        self._open_file()
 
         # get info for index if it exists
         self._init_index()
 
-    def _open_file(self, mode):
-        self._sf = SimpleFile(self.filename, mode=mode)
+    def _open_file(self):
+        import fitsio
+        self._fits = fitsio.FITS(self.filename, 'rw')
+
+    def _get_hdu(self):
+        return self._fits[self._ext]
 
     def _clear(self):
         """
         Clear out all the metadata for this column.
         """
 
         super()._clear()
 
         if self.has_data:
-            del self._sf
+            del self._fits
+            del self._dtype
 
         self._has_index = False
 
     @property
     def has_data(self):
         """
         returns True if this column has some data
         """
-        return hasattr(self, '_sf')
+        has_data = False
+
+        if hasattr(self, '_fits'):
+            if len(self._fits) > 1:
+                hdu = self._get_hdu()
+                if hdu.has_data():
+                    has_data = True
+        # import IPython; IPython.embed()
+        return has_data
 
     def ensure_has_data(self):
         """
         raise RuntimeError if no data is present
         """
         if not self.has_data:
             raise ValueError('this column has no associated data')
@@ -320,46 +333,56 @@
     @property
     def dtype(self):
         """
         get the data type of the column
         """
         self.ensure_has_data()
 
-        return self._sf.dtype
+        if not hasattr(self, '_dtype'):
+            hdu = self._get_hdu()
+            dtype, _, _ = hdu.get_rec_dtype()
+            self._converted_dtype, self._convert_unicode = (
+                util.maybe_convert_ascii_dtype_to_unicode(dtype)
+            )
+            descr = dtype.descr
+            assert len(descr) == 1
+            assert descr[0][0] == 'data'
+            self._dtype = dtype
+
+        return self._dtype
 
     @property
     def index_dtype(self):
         return get_index_dtype(self.dtype)
 
     @property
-    def shape(self):
+    def nrows(self):
         """
         get the shape of the column
         """
         self.ensure_has_data()
 
-        return self._sf.shape
+        hdu = self._get_hdu()
+        return hdu.get_nrows()
 
     @property
-    def nrows(self):
+    def shape(self):
         """
         get the shape of the column
         """
         self.ensure_has_data()
 
-        return self._sf.shape[0]
+        return (self.nrows, )
 
     @property
     def size(self):
         """
         get the size of the columns
         """
-        self.ensure_has_data()
-
-        return self._sf.size
+        return self.nrows
 
     @property
     def data_size_bytes(self):
         return self.dtype.itemsize * self.size
 
     @property
     def data_size_gb(self):
@@ -392,69 +415,93 @@
         # make sure the data type of the input equals that of the column
         if not isinstance(data, np.ndarray):
             raise ValueError("For 'array' columns data must be a numpy array")
 
         if data.dtype.names is not None:
             raise ValueError('do not enter data with fields')
 
-        if not self.has_data:
-            self._open_file('w+')
+        if data.ndim > 1:
+            raise ValueError('data must be one dimensional array')
 
-        self._sf.write(data)
+        self._write_data_as_rec(data)
 
         if self.has_index:
             self._update_index()
 
+    def _write_data_as_rec(self, data):
+        view_data = self._get_rec_view(data)
+
+        if not self.has_data:
+            self._fits.write(view_data)
+        else:
+            hdu = self._fits[self._ext]
+            hdu.append(view_data)
+
+    def _get_rec_view(self, data):
+        view_dtype = [('data', data.dtype.descr[0][1])]
+        return data.view(view_dtype)
+
     def __getitem__(self, arg):
         """
         Item lookup method, e.g. col[..] meaning slices or
         sequences, etc.
         """
-        if not hasattr(self, '_sf'):
-            raise ValueError('no file loaded yet')
 
-        use_arg = util.extract_rows(arg, sort=True)
-        return self._sf[use_arg]
+        self.ensure_has_data()
+
+        hdu = self._get_hdu()
+
+        rows = util.extract_rows(arg, sort=True)
+
+        if rows is None:
+            data = hdu[:]['data']
+        elif isinstance(rows, slice):
+            data = hdu[rows]['data']
+        else:
+            data = np.zeros(rows.size, dtype=self.dtype)
+            hdu._FITS.read_rows_as_rec(self._ext+1, data, rows)
+            if self._convert_unicode:
+                data = data.astype(self._converted_dtype, copy=False)
+            data = data['data']
+            if rows.ndim == 0:
+                data = data[0]
+
+        return data
 
     def __setitem__(self, arg, values):
         """
         Item lookup method, e.g. col[..] meaning slices or
         sequences, etc.
         """
-        if not hasattr(self, '_sf'):
-            raise ValueError('no file loaded yet')
+        raise RuntimeError('fix writing')
 
-        self._sf[arg] = values
+        if not hasattr(self, '_fits'):
+            raise ValueError('no file loaded yet')
 
     def read(self, rows=None):
         """
         read data from this column
 
         Parameters
         ----------
         rows: sequence, slice, Indices or None, optional
             A subset of the rows to read.
         """
-        if not hasattr(self, '_sf'):
+        if not hasattr(self, '_fits'):
             raise ValueError('no file loaded yet')
 
         return self[rows]
-        # if rows is None:
-        #     return self._sf[:]
-        # else:
-        #     use_rows = util.extract_rows(rows, sort=True)
-        #     return self._sf[use_rows]
 
     def _delete(self):
         """
         Attempt to delete the data file associated with this column
         """
 
         if hasattr(self, '_sf'):
-            del self._sf
+            del self._fits
 
         super()._delete()
 
         # remove index if it exists
         self.delete_index()
 
     #
@@ -512,43 +559,47 @@
                 print(f'{tfile} -> {self.index_filename}')
 
             shutil.move(tfile, self.index_filename)
 
         self._init_index()
 
     def _write_index_memory(self, fname):
+        import fitsio
+
         if self.verbose:
             print(f'creating index for {self.name} in memory')
 
         dt = self.index_dtype
+
         index_data = np.zeros(self.shape[0], dtype=dt)
         index_data['index'] = np.arange(index_data.size)
         index_data['value'] = self[:]
 
         index_data.sort(order='value')
 
         # set up file name and data type info
-        with SimpleFile(fname, mode='w+') as sf:
-            sf.write(index_data)
+        with fitsio.FITS(fname, mode='rw', clobber=True) as output:
+            output.write(index_data)
 
     def _write_index_mergesort(self, tmpdir, fname):
         from .mergesort import create_mergesort_index
 
         if self.verbose:
             print(f'creating index for {self.name} with mergesort on disk')
 
         chunksize_bytes = int(self._cache_mem_gb * 1024**3)
 
         bytes_per_element = self.index_dtype.itemsize
+
         # need factor of two because we keep both the cache and the scratch in
         # mergesort
         chunksize = chunksize_bytes // (bytes_per_element * 2)
 
         create_mergesort_index(
-            infile=self.filename,
+            source=self,
             outfile=fname,
             chunksize=chunksize,
             tmpdir=tmpdir,
             verbose=self.verbose,
         )
 
     def update_index(self):
@@ -570,33 +621,36 @@
 
         self._init_index()
 
     def _init_index(self):
         """
         If index file exists, load some info
         """
+        import fitsio
+
         index_fname = self.index_filename
         if os.path.exists(index_fname):
             self._has_index = True
-            self._index = SimpleFile(index_fname, mode='r+')
+            self._index = fitsio.FITS(index_fname, 'rw')
+            self._iarr1 = np.zeros(1, dtype=self.index_dtype)
         else:
             self._has_index = False
             self._index = None
 
     @property
     def index_filename(self):
         """
         get the filename for the index of this column
         """
         if self.filename is None:
             return None
 
         # remove the final extension
         index_fname = '.'.join(self.filename.split('.')[0:-1])
-        index_fname = index_fname+'__index.sf'
+        index_fname = index_fname+'.index'
         return index_fname
 
     def match(self, values):
         """
         get indices of entries that match the input value or values
 
         Parameters
@@ -638,60 +692,95 @@
 
     def __eq__(self, val):
         """
         get exact equality
         """
         return self.between(val, val)
 
+    def _read_one_from_index(self, index):
+        iarr1 = self._iarr1
+        self._index._FITS.read_as_rec(self._ext+1, index+1, index+1, iarr1)
+        val = iarr1['value'][0]
+        if self._convert_unicode:
+            return str(val, 'utf-8')
+        return val
+
+    def _bisect_right(self, val):
+        return _bisect_right(
+            func=self._read_one_from_index,
+            x=val,
+            lo=0,
+            hi=self.nrows,
+        )
+
+    def _bisect_left(self, val):
+        return _bisect_left(
+            func=self._read_one_from_index,
+            x=val,
+            lo=0,
+            hi=self.nrows,
+        )
+
     # one-sided range operators
     def __gt__(self, val):
         """
         bisect_right returns i such that data[i:] are all strictly > val
         """
         self.verify_index_available()
+        i = self._bisect_right(val)
+        indices = self._index[1]['index'][i:].copy()
 
-        mmap = self._index.mmap
-        i = bisect.bisect_right(mmap['value'], val)
-        indices = mmap['index'][i:].copy()
+        # mmap = self._index.mmap
+        # i = bisect.bisect_right(mmap['value'], val)
+        # indices = mmap['index'][i:].copy()
 
         return Indices(indices)
 
     def __ge__(self, val):
         """
         bisect_left returns i such that data[i:] are all strictly >= val
         """
         self.verify_index_available()
 
-        mmap = self._index.mmap
-        i = bisect.bisect_left(mmap['value'], val)
-        indices = mmap['index'][i:].copy()
+        i = self._bisect_left(val)
+        indices = self._index[1]['index'][i:].copy()
+
+        # mmap = self._index.mmap
+        # i = bisect.bisect_left(mmap['value'], val)
+        # indices = mmap['index'][i:].copy()
 
         return Indices(indices)
 
     def __lt__(self, val):
         """
         bisect_left returns i such that data[:i] are all strictly < val
         """
         self.verify_index_available()
 
-        mmap = self._index.mmap
-        i = bisect.bisect_left(mmap['value'], val)
-        indices = mmap['index'][:i].copy()
+        i = self._bisect_left(val)
+        indices = self._index[1]['index'][:i].copy()
+
+        # mmap = self._index.mmap
+        # i = bisect.bisect_left(mmap['value'], val)
+        # indices = mmap['index'][:i].copy()
 
         return Indices(indices)
 
     def __le__(self, val):
         """
         bisect_right returns i such that data[:i] are all strictly <= val
         """
         self.verify_index_available()
 
-        mmap = self._index.mmap
-        i = bisect.bisect_right(mmap['value'], val)
-        indices = mmap['index'][:i].copy()
+        i = self._bisect_right(val)
+        indices = self._index[1]['index'][:i].copy()
+
+        # mmap = self._index.mmap
+        # i = bisect.bisect_right(mmap['value'], val)
+        # indices = mmap['index'][:i].copy()
 
         return Indices(indices)
 
     def between(self, low, high, interval='[]'):
         """
         Find all entries in the range low,high, inclusive by default.
 
@@ -727,46 +816,55 @@
         # combine with the results of another query and extract the
         # index array
         ind = columns.where( (col1.between(low,high)) & (col2 == value2) )
         """
 
         self.verify_index_available()
 
-        mmap = self._index.mmap
+        # mmap = self._index.mmap
         if interval == '[]':
             # bisect_left returns i such that data[i:] are all strictly >= val
-            ilow = bisect.bisect_left(mmap['value'], low)
+            # ilow = bisect.bisect_left(mmap['value'], low)
+            ilow = self._bisect_left(low)
 
             # bisect_right returns i such that data[:i] are all strictly <= val
-            ihigh = bisect.bisect_right(mmap['value'], high)
+            # ihigh = bisect.bisect_right(mmap['value'], high)
+            ihigh = self._bisect_right(high)
 
         elif interval == '(]':
             # bisect_right returns i such that data[i:] are all strictly > val
-            ilow = bisect.bisect_right(mmap['value'], low)
+            # ilow = bisect.bisect_right(mmap['value'], low)
+            ilow = self._bisect_right(low)
 
             # bisect_right returns i such that data[:i] are all strictly <= val
-            ihigh = bisect.bisect_right(mmap['value'], high)
+            # ihigh = bisect.bisect_right(mmap['value'], high)
+            ihigh = self._bisect_right(high)
 
         elif interval == '[)':
             # bisect_left returns i such that data[:i] are all strictly >= val
-            ilow = bisect.bisect_left(mmap['value'], low)
+            # ilow = bisect.bisect_left(mmap['value'], low)
+            ilow = self._bisect_left(low)
 
             # bisect_left returns i such that data[:i] are all strictly < val
-            ihigh = bisect.bisect_left(mmap['value'], high)
+            # ihigh = bisect.bisect_left(mmap['value'], high)
+            ihigh = self._bisect_left(high)
 
         elif interval == '()':
             # bisect_right returns i such that data[i:] are all strictly > val
-            ilow = bisect.bisect_right(mmap['value'], low)
+            # ilow = bisect.bisect_right(mmap['value'], low)
+            ilow = self._bisect_right(low)
 
             # bisect_left returns i such that data[:i] are all strictly < val
-            ihigh = bisect.bisect_left(mmap['value'], high)
+            # ihigh = bisect.bisect_left(mmap['value'], high)
+            ihigh = self._bisect_left(high)
         else:
             raise ValueError('bad interval type: %s' % interval)
 
-        indices = mmap['index'][ilow:ihigh].copy()
+        # indices = mmap['index'][ilow:ihigh].copy()
+        indices = self._index[1]['index'][ilow:ihigh]
 
         return Indices(indices)
 
     def _get_repr_list(self, full=False):
         """
 
         Get a list of metadat for this column.
@@ -776,41 +874,43 @@
 
         if not full:
             s = ''
             if self.name is not None:
                 s += 'Column: %-15s' % self.name
 
             s += ' type: %10s' % self.type
+            if self.has_data:
 
-            if self.shape is not None:
-                s += ' shape: %12s' % (self.shape,)
+                # if self.shape is not None:
+                #     s += ' shape: %12s' % (self.shape,)
+                s += ' nrows: %12s' % self.nrows
 
-            if self.name is not None:
-                s += ' has index: %s' % self.has_index
+                if self.name is not None:
+                    s += ' has index: %s' % self.has_index
 
             s = [s]
         else:
             s = []
             if self.name is not None:
                 s += ['name: %s' % self.name]
 
             if self.filename is not None:
                 s += ['filename: %s' % self.filename]
 
             s += ['type: array']
 
-            if self.shape is not None:
-                s += ['shape: %s' % (self.shape,)]
-
-            if self.name is not None:
+            if self.has_data:
                 s += ['has index: %s' % self.has_index]
 
-            if self.dtype is not None:
                 c_dtype = self.dtype.descr[0][1]
-                s += ["dtype: %s" % c_dtype]
+                s += ['dtype: %s' % c_dtype]
+
+                # if self.shape is not None:
+                #     s += ['shape: %s' % (self.shape,)]
+                s += ['nrows: %s' % self.nrows]
 
             s = [indent + tmp for tmp in s]
             s = ['Column: '] + s
 
         return s
 
 
@@ -885,40 +985,35 @@
 def get_index_dtype(dtype):
     return np.dtype([
         ('index', 'i8'),
         ('value', dtype.descr[0][1]),
     ])
 
 
-def _do_test_create_index(tmpdir, cache_mem, seed=999, num=1_000_000):
-    import os
-    import numpy as np
-    from . import sfile
-    from .columns import Columns
-
-    cdir = os.path.join(tmpdir, 'test.cols')
-    cols = Columns(cdir, cache_mem=cache_mem, verbose=True)
-
-    rng = np.random.RandomState(seed)
-    data = np.zeros(num, dtype=[('rand', 'f8')])
-    data['rand'] = rng.uniform(size=num)
-
-    cols.append(data)
-    cols['rand'].create_index()
-    ifile = cols['rand'].index_filename
-    idata = sfile.read(ifile)
-
-    s = data['rand'].argsort()
-    assert np.all(idata['value'] == data['rand'][s])
-
-
-def test_create_index(cache_mem=0.01, seed=999, num=1_000_000, keep=False):
-    import tempfile
-    if keep:
-        _do_test_create_index(
-            tmpdir='.', cache_mem=cache_mem, seed=seed, num=num,
-        )
-    else:
-        with tempfile.TemporaryDirectory(dir='.') as tmpdir:
-            _do_test_create_index(
-                tmpdir=tmpdir, cache_mem=cache_mem, seed=seed, num=num,
-            )
+def _bisect_right(func, x, lo, hi):
+    """
+    bisect right with function call to get value
+    """
+
+    while lo < hi:
+        mid = (lo + hi) // 2
+        if x < func(mid):
+            hi = mid
+        else:
+            lo = mid + 1
+
+    return lo
+
+
+def _bisect_left(func, x, lo, hi):
+    """
+    bisect left with function call to get value
+    """
+
+    while lo < hi:
+        mid = (lo + hi) // 2
+        if func(mid) < x:
+            lo = mid + 1
+        else:
+            hi = mid
+
+    return lo
```

### Comparing `pycolumns-0.9.2/pycolumns/columns.py` & `pycolumns-1.0.0/pycolumns/columns.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 todo
 
+    - allow update index without completely redoing it
     - tests for sub columns
     - Maybe add option "unsort" to put indices back in original unsorted order
     - add updating a set of columns with indices= and data=
         - already can do column by itself
         - Would need to think carefully if we wanted to optimize by sorting
           etc. to keep things consistent
     - note if we move to not using memmap, will need to maybe think about when
@@ -35,183 +36,14 @@
     ----------
     dir: str
         Path to database
     cache_mem: number, optional
         Cache memory for index creation in gigabytes.  Default 1.0
     verbose: bool, optional
         If set to True, print messages
-
-    Examples
-    ---------
-    >>> import pycolumns as pyc
-
-    # instantiate a column database from the specified coldir
-    >>> c = pyc.Columns('/some/path/mycols.cols')
-
-    # display some info about the columns
-    >>> c
-    Columns Directory:
-
-      dir: /some/path/mydata.cols
-      Columns:
-        name             type  dtype index  shape
-        --------------------------------------------------
-        ccd             array    <i2 True   (64348146,)
-        dec             array    <f8 False  (64348146,)
-        exposurename    array   |S20 True   (64348146,)
-        id              array    <i8 True   (64348146,)
-        imag            array    <f4 False  (64348146,)
-        ra              array    <f8 False  (64348146,)
-        x               array    <f4 False  (64348146,)
-        y               array    <f4 False  (64348146,)
-        g               array    <f8 False  (64348146, 2)
-        meta             dict
-
-
-      Sub-Columns Directories:
-        name
-        --------------------------------------------------
-        psfstars
-
-    # display info about column 'id'
-    >>> c['id']
-    Column:
-      "id"
-      filename: ./id.array
-      type: col
-      shape: (64348146,)
-      has index: False
-      dtype: <i8
-
-    # number of rows in table
-    >>> c.nrows
-
-    # read all columns into a single rec array.  By default the dict
-    # columns are not loaded
-
-    >>> data = c.read()
-
-    # using asdict=True puts the data into a dict.  The dict data
-    # are loaded in this case
-    >>> data = c.read(asdict=True)
-
-    # specify columns
-    >>> data = c.read(columns=['id', 'flux'])
-
-    # dict columns can be specified if asdict is True.  Dicts can also
-    # be read as single columns, see below
-    >>> data = c.read(columns=['id', 'flux', 'meta'], asdict=True)
-
-    # specifying a set of rows as sequence/array or slice
-    >>> data = c.read(columns=['id', 'flux'], rows=[3, 225, 1235])
-    >>> data = c.read(columns=['id', 'flux'], rows=slice(10, 20))
-
-    # read all data from column 'id' as an array rather than recarray
-    # alternative syntaxes
-    >>> ind = c['id'][:]
-    >>> ind = c['id'].read()
-    >>> ind = c.read_column('id')
-
-    # read a subset of rows
-    # slicing
-    >>> ind = c['id'][25:125]
-
-    # specifying a set of rows
-    >>> rows = [3, 225, 1235]
-    >>> ind = c['id'][rows]
-    >>> ind = c.read_column('id', rows=rows)
-
-    # reading a dict column
-    >>> meta = c['meta'].read()
-
-    # Create indexes for fast searching
-    >>> c['id'].create_index()
-
-    # get indices for some conditions
-    >>> ind = c['id'] > 25
-    >>> ind = c['id'].between(25, 35)
-    >>> ind = c['id'] == 25
-
-    # read the corresponding data
-    >>> ccd = c['ccd'][ind]
-    >>> data = c.read(columns=['ra', 'dec'], rows=ind)
-
-    # composite searches over multiple columns
-    >>> ind = (c['id'] == 25) & (col['ra'] < 15.23)
-    >>> ind = c['id'].between(15, 25) | (c['id'] == 55)
-    >>> ind = c['id'].between(15, 250) & (c['id'] != 66) & (c['ra'] < 100)
-
-    # write columns from the fields in a rec array names in the data correspond
-    # to column names.  If this is the first time writing data, the columns are
-    # created, and on subsequent writes, the columns must match
-
-    >>> c.append(recdata)
-    >>> c.append(new_data)
-
-    # append data from the fields in a FITS file
-    >>> c.from_fits(fitsfile_name)
-
-    # add a dict column.
-    >>> c.create_column('weather', 'dict')
-    >>> c['weather'].write({'temp': 30.1, 'humid': 0.5})
-
-    # overwrite dict column
-    >>> c['weather'].write({'temp': 33.2, 'humid': 0.3, 'windspeed': 60.5})
-
-    # you should not generally create array columns, since they
-    # can get out of sync with existing columns.  This will by default
-    # raise an exception, but you can send verify=False if you know
-    # what you are doing.  In the future support will be added for this.
-    >>> c.create_column('test', 'array')
-
-    # update values for an array column
-    >>> c['id'][35] = 10
-    >>> c['id'][35:35+3] = [8, 9, 10]
-    >>> c['id'][rows] = idvalues
-
-    # get the column names
-    >>> c.colnames
-    ['ccd', 'dec', 'exposurename', 'id', 'imag', 'ra', 'x', 'y', 'g',
-     'meta', 'psfstars']
-    # only array columns
-    >>> c.array_colnames
-    ['ccd', 'dec', 'exposurename', 'id', 'imag', 'ra', 'x', 'y', 'g']
-    # only dict columns
-    >>> c.dict_colnames
-    ['meta', 'weather']
-    # only sub pycolumns directories
-    >>> c.cols_colnames
-    ['psfstars']
-
-    # reload all columns or specified column/column list
-    >>> c.reload()
-
-    # delete all data.  This will ask for confirmation
-    >>> c.delete()
-
-    # delete column and its data
-    >>> c.delete_column('ra')
-
-    # to modify the amount of memory used during index creation, specify
-    # cache_mem in gigabytes.  Default 1 gig
-    >>> cols = pyc.Columns(fname, cache_mem=0.5)
-
-    # columns can actually be another pycolumns directory
-    >>> psfcols = cols['psfstars']
-    >>> psfcols
-      dir: /some/path/mydata.cols/psfstars.cols
-      Columns:
-        name             type  dtype index  shape
-        --------------------------------------------------
-        ccd             array    <i2 True   (64348146,)
-        id              array    <i8 True   (64348146,)
-        imag            array    <f4 False  (64348146,)
-        x               array    <f4 False  (64348146,)
-        y               array    <f4 False  (64348146,)
-        ...etc
     """
 
     def __init__(self, dir=None, cache_mem=1, verbose=False):
         self._type = 'cols'
         self._verbose = verbose
         self._cache_mem_gb = float(cache_mem)
         self._set_dir(dir)
@@ -221,45 +53,45 @@
     def nrows(self):
         """
         number of rows in table
         """
         return self._nrows
 
     @property
-    def colnames(self):
+    def names(self):
         """
         Get a list of all column names
         """
         return list(self.keys())
 
     @property
-    def array_colnames(self):
+    def column_names(self):
         """
-        Get a list of the array column names
+        Get a list of all column names
         """
-        return [c for c in self.keys() if self[c].type == 'array']
+        return [c for c in self if self[c].type == 'array']
 
     @property
-    def dict_colnames(self):
+    def dict_names(self):
         """
         Get a list of the array column names
         """
-        return [c for c in self.keys() if self[c].type == 'dict']
+        return [c for c in self if self[c].type == 'dict']
 
     @property
-    def cols_colnames(self):
+    def subcols_names(self):
         """
         Get a list of the array column names
         """
-        return [c for c in self.keys() if self[c].type == 'cols']
+        return [c for c in self if self[c].type == 'cols']
 
     @property
     def type(self):
         """
-        get the data type of the column
+        Get the type (cols for Columns)
         """
         return self._type
 
     @property
     def dir(self):
         return self._dir
 
@@ -296,16 +128,16 @@
             answer = input('really delete all data? (y/n) ')
             if answer.lower() == 'y':
                 yes = True
 
         if not yes:
             return
 
-        for colname in self:
-            self.delete_column(colname, yes=True)
+        for name in self:
+            self.delete_column(name, yes=True)
 
     def _dirbase(self):
         """
         Return the dir basename minus any extension
         """
         if self.dir is not None:
             bname = os.path.basename(self.dir)
@@ -505,19 +337,19 @@
         names = data.dtype.names
         if names is None:
             raise ValueError('append() takes a structured array as input')
 
         if len(self) > 0:
             # make sure the input data matches the existing column names
             in_names = set(names)
-            a_names = set(self.array_colnames)
-            if in_names != a_names:
+            column_names = set(self.column_names)
+            if in_names != column_names:
                 raise ValueError(
                     f'input columns {in_names}'
-                    f'do not match existing array columns {a_names}'
+                    f'do not match existing table columns {column_names}'
                 )
 
         for name in names:
             self._append_column(name, data[name])
 
         # make sure the array columns all have the same length
         if verify:
@@ -598,15 +430,15 @@
         parameters
         ----------
         name: string
             Name of column to delete
         yes: bool
             If True, don't prompt for confirmation
         """
-        if name not in self:
+        if name not in self.colnumn_names:
             print("cannot delete column '%s', it does not exist" % name)
 
         if not yes:
             answer = input("really delete column '%s'? (y/n) " % name)
             if answer.lower() == 'y':
                 yes = True
 
@@ -629,15 +461,16 @@
         """
         read multiple columns from the database
 
         Parameters
         ----------
         columns: sequence or string
             Can be a scalar string or a sequence of strings.  Defaults to all
-            array columns if asdict is False, all columns if asdict is True
+            array columns if asdict is False, but will include
+            dicts if asdict is True
         rows: sequence, slice or scalar
             Sequence of row numbers.  Defaults to all.
         asdict: bool, optional
             If set to True, read the requested columns into a dict.
         """
 
         columns = self._extract_columns(columns=columns, asdict=asdict)
@@ -650,15 +483,15 @@
         if asdict:
             # Just putting the arrays into a dictionary.
             data = {}
 
             for colname in columns:
 
                 if self.verbose:
-                    print('\treading column: %s' % colname)
+                    print('    reading column: %s' % colname)
 
                 # just read the data and put in dict, simpler than below
                 col = self[colname]
                 if col.type == 'array':
                     data[colname] = col.read(rows=rows)
                 else:
                     data[colname] = col.read()
@@ -683,15 +516,15 @@
             # copying into a single array with fields
             dtype = self._extract_dtype(columns)
 
             data = np.empty(n_rows2read, dtype=dtype)
 
             for colname in columns:
                 if self.verbose:
-                    print('\treading column: %s' % colname)
+                    print('    reading column: %s' % colname)
 
                 col = self[colname]
                 data[colname][:] = col.read(rows=rows)
 
         return data
 
     def _extract_dtype(self, columns):
@@ -705,14 +538,15 @@
 
             dt = (colname, descr)
             if len(shape) > 1:
                 dt = dt + shape[1:]
 
             dtype.append(dt)
 
+        dtype, _ = util.maybe_convert_ascii_dtype_to_unicode(np.dtype(dtype))
         return dtype
 
     read_columns = read
 
     def read_column(self, colname, rows=None):
         """
         Only numpy, fixed length for now.  Eventually allow pickled columns.
@@ -727,21 +561,19 @@
         extract the columns to read.  If no columns are sent then the behavior
         depends on the asdict parameter
             - if asdict is False, read all array columns
             - if asdict is True, read all columns
         """
         if columns is None:
 
-            keys = sorted(self.keys())
-
             if asdict:
+                keys = sorted(self.keys())
                 columns = keys
             else:
-                # just get the array columns
-                columns = [c for c in keys if self[c].type == 'array']
+                columns = self.column_names
 
         else:
             if isinstance(columns, str):
                 columns = [columns]
 
             for c in columns:
                 if c not in self:
@@ -764,51 +596,66 @@
         """
         indent = '  '
         s = []
         if self.dir is not None:
             dbase = self._dirbase()
             s += [dbase]
             s += ['dir: '+self.dir]
+            s += ['nrows: %s' % self.nrows]
 
+        s += ['']
         subcols = []
         if len(self) > 0:
             s += ['Columns:']
-            cnames = 'name', 'type', 'dtype', 'index', 'shape'
-            s += ['  %-15s %5s %6s %-6s %s' % cnames]
-            s += ['  '+'-'*(50)]
+            cnames = 'name', 'dtype', 'index'
+            s += ['  %-15s %6s %-6s' % cnames]
+            s += ['  '+'-'*(28)]
+
+            dicts = ['Dictionaries:']
+            dicts += ['  %-15s' % ('name',)]
+            dicts += ['  '+'-'*(28)]
 
             subcols = ['Sub-Columns Directories:']
             subcols += ['  %-15s' % ('name',)]
-            subcols += ['  '+'-'*(50)]
+            subcols += ['  '+'-'*(28)]
 
             for name in sorted(self):
                 c = self[name]
                 if isinstance(c, ColumnBase):
 
                     name = c.name
 
                     if len(name) > 15:
-                        s += ['  %s' % name]
-                        s += ['%23s' % (c.type,)]
+                        name_entry = ['  %s' % name]
+                        # s += ['%23s' % (c.type,)]
                     else:
-                        s += ['  %-15s %5s' % (c.name, c.type)]
+                        name_entry = ['  %-15s' % c.name]
 
                     if c.type == 'array':
+                        s += name_entry
                         c_dtype = c.dtype.descr[0][1]
                         s[-1] += ' %6s' % c_dtype
                         s[-1] += ' %-6s' % self[name].has_index
-                        s[-1] += ' %s' % (self[name].shape,)
-
+                        # s[-1] += ' %s' % self[name].nrows
+                    elif c.type == 'dict':
+                        dicts += name_entry
+                    else:
+                        raise ValueError(f'bad type: {c.type}')
                 else:
                     cdir = os.path.basename(c.dir).replace('.cols', '')
                     subcols += ['  %s' % cdir]
 
         s = [indent + tmp for tmp in s]
         s = ['Columns Directory: '] + s
 
+        if len(dicts) > 3:
+            s += [indent]
+            dicts = [indent + tmp for tmp in dicts]
+            s += dicts
+
         if len(subcols) > 3:
             s += [indent]
             subcols = [indent + tmp for tmp in subcols]
             s += subcols
 
         return s
```

### Comparing `pycolumns-0.9.2/pycolumns/indices.py` & `pycolumns-1.0.0/pycolumns/indices.py`

 * *Files 17% similar despite different names*

```diff
@@ -23,15 +23,18 @@
         Indices([4, 5])
         >>> (i1 | i2)
         Indices([3, 4, 5, 6])
 
     """
     def __new__(self, init_data, copy=False):
         self._is_sorted = False
-        arr = np.array(init_data, copy=copy)
+
+        # always force native byte order since we send this to C code
+        # when using fitsio
+        arr = np.array(init_data, dtype='i8', copy=copy)
         shape = arr.shape
 
         ret = np.ndarray.__new__(self, shape, arr.dtype,
                                  buffer=arr)
         return ret
 
     @property
```

### Comparing `pycolumns-0.9.2/pycolumns/sfile.py` & `pycolumns-1.0.0/pycolumns/sfile.py`

 * *Files identical despite different names*

### Comparing `pycolumns-0.9.2/pycolumns/tests/test_create.py` & `pycolumns-1.0.0/pycolumns/tests/test_create.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,27 +16,29 @@
     num = 20
 
     rng = np.random.RandomState(seed)
 
     with tempfile.TemporaryDirectory() as tmpdir:
         cdir = os.path.join(tmpdir, 'test.cols')
         cols = Columns(cdir, cache_mem=cache_mem, verbose=verbose)
-        assert len(cols.colnames) == 0
+        assert len(cols.names) == 0
 
         assert cols.dir == cdir
         assert cols.verbose == verbose
         assert cols.cache_mem == cache_mem
 
-        data = np.zeros(num, dtype=[('id', 'i8'), ('rand', 'f4')])
+        dtype = [('id', 'i8'), ('rand', 'f4'), ('scol', 'U5')]
+        data = np.zeros(num, dtype=dtype)
         data['id'] = np.arange(num)
         data['rand'] = rng.uniform(size=num)
+        data['scol'] = [str(val) for val in data['id']]
 
         cols.append(data)
 
-        assert len(cols.colnames) == len(data.dtype.names)
+        assert len(cols.names) == len(data.dtype.names)
         meta = {'version': '0.1', 'seeing': 0.9}
         cols.create_column('meta', 'dict')
         cols['meta'].write(meta)
 
         rmeta = cols['meta'].read()
         assert rmeta == meta
 
@@ -54,28 +56,29 @@
             tdata = cols[name][:]
             assert np.all(data[name] == tdata)
 
         # make sure we can append more data
         cols.append(data)
         assert cols['id'].size == num * 2
         assert cols['rand'].size == num * 2
+        assert cols['scol'].size == num * 2
 
         # don't allow appending with new columns
         with pytest.raises(ValueError):
             bad_data = np.zeros(3, dtype=[('blah', 'f4')])
             cols.append(bad_data)
 
         with pytest.raises(ValueError):
             bad_data = np.zeros(
                 3,
-                dtype=[('id', 'i8'), ('rand', 'f4'), ('extra', 'i2')],
+                dtype=dtype + [('extra', 'i2')],
             )
             cols.append(bad_data)
 
         # can currently update column at a time
-        cols['rand'][5] = 35
-        assert cols['rand'][5] == 35
+        # cols['rand'][5] = 35
+        # assert cols['rand'][5] == 35
 
-        idx = [8, 12]
-        vals = [1.0, 2.0]
-        cols['rand'][idx] = vals
-        assert np.all(cols['rand'][idx] == vals)
+        # idx = [8, 12]
+        # vals = [1.0, 2.0]
+        # cols['rand'][idx] = vals
+        # assert np.all(cols['rand'][idx] == vals)
```

### Comparing `pycolumns-0.9.2/pycolumns/tests/test_query.py` & `pycolumns-1.0.0/pycolumns/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `pycolumns-0.9.2/pycolumns/util.py` & `pycolumns-1.0.0/pycolumns/util.py`

 * *Files 18% similar despite different names*

```diff
@@ -115,7 +115,39 @@
         newdt.append(descr)
 
     new_data = np.zeros(data.size, dtype=newdt)
     for n in data.dtype.names:
         new_data[n] = data[n]
 
     return new_data
+
+
+def maybe_decode_fits_ascii_strings_to_unicode_py3(array):
+    new_dtype, do_conversion = (
+        maybe_convert_ascii_dtype_to_unicode(array.dtype)
+    )
+    if do_conversion:
+        array = array.astype(new_dtype, copy=False)
+    return array
+
+
+def maybe_convert_ascii_dtype_to_unicode(dtype):
+
+    do_conversion = False
+    new_dt = []
+    for dt in dtype.descr:
+        if 'S' in dt[1]:
+            do_conversion = True
+            if len(dt) == 3:
+                new_dt.append((
+                    dt[0],
+                    dt[1].replace('S', 'U').replace('|', ''),
+                    dt[2]))
+            else:
+                new_dt.append((
+                    dt[0],
+                    dt[1].replace('S', 'U').replace('|', '')))
+        else:
+            new_dt.append(dt)
+
+    new_dtype = np.dtype(new_dt)
+    return new_dtype, do_conversion
```

### Comparing `pycolumns-0.9.2/pycolumns.egg-info/PKG-INFO` & `pycolumns-1.0.0/pycolumns.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,171 +1,205 @@
 Metadata-Version: 2.1
 Name: pycolumns
-Version: 0.9.2
+Version: 1.0.0
 Summary: A simple, efficient, pythonic column data store
 Home-page: https://github.com/esheldon/pycolumns
 License: MIT
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENSE
 
 A simple, efficient column-oriented, pythonic data store.
 
 The focus is currently on efficiency of reading and writing.  The code is pure
-python but searching and reading data is fast due to the use of numpy memory
-maps and column indexing.  Basic consistency is ensured but the database is not
-fully ACID.
+python but searching and reading data is fast due to the use of the fitsio
+package for column data and index data.  Basic consistency is ensured for
+the columns in the table, but the database is not fully ACID.
 
 The storage is a simple directory with files on disk.
 
 Examples
 --------
 
 ```python
 >>> import pycolumns as pyc
 
 # instantiate a column database from the specified coldir
->>> c=pyc.Columns('/some/path/mycols.cols')
+>>> c = pyc.Columns('/some/path/mycols.cols')
 
 # display some info about the columns
 >>> c
-Column Directory:
+Columns Directory:
 
+  mydata
   dir: /some/path/mydata.cols
+  nrows: 64348146
   Columns:
-    name             type  dtype index  shape
-    --------------------------------------------------
-    ccd             array    <i2 True   (64348146,)
-    dec             array    <f8 False  (64348146,)
-    exposurename    array   |S20 True   (64348146,)
-    id              array    <i8 False  (64348146,)
-    imag            array    <f4 False  (64348146,)
-    ra              array    <f8 False  (64348146,)
-    x               array    <f4 False  (64348146,)
-    y               array    <f4 False  (64348146,)
-    g               array    <f8 False  (64348146, 2)
-    meta             dict
+    name             dtype index
+    -----------------------------
+    ccd                <i2 True
+    dec                <f8 False
+    exposurename      |S20 True
+    id                 <i8 True
+    imag               <f4 False
+    ra                 <f8 False
+    x                  <f4 False
+    y                  <f4 False
+    g                  <f8 False
 
+  Dictionaries
+    name
+    -----------------------------
+    meta
 
-  Sub-Column Directories:
+  Sub-Columns Directories:
     name
-    --------------------------------------------------
+    -----------------------------
     psfstars
 
 # display info about column 'id'
 >>> c['id']
 Column:
-  "id"
+  name: id
   filename: ./id.array
-  type: col
-  shape: (64348146,)
-  has index: False
+  type: array
   dtype: <i8
+  has index: False
+  nrows: 64348146
 
-# get the column names
->>> c.colnames
-['ccd', 'dec', 'exposurename', 'id', 'imag', 'ra', 'x', 'y', 'g', 'meta']
+# number of rows in table
+>>> c.nrows
 
-# reload all columns or specified column/column list
->>> c.reload(name=None)
+# read all columns into a single rec array.  By default the dict
+# columns are not loaded
 
-# read all data from array column 'id'
-# alternative syntaxes, including numpy style slicing
+>>> data = c.read()
+
+# using asdict=True puts the data into a dict.  The dict data
+# are also loaded in this case
+>>> data = c.read(asdict=True)
+
+# specify columns
+>>> data = c.read(columns=['id', 'flux'])
+
+# dict columns can be specified if asdict is True.  Dicts can also
+# be read as single columns, see below
+>>> data = c.read(columns=['id', 'flux', 'meta'], asdict=True)
+
+# specifying a set of rows as sequence/array or slice
+>>> data = c.read(columns=['id', 'flux'], rows=[3, 225, 1235])
+>>> data = c.read(columns=['id', 'flux'], rows=slice(10, 20))
+
+# read all data from column 'id' as an array rather than recarray
+# alternative syntaxes
 >>> ind = c['id'][:]
 >>> ind = c['id'].read()
 >>> ind = c.read_column('id')
 
-# dict columns are read as a dict. No slicing for dicts
->>> meta = c['meta'].read()
-
 # read a subset of rows
 # slicing
 >>> ind = c['id'][25:125]
 
 # specifying a set of rows
->>> rows=[3, 225, 1235]
+>>> rows = [3, 225, 1235]
 >>> ind = c['id'][rows]
 >>> ind = c.read_column('id', rows=rows)
 
-# read all columns into a single rec array.  By default the dict
-# columns are not loaded
-
->>> data = c.read()
-
-# using asdict=True puts the data into a dict.  The dict data
-# are loaded in this case
->>> data = c.read(asdict=True)
-
-# specify columns
->>> data = c.read(columns=['id', 'flux'], rows=rows)
-
-# dict columns can be specified if asdict is True
->>> data = c.read(columns=['id', 'flux', 'meta'], asdict=True)
+# reading a dictionary column
+>>> meta = c['meta'].read()
 
 # Create indexes for fast searching
 >>> c['id'].create_index()
 
-# get indices for some condition
+# get indices for some conditions
 >>> ind = c['id'] > 25
 >>> ind = c['id'].between(25, 35)
 >>> ind = c['id'] == 25
 
-# find all matches
->>> ind = c['id'].match([35, 77])
-
 # read the corresponding data
 >>> ccd = c['ccd'][ind]
 >>> data = c.read(columns=['ra', 'dec'], rows=ind)
 
 # composite searches over multiple columns
 >>> ind = (c['id'] == 25) & (col['ra'] < 15.23)
 >>> ind = c['id'].between(15, 25) | (c['id'] == 55)
 >>> ind = c['id'].between(15, 250) & (c['id'] != 66) & (c['ra'] < 100)
->>> ind = c['id'].between(15, 250) & c['id'].match([35, 99])
 
-# speed up reads by sorting indices
->>> ind.sort()
->>> data = c.read(columns=['ra', 'dec'], rows=ind)
+# write columns from the fields in a rec array names in the data correspond
+# to column names.  If this is the first time writing data, the columns are
+# created, and on subsequent writes, the columns must match
+
+>>> c.append(recdata)
+>>> c.append(new_data)
+
+# append data from the fields in a FITS file
+>>> c.from_fits(fitsfile_name)
 
-# you can check if the index is already sorted
->>> if not ind.is_sorted:
->>>    ind.sort()
+# add a dictionary column.
+>>> c.create_column('weather', 'dict')
+>>> c['weather'].write({'temp': 30.1, 'humid': 0.5})
+
+# overwrite dict column
+>>> c['weather'].write({'temp': 33.2, 'humid': 0.3, 'windspeed': 60.5})
+
+# you should not generally create array columns, since they
+# can get out of sync with existing columns.  This will by default
+# raise an exception, but you can send verify=False if you know
+# what you are doing.  In the future special support will be added for
+# adding new columns
+>>> c.create_column('test', 'array')
 
-# update values for a column
+# update values for an array column
 >>> c['id'][35] = 10
 >>> c['id'][35:35+3] = [8, 9, 10]
 >>> c['id'][rows] = idvalues
 
-# write multiple columns from the fields in a rec array
-# names in the data correspond to column names.
-# If columns are not present, they are created
-# but row count consistency must be maintained for all array
-# columns and this is checked.
+# get all names, including dictionary and sub Columns
+# same as list(c.keys())
+>>> c.names
+['ccd', 'dec', 'exposurename', 'id', 'imag', 'ra', 'x', 'y', 'g',
+ 'meta', 'psfstars']
+
+# only array column names
+>>> c.column_names
+['ccd', 'dec', 'exposurename', 'id', 'imag', 'ra', 'x', 'y', 'g']
+
+# only dict columns
+>>> c.dict_names
+['meta', 'weather']
+
+# only sub Columns directories
+>>> c.subcols_names
+['psfstars']
 
->>> c.append(recdata)
+# reload all columns or specified column/column list
+>>> c.reload()
 
-# append data from the fields in a FITS file
->>> c.from_fits(fitsfile_name)
+# delete all data.  This will ask for confirmation
+>>> c.delete()
+
+# delete column and its data
+>>> c.delete_column('ra')
 
-# add a dict column
->>> c.create_column('meta')
->>> c['meta'].write({'test': 'hello'})
->>> d = c['meta'].read()
-
-# heirarchical sets of columns are also supported
->>> c['psfstars']
-Column Directory:
+# to configure the amount of memory used during index creation, specify
+# cache_mem in gigabytes.  Default 1 gig
+>>> cols = pyc.Columns(fname, cache_mem=0.5)
 
+# columns can actually be another pycolumns directory
+>>> psfcols = cols['psfstars']
+>>> psfcols
   dir: /some/path/mydata.cols/psfstars.cols
   Columns:
     name             type  dtype index  shape
     --------------------------------------------------
-    ccd             array    <i2 True   (348146,)
-    exposurename    array   |S20 True   (348146,)
-    x               array    <f4 False  (348146,)
-    y               array    <f4 False  (348146,)
+    ccd             array    <i2 True   (64348146,)
+    id              array    <i8 True   (64348146,)
+    imag            array    <f4 False  (64348146,)
+    x               array    <f4 False  (64348146,)
+    y               array    <f4 False  (64348146,)
+    ...etc
 ```
 
 Dependencies
 ------------
 numpy
```

### Comparing `pycolumns-0.9.2/setup.py` & `pycolumns-1.0.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,9 +19,10 @@
     packages=find_packages(),
     license='MIT',
     url='https://github.com/esheldon/pycolumns',
     version=__version__,
     description='A simple, efficient, pythonic column data store',
     long_description=long_description,
     long_description_content_type='text/markdown; charset=UTF-8; variant=GFM',
-    install_requires=['numpy'],
+    setup_requires=['numpy', 'fitsio'],
+    install_requires=['numpy', 'fitsio'],
 )
```

