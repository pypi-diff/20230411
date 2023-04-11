# Comparing `tmp/apkutils-1.2.2.tar.gz` & `tmp/apkutils-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apkutils-1.2.2.tar", max compression
+gzip compressed data, was "apkutils-1.2.4.tar", max compression
```

## Comparing `apkutils-1.2.2.tar` & `apkutils-1.2.4.tar`

### file list

```diff
@@ -1,52 +1,51 @@
--rw-r--r--   0        0        0     1065 2022-05-31 07:54:58.254915 apkutils-1.2.2/LICENSE
--rw-r--r--   0        0        0       50 2022-09-14 09:52:54.915766 apkutils-1.2.2/apkutils/__init__.py
--rw-r--r--   0        0        0    20939 2022-09-14 09:52:34.047259 apkutils-1.2.2/apkutils/apk.py
--rw-r--r--   0        0        0    73591 2022-08-26 10:33:28.841371 apkutils-1.2.2/apkutils/apkfile.py
--rw-r--r--   0        0        0   109800 2022-08-04 10:26:56.192509 apkutils-1.2.2/apkutils/axml/__init__.py
--rw-r--r--   0        0        0     7039 2022-05-31 07:54:58.257056 apkutils-1.2.2/apkutils/axml/bytecode.py
--rw-r--r--   0        0        0     2115 2022-05-31 07:54:58.257183 apkutils-1.2.2/apkutils/axml/public.py
--rw-r--r--   0        0        0   191132 2022-05-31 07:54:58.257843 apkutils-1.2.2/apkutils/axml/public.xml
--rw-r--r--   0        0        0     2083 2022-05-31 07:54:58.257993 apkutils-1.2.2/apkutils/axml/types.py
--rw-r--r--   0        0        0      807 2022-05-31 07:54:58.258124 apkutils-1.2.2/apkutils/cert.py
--rw-r--r--   0        0        0     3372 2022-09-14 06:39:15.359845 apkutils-1.2.2/apkutils/cli.py
--rw-r--r--   0        0        0      596 2022-05-31 07:54:58.258417 apkutils-1.2.2/apkutils/dex/__init__.py
--rw-r--r--   0        0        0     2787 2022-05-31 07:54:58.258530 apkutils-1.2.2/apkutils/dex/byteio.py
--rw-r--r--   0        0        0     7947 2022-05-31 07:54:58.258662 apkutils-1.2.2/apkutils/dex/dalvik.py
--rw-r--r--   0        0        0     4237 2022-05-31 07:54:58.258790 apkutils-1.2.2/apkutils/dex/dalvikformats.py
--rw-r--r--   0        0        0    12065 2022-07-13 08:37:53.407526 apkutils-1.2.2/apkutils/dex/dexparser.py
--rw-r--r--   0        0        0     1541 2022-05-31 07:54:58.259050 apkutils-1.2.2/apkutils/dex/flags.py
--rw-r--r--   0        0        0      596 2022-05-31 07:54:58.259207 apkutils-1.2.2/apkutils/dex/jvm/__init__.py
--rw-r--r--   0        0        0     1703 2022-05-31 07:54:58.259335 apkutils-1.2.2/apkutils/dex/jvm/arraytypes.py
--rw-r--r--   0        0        0     6678 2022-05-31 07:54:58.259463 apkutils-1.2.2/apkutils/dex/jvm/constantpool.py
--rw-r--r--   0        0        0      596 2022-05-31 07:54:58.259616 apkutils-1.2.2/apkutils/dex/jvm/constants/__init__.py
--rw-r--r--   0        0        0     6062 2022-05-31 07:54:58.259711 apkutils-1.2.2/apkutils/dex/jvm/constants/calc.py
--rw-r--r--   0        0        0     5657 2022-05-31 07:54:58.259839 apkutils-1.2.2/apkutils/dex/jvm/constants/genlookup.py
--rw-r--r--   0        0        0  1800593 2022-05-31 07:54:58.264922 apkutils-1.2.2/apkutils/dex/jvm/constants/lookup.py
--rw-r--r--   0        0        0      728 2022-05-31 07:54:58.265493 apkutils-1.2.2/apkutils/dex/jvm/error.py
--rw-r--r--   0        0        0     2867 2022-05-31 07:54:58.265628 apkutils-1.2.2/apkutils/dex/jvm/genmathops.py
--rw-r--r--   0        0        0     7859 2022-05-31 07:54:58.265767 apkutils-1.2.2/apkutils/dex/jvm/ir.py
--rw-r--r--   0        0        0     3479 2022-05-31 07:54:58.265895 apkutils-1.2.2/apkutils/dex/jvm/jvmops.py
--rw-r--r--   0        0        0     5689 2022-05-31 07:54:58.266026 apkutils-1.2.2/apkutils/dex/jvm/mathops.py
--rw-r--r--   0        0        0      596 2022-05-31 07:54:58.266199 apkutils-1.2.2/apkutils/dex/jvm/optimization/__init__.py
--rw-r--r--   0        0        0     3059 2022-05-31 07:54:58.266330 apkutils-1.2.2/apkutils/dex/jvm/optimization/consts.py
--rw-r--r--   0        0        0     3199 2022-05-31 07:54:58.266475 apkutils-1.2.2/apkutils/dex/jvm/optimization/jumps.py
--rw-r--r--   0        0        0     1550 2022-05-31 07:54:58.266602 apkutils-1.2.2/apkutils/dex/jvm/optimization/options.py
--rw-r--r--   0        0        0     8878 2022-05-31 07:54:58.266746 apkutils-1.2.2/apkutils/dex/jvm/optimization/registers.py
--rw-r--r--   0        0        0     8891 2022-05-31 07:54:58.266903 apkutils-1.2.2/apkutils/dex/jvm/optimization/stack.py
--rw-r--r--   0        0        0     1310 2022-05-31 07:54:58.267033 apkutils-1.2.2/apkutils/dex/jvm/scalartypes.py
--rw-r--r--   0        0        0     4130 2022-05-31 07:54:58.267174 apkutils-1.2.2/apkutils/dex/jvm/writebytecode.py
--rw-r--r--   0        0        0     4080 2022-05-31 07:54:58.267299 apkutils-1.2.2/apkutils/dex/jvm/writeclass.py
--rw-r--r--   0        0        0    24612 2022-05-31 07:54:58.267504 apkutils-1.2.2/apkutils/dex/jvm/writeir.py
--rw-r--r--   0        0        0     1767 2022-05-31 07:54:58.267651 apkutils-1.2.2/apkutils/dex/mutf8.py
--rw-r--r--   0        0        0     4029 2022-05-31 07:54:58.267775 apkutils-1.2.2/apkutils/dex/treelist.py
--rw-r--r--   0        0        0      596 2022-05-31 07:54:58.267939 apkutils-1.2.2/apkutils/dex/typeinference/__init__.py
--rw-r--r--   0        0        0    11171 2022-05-31 07:54:58.268117 apkutils-1.2.2/apkutils/dex/typeinference/typeinference.py
--rw-r--r--   0        0        0     1158 2022-05-31 07:54:58.268273 apkutils-1.2.2/apkutils/dex/util.py
--rw-r--r--   0        0        0        0 2022-05-31 07:54:58.268396 apkutils-1.2.2/apkutils/elf/__init__.py
--rw-r--r--   0        0        0     6655 2022-05-31 07:54:58.268536 apkutils-1.2.2/apkutils/elf/elfparser.py
--rwxr-xr-x   0        0        0    69313 2022-05-31 07:54:58.269027 apkutils-1.2.2/apkutils/gdiff.py
--rw-r--r--   0        0        0    16570 2022-05-31 07:54:58.269275 apkutils-1.2.2/apkutils/intersection.py
--rw-r--r--   0        0        0     6155 2022-05-31 07:54:58.269463 apkutils-1.2.2/apkutils/wildcard.py
--rw-r--r--   0        0        0     1006 2022-09-14 09:52:48.900930 apkutils-1.2.2/pyproject.toml
--rw-r--r--   0        0        0     1073 2022-09-14 09:54:26.641758 apkutils-1.2.2/setup.py
--rw-r--r--   0        0        0      989 2022-09-14 09:54:26.642244 apkutils-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2022-05-31 07:54:58.000000 apkutils-1.2.4/LICENSE
+-rw-r--r--   0        0        0       50 2023-04-10 10:31:15.874650 apkutils-1.2.4/apkutils/__init__.py
+-rw-r--r--   0        0        0    21012 2023-04-10 10:30:31.372606 apkutils-1.2.4/apkutils/apk.py
+-rw-r--r--   0        0        0    73591 2022-08-26 10:33:28.000000 apkutils-1.2.4/apkutils/apkfile.py
+-rw-r--r--   0        0        0   110042 2023-04-10 10:30:12.131157 apkutils-1.2.4/apkutils/axml/__init__.py
+-rw-r--r--   0        0        0     7039 2022-05-31 07:54:58.000000 apkutils-1.2.4/apkutils/axml/bytecode.py
+-rw-r--r--   0        0        0     2115 2022-05-31 07:54:58.000000 apkutils-1.2.4/apkutils/axml/public.py
+-rw-r--r--   0        0        0   191132 2022-05-31 07:54:58.000000 apkutils-1.2.4/apkutils/axml/public.xml
+-rw-r--r--   0        0        0     2083 2022-05-31 07:54:58.000000 apkutils-1.2.4/apkutils/axml/types.py
+-rw-r--r--   0        0        0      807 2022-05-31 07:54:58.000000 apkutils-1.2.4/apkutils/cert.py
+-rw-r--r--   0        0        0     3451 2023-04-10 10:30:36.237311 apkutils-1.2.4/apkutils/cli.py
+-rw-r--r--   0        0        0      596 2022-05-31 07:54:58.000000 apkutils-1.2.4/apkutils/dex/__init__.py
+-rw-r--r--   0        0        0     2787 2022-05-31 07:54:58.000000 apkutils-1.2.4/apkutils/dex/byteio.py
+-rw-r--r--   0        0        0     7947 2022-05-31 07:54:58.000000 apkutils-1.2.4/apkutils/dex/dalvik.py
+-rw-r--r--   0        0        0     4237 2022-05-31 07:54:58.000000 apkutils-1.2.4/apkutils/dex/dalvikformats.py
+-rw-r--r--   0        0        0    12065 2022-07-13 08:37:53.000000 apkutils-1.2.4/apkutils/dex/dexparser.py
+-rw-r--r--   0        0        0     1541 2022-05-31 07:54:58.000000 apkutils-1.2.4/apkutils/dex/flags.py
+-rw-r--r--   0        0        0      596 2022-05-31 07:54:58.000000 apkutils-1.2.4/apkutils/dex/jvm/__init__.py
+-rw-r--r--   0        0        0     1703 2022-05-31 07:54:58.000000 apkutils-1.2.4/apkutils/dex/jvm/arraytypes.py
+-rw-r--r--   0        0        0     6678 2022-05-31 07:54:58.000000 apkutils-1.2.4/apkutils/dex/jvm/constantpool.py
+-rw-r--r--   0        0        0      596 2022-05-31 07:54:58.000000 apkutils-1.2.4/apkutils/dex/jvm/constants/__init__.py
+-rw-r--r--   0        0        0     6062 2022-05-31 07:54:58.000000 apkutils-1.2.4/apkutils/dex/jvm/constants/calc.py
+-rw-r--r--   0        0        0     5657 2022-05-31 07:54:58.000000 apkutils-1.2.4/apkutils/dex/jvm/constants/genlookup.py
+-rw-r--r--   0        0        0  1800593 2022-05-31 07:54:58.000000 apkutils-1.2.4/apkutils/dex/jvm/constants/lookup.py
+-rw-r--r--   0        0        0      728 2022-05-31 07:54:58.000000 apkutils-1.2.4/apkutils/dex/jvm/error.py
+-rw-r--r--   0        0        0     2867 2022-05-31 07:54:58.000000 apkutils-1.2.4/apkutils/dex/jvm/genmathops.py
+-rw-r--r--   0        0        0     7859 2022-05-31 07:54:58.000000 apkutils-1.2.4/apkutils/dex/jvm/ir.py
+-rw-r--r--   0        0        0     3479 2022-05-31 07:54:58.000000 apkutils-1.2.4/apkutils/dex/jvm/jvmops.py
+-rw-r--r--   0        0        0     5689 2022-05-31 07:54:58.000000 apkutils-1.2.4/apkutils/dex/jvm/mathops.py
+-rw-r--r--   0        0        0      596 2022-05-31 07:54:58.000000 apkutils-1.2.4/apkutils/dex/jvm/optimization/__init__.py
+-rw-r--r--   0        0        0     3059 2022-05-31 07:54:58.000000 apkutils-1.2.4/apkutils/dex/jvm/optimization/consts.py
+-rw-r--r--   0        0        0     3199 2022-05-31 07:54:58.000000 apkutils-1.2.4/apkutils/dex/jvm/optimization/jumps.py
+-rw-r--r--   0        0        0     1550 2022-05-31 07:54:58.000000 apkutils-1.2.4/apkutils/dex/jvm/optimization/options.py
+-rw-r--r--   0        0        0     8878 2022-05-31 07:54:58.000000 apkutils-1.2.4/apkutils/dex/jvm/optimization/registers.py
+-rw-r--r--   0        0        0     8891 2022-05-31 07:54:58.000000 apkutils-1.2.4/apkutils/dex/jvm/optimization/stack.py
+-rw-r--r--   0        0        0     1310 2022-05-31 07:54:58.000000 apkutils-1.2.4/apkutils/dex/jvm/scalartypes.py
+-rw-r--r--   0        0        0     4130 2022-05-31 07:54:58.000000 apkutils-1.2.4/apkutils/dex/jvm/writebytecode.py
+-rw-r--r--   0        0        0     4080 2022-05-31 07:54:58.000000 apkutils-1.2.4/apkutils/dex/jvm/writeclass.py
+-rw-r--r--   0        0        0    24612 2022-05-31 07:54:58.000000 apkutils-1.2.4/apkutils/dex/jvm/writeir.py
+-rw-r--r--   0        0        0     1767 2022-05-31 07:54:58.000000 apkutils-1.2.4/apkutils/dex/mutf8.py
+-rw-r--r--   0        0        0     4029 2022-05-31 07:54:58.000000 apkutils-1.2.4/apkutils/dex/treelist.py
+-rw-r--r--   0        0        0      596 2022-05-31 07:54:58.000000 apkutils-1.2.4/apkutils/dex/typeinference/__init__.py
+-rw-r--r--   0        0        0    11171 2022-05-31 07:54:58.000000 apkutils-1.2.4/apkutils/dex/typeinference/typeinference.py
+-rw-r--r--   0        0        0     1158 2022-05-31 07:54:58.000000 apkutils-1.2.4/apkutils/dex/util.py
+-rw-r--r--   0        0        0        0 2022-05-31 07:54:58.000000 apkutils-1.2.4/apkutils/elf/__init__.py
+-rw-r--r--   0        0        0     6655 2022-05-31 07:54:58.000000 apkutils-1.2.4/apkutils/elf/elfparser.py
+-rwxr-xr-x   0        0        0    69313 2022-05-31 07:54:58.000000 apkutils-1.2.4/apkutils/gdiff.py
+-rw-r--r--   0        0        0    16570 2022-05-31 07:54:58.000000 apkutils-1.2.4/apkutils/intersection.py
+-rw-r--r--   0        0        0     6155 2022-05-31 07:54:58.000000 apkutils-1.2.4/apkutils/wildcard.py
+-rw-r--r--   0        0        0     1006 2023-04-10 10:30:19.547734 apkutils-1.2.4/pyproject.toml
+-rw-r--r--   0        0        0     1191 1970-01-01 00:00:00.000000 apkutils-1.2.4/PKG-INFO
```

### Comparing `apkutils-1.2.2/LICENSE` & `apkutils-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.2/apkutils/apk.py` & `apkutils-1.2.4/apkutils/apk.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,22 +88,23 @@
 
     def _init_manifest(self):
         ANDROID_MANIFEST = "AndroidManifest.xml"
         try:
             if ANDROID_MANIFEST in self.afile.namelist():
                 data = self.afile.read(ANDROID_MANIFEST)
                 try:
-                    self.axml = AXMLPrinter(data).get_xml_obj()
+                    self.axml = AXMLPrinter(data, True).get_xml_obj()
                     if self.axml is None:
                         return
                     buff = etree.tostring(
                         self.axml, pretty_print=True, encoding="utf-8"
                     )
+                    if buff is None:
+                        return
                     self.manifest = buff.decode("UTF-8")
-
                 except:
                     traceback.print_exc()
                     return
         except:
             traceback.print_exc()
             return
```

### Comparing `apkutils-1.2.2/apkutils/apkfile.py` & `apkutils-1.2.4/apkutils/apkfile.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.2/apkutils/axml/__init__.py` & `apkutils-1.2.4/apkutils/axml/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,17 +5,18 @@
 import logging
 import re
 import sys
 from collections import defaultdict
 from struct import pack, unpack
 from xml.sax.saxutils import escape
 
+from lxml import etree
+
 from apkutils.axml import bytecode, public
 from apkutils.axml.types import *
-from lxml import etree
 
 log = logging.getLogger("axml")
 
 
 # Constants for ARSC Files
 # see http://androidxref.com/9.0.0_r3/xref/frameworks/base/libs/androidfw/include/androidfw/ResourceTypes.h#215
 RES_NULL_TYPE = 0x0000
