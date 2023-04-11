# Comparing `tmp/cnd_cr_obj_naming-0.2.1-py3-none-any.whl.zip` & `tmp/cnd_cr_obj_naming-0.2.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 3422 bytes, number of entries: 9
--rw-rw-rw-  2.0 unx        5 b- defN 23-Apr-09 15:43 cr_obj_naming/VERSION
--rw-r--r--  2.0 unx      187 b- defN 23-Apr-09 15:43 cr_obj_naming/__init__.py
--rw-r--r--  2.0 unx      122 b- defN 23-Apr-09 15:43 cr_obj_naming/__version__.py
--rw-r--r--  2.0 unx     1273 b- defN 23-Apr-09 15:43 cr_obj_naming/cnd_consul.py
--rw-r--r--  2.0 unx     1433 b- defN 23-Apr-09 15:43 cr_obj_naming/obj_naming.py
--rw-r--r--  2.0 unx      825 b- defN 23-Apr-09 15:43 cnd_cr_obj_naming-0.2.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-09 15:43 cnd_cr_obj_naming-0.2.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 23-Apr-09 15:43 cnd_cr_obj_naming-0.2.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      745 b- defN 23-Apr-09 15:43 cnd_cr_obj_naming-0.2.1.dist-info/RECORD
-9 files, 4696 bytes uncompressed, 2124 bytes compressed:  54.8%
+Zip file size: 3475 bytes, number of entries: 9
+-rw-rw-rw-  2.0 unx        5 b- defN 23-Apr-11 21:16 cr_obj_naming/VERSION
+-rw-r--r--  2.0 unx      187 b- defN 23-Apr-11 21:16 cr_obj_naming/__init__.py
+-rw-r--r--  2.0 unx      122 b- defN 23-Apr-11 21:16 cr_obj_naming/__version__.py
+-rw-r--r--  2.0 unx     1459 b- defN 23-Apr-11 21:16 cr_obj_naming/cnd_consul.py
+-rw-r--r--  2.0 unx     1433 b- defN 23-Apr-11 21:16 cr_obj_naming/obj_naming.py
+-rw-r--r--  2.0 unx      825 b- defN 23-Apr-11 21:17 cnd_cr_obj_naming-0.2.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-11 21:17 cnd_cr_obj_naming-0.2.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 23-Apr-11 21:17 cnd_cr_obj_naming-0.2.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      745 b- defN 23-Apr-11 21:17 cnd_cr_obj_naming-0.2.3.dist-info/RECORD
+9 files, 4882 bytes uncompressed, 2177 bytes compressed:  55.4%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: cr_obj_naming/cnd_consul.py
 Comment: 
 
 Filename: cr_obj_naming/obj_naming.py
 Comment: 
 
-Filename: cnd_cr_obj_naming-0.2.1.dist-info/METADATA
+Filename: cnd_cr_obj_naming-0.2.3.dist-info/METADATA
 Comment: 
 
-Filename: cnd_cr_obj_naming-0.2.1.dist-info/WHEEL
+Filename: cnd_cr_obj_naming-0.2.3.dist-info/WHEEL
 Comment: 
 
-Filename: cnd_cr_obj_naming-0.2.1.dist-info/top_level.txt
+Filename: cnd_cr_obj_naming-0.2.3.dist-info/top_level.txt
 Comment: 
 
-Filename: cnd_cr_obj_naming-0.2.1.dist-info/RECORD
+Filename: cnd_cr_obj_naming-0.2.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cr_obj_naming/VERSION

```diff
@@ -1 +1 @@
-0.2.1
+0.2.3
```

## cr_obj_naming/cnd_consul.py

