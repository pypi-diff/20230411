# Comparing `tmp/apkutils-1.2.4.tar.gz` & `tmp/apkutils-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apkutils-1.2.4.tar", max compression
+gzip compressed data, was "apkutils-1.3.0.tar", max compression
```

## Comparing `apkutils-1.2.4.tar` & `apkutils-1.3.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0     1065 2022-05-31 07:54:58.000000 apkutils-1.2.4/LICENSE
--rw-r--r--   0        0        0       50 2023-04-10 10:31:15.874650 apkutils-1.2.4/apkutils/__init__.py
--rw-r--r--   0        0        0    21012 2023-04-10 10:30:31.372606 apkutils-1.2.4/apkutils/apk.py
--rw-r--r--   0        0        0    73591 2022-08-26 10:33:28.000000 apkutils-1.2.4/apkutils/apkfile.py
--rw-r--r--   0        0        0   110042 2023-04-10 10:30:12.131157 apkutils-1.2.4/apkutils/axml/__init__.py
--rw-r--r--   0        0        0     7039 2022-05-31 07:54:58.000000 apkutils-1.2.4/apkutils/axml/bytecode.py
--rw-r--r--   0        0        0     2115 2022-05-31 07:54:58.000000 apkutils-1.2.4/apkutils/axml/public.py
--rw-r--r--   0        0        0   191132 2022-05-31 07:54:58.000000 apkutils-1.2.4/apkutils/axml/public.xml
--rw-r--r--   0        0        0     2083 2022-05-31 07:54:58.000000 apkutils-1.2.4/apkutils/axml/types.py
--rw-r--r--   0        0        0      807 2022-05-31 07:54:58.000000 apkutils-1.2.4/apkutils/cert.py
--rw-r--r--   0        0        0     3451 2023-04-10 10:30:36.237311 apkutils-1.2.4/apkutils/cli.py
--rw-r--r--   0        0        0      596 2022-05-31 07:54:58.000000 apkutils-1.2.4/apkutils/dex/__init__.py
--rw-r--r--   0        0        0     2787 2022-05-31 07:54:58.000000 apkutils-1.2.4/apkutils/dex/byteio.py
--rw-r--r--   0        0        0     7947 2022-05-31 07:54:58.000000 apkutils-1.2.4/apkutils/dex/dalvik.py
--rw-r--r--   0        0        0     4237 2022-05-31 07:54:58.000000 apkutils-1.2.4/apkutils/dex/dalvikformats.py
--rw-r--r--   0        0        0    12065 2022-07-13 08:37:53.000000 apkutils-1.2.4/apkutils/dex/dexparser.py
--rw-r--r--   0        0        0     1541 2022-05-31 07:54:58.000000 apkutils-1.2.4/apkutils/dex/flags.py
--rw-r--r--   0        0        0      596 2022-05-31 07:54:58.000000 apkutils-1.2.4/apkutils/dex/jvm/__init__.py
--rw-r--r--   0        0        0     1703 2022-05-31 07:54:58.000000 apkutils-1.2.4/apkutils/dex/jvm/arraytypes.py
--rw-r--r--   0        0        0     6678 2022-05-31 07:54:58.000000 apkutils-1.2.4/apkutils/dex/jvm/constantpool.py
--rw-r--r--   0        0        0      596 2022-05-31 07:54:58.000000 apkutils-1.2.4/apkutils/dex/jvm/constants/__init__.py
--rw-r--r--   0        0        0     6062 2022-05-31 07:54:58.000000 apkutils-1.2.4/apkutils/dex/jvm/constants/calc.py
--rw-r--r--   0        0        0     5657 2022-05-31 07:54:58.000000 apkutils-1.2.4/apkutils/dex/jvm/constants/genlookup.py
--rw-r--r--   0        0        0  1800593 2022-05-31 07:54:58.000000 apkutils-1.2.4/apkutils/dex/jvm/constants/lookup.py
--rw-r--r--   0        0        0      728 2022-05-31 07:54:58.000000 apkutils-1.2.4/apkutils/dex/jvm/error.py
--rw-r--r--   0        0        0     2867 2022-05-31 07:54:58.000000 apkutils-1.2.4/apkutils/dex/jvm/genmathops.py
--rw-r--r--   0        0        0     7859 2022-05-31 07:54:58.000000 apkutils-1.2.4/apkutils/dex/jvm/ir.py
--rw-r--r--   0        0        0     3479 2022-05-31 07:54:58.000000 apkutils-1.2.4/apkutils/dex/jvm/jvmops.py
--rw-r--r--   0        0        0     5689 2022-05-31 07:54:58.000000 apkutils-1.2.4/apkutils/dex/jvm/mathops.py
--rw-r--r--   0        0        0      596 2022-05-31 07:54:58.000000 apkutils-1.2.4/apkutils/dex/jvm/optimization/__init__.py
--rw-r--r--   0        0        0     3059 2022-05-31 07:54:58.000000 apkutils-1.2.4/apkutils/dex/jvm/optimization/consts.py
--rw-r--r--   0        0        0     3199 2022-05-31 07:54:58.000000 apkutils-1.2.4/apkutils/dex/jvm/optimization/jumps.py
--rw-r--r--   0        0        0     1550 2022-05-31 07:54:58.000000 apkutils-1.2.4/apkutils/dex/jvm/optimization/options.py
--rw-r--r--   0        0        0     8878 2022-05-31 07:54:58.000000 apkutils-1.2.4/apkutils/dex/jvm/optimization/registers.py
--rw-r--r--   0        0        0     8891 2022-05-31 07:54:58.000000 apkutils-1.2.4/apkutils/dex/jvm/optimization/stack.py
--rw-r--r--   0        0        0     1310 2022-05-31 07:54:58.000000 apkutils-1.2.4/apkutils/dex/jvm/scalartypes.py
--rw-r--r--   0        0        0     4130 2022-05-31 07:54:58.000000 apkutils-1.2.4/apkutils/dex/jvm/writebytecode.py
--rw-r--r--   0        0        0     4080 2022-05-31 07:54:58.000000 apkutils-1.2.4/apkutils/dex/jvm/writeclass.py
--rw-r--r--   0        0        0    24612 2022-05-31 07:54:58.000000 apkutils-1.2.4/apkutils/dex/jvm/writeir.py
--rw-r--r--   0        0        0     1767 2022-05-31 07:54:58.000000 apkutils-1.2.4/apkutils/dex/mutf8.py
--rw-r--r--   0        0        0     4029 2022-05-31 07:54:58.000000 apkutils-1.2.4/apkutils/dex/treelist.py
--rw-r--r--   0        0        0      596 2022-05-31 07:54:58.000000 apkutils-1.2.4/apkutils/dex/typeinference/__init__.py
--rw-r--r--   0        0        0    11171 2022-05-31 07:54:58.000000 apkutils-1.2.4/apkutils/dex/typeinference/typeinference.py
--rw-r--r--   0        0        0     1158 2022-05-31 07:54:58.000000 apkutils-1.2.4/apkutils/dex/util.py
--rw-r--r--   0        0        0        0 2022-05-31 07:54:58.000000 apkutils-1.2.4/apkutils/elf/__init__.py
--rw-r--r--   0        0        0     6655 2022-05-31 07:54:58.000000 apkutils-1.2.4/apkutils/elf/elfparser.py
--rwxr-xr-x   0        0        0    69313 2022-05-31 07:54:58.000000 apkutils-1.2.4/apkutils/gdiff.py
--rw-r--r--   0        0        0    16570 2022-05-31 07:54:58.000000 apkutils-1.2.4/apkutils/intersection.py
--rw-r--r--   0        0        0     6155 2022-05-31 07:54:58.000000 apkutils-1.2.4/apkutils/wildcard.py
--rw-r--r--   0        0        0     1006 2023-04-10 10:30:19.547734 apkutils-1.2.4/pyproject.toml
--rw-r--r--   0        0        0     1191 1970-01-01 00:00:00.000000 apkutils-1.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1065 2022-05-31 07:54:58.000000 apkutils-1.3.0/LICENSE
+-rw-r--r--   0        0        0       50 2023-04-11 08:51:48.957974 apkutils-1.3.0/apkutils/__init__.py
+-rw-r--r--   0        0        0    21364 2023-04-11 08:42:08.633938 apkutils-1.3.0/apkutils/apk.py
+-rw-r--r--   0        0        0    74509 2023-04-11 07:35:49.515179 apkutils-1.3.0/apkutils/apkfile.py
+-rw-r--r--   0        0        0   109909 2023-04-11 08:50:18.990039 apkutils-1.3.0/apkutils/axml/__init__.py
+-rw-r--r--   0        0        0     7039 2022-05-31 07:54:58.000000 apkutils-1.3.0/apkutils/axml/bytecode.py
+-rw-r--r--   0        0        0     2115 2022-05-31 07:54:58.000000 apkutils-1.3.0/apkutils/axml/public.py
+-rw-r--r--   0        0        0   191132 2022-05-31 07:54:58.000000 apkutils-1.3.0/apkutils/axml/public.xml
+-rw-r--r--   0        0        0     2083 2022-05-31 07:54:58.000000 apkutils-1.3.0/apkutils/axml/types.py
+-rw-r--r--   0        0        0      807 2022-05-31 07:54:58.000000 apkutils-1.3.0/apkutils/cert.py
+-rw-r--r--   0        0        0     4209 2023-04-11 07:59:16.076423 apkutils-1.3.0/apkutils/cli.py
+-rw-r--r--   0        0        0      596 2022-05-31 07:54:58.000000 apkutils-1.3.0/apkutils/dex/__init__.py
+-rw-r--r--   0        0        0     2787 2022-05-31 07:54:58.000000 apkutils-1.3.0/apkutils/dex/byteio.py
+-rw-r--r--   0        0        0     7947 2022-05-31 07:54:58.000000 apkutils-1.3.0/apkutils/dex/dalvik.py
+-rw-r--r--   0        0        0     4237 2022-05-31 07:54:58.000000 apkutils-1.3.0/apkutils/dex/dalvikformats.py
+-rw-r--r--   0        0        0    12065 2022-07-13 08:37:53.000000 apkutils-1.3.0/apkutils/dex/dexparser.py
+-rw-r--r--   0        0        0     1541 2022-05-31 07:54:58.000000 apkutils-1.3.0/apkutils/dex/flags.py
+-rw-r--r--   0        0        0      596 2022-05-31 07:54:58.000000 apkutils-1.3.0/apkutils/dex/jvm/__init__.py
+-rw-r--r--   0        0        0     1703 2022-05-31 07:54:58.000000 apkutils-1.3.0/apkutils/dex/jvm/arraytypes.py
+-rw-r--r--   0        0        0     6678 2022-05-31 07:54:58.000000 apkutils-1.3.0/apkutils/dex/jvm/constantpool.py
+-rw-r--r--   0        0        0      596 2022-05-31 07:54:58.000000 apkutils-1.3.0/apkutils/dex/jvm/constants/__init__.py
+-rw-r--r--   0        0        0     6062 2022-05-31 07:54:58.000000 apkutils-1.3.0/apkutils/dex/jvm/constants/calc.py
+-rw-r--r--   0        0        0     5657 2022-05-31 07:54:58.000000 apkutils-1.3.0/apkutils/dex/jvm/constants/genlookup.py
+-rw-r--r--   0        0        0  1800593 2022-05-31 07:54:58.000000 apkutils-1.3.0/apkutils/dex/jvm/constants/lookup.py
+-rw-r--r--   0        0        0      728 2022-05-31 07:54:58.000000 apkutils-1.3.0/apkutils/dex/jvm/error.py
+-rw-r--r--   0        0        0     2867 2022-05-31 07:54:58.000000 apkutils-1.3.0/apkutils/dex/jvm/genmathops.py
+-rw-r--r--   0        0        0     7859 2022-05-31 07:54:58.000000 apkutils-1.3.0/apkutils/dex/jvm/ir.py
+-rw-r--r--   0        0        0     3479 2022-05-31 07:54:58.000000 apkutils-1.3.0/apkutils/dex/jvm/jvmops.py
+-rw-r--r--   0        0        0     5689 2022-05-31 07:54:58.000000 apkutils-1.3.0/apkutils/dex/jvm/mathops.py
+-rw-r--r--   0        0        0      596 2022-05-31 07:54:58.000000 apkutils-1.3.0/apkutils/dex/jvm/optimization/__init__.py
+-rw-r--r--   0        0        0     3059 2022-05-31 07:54:58.000000 apkutils-1.3.0/apkutils/dex/jvm/optimization/consts.py
+-rw-r--r--   0        0        0     3199 2022-05-31 07:54:58.000000 apkutils-1.3.0/apkutils/dex/jvm/optimization/jumps.py
+-rw-r--r--   0        0        0     1550 2022-05-31 07:54:58.000000 apkutils-1.3.0/apkutils/dex/jvm/optimization/options.py
+-rw-r--r--   0        0        0     8878 2022-05-31 07:54:58.000000 apkutils-1.3.0/apkutils/dex/jvm/optimization/registers.py
+-rw-r--r--   0        0        0     8891 2022-05-31 07:54:58.000000 apkutils-1.3.0/apkutils/dex/jvm/optimization/stack.py
+-rw-r--r--   0        0        0     1310 2022-05-31 07:54:58.000000 apkutils-1.3.0/apkutils/dex/jvm/scalartypes.py
+-rw-r--r--   0        0        0     4130 2022-05-31 07:54:58.000000 apkutils-1.3.0/apkutils/dex/jvm/writebytecode.py
+-rw-r--r--   0        0        0     4080 2022-05-31 07:54:58.000000 apkutils-1.3.0/apkutils/dex/jvm/writeclass.py
+-rw-r--r--   0        0        0    24612 2022-05-31 07:54:58.000000 apkutils-1.3.0/apkutils/dex/jvm/writeir.py
+-rw-r--r--   0        0        0     1767 2022-05-31 07:54:58.000000 apkutils-1.3.0/apkutils/dex/mutf8.py
+-rw-r--r--   0        0        0     4029 2022-05-31 07:54:58.000000 apkutils-1.3.0/apkutils/dex/treelist.py
+-rw-r--r--   0        0        0      596 2022-05-31 07:54:58.000000 apkutils-1.3.0/apkutils/dex/typeinference/__init__.py
+-rw-r--r--   0        0        0    11171 2022-05-31 07:54:58.000000 apkutils-1.3.0/apkutils/dex/typeinference/typeinference.py
+-rw-r--r--   0        0        0     1158 2022-05-31 07:54:58.000000 apkutils-1.3.0/apkutils/dex/util.py
+-rw-r--r--   0        0        0        0 2022-05-31 07:54:58.000000 apkutils-1.3.0/apkutils/elf/__init__.py
+-rw-r--r--   0        0        0     6655 2022-05-31 07:54:58.000000 apkutils-1.3.0/apkutils/elf/elfparser.py
+-rwxr-xr-x   0        0        0    69313 2022-05-31 07:54:58.000000 apkutils-1.3.0/apkutils/gdiff.py
+-rw-r--r--   0        0        0    16570 2022-05-31 07:54:58.000000 apkutils-1.3.0/apkutils/intersection.py
+-rw-r--r--   0        0        0     6155 2022-05-31 07:54:58.000000 apkutils-1.3.0/apkutils/wildcard.py
+-rw-r--r--   0        0        0     1006 2023-04-11 07:57:06.813221 apkutils-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1191 1970-01-01 00:00:00.000000 apkutils-1.3.0/PKG-INFO
```

### Comparing `apkutils-1.2.4/LICENSE` & `apkutils-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.4/apkutils/apk.py` & `apkutils-1.3.0/apkutils/apk.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,18 +49,18 @@
         self.trees = None  # 代码结构序列字典
         self._classes = None
         self._methods_refx = None
         self._package_name = None  # 包名
         self._app_name = None
         self._application_icon_addr = None
 