@@ -99,37 +100,45 @@
     """
     StringBlock is a CHUNK inside an AXML File: `ResStringPool_header`
     It contains all strings, which are used by referecing to ID's
 
     See http://androidxref.com/9.0.0_r3/xref/frameworks/base/libs/androidfw/include/androidfw/ResourceTypes.h#436
     """
 
-    def __init__(self, buff, header):
+    def __init__(self, buff, header, is_android_manifest=False):
         """
         :param buff: buffer which holds the string block
         :param header: a instance of :class:`~ARSCHeader`
         """
         self._cache = {}
         self.header = header
-        # We already read the header (which was chunk_type and chunk_size
-        # Now, we read the string_count:
+
         self.stringCount = unpack("<I", buff.read(4))[0]
-        # style_count
-        self.styleCount = unpack("<I", buff.read(4))[0]
+        
+        self.styleCount = 0
+        if is_android_manifest:
+            buff.read(4)
+        else:
+            self.styleCount = unpack("<I", buff.read(4))[0]
 
-        # flags
+        # flags is_utf8
         self.flags = unpack("<I", buff.read(4))[0]
         self.m_isUTF8 = (self.flags & UTF8_FLAG) != 0
 
         # string_pool_offset
         # The string offset is counted from the beginning of the string section
         self.stringsOffset = unpack("<I", buff.read(4))[0]
