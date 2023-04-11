# Comparing `tmp/dissect.extfs-3.4.dev3.tar.gz` & `tmp/dissect.extfs-3.5.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.extfs-3.4.dev3.tar", last modified: Thu Mar 16 13:03:35 2023, max compression
+gzip compressed data, was "dissect.extfs-3.5.dev2.tar", last modified: Tue Apr 11 14:16:10 2023, max compression
```

## Comparing `dissect.extfs-3.4.dev3.tar` & `dissect.extfs-3.5.dev2.tar`

### file list

```diff
@@ -1,32 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:03:35.480245 dissect.extfs-3.4.dev3/
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-03-16 13:03:20.000000 dissect.extfs-3.4.dev3/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-03-16 13:03:20.000000 dissect.extfs-3.4.dev3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-16 13:03:20.000000 dissect.extfs-3.4.dev3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-03-16 13:03:35.480245 dissect.extfs-3.4.dev3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-03-16 13:03:20.000000 dissect.extfs-3.4.dev3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:03:35.472245 dissect.extfs-3.4.dev3/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:03:35.476245 dissect.extfs-3.4.dev3/dissect/extfs/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-03-16 13:03:20.000000 dissect.extfs-3.4.dev3/dissect/extfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23393 2023-03-16 13:03:20.000000 dissect.extfs-3.4.dev3/dissect/extfs/c_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-03-16 13:03:20.000000 dissect.extfs-3.4.dev3/dissect/extfs/c_jdb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-03-16 13:03:20.000000 dissect.extfs-3.4.dev3/dissect/extfs/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    18307 2023-03-16 13:03:20.000000 dissect.extfs-3.4.dev3/dissect/extfs/extfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-03-16 13:03:20.000000 dissect.extfs-3.4.dev3/dissect/extfs/journal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:03:35.476245 dissect.extfs-3.4.dev3/dissect.extfs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-03-16 13:03:35.000000 dissect.extfs-3.4.dev3/dissect.extfs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-03-16 13:03:35.000000 dissect.extfs-3.4.dev3/dissect.extfs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 13:03:35.000000 dissect.extfs-3.4.dev3/dissect.extfs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-03-16 13:03:35.000000 dissect.extfs-3.4.dev3/dissect.extfs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-16 13:03:35.000000 dissect.extfs-3.4.dev3/dissect.extfs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-03-16 13:03:25.000000 dissect.extfs-3.4.dev3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-16 13:03:35.480245 dissect.extfs-3.4.dev3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:03:35.476245 dissect.extfs-3.4.dev3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 13:03:20.000000 dissect.extfs-3.4.dev3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-03-16 13:03:20.000000 dissect.extfs-3.4.dev3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:03:35.480245 dissect.extfs-3.4.dev3/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-03-16 13:03:20.000000 dissect.extfs-3.4.dev3/tests/data/ext4.bin.gz
--rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-03-16 13:03:20.000000 dissect.extfs-3.4.dev3/tests/data/ext4_symlink_test1.bin.gz
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-03-16 13:03:20.000000 dissect.extfs-3.4.dev3/tests/data/ext4_symlink_test2.bin.gz
--rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-03-16 13:03:20.000000 dissect.extfs-3.4.dev3/tests/data/ext4_symlink_test3.bin.gz
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-03-16 13:03:20.000000 dissect.extfs-3.4.dev3/tests/test_ext4.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-03-16 13:03:20.000000 dissect.extfs-3.4.dev3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:16:10.531741 dissect.extfs-3.5.dev2/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-11 14:15:55.000000 dissect.extfs-3.5.dev2/.gitattributes
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-11 14:15:55.000000 dissect.extfs-3.5.dev2/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-11 14:15:55.000000 dissect.extfs-3.5.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-11 14:15:55.000000 dissect.extfs-3.5.dev2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-04-11 14:16:10.527741 dissect.extfs-3.5.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-04-11 14:15:55.000000 dissect.extfs-3.5.dev2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:16:10.519741 dissect.extfs-3.5.dev2/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:16:10.527741 dissect.extfs-3.5.dev2/dissect/extfs/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-11 14:15:55.000000 dissect.extfs-3.5.dev2/dissect/extfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23393 2023-04-11 14:15:55.000000 dissect.extfs-3.5.dev2/dissect/extfs/c_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-04-11 14:15:55.000000 dissect.extfs-3.5.dev2/dissect/extfs/c_jdb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-11 14:15:55.000000 dissect.extfs-3.5.dev2/dissect/extfs/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19098 2023-04-11 14:15:55.000000 dissect.extfs-3.5.dev2/dissect/extfs/extfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-04-11 14:15:55.000000 dissect.extfs-3.5.dev2/dissect/extfs/journal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:16:10.523741 dissect.extfs-3.5.dev2/dissect.extfs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-04-11 14:16:10.000000 dissect.extfs-3.5.dev2/dissect.extfs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-11 14:16:10.000000 dissect.extfs-3.5.dev2/dissect.extfs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 14:16:10.000000 dissect.extfs-3.5.dev2/dissect.extfs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-11 14:16:10.000000 dissect.extfs-3.5.dev2/dissect.extfs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-11 14:16:10.000000 dissect.extfs-3.5.dev2/dissect.extfs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-04-11 14:16:00.000000 dissect.extfs-3.5.dev2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 14:16:10.531741 dissect.extfs-3.5.dev2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:16:10.527741 dissect.extfs-3.5.dev2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:15:56.000000 dissect.extfs-3.5.dev2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-11 14:15:55.000000 dissect.extfs-3.5.dev2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:16:10.527741 dissect.extfs-3.5.dev2/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-04-11 14:15:56.000000 dissect.extfs-3.5.dev2/tests/data/ext4.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-04-11 14:15:56.000000 dissect.extfs-3.5.dev2/tests/data/ext4_sparse.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-04-11 14:15:56.000000 dissect.extfs-3.5.dev2/tests/data/ext4_symlink_test1.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-04-11 14:15:56.000000 dissect.extfs-3.5.dev2/tests/data/ext4_symlink_test2.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-04-11 14:15:56.000000 dissect.extfs-3.5.dev2/tests/data/ext4_symlink_test3.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-04-11 14:15:56.000000 dissect.extfs-3.5.dev2/tests/test_ext4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-11 14:15:56.000000 dissect.extfs-3.5.dev2/tox.ini
```

### Comparing `dissect.extfs-3.4.dev3/LICENSE` & `dissect.extfs-3.5.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.4.dev3/PKG-INFO` & `dissect.extfs-3.5.dev2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.extfs
-Version: 3.4.dev3
+Version: 3.5.dev2
 Summary: A Dissect module implementing a parser for the ExtFS file system, the native filesystem for Linux operating systems
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.extfs
 Project-URL: repository, https://github.com/fox-it/dissect.extfs
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dissect.extfs-3.4.dev3/README.md` & `dissect.extfs-3.5.dev2/README.md`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.4.dev3/dissect/extfs/c_ext.py` & `dissect.extfs-3.5.dev2/dissect/extfs/c_ext.py`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.4.dev3/dissect/extfs/c_jdb2.py` & `dissect.extfs-3.5.dev2/dissect/extfs/c_jdb2.py`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.4.dev3/dissect/extfs/extfs.py` & `dissect.extfs-3.5.dev2/dissect/extfs/extfs.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,19 @@
+from __future__ import annotations
+
 import io
 import logging
 import os
 import stat
+from datetime import datetime
 from functools import lru_cache
+from typing import BinaryIO, Iterator, Optional, Union
 from uuid import UUID
 
+from dissect.cstruct import Instance
 from dissect.util import ts
 from dissect.util.stream import RangeStream, RunlistStream
 
 from dissect.extfs.c_ext import (
     EXT2,
     EXT3,
     EXT4,
@@ -26,15 +31,15 @@
 from dissect.extfs.journal import JDB2
 
 log = logging.getLogger(__name__)
 log.setLevel(os.getenv("DISSECT_LOG_EXTFS", "CRITICAL"))
 
 
 class ExtFS:
-    def __init__(self, fh):
+    def __init__(self, fh: BinaryIO):
         self.fh = fh
         # self._path_cache = {}
         self._journal = None
 
         fh.seek(c_ext.EXT2_SBOFF)
         sb = c_ext.ext4_super_block(fh)
         self.sb = sb
@@ -85,16 +90,19 @@
         self.groups_count = ((self.last_block - sb.s_first_data_block) // sb.s_blocks_per_group) + 1
 
         self.uuid = UUID(bytes=sb.s_uuid)
         self.last_mount = sb.s_last_mounted.split(b"\x00")[0].decode(errors="surrogateescape")
 
         self.root = self.get_inode(c_ext.EXT2_ROOT_INO, "/")
 
+        self.get_inode = lru_cache(1024)(self.get_inode)
+        self._read_group_desc = lru_cache(356)(self._read_group_desc)
+
     @property
-    def journal(self):
+    def journal(self) -> JDB2:
         if not self._journal:
             if not self.sb.s_feature_compat & c_ext.EXT3_FEATURE_COMPAT_HAS_JOURNAL:
                 raise Error("Journal not supported")
 
             inum = self.sb.s_journal_inum
             if inum == 0:
                 raise Error(
@@ -102,15 +110,15 @@
                 )
 
             inode = self.get_inode(inum)
             self._journal = JDB2(inode.open())
 
         return self._journal
 
-    def get(self, path, node=None):
+    def get(self, path: Union[str, int], node: Optional[INode] = None) -> INode:
         if isinstance(path, int):
             return self.get_inode(path)
 
         node = node if node else self.root
         parts = path.split("/")
         for part_num, part in enumerate(parts):
             if not part:
@@ -124,27 +132,32 @@
                     node = entry
                     break
             else:
                 raise FileNotFoundError(f"File not found: {path}")
 
         return node
 
-    @lru_cache(1024)
-    def get_inode(self, inum, filename=None, filetype=None, parent=None, lazy=False):
+    def get_inode(
+        self,
+        inum: int,
+        filename: Optional[str] = None,
+        filetype: Optional[int] = None,
+        parent: Optional[INode] = None,
+        lazy: bool = False,
+    ) -> INode:
         if inum < c_ext.EXT2_BAD_INO or inum > self.sb.s_inodes_count:
             raise Error(f"inum out of range {c_ext.EXT2_BAD_INO}-{self.sb.s_inodes_count}: {inum}")
 
         inode = INode(self, inum, filename, filetype, parent=parent)
         if not lazy:
             inode._inode = inode._read_inode()
 
         return inode
 
-    @lru_cache(256)
-    def _read_group_desc(self, group_num):
+    def _read_group_desc(self, group_num: int) -> Instance:
         if group_num >= self.groups_count:
             raise Error("Group number exceeds amount of groups")
 
         offset = self.groups_offset + group_num * self._group_desc_size
         self.fh.seek(offset)
         group_desc = self._group_desc_struct(self.fh)
 
@@ -160,15 +173,22 @@
         if block_bitmap > self.last_block or inode_bitmap > self.last_block or table_block > self.last_block:
             raise Error("Group descriptor block locations exceed last block")
 
         return group_desc
 
 
 class INode:
-    def __init__(self, extfs, inum, filename=None, filetype=None, parent=None):
+    def __init__(
+        self,
+        extfs: ExtFS,
+        inum: int,
+        filename: Optional[str] = None,
+        filetype: Optional[int] = None,
+        parent: Optional[INode] = None,
+    ):
         self.extfs = extfs
         self.inum = inum
         self.parent = parent
         self._inode = None
 
         self.filename = filename
         self._filetype = filetype
@@ -176,157 +196,158 @@
         self._link = None
         self._link_inode = None
         self._xattr = None
 
         self._dirlist = None
         self._runlist = None
 
-    def _read_inode(self):
+    def __repr__(self) -> str:
+        return f"<inode {self.inum}>"
+
+    def _read_inode(self) -> Instance:
         block_group_num, index = divmod(self.inum - 1, self.extfs.sb.s_inodes_per_group)
         block_group = self.extfs._read_group_desc(block_group_num)
 
         if self.extfs._group_desc_struct == c_ext.ext4_group_desc:
             table_block = (block_group.bg_inode_table_hi << 32) | block_group.bg_inode_table_lo
         else:
             table_block = block_group.bg_inode_table_lo
 
         offset = table_block * self.extfs.block_size + index * self.extfs.sb.s_inode_size
         self.extfs.fh.seek(offset)
         return c_ext.ext4_inode(self.extfs.fh)
 
     @property
-    def inode(self):
+    def inode(self) -> Instance:
         if not self._inode:
             self._inode = self._read_inode()
         return self._inode
 
     @property
-    def size(self):
+    def size(self) -> int:
         if not self._size:
             self._size = (self.inode.i_size_high << 32) + self.inode.i_size_lo
         return self._size
 
     @property
-    def filetype(self):
+    def filetype(self) -> int:
         if not self._filetype:
             self._filetype = stat.S_IFMT(self.inode.i_mode)
         return self._filetype
 
     @property
-    def link(self):
+    def link(self) -> str:
         if self.filetype != stat.S_IFLNK:
             raise NotASymlinkError(f"{self!r} is not a symlink")
 
         if not self._link:
             self._link = self.open().read().decode(errors="surrogateescape")
         return self._link
 
     @property
-    def link_inode(self):
+    def link_inode(self) -> INode:
         if not self._link_inode:
             # Relative lookups work because . and .. are actual directory entries
             link = self.link
             if link.startswith("/"):
                 relnode = None
             else:
                 relnode = self.parent
             self._link_inode = self.extfs.get(self.link, relnode)
         return self._link_inode
 
     @property
-    def xattr(self):
+    def xattr(self) -> list[XAttr]:
         if not self._xattr:
             xattr = []
 
             if self.inode.i_extra.strip(b"\x00"):
                 buf = io.BytesIO(self.inode.i_extra)
                 hdr = c_ext.ext4_xattr_ibody_header(buf)
                 if hdr.h_magic != c_ext.EXT4_XATTR_MAGIC:
                     raise Error("Invalid xattr magic value")
 
-                for entry in _iter_xattr(self, buf, len(self.inode.i_extra), 4):
-                    xattr.append(entry)
+                xattr.extend(_iter_xattr(self, buf, len(self.inode.i_extra), 4))
 
             if self.inode.i_file_acl_lo:
                 block = (self.inode.i_file_acl_high << 32) | self.inode.i_file_acl_lo
                 block_offset = block * self.extfs.block_size
 
                 buf = RangeStream(self.extfs.fh, block_offset, self.extfs.block_size)
                 hdr = c_ext.ext4_xattr_header(buf)
                 if hdr.h_magic != c_ext.EXT4_XATTR_MAGIC:
                     raise Error("Invalid xattr magic value")
 
-                for entry in _iter_xattr(self, buf, buf.size):
-                    xattr.append(entry)
+                xattr.extend(_iter_xattr(self, buf, buf.size))
 
             self._xattr = xattr
         return self._xattr
 
     @property
-    def atime(self):
+    def atime(self) -> datetime:
         return ts.from_unix_ns(self.atime_ns)
 
     @property
-    def atime_ns(self):
+    def atime_ns(self) -> int:
         time = self.inode.i_atime
         time_extra = self.inode.i_atime_extra if self.extfs.sb.s_inode_size > 128 else 0
 
         return _parse_ns_ts(time, time_extra)
 
     @property
-    def mtime(self):
+    def mtime(self) -> datetime:
         return ts.from_unix_ns(self.mtime_ns)
 
     @property
-    def mtime_ns(self):
+    def mtime_ns(self) -> int:
         time = self.inode.i_mtime
         time_extra = self.inode.i_mtime_extra if self.extfs.sb.s_inode_size > 128 else 0
 
         return _parse_ns_ts(time, time_extra)
 
     @property
-    def ctime(self):
+    def ctime(self) -> datetime:
         return ts.from_unix_ns(self.ctime_ns)
 
     @property
-    def ctime_ns(self):
+    def ctime_ns(self) -> int:
         time = self.inode.i_ctime
         time_extra = self.inode.i_ctime_extra if self.extfs.sb.s_inode_size > 128 else 0
 
         return _parse_ns_ts(time, time_extra)
 
     @property
-    def dtime(self):
+    def dtime(self) -> datetime:
         return ts.from_unix(self.inode.i_dtime)
 
     @property
-    def crtime(self):
+    def crtime(self) -> Optional[datetime]:
         time_ns = self.crtime_ns
         if time_ns is None:
             return None
         return ts.from_unix_ns(time_ns)
 
     @property
-    def crtime_ns(self):
+    def crtime_ns(self) -> Optional[int]:
         if self.extfs.sb.s_inode_size <= 128:
             return None
 
         time = self.inode.i_crtime
         time_extra = self.inode.i_crtime_extra
 
         return _parse_ns_ts(time, time_extra)
 
-    def listdir(self):
+    def listdir(self) -> dict[str, INode]:
         if not self._dirlist:
             self._dirlist = {node.filename: node for node in self.iterdir()}
         return self._dirlist
 
     dirlist = listdir
 
-    def iterdir(self):
+    def iterdir(self) -> Iterator[INode]:
         if self.filetype != stat.S_IFDIR:
             raise NotADirectoryError(f"{self!r} is not a directory")
 
         buf = self.open()
         offset = 0
 
         while offset < self.size - 12:
@@ -345,43 +366,43 @@
                     ftype = FILETYPES[ftype]
 
                 yield self.extfs.get_inode(direntry.inode, fname, ftype, parent=self, lazy=True)
 
             offset += direntry.rec_len
             buf.seek(offset)
 
-    def dataruns(self):
+    def dataruns(self) -> list[tuple[Optional[int], int]]:
         if not self._runlist:
+            expected_runs = (self.size + self.extfs.block_size - 1) // self.extfs.block_size
+
             if self.inode.i_flags & c_ext.EXT4_EXTENTS_FL:
                 buf = io.BytesIO(self.inode.i_block)
 
                 runs = []
                 run_offset = 0
-                extents = list(_parse_extents(self, buf))
 
-                if not extents:
-                    # Completely sparse run
-                    runs = [(None, (self.size + self.extfs.block_size - 1) // self.extfs.block_size)]
-                else:
-                    for extent in extents:
-                        # Account for uninitialized extents
-                        if extent.ee_len > 0x8000:
-                            uninitialized_gap = extent.ee_len - 0x8000
-                            runs.append((None, uninitialized_gap))
-                            run_offset += uninitialized_gap
-                            continue
+                for extent in _parse_extents(self, buf):
+                    # Account for uninitialized extents
+                    if extent.ee_len > 0x8000:
+                        uninitialized_gap = extent.ee_len - 0x8000
+                        runs.append((None, uninitialized_gap))
+                        run_offset += uninitialized_gap
+                        continue
+
+                    # Account for sparse gaps
+                    if extent.ee_block != run_offset:
+                        sparse_gap = extent.ee_block - run_offset
+                        runs.append((None, sparse_gap))
+                        run_offset += sparse_gap
 
-                        # Account for sparse gaps
-                        if extent.ee_block != run_offset:
-                            sparse_gap = extent.ee_block - run_offset
-                            runs.append((None, sparse_gap))
-                            run_offset += sparse_gap
+                    runs.append(((extent.ee_start_hi << 32) | extent.ee_start_lo, extent.ee_len))
+                    run_offset += extent.ee_len
 
-                        runs.append(((extent.ee_start_hi << 32) | extent.ee_start_lo, extent.ee_len))
-                        run_offset += extent.ee_len
+                if run_offset < expected_runs:
+                    runs.append((None, expected_runs - run_offset))
 
                 self._runlist = runs
             else:
                 i_blocks = c_ext.uint32[15](self.inode.i_block)
                 num_blocks = (self.size + self.extfs.block_size - 1) // self.extfs.block_size
                 num_direct_blocks = min(num_blocks, c_ext.EXT2_NDIR_BLOCKS)
 
@@ -413,49 +434,46 @@
                         else:
                             if run_offset == 0:
                                 runs.append((None, run_size))
                             else:
                                 runs.append((run_offset, run_size))
                             run_offset = block
                             run_size = 1
-                    else:
-                        runs.append((run_offset, run_size))
+
+                    runs.append((run_offset, run_size))
 
                 self._runlist = runs
 
         return self._runlist
 
-    def open(self):
+    def open(self) -> BinaryIO:
         if self.inode.i_flags & c_ext.EXT4_INLINE_DATA_FL or self.filetype == stat.S_IFLNK and self.size < 60:
             buf = io.BytesIO(memoryview(self.inode.i_block)[: self.size])
             # Need to add a size attribute to maintain compatibility with dissect streams
             buf.size = self.size
             return buf
         return RunlistStream(self.extfs.fh, self.dataruns(), self.size, self.extfs.block_size)
 
-    def __repr__(self):
-        return f"<inode {self.inum}>"
-
 
 class XAttr:
-    def __init__(self, extfs, inode, entry, value):
+    def __init__(self, extfs: ExtFS, inode: INode, entry: Instance, value: bytes):
         self.extfs = extfs
         self.inode = inode
         self.entry = entry
 
         self.prefix = XATTR_PREFIX_MAP.get(entry.e_name_index, "unknown_prefix")
         self._name = XATTR_NAME_MAP.get(entry.e_name_index, entry.e_name.decode(errors="surrogateescape"))
         self.name = self.prefix + self._name
         self.value = value
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f"<xattr name={self.name} value={self.value} inode={self.inode}>"
 
 
-def _parse_indirect(inode, offset, num_blocks, level):
+def _parse_indirect(inode: INode, offset: int, num_blocks: int, level: int) -> list[int]:
     offsets_per_block = inode.extfs.block_size // 4
 
     if level == 1:
         read_blocks = min(num_blocks, offsets_per_block)
         inode.extfs.fh.seek(offset * inode.extfs.block_size)
         return c_ext.uint32[read_blocks](inode.extfs.fh)
     else:
@@ -471,15 +489,15 @@
             parsed_blocks = _parse_indirect(inode, addr, num_blocks, level - 1)
             num_blocks -= len(parsed_blocks)
             blocks.extend(parsed_blocks)
 
         return blocks
 
 
-def _parse_extents(inode, buf):
+def _parse_extents(inode: INode, buf: bytes) -> Iterator[Instance]:
     extent_header = c_ext.ext4_extent_header(buf)
 
     if extent_header.eh_magic != 0xF30A:
         raise Error("Invalid extent_header magic")
 
     if extent_header.eh_depth == 0:
         for _ in range(extent_header.eh_entries):
@@ -489,19 +507,18 @@
         for _ in range(extent_header.eh_entries):
             idx = c_ext.ext4_extent_idx(buf)
             child = (idx.ei_leaf_hi << 32) | idx.ei_leaf_lo
 
             fh = inode.extfs.fh
             fh.seek(child * inode.extfs.block_size)
             blockbuf = io.BytesIO(fh.read(inode.extfs.block_size))
-            for extent in _parse_extents(inode, blockbuf):
-                yield extent
+            yield from _parse_extents(inode, blockbuf)
 
 
-def _iter_xattr(inode, buf, end, value_offset=0):
+def _iter_xattr(inode: INode, buf: BinaryIO, end: int, value_offset: int = 0) -> Iterator[XAttr]:
     offset = buf.tell()
     while True:
         try:
             if offset > end:
                 break
 
             buf.seek(offset)
@@ -519,14 +536,14 @@
             yield XAttr(inode.extfs, inode, entry, value)
 
             offset += (len(entry) + c_ext.EXT4_XATTR_ROUND) & (~c_ext.EXT4_XATTR_ROUND & 0xFFFFFFFF)
         except EOFError:
             break
 
 
-def _parse_ns_ts(time, time_extra):
+def _parse_ns_ts(time: int, time_extra: int) -> int:
     # The low 2 bits of time_extra are used to extend the time field
     # The remaining 30 bits are nanoseconds
     time |= (time_extra & 0b11) << 32
     ns = time_extra >> 2
 
     return (time * 1000000000) + ns
```