-        self._init_manifest()
-        self._init_arsc()
-        self._init_app_icons()
-        self._init_dex_strings()
+        # self._init_manifest()
+        # self._init_arsc()
+        # self._init_app_icons()
+        # self._init_dex_strings()
 
     @classmethod
     def from_file(cls, path):
         cls.apk_path = path
         return cls.from_io(path)
 
     @classmethod
@@ -68,14 +68,30 @@
         return cls.from_io(io.BytesIO(_bytes))
 
     @classmethod
     def from_io(cls, _io):
         cls.afile = apkfile.ZipFile(_io, "r")
         return cls()
 
+    def parse_manifest(self):
+        self._init_manifest()
+        return self
+    
+    def parse_dex(self):
+        self._init_dex_strings()
+        return self
+    
+    def parse_arsc(self):
+        self._init_arsc()
+        return self
+    
+    def parse_app_icons(self):
+        self._init_app_icons()
+        return self
+
     def __enter__(self):
         return self
 
     def __exit__(self, *args, **kwargs):
         self.close()
 
     def close(self):
@@ -130,22 +146,22 @@
         if application_tag is None:
             return
         self._application = application_tag.get("android:name", "")
         self._application_icon_addr = (
             application_tag.get("android:icon", "").lower().replace("@", "0x")
         )
         self._application_label_id = (
-            application_tag.get("android:label").lower().replace("@", "0x")
+            application_tag.get("android:label", "").lower().replace("@", "0x")
         )
 
         self._activities_icon_addrs = []
 
         def find_activities(tag):
             for item in soup.select(tag):