+        
         # style_pool_offset
         # The styles offset is counted as well from the beginning of the string section
-        self.stylesOffset = unpack("<I", buff.read(4))[0]
+        self.stylesOffset = 0
+        if is_android_manifest:
+            buff.read(4)
+        else:
+            self.stylesOffset = unpack("<I", buff.read(4))[0]
 
         # Check if they supplied a stylesOffset even if the count is 0:
         if self.styleCount == 0 and self.stylesOffset > 0:
             log.info(
                 "Styles Offset given, but styleCount is zero. "
                 "This is not a problem but could indicate packers."
             )
@@ -138,22 +147,29 @@
         self.m_styleOffsets = []
         self.m_charbuff = ""
         self.m_styles = []
 
         # Next, there is a list of string following.
         # This is only a list of offsets (4 byte each)
         for i in range(self.stringCount):
-            self.m_stringOffsets.append(unpack("<I", buff.read(4))[0])
+            offset = unpack("<I", buff.read(4))[0]
+            self.m_stringOffsets.append(offset)
+            
+            # NOTE 如果offset是0，说明有问题
+            if i > 0 and offset == 0:
+                self.stringCount = i
+                buff.set_idx(buff.get_idx()-4)
+                break
+        
 
         # And a list of styles
         # again, a list of offsets
         for i in range(self.styleCount):
             self.m_styleOffsets.append(unpack("<I", buff.read(4))[0])
 