### Comparing `dissect.extfs-3.4.dev3/dissect/extfs/journal.py` & `dissect.extfs-3.5.dev2/dissect/extfs/journal.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,52 @@
+from __future__ import annotations
+
 import datetime
 import io
+from typing import BinaryIO, Iterator, Optional
 
+from dissect.cstruct import Instance
 from dissect.util.stream import RangeStream
 
 from dissect.extfs.c_jdb2 import c_jdb2
 from dissect.extfs.exceptions import Error
 
 
 class JDB2:
-    def __init__(self, fh):
+    def __init__(self, fh: BinaryIO):
         self.fh = fh
 
         sb = c_jdb2.journal_superblock(self.fh)
         self.sb = sb
 
         if sb.s_header.h_magic != c_jdb2.JBD2_MAGIC_NUMBER:
             raise Error("Not a valid JDB2 journal (magic mismatch)")
 
         self.block_size = sb.s_blocksize
         self._blocktag = c_jdb2.journal_block_tag
         if sb.s_feature_incompat & c_jdb2.JBD2_FEATURE_INCOMPAT_CSUM_V3:
             self._blocktag = c_jdb2.journal_block_tag3
 
-    def read_block(self, block, count=1):
+    def read_block(self, block: int, count: int = 1) -> bytes:
         offset = block * self.block_size
         self.fh.seek(offset)
         return self.fh.read(self.block_size * count)
 