-                name = item["android:name"]
+                name = item.get("android:name", "none")
                 if name.startswith("."):
                     name = self._package_name + name
 
                 enabled = item.get("android:enabled", True)
                 if enabled is False:
                     continue
```

### Comparing `apkutils-1.2.4/apkutils/apkfile.py` & `apkutils-1.3.0/apkutils/apkfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -1247,14 +1247,18 @@
         """Read all the files and check the CRC."""
         chunk_size = 2 ** 20
         for zinfo in self.filelist:
             try:
                 # Read by chunks, to avoid an OverflowError or a
                 # MemoryError with very large embedded files.
                 with self.open(zinfo.filename, "r") as f:
+                    name = zinfo.filename.split(os.path.sep)[-1]
+                    if len(name) > 255:
+                        print("存在超过255个字符串的文件名，跳过")
+                        continue
                     while f.read(chunk_size):  # Check CRC-32
                         pass
             except BadZipFile:
                 return zinfo.filename
 
     def getinfo(self, name):
         """Return the instance of ZipInfo given 'name'."""
@@ -1358,23 +1362,25 @@
             # NOTE 添加加密flag，对抗
             # if zinfo.flag_bits & 0x40:
             # # strong encryption
             # raise NotImplementedError("strong encryption (flag bit 6)")
 
             if zinfo.flag_bits & 0x800:
                 # UTF-8 filename