```diff
@@ -1,23 +1,27 @@
 import consul
 import json
 
 
 class CndConsul():
-	def __init__(self, host, port, token, path, print):
+	def __init__(self, host, port, token, path, print, scheme='https', verify=False):
 		self._print = print
 		self.consul_creds = {}
 		self.consul_creds["host"] = host
 		self.consul_creds["token"] = token
 		self.consul_creds["path"] = path
 		self.consul_creds["port"] = port
+		self.consul_creds["scheme"] = scheme
+		self.consul_creds["verify"] = verify
 		self.consul = consul.Consul(
 			host=self.consul_creds["host"],
 			port=self.consul_creds["port"],
-			token=self.consul_creds["token"]
+			token=self.consul_creds["token"],
+			scheme=self.consul_creds["scheme"],
+			verify=self.consul_creds["verify"]
 		)
 
 	def full_path(self, deployment_id=None):
 		str = f'{self.consul_creds["path"]}/'
 		if deployment_id is not None:
 			str = f'{str}{deployment_id}'
 		self._print.trace_d(f'Path : {str}')
```

## Comparing `cnd_cr_obj_naming-0.2.1.dist-info/METADATA` & `cnd_cr_obj_naming-0.2.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnd-cr-obj-naming
-Version: 0.2.1
+Version: 0.2.3
 Summary: Base for vro Custom Resource Object Naming
 Home-page: https://gitlab.com/changendevops/cloudtools/cnd-cr-object.git
 Author: Denis FABIEN
 Author-email: denis.fabien@changendevops.com
 License: MIT/X11
 Project-URL: Documentation, https://changendevops.com
 Project-URL: Source, https://gitlab.com/changendevops/cloudtools/cnd-cr-object.git
```

## Comparing `cnd_cr_obj_naming-0.2.1.dist-info/RECORD` & `cnd_cr_obj_naming-0.2.3.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-cr_obj_naming/VERSION,sha256=GWZm1qfrRYP7nLHhWZcQELLim1t1Kqc_RW4OIGG2Ql8,5
+cr_obj_naming/VERSION,sha256=XSSKc1S0uwOYYmkC_fs0xKSWJb5x9x3if9NA5sO4Xkw,5
 cr_obj_naming/__init__.py,sha256=1uv3gz09BL1cmYDLPne0PkqXcvqxLP9jy2DjeeyDCrA,187
 cr_obj_naming/__version__.py,sha256=ikxlExFPaHGK8AzUG9pDnI7Sm8GtkjdM12d5iJMRgik,122
-cr_obj_naming/cnd_consul.py,sha256=VWblp70qx6CJ4aiSLsWKciUfBgs9v53aUOj8Yl17rTk,1273
+cr_obj_naming/cnd_consul.py,sha256=BGjFqm0UO2TQf-VW_ZhpfyRw0zF6JGswis0XTmTh9Ok,1459
 cr_obj_naming/obj_naming.py,sha256=EFivRyeS8NsRD-QrIrWDAVnkC1BGkgvu0An9vB10m2A,1433
-cnd_cr_obj_naming-0.2.1.dist-info/METADATA,sha256=F4H9UmZH3uTmHV8PKnDbVC41NT7Q9lMWoFGg8xbpM7Q,825
-cnd_cr_obj_naming-0.2.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-cnd_cr_obj_naming-0.2.1.dist-info/top_level.txt,sha256=IxheoHqwoyK8b3XMzAfOoe8Owc9qJeKmqwl2BTPOmBU,14
-cnd_cr_obj_naming-0.2.1.dist-info/RECORD,,
+cnd_cr_obj_naming-0.2.3.dist-info/METADATA,sha256=Fdi0D99PN_ZXnIXGQ1jy_VTgeYqZL0RE7ymGTK_ZHG4,825
+cnd_cr_obj_naming-0.2.3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+cnd_cr_obj_naming-0.2.3.dist-info/top_level.txt,sha256=IxheoHqwoyK8b3XMzAfOoe8Owc9qJeKmqwl2BTPOmBU,14
+cnd_cr_obj_naming-0.2.3.dist-info/RECORD,,
```