-    def commits(self):
+    def commits(self) -> Iterator[CommitBlock]:
         cur_seq = None
 
         for block in self.commits_all():
             if not cur_seq:
                 cur_seq = block.sequence
 
             if block.sequence == cur_seq:
                 cur_seq += 1
                 yield block
 
-    def commits_all(self):
+    def commits_all(self) -> Iterator[CommitBlock]:
         desc_buf = {}
 
         for block in self.walk():
             if isinstance(block, DescriptorBlock):
                 if block.sequence not in desc_buf:
                     desc_buf[block.sequence] = []
 
@@ -51,15 +55,15 @@
                 block.descriptors = desc_buf.get(block.sequence, [])
 
                 if block.sequence in desc_buf:
                     del desc_buf[block.sequence]
 
                 yield block
 
-    def walk(self):
+    def walk(self) -> Iterator[CommitBlock]:
         block_num = self.sb.s_first
 
         while block_num < self.sb.s_maxlen - 1:
             offset = block_num * self.block_size
             self.fh.seek(offset)
 
             header = c_jdb2.journal_header(self.fh)
@@ -75,65 +79,67 @@
             elif header.h_blocktype == c_jdb2.JBD2_REVOKE_BLOCK:
                 pass
 
             block_num += 1
 
 
 class DescriptorBlock:
-    def __init__(self, jdb2, header, block):
+    def __init__(self, jdb2: JDB2, header: Instance, block: int):
         self.jdb2 = jdb2
         self.header = header
         self.journal_block = block
 
         self.sequence = self.header.h_sequence
 
-    def tags(self):
+    def __repr__(self) -> str:
+        return f"<descriptor_block sequence={self.sequence} journal_block={self.journal_block}>"
+
+    def tags(self) -> Iterator[DescriptorBlockTag]:
         self.jdb2.fh.seek((self.journal_block * self.jdb2.block_size) + c_jdb2.journal_header.size)
 
         block_count = 1
         while True:
             tag = self.jdb2._blocktag(self.jdb2.fh)
             yield DescriptorBlockTag(self, tag, self.journal_block + block_count)
 
             if tag.t_flags & c_jdb2.JBD2_FLAG_LAST_TAG:
                 break
 
             if not tag.t_flags & c_jdb2.JBD2_FLAG_SAME_UUID:
                 self.jdb2.fh.seek(16, io.SEEK_CUR)
             block_count += 1
 
-    def __repr__(self):
-        return f"<descriptor_block sequence={self.sequence} journal_block={self.journal_block}>"
-
 
 class DescriptorBlockTag:
-    def __init__(self, descriptor, tag, journal_block):
+    def __init__(self, descriptor: DescriptorBlock, tag: Instance, journal_block: int):
         self.descriptor = descriptor
         self.tag = tag
         self.journal_block = journal_block
 
         self.block = (self.tag.t_blocknr_high << 32) | self.tag.t_blocknr
 