-                fname_str = fname.decode("utf-8")
+                # NOTE 如果有错误，则忽略
+                fname_str = fname.decode("utf-8", errors="ignore")
             else:
                 fname_str = fname.decode("cp437")
 
-            if fname_str != zinfo.orig_filename:
-                raise BadZipFile(
-                    "File name in directory %r and header %r differ."
-                    % (zinfo.orig_filename, fname)
-                )
+            # TODO 存在编码问题
+            # if fname_str != zinfo.orig_filename:
+            #     raise BadZipFile(
+            #         "File name in directory %r and header %r differ."
+            #         % (zinfo.orig_filename, fname)
+            #     )
 
             return ZipExtFile(zef_file, mode, zinfo, None, True)
         except Exception as ignore:
             zef_file.close()
             raise
 
     def extract(self, member, path=None, pwd=None):
@@ -1435,17 +1441,30 @@
         arcname = os.path.sep.join(
             x for x in arcname.split(os.path.sep) if x not in invalid_path_parts
         )
         if os.path.sep == "\\":
             # filter illegal characters on Windows
             arcname = self._sanitize_windows_name(arcname, os.path.sep)
 
+        # NOTE 文件名超过255无法写入
+        arr = arcname.split(os.path.sep)
+        name = arr[-1]
+        if len(name) > 255:
+            extension = os.path.splitext(name)[1]
+            name = "too_long_" + str(crc32(name.encode("utf-8"))) + extension
+            arr = arr[:-1]
+            print("{} 存在超过255个字符的文件名，跳过解压。".format(os.path.sep.join(arr)))
+            # arr.append(name)
+            # arcname = os.path.sep.join(arr)
+            # FIXME 对于该类文件名暂时无法解压，暂时跳过
+            return
+
         targetpath = os.path.join(targetpath, arcname)
         targetpath = os.path.normpath(targetpath)