-        # FIXME it is probably better to parse n strings and not calculate the size
         size = self.header.size - self.stringsOffset
 
         # if there are styles as well, we do not want to read them too.
         # Only read them, if no
         if self.stylesOffset != 0 and self.styleCount != 0:
             size = self.stylesOffset - self.stringsOffset
 
@@ -166,15 +182,15 @@
             size = self.header.size - self.stylesOffset
 
             if (size % 4) != 0:
                 log.warning("Size of styles is not aligned by four bytes.")
 
             for i in range(0, size // 4):
                 self.m_styles.append(unpack("<I", buff.read(4))[0])
-
+        
     def __repr__(self):
         return "<StringPool #strings={}, #styles={}, UTF8={}>".format(
             self.stringCount, self.styleCount, self.m_isUTF8
         )
 
     def __getitem__(self, idx):
         """
@@ -393,21 +409,21 @@
     the AXMLParser only.
     The parser will set `is_valid()` to False if it parses something not valid.
     Messages what is wrong are logged.
 
     See http://androidxref.com/9.0.0_r3/xref/frameworks/base/libs/androidfw/include/androidfw/ResourceTypes.h#563
     """
 
-    def __init__(self, raw_buff):
+    def __init__(self, raw_buff, is_android_manifest=False):
         self._reset()
 
         self._valid = True
         self.axml_tampered = False
         self.buff = bytecode.BuffHandle(raw_buff)
-
+        
         # Minimum is a single ARSCHeader, which would be a strange edge case...
         if self.buff.size() < 8:
             log.error(
                 "Filesize is too small to be a valid AXML file! Filesize: {}".format(
                     self.buff.size()
                 )
             )
@@ -467,20 +483,18 @@
                 "Was something appended to the file? Trying to parse it anyways.".format(
                     self.filesize, self.buff.size()
                 )
             )
 
         # Not that severe of an error, we have plenty files where this is not
         # set correctly