-    def open(self):
+    def __repr__(self) -> str:
+        return f"<block_tag block={self.block} journal_block={self.journal_block} flags=0x{self.tag.t_flags:x}>"
+
+    def open(self) -> BinaryIO:
         block_size = self.descriptor.jdb2.block_size
         return RangeStream(self.descriptor.jdb2.fh, self.journal_block * block_size, block_size)
 
-    def __repr__(self):
-        return f"<block_tag block={self.block} journal_block={self.journal_block} flags=0x{self.tag.t_flags:x}>"
-
 
 class CommitBlock:
-    def __init__(self, jdb2, header, journal_block, descriptors=None):
+    def __init__(
+        self, jdb2: JDB2, header: Instance, journal_block: int, descriptors: Optional[list[DescriptorBlock]] = None
+    ):
         self.jdb2 = jdb2
         self.header = header
         self.journal_block = journal_block
         self.descriptors = descriptors if descriptors else []
 
         self.sequence = self.header.h_sequence
         self.ts = datetime.datetime.utcfromtimestamp(self.header.h_commit_sec)
         self.ts += datetime.timedelta(microseconds=self.header.h_commit_nsec // 1000)
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return (
             f"<commit sequence={self.sequence} journal_block={self.journal_block} "
             f"ts={self.ts} num_descriptors={len(self.descriptors)}>"
         )
```

### Comparing `dissect.extfs-3.4.dev3/dissect.extfs.egg-info/PKG-INFO` & `dissect.extfs-3.5.dev2/dissect.extfs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.extfs
-Version: 3.4.dev3
+Version: 3.5.dev2
 Summary: A Dissect module implementing a parser for the ExtFS file system, the native filesystem for Linux operating systems
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.extfs
 Project-URL: repository, https://github.com/fox-it/dissect.extfs
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dissect.extfs-3.4.dev3/dissect.extfs.egg-info/SOURCES.txt` & `dissect.extfs-3.5.dev2/dissect.extfs.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+.gitattributes
 COPYRIGHT
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 tox.ini
 dissect.extfs.egg-info/PKG-INFO
@@ -15,10 +16,11 @@
 dissect/extfs/exceptions.py
 dissect/extfs/extfs.py
 dissect/extfs/journal.py
 tests/__init__.py
 tests/conftest.py
 tests/test_ext4.py
 tests/data/ext4.bin.gz
+tests/data/ext4_sparse.bin.gz
 tests/data/ext4_symlink_test1.bin.gz
 tests/data/ext4_symlink_test2.bin.gz
 tests/data/ext4_symlink_test3.bin.gz
```

### Comparing `dissect.extfs-3.4.dev3/pyproject.toml` & `dissect.extfs-3.5.dev2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.4.dev3/tests/data/ext4.bin.gz` & `dissect.extfs-3.5.dev2/tests/data/ext4.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.4.dev3/tests/data/ext4_symlink_test1.bin.gz` & `dissect.extfs-3.5.dev2/tests/data/ext4_symlink_test1.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.4.dev3/tests/data/ext4_symlink_test2.bin.gz` & `dissect.extfs-3.5.dev2/tests/data/ext4_symlink_test2.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.4.dev3/tests/data/ext4_symlink_test3.bin.gz` & `dissect.extfs-3.5.dev2/tests/data/ext4_symlink_test3.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.4.dev3/tests/test_ext4.py` & `dissect.extfs-3.5.dev2/tests/test_ext4.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,86 +1,109 @@
 import datetime
 import gzip
 import stat
 from io import BytesIO
+from logging import Logger
+from typing import BinaryIO
 from unittest.mock import call, patch
 
 import pytest
 
-from dissect.extfs import INode, c_ext, extfs
+from dissect.extfs.c_ext import c_ext
+from dissect.extfs.extfs import EXT4, ExtFS, INode
 
 
-def test_ext4(ext4_simple):
-    e = extfs.ExtFS(ext4_simple)
+def test_ext4(ext4_bin: BinaryIO):
+    extfs = ExtFS(ext4_bin)
 
-    assert e.type == extfs.EXT4
-    assert e.block_count == 2048
-    assert e.groups_count == 1
-    assert e.groups_offset == 2048
-    assert e._group_desc_size == 64
-    assert str(e.uuid) == "ab98e08e-e2da-4bc9-bfc6-1ac5eafb1001"
-    assert e.last_mount == "/tmp/mnt"
+    assert extfs.type == EXT4
+    assert extfs.block_count == 2048
+    assert extfs.groups_count == 1
+    assert extfs.groups_offset == 2048
+    assert extfs._group_desc_size == 64
+    assert str(extfs.uuid) == "ab98e08e-e2da-4bc9-bfc6-1ac5eafb1001"
+    assert extfs.last_mount == "/tmp/mnt"
 
-    root = e.root
+    root = extfs.root
     assert root.size == 1024
     assert root.filetype == stat.S_IFDIR
     assert root.filename == "/"
     assert sorted(root.dirlist().keys()) == [".", "..", "lost+found", "test_file", "xattr_cap"]
 
-    inode = e.get("test_file")
+    inode = extfs.get("test_file")
     assert inode.size == 26
     assert inode.filetype == stat.S_IFREG
     assert inode.filename == "test_file"
     assert inode.open().read() == b"dissect test file in ext4\n"
 
     assert inode.atime == datetime.datetime(2018, 5, 29, 8, 57, 58, tzinfo=datetime.timezone.utc)
     assert inode.atime_ns == 1527584278000000000
 
-    assert e.journal
-    assert len(list(e.journal.commits())) == 2
+    assert extfs.journal
+    assert len(list(extfs.journal.commits())) == 2
 
 
-def test_xattr(ext4_simple):
-    e = extfs.ExtFS(ext4_simple)
+def test_xattr(ext4_bin: BinaryIO):
+    e = ExtFS(ext4_bin)
 
     inode = e.get("xattr_cap")
 
     xattrs = inode.xattr
     assert len(xattrs) == 2
     assert xattrs[0].name == "security.selinux"
     assert xattrs[0].value == b"unconfined_u:object_r:unlabeled_t:s0\x00"
     assert xattrs[1].name == "security.capability"
     assert xattrs[1].value == b"\x01\x00\x00\x02\x00\x04@\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00"
 
 
+def test_sparse(ext4_sparse_bin: BinaryIO):
+    extfs = ExtFS(ext4_sparse_bin)
+
+    sparse_start = extfs.get("sparse_start")
+    assert sparse_start.size == 0x3C000
+    assert sparse_start.dataruns() == [(None, 160), (1833, 80)]
+
+    sparse_hole = extfs.get("sparse_hole")
+    assert sparse_hole.size == 0x3C000
+    assert sparse_hole.dataruns() == [(1537, 80), (None, 80), (1697, 80)]
+
+    sparse_end = extfs.get("sparse_end")
+    assert sparse_end.size == 0x28000
+    assert sparse_end.dataruns() == [(1793, 40), (None, 120)]
+
+    sparse_all = extfs.get("sparse_all")
+    assert sparse_all.size == 0x500000
+    assert sparse_all.dataruns() == [(None, 5120)]
+
+
 @pytest.mark.parametrize(
     "image_file",
     [
         ("tests/data/ext4_symlink_test1.bin.gz"),
         ("tests/data/ext4_symlink_test2.bin.gz"),
         ("tests/data/ext4_symlink_test3.bin.gz"),
     ],
 )
-def test_symlinks(image_file):
+def test_symlinks(image_file: str):
     path = "/path/to/dir/with/file.ext"
     expect = b"resolved!\n"
 
     def resolve(node):
         while node.filetype == stat.S_IFLNK:
             node = node.link_inode
         return node
 
     with gzip.open(image_file, "rb") as disk:
-        assert resolve(extfs.ExtFS(disk).get(path)).open().read() == expect
+        assert resolve(ExtFS(disk).get(path)).open().read() == expect
 
 
 @patch("dissect.extfs.extfs.INode.open", return_value=BytesIO(b"\x00" * 16))
 @patch("dissect.extfs.extfs.log", create=True, return_value=None)
 @patch("dissect.extfs.extfs.ExtFS")
-def test_infinite_loop_protection(ExtFS, log, *args):
+def test_infinite_loop_protection(ExtFS: ExtFS, log: Logger, *args):
     ExtFS.sb.s_inodes_count = 69
-    ExtFS._dirtype = c_ext.c_ext.ext2_dir_entry_2
+    ExtFS._dirtype = c_ext.ext2_dir_entry_2
     inode = INode(ExtFS, 1, filetype=stat.S_IFDIR)
     inode._size = 16
     for _ in inode.iterdir():
         pass
     assert call.critical("Zero-length directory entry in %s (offset 0x%x)", inode, 0) in log.mock_calls
```

### Comparing `dissect.extfs-3.4.dev3/tox.ini` & `dissect.extfs-3.5.dev2/tox.ini`

 * *Files identical despite different names*