-
+        
         # Create all upper directories if necessary.
         upperdirs = os.path.dirname(targetpath)
         if upperdirs and not os.path.exists(upperdirs):
             os.makedirs(upperdirs)
 
         if member.filename[-1] == "/":
             if not os.path.isdir(targetpath):
```

### Comparing `apkutils-1.2.4/apkutils/axml/__init__.py` & `apkutils-1.3.0/apkutils/axml/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,14 +116,15 @@
         
         self.styleCount = 0
         if is_android_manifest:
             buff.read(4)
         else:
             self.styleCount = unpack("<I", buff.read(4))[0]
 
+        
         # flags is_utf8
         self.flags = unpack("<I", buff.read(4))[0]
         self.m_isUTF8 = (self.flags & UTF8_FLAG) != 0
 
         # string_pool_offset
         # The string offset is counted from the beginning of the string section
         self.stringsOffset = unpack("<I", buff.read(4))[0]
@@ -138,32 +139,30 @@
 
         # Check if they supplied a stylesOffset even if the count is 0:
         if self.styleCount == 0 and self.stylesOffset > 0:
             log.info(
                 "Styles Offset given, but styleCount is zero. "
                 "This is not a problem but could indicate packers."
             )
-
+        
         self.m_stringOffsets = []
         self.m_styleOffsets = []
         self.m_charbuff = ""
         self.m_styles = []
 