-        # FIXME 异常
         if axml_header.type != RES_XML_TYPE:
             self.axml_tampered = True
             log.warning(
-                "AXML file has an unusual resource type! "
-                "Malware likes to to such stuff to anti androguard! "
+                "AXML有一个不常见的资源类型! "
                 "But we try to parse it anyways. Resource Type: 0x{:04x}".format(
                     axml_header.type
                 )
             )
 
         # Now we parse the STRING POOL
         try:
@@ -495,16 +509,16 @@
                 "This does not look like an AXML file. String chunk header size does not equal 28! header size = {}".format(
                     header.header_size
                 )
             )
             self._valid = False
             return
 
-        self.sb = StringBlock(self.buff, header)
-
+        self.sb = StringBlock(self.buff, header, is_android_manifest)
+        
         # Stores resource ID mappings, if any
         self.m_resourceIDs = []
 
         # Store a list of prefix/uri mappings encountered
         self.namespaces = []
 
     def is_valid(self):
@@ -561,19 +575,17 @@
 
                 for i in range((h.size - h.header_size) // 4):
                     self.m_resourceIDs.append(unpack("<L", self.buff.read(4))[0])
 
                 continue
 
             # Parse now the XML chunks.
-            # unknown chunk types might cause problems, but we can skip them!
             if h.type < RES_XML_FIRST_CHUNK_TYPE or h.type > RES_XML_LAST_CHUNK_TYPE:
                 # h.size is the size of the whole chunk including the header.
-                # We read already 8 bytes of the header, thus we need to
-                # subtract them.
+                # We read already 8 bytes of the header, thus we need to subtract them.
                 log.error(
                     "Not a XML resource chunk type: 0x{:04x}. Skipping {} bytes".format(
                         h.type, h.size
                     )
                 )
                 self.buff.set_idx(h.end)
                 continue
@@ -666,15 +678,16 @@
                 # * class_attribute
                 # After that, there are two lists of attributes, 20 bytes each
 
                 # Namespace URI (String ID)
                 (self.m_namespaceUri,) = unpack("<L", self.buff.read(4))
                 # Name of the Tag (String ID)
                 (self.m_name,) = unpack("<L", self.buff.read(4))
-                # FIXME: Flags
+                
+                # NOTE : Flags skip
                 _ = self.buff.read(4)
                 # Attribute Count
                 (attributeCount,) = unpack("<L", self.buff.read(4))
                 # Class Attribute
                 (self.m_classAttribute,) = unpack("<L", self.buff.read(4))
 
                 self.m_idAttribute = (attributeCount >> 16) - 1
@@ -1003,16 +1016,16 @@
 
     A Reference Implementation can be found at http://androidxref.com/9.0.0_r3/xref/frameworks/base/tools/aapt/XMLNode.cpp
     """
 
     __charrange = None
     __replacement = None
 
-    def __init__(self, raw_buff):
-        self.axml = AXMLParser(raw_buff)
+    def __init__(self, raw_buff, is_android_manifest=False):
+        self.axml = AXMLParser(raw_buff, is_android_manifest)
 
         self.root = None
         self.packerwarning = False
         cur = []
 
         while self.axml.is_valid():
             _type = next(self.axml)
```

### Comparing `apkutils-1.2.2/apkutils/axml/bytecode.py` & `apkutils-1.2.4/apkutils/axml/bytecode.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.2/apkutils/axml/public.py` & `apkutils-1.2.4/apkutils/axml/public.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.2/apkutils/axml/public.xml` & `apkutils-1.2.4/apkutils/axml/public.xml`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.2/apkutils/axml/types.py` & `apkutils-1.2.4/apkutils/axml/types.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.2/apkutils/cert.py` & `apkutils-1.2.4/apkutils/cert.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.2/apkutils/cli.py` & `apkutils-1.2.4/apkutils/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,17 +2,16 @@
 import binascii
 import sys
 
 import click
 from pygments import highlight
 from pygments.formatters.terminal import TerminalFormatter
 from pygments.lexers import get_lexer_by_name
-from apkutils import apkfile
 
-from apkutils import APK, __version__
+from apkutils import APK, __version__, apkfile
 
 
 @click.group()
 @click.version_option(__version__)
 def main():
     pass
 
@@ -26,17 +25,21 @@
 
 
 @main.command()
 @click.argument("path")
 def manifest(path):
     """打印清单"""
     apk = APK.from_file(path)
+    manifest = apk.get_manifest()
+    if manifest is None:
+        print("Manifest is None!")
+        return
 
     sys.stdout.write(
-        highlight(apk.get_manifest(), get_lexer_by_name("xml"), TerminalFormatter())
+        highlight(manifest, get_lexer_by_name("xml"), TerminalFormatter())
     )
 
     print(apk.get_manifest_main_activities())
 
 
 @main.command()
 @click.argument("path")
```

### Comparing `apkutils-1.2.2/apkutils/dex/__init__.py` & `apkutils-1.2.4/apkutils/dex/__init__.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.2/apkutils/dex/byteio.py` & `apkutils-1.2.4/apkutils/dex/byteio.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.2/apkutils/dex/dalvik.py` & `apkutils-1.2.4/apkutils/dex/dalvik.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.2/apkutils/dex/dalvikformats.py` & `apkutils-1.2.4/apkutils/dex/dalvikformats.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.2/apkutils/dex/dexparser.py` & `apkutils-1.2.4/apkutils/dex/dexparser.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.2/apkutils/dex/flags.py` & `apkutils-1.2.4/apkutils/dex/flags.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.2/apkutils/dex/jvm/__init__.py` & `apkutils-1.2.4/apkutils/dex/jvm/__init__.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.2/apkutils/dex/jvm/arraytypes.py` & `apkutils-1.2.4/apkutils/dex/jvm/arraytypes.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.2/apkutils/dex/jvm/constantpool.py` & `apkutils-1.2.4/apkutils/dex/jvm/constantpool.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.2/apkutils/dex/jvm/constants/__init__.py` & `apkutils-1.2.4/apkutils/dex/jvm/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.2/apkutils/dex/jvm/constants/calc.py` & `apkutils-1.2.4/apkutils/dex/jvm/constants/calc.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.2/apkutils/dex/jvm/constants/genlookup.py` & `apkutils-1.2.4/apkutils/dex/jvm/constants/genlookup.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.2/apkutils/dex/jvm/constants/lookup.py` & `apkutils-1.2.4/apkutils/dex/jvm/constants/lookup.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.2/apkutils/dex/jvm/error.py` & `apkutils-1.2.4/apkutils/dex/jvm/error.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.2/apkutils/dex/jvm/genmathops.py` & `apkutils-1.2.4/apkutils/dex/jvm/genmathops.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.2/apkutils/dex/jvm/ir.py` & `apkutils-1.2.4/apkutils/dex/jvm/ir.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.2/apkutils/dex/jvm/jvmops.py` & `apkutils-1.2.4/apkutils/dex/jvm/jvmops.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.2/apkutils/dex/jvm/mathops.py` & `apkutils-1.2.4/apkutils/dex/jvm/mathops.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.2/apkutils/dex/jvm/optimization/__init__.py` & `apkutils-1.2.4/apkutils/dex/jvm/optimization/__init__.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.2/apkutils/dex/jvm/optimization/consts.py` & `apkutils-1.2.4/apkutils/dex/jvm/optimization/consts.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.2/apkutils/dex/jvm/optimization/jumps.py` & `apkutils-1.2.4/apkutils/dex/jvm/optimization/jumps.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.2/apkutils/dex/jvm/optimization/options.py` & `apkutils-1.2.4/apkutils/dex/jvm/optimization/options.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.2/apkutils/dex/jvm/optimization/registers.py` & `apkutils-1.2.4/apkutils/dex/jvm/optimization/registers.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.2/apkutils/dex/jvm/optimization/stack.py` & `apkutils-1.2.4/apkutils/dex/jvm/optimization/stack.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.2/apkutils/dex/jvm/scalartypes.py` & `apkutils-1.2.4/apkutils/dex/jvm/scalartypes.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.2/apkutils/dex/jvm/writebytecode.py` & `apkutils-1.2.4/apkutils/dex/jvm/writebytecode.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.2/apkutils/dex/jvm/writeclass.py` & `apkutils-1.2.4/apkutils/dex/jvm/writeclass.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.2/apkutils/dex/jvm/writeir.py` & `apkutils-1.2.4/apkutils/dex/jvm/writeir.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.2/apkutils/dex/mutf8.py` & `apkutils-1.2.4/apkutils/dex/mutf8.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.2/apkutils/dex/treelist.py` & `apkutils-1.2.4/apkutils/dex/treelist.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.2/apkutils/dex/typeinference/__init__.py` & `apkutils-1.2.4/apkutils/dex/typeinference/__init__.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.2/apkutils/dex/typeinference/typeinference.py` & `apkutils-1.2.4/apkutils/dex/typeinference/typeinference.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.2/apkutils/dex/util.py` & `apkutils-1.2.4/apkutils/dex/util.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.2/apkutils/elf/elfparser.py` & `apkutils-1.2.4/apkutils/elf/elfparser.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.2/apkutils/gdiff.py` & `apkutils-1.2.4/apkutils/gdiff.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.2/apkutils/intersection.py` & `apkutils-1.2.4/apkutils/intersection.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.2/apkutils/wildcard.py` & `apkutils-1.2.4/apkutils/wildcard.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.2/pyproject.toml` & `apkutils-1.2.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
   "Natural Language :: Chinese (Simplified)",
   "Development Status :: 3 - Alpha",
 ]
 description = "一个APK解析库"
 license = "MIT"
 name = "apkutils"
 repository = "https://gitee.com/kin9-0rz/apkutils"
-version = "1.2.2"
+version = "1.2.4"
 
 [tool.poetry.dependencies]
 Pygments = "^2.12.0"
 beautifulsoup4 = "^4.10.0"
 click = "^8.0.3"
 cryptography = "^35.0.0"
 lxml = "^4.6.4"
```

### Comparing `apkutils-1.2.2/PKG-INFO` & `apkutils-1.2.4/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 Metadata-Version: 2.1
 Name: apkutils
-Version: 1.2.2
+Version: 1.2.4
 Summary: 一个APK解析库
 Home-page: https://gitee.com/kin9-0rz/apkutils
 License: MIT
 Author: kin9-0rz
 Author-email: kin9-0rz@outlook.com
 Requires-Python: >=3.8
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: Pygments (>=2.12.0,<3.0.0)
 Requires-Dist: beautifulsoup4 (>=4.10.0,<5.0.0)
 Requires-Dist: click (>=8.0.3,<9.0.0)
```