-        # Next, there is a list of string following.
-        # This is only a list of offsets (4 byte each)
         for i in range(self.stringCount):
             offset = unpack("<I", buff.read(4))[0]
             self.m_stringOffsets.append(offset)
             
-            # NOTE 如果offset是0，说明有问题
-            if i > 0 and offset == 0:
+            # NOTE stringCount 有可能是伪造的
+            # 正常情况下，stringCount + 8，就是buff当前的位置
+            if self.stringsOffset + 8 == buff.get_idx():
                 self.stringCount = i
-                buff.set_idx(buff.get_idx()-4)
+                buff.set_idx(buff.get_idx())
                 break
-        
 
         # And a list of styles
         # again, a list of offsets
         for i in range(self.styleCount):
             self.m_styleOffsets.append(unpack("<I", buff.read(4))[0])
 
         size = self.header.size - self.stringsOffset
@@ -183,14 +182,16 @@
 
             if (size % 4) != 0:
                 log.warning("Size of styles is not aligned by four bytes.")
 
             for i in range(0, size // 4):
                 self.m_styles.append(unpack("<I", buff.read(4))[0])
         
+        # self.show()
+        
     def __repr__(self):
         return "<StringPool #strings={}, #styles={}, UTF8={}>".format(
             self.stringCount, self.styleCount, self.m_isUTF8
         )
 
     def __getitem__(self, idx):
         """
@@ -282,17 +283,19 @@
 
         data = self.m_charbuff[offset : offset + encoded_bytes]
 
         if (
             self.m_charbuff[offset + encoded_bytes : offset + encoded_bytes + 2]
             != b"\x00\x00"
         ):
-            raise ResParserError(
-                "UTF-16 String is not null terminated! At offset={}".format(offset)
-            )
+            # raise ResParserError(
+            #     "UTF-16 String is not null terminated! At offset={}".format(offset)
+            # )
+            # NOTE 清单被混淆，暂时使用这个做替换，这种处理方式，不大好
+            return "android"
 
         return self._decode_bytes(data, "utf-16", str_len)
 
     @staticmethod
     def _decode_bytes(data, encoding, str_len):
         """
         Generic decoding with length check.
@@ -302,17 +305,17 @@
 
         :param data: bytes
         :param encoding: encoding name ("utf-8" or "utf-16")
         :param str_len: length of the decoded string
         :return: str
         """
         # string = data.decode(encoding, 'replace')
-        # * 直接忽略，避免乱码
+        # NOTE 直接忽略，避免乱码
         string = data.decode(encoding, "ignore")
-        # * 移除日志，没有必要输出
+        # NOTE 移除日志，没有必要输出
         # if len(string) != str_len:
         #     log.warning("invalid decoded string length")
         return string
 
     def _decode_length(self, offset, sizeof_char):
         """
         Generic Length Decoding at offset of string
@@ -481,24 +484,17 @@
             log.warning(
                 "Declared filesize ({}) is smaller than total file size ({}). "
                 "Was something appended to the file? Trying to parse it anyways.".format(
                     self.filesize, self.buff.size()
                 )
             )
 
-        # Not that severe of an error, we have plenty files where this is not
-        # set correctly
+        # NOTE 判断是否是AXML文件，没啥用
         if axml_header.type != RES_XML_TYPE:
             self.axml_tampered = True
-            log.warning(
-                "AXML有一个不常见的资源类型! "
-                "But we try to parse it anyways. Resource Type: 0x{:04x}".format(
-                    axml_header.type
-                )
-            )
 
         # Now we parse the STRING POOL
         try:
             header = ARSCHeader(self.buff, expected_type=RES_STRING_POOL_TYPE)
         except ResParserError as e:
             log.error("Error parsing resource header of string pool: %s", e)
             self._valid = False
@@ -1720,15 +1716,14 @@
                 "Out of range dimension unit index for {}: {}".format(
                     complexToFloat(ate.key.get_data()),
                     ate.key.get_data() & COMPLEX_UNIT_MASK,
                 )
             )
             return [ate.get_value(), ate.key.get_data()]
 
-    # FIXME
     def get_resource_style(self, ate):
         return ["", ""]
 
     def get_packages_names(self):
         """
         Retrieve a list of all package names, which are available
         in the given resources.arsc.
```

### Comparing `apkutils-1.2.4/apkutils/axml/bytecode.py` & `apkutils-1.3.0/apkutils/axml/bytecode.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.4/apkutils/axml/public.py` & `apkutils-1.3.0/apkutils/axml/public.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.4/apkutils/axml/public.xml` & `apkutils-1.3.0/apkutils/axml/public.xml`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.4/apkutils/axml/types.py` & `apkutils-1.3.0/apkutils/axml/types.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.4/apkutils/cert.py` & `apkutils-1.3.0/apkutils/cert.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.4/apkutils/cli.py` & `apkutils-1.3.0/apkutils/cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,26 +13,41 @@
 @click.group()
 @click.version_option(__version__)
 def main():
     pass
 
 
 # TODO 增加解压命令
-# @main.command()
-# @click.argument("args")
-# def unzip(args):
-#     """解压文件, help可以看命令"""
-#     apkfile.main(args)
-
+@main.command()
+@click.argument("path", type=click.Path(exists=True))
+# @click.option("-l", is_flag=True, help="Show listing of a zipfile")
+@click.option("-t", is_flag=True, help="Test if a zipfile is valid")
+@click.option("-e", is_flag=True, help="Extract zipfile into target dir")
+@click.option("-o", "--output", default="out", help="Output directory")
+def unzip(path, t, e, output):
+    """解压文件，默认显示zip文件"""
+    if e:
+        with apkfile.ZipFile(path, "r") as zf:
+            zf.extractall(output)
+    elif t:
+        with apkfile.ZipFile(path, "r") as zf:
+            badfile = zf.testzip()
+        if badfile:
+            print("The following enclosed file is corrupted: {!r}".format(badfile))
+        print("Done testing")
+    else:
+        with apkfile.ZipFile(path, "r") as zf:
+            zf.printdir()
+    
 
 @main.command()
 @click.argument("path")
 def manifest(path):
     """打印清单"""
-    apk = APK.from_file(path)
+    apk = APK.from_file(path).parse_manifest()
     manifest = apk.get_manifest()
     if manifest is None:
         print("Manifest is None!")
         return
 
     sys.stdout.write(
         highlight(manifest, get_lexer_by_name("xml"), TerminalFormatter())
@@ -83,15 +98,15 @@
     sys.stdout.write(highlight(data, get_lexer_by_name("xml"), TerminalFormatter()))
 
 
 @main.command()
 @click.argument("path")
 def strings(path):
     """打印Dex中的字符串"""
-    apk = APK.from_file(path)
+    apk = APK.from_file(path).parse_dex()
     s = sorted(apk.get_dex_strings())
     for item in s:
         print(item)
 
 
 @main.command()
 @click.argument("path")
@@ -116,15 +131,15 @@
 @click.option(
     "-m",
     "--method",
     help="指定方法，如 top/cls->mtd(Landroid/app/Application;Ljava/lang/String;Ljava/lang/String;)V",
 )
 def mtds(path, method):
     """获取指定方法中的所有字符串"""
-    apk = APK.from_file(path)
+    apk = APK.from_file(path).parse_dex()
     strs = apk.get_dex_method_strings(method)
     if strs is None:
         return
 
     for item in strs:
         print(item)
 
@@ -134,15 +149,15 @@
 @click.option(
     "-m",
     "--method",
     help="指定方法，如 top/cls->mtd(Landroid/app/Application;Ljava/lang/String;Ljava/lang/String;)V",
 )
 def xref(path, method):
     """获取方法的引用方法"""
-    apk = APK.from_file(path)
+    apk = APK.from_file(path).parse_dex()
     strs = apk.xref(method)
     if strs is None:
         return
 
     for item in strs:
         print(item)
```

### Comparing `apkutils-1.2.4/apkutils/dex/__init__.py` & `apkutils-1.3.0/apkutils/dex/__init__.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.4/apkutils/dex/byteio.py` & `apkutils-1.3.0/apkutils/dex/byteio.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.4/apkutils/dex/dalvik.py` & `apkutils-1.3.0/apkutils/dex/dalvik.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.4/apkutils/dex/dalvikformats.py` & `apkutils-1.3.0/apkutils/dex/dalvikformats.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.4/apkutils/dex/dexparser.py` & `apkutils-1.3.0/apkutils/dex/dexparser.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.4/apkutils/dex/flags.py` & `apkutils-1.3.0/apkutils/dex/flags.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.4/apkutils/dex/jvm/__init__.py` & `apkutils-1.3.0/apkutils/dex/jvm/__init__.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.4/apkutils/dex/jvm/arraytypes.py` & `apkutils-1.3.0/apkutils/dex/jvm/arraytypes.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.4/apkutils/dex/jvm/constantpool.py` & `apkutils-1.3.0/apkutils/dex/jvm/constantpool.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.4/apkutils/dex/jvm/constants/__init__.py` & `apkutils-1.3.0/apkutils/dex/jvm/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.4/apkutils/dex/jvm/constants/calc.py` & `apkutils-1.3.0/apkutils/dex/jvm/constants/calc.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.4/apkutils/dex/jvm/constants/genlookup.py` & `apkutils-1.3.0/apkutils/dex/jvm/constants/genlookup.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.4/apkutils/dex/jvm/constants/lookup.py` & `apkutils-1.3.0/apkutils/dex/jvm/constants/lookup.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.4/apkutils/dex/jvm/error.py` & `apkutils-1.3.0/apkutils/dex/jvm/error.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.4/apkutils/dex/jvm/genmathops.py` & `apkutils-1.3.0/apkutils/dex/jvm/genmathops.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.4/apkutils/dex/jvm/ir.py` & `apkutils-1.3.0/apkutils/dex/jvm/ir.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.4/apkutils/dex/jvm/jvmops.py` & `apkutils-1.3.0/apkutils/dex/jvm/jvmops.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.4/apkutils/dex/jvm/mathops.py` & `apkutils-1.3.0/apkutils/dex/jvm/mathops.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.4/apkutils/dex/jvm/optimization/__init__.py` & `apkutils-1.3.0/apkutils/dex/jvm/optimization/__init__.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.4/apkutils/dex/jvm/optimization/consts.py` & `apkutils-1.3.0/apkutils/dex/jvm/optimization/consts.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.4/apkutils/dex/jvm/optimization/jumps.py` & `apkutils-1.3.0/apkutils/dex/jvm/optimization/jumps.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.4/apkutils/dex/jvm/optimization/options.py` & `apkutils-1.3.0/apkutils/dex/jvm/optimization/options.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.4/apkutils/dex/jvm/optimization/registers.py` & `apkutils-1.3.0/apkutils/dex/jvm/optimization/registers.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.4/apkutils/dex/jvm/optimization/stack.py` & `apkutils-1.3.0/apkutils/dex/jvm/optimization/stack.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.4/apkutils/dex/jvm/scalartypes.py` & `apkutils-1.3.0/apkutils/dex/jvm/scalartypes.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.4/apkutils/dex/jvm/writebytecode.py` & `apkutils-1.3.0/apkutils/dex/jvm/writebytecode.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.4/apkutils/dex/jvm/writeclass.py` & `apkutils-1.3.0/apkutils/dex/jvm/writeclass.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.4/apkutils/dex/jvm/writeir.py` & `apkutils-1.3.0/apkutils/dex/jvm/writeir.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.4/apkutils/dex/mutf8.py` & `apkutils-1.3.0/apkutils/dex/mutf8.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.4/apkutils/dex/treelist.py` & `apkutils-1.3.0/apkutils/dex/treelist.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.4/apkutils/dex/typeinference/__init__.py` & `apkutils-1.3.0/apkutils/dex/typeinference/__init__.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.4/apkutils/dex/typeinference/typeinference.py` & `apkutils-1.3.0/apkutils/dex/typeinference/typeinference.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.4/apkutils/dex/util.py` & `apkutils-1.3.0/apkutils/dex/util.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.4/apkutils/elf/elfparser.py` & `apkutils-1.3.0/apkutils/elf/elfparser.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.4/apkutils/gdiff.py` & `apkutils-1.3.0/apkutils/gdiff.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.4/apkutils/intersection.py` & `apkutils-1.3.0/apkutils/intersection.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.4/apkutils/wildcard.py` & `apkutils-1.3.0/apkutils/wildcard.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.2.4/pyproject.toml` & `apkutils-1.3.0/pyproject.toml`

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
-version = "1.2.4"
+version = "1.3.0"
 
 [tool.poetry.dependencies]
 Pygments = "^2.12.0"
 beautifulsoup4 = "^4.10.0"
 click = "^8.0.3"
 cryptography = "^35.0.0"
 lxml = "^4.6.4"
```

### Comparing `apkutils-1.2.4/PKG-INFO` & `apkutils-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apkutils
-Version: 1.2.4
+Version: 1.3.0
 Summary: 一个APK解析库
 Home-page: https://gitee.com/kin9-0rz/apkutils
 License: MIT
 Author: kin9-0rz
 Author-email: kin9-0rz@outlook.com
 Requires-Python: >=3.8
 Classifier: Development Status :: 3 - Alpha
```

