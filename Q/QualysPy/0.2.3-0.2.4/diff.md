# Comparing `tmp/qualyspy-0.2.3.tar.gz` & `tmp/qualyspy-0.2.4.tar.gz`

## Comparing `qualyspy-0.2.3.tar` & `qualyspy-0.2.4.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 qualyspy-0.2.3/.vscode/launch.json
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 qualyspy-0.2.3/.vscode/settings.json
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 qualyspy-0.2.3/.vscode/tasks.json
--rwxr-xr-x   0        0        0      112 2020-02-02 00:00:00.000000 qualyspy-0.2.3/debug/build.sh
--rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 qualyspy-0.2.3/debug/dtd.txt
--rw-r--r--   0        0        0     5215 2020-02-02 00:00:00.000000 qualyspy-0.2.3/debug/output.txt
--rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 qualyspy-0.2.3/debug/parse_dtd.py
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 qualyspy-0.2.3/debug/quickscan.py
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 qualyspy-0.2.3/debug/remove_cookies.py
--rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 qualyspy-0.2.3/debug/test.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 qualyspy-0.2.3/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 qualyspy-0.2.3/docs/make.bat
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 qualyspy-0.2.3/docs/source/conf.py
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 qualyspy-0.2.3/docs/source/index.rst
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 qualyspy-0.2.3/docs/source/modules.rst
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 qualyspy-0.2.3/docs/source/qualyspy.assets.host_list.rst
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 qualyspy-0.2.3/docs/source/qualyspy.assets.host_list_detection.rst
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 qualyspy-0.2.3/docs/source/qualyspy.qualysapi.rst
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 qualyspy-0.2.3/docs/source/qualyspy.qutils.rst
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 qualyspy-0.2.3/docs/source/qualyspy.rst
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 qualyspy-0.2.3/docs/source/qualyspy.scan_configuration.knowledgebase.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.2.3/qualyspy/__init__.py
--rw-r--r--   0        0        0    17347 2020-02-02 00:00:00.000000 qualyspy-0.2.3/qualyspy/qualysapi.py
--rw-r--r--   0        0        0    16528 2020-02-02 00:00:00.000000 qualyspy-0.2.3/qualyspy/qutils.py
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 qualyspy-0.2.3/qualyspy/urls.json
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 qualyspy-0.2.3/qualyspy/asset_mgmt_tagging/__init__.py
--rw-r--r--   0        0        0     4056 2020-02-02 00:00:00.000000 qualyspy-0.2.3/qualyspy/asset_mgmt_tagging/asset.py
--rw-r--r--   0        0        0     9905 2020-02-02 00:00:00.000000 qualyspy-0.2.3/qualyspy/asset_mgmt_tagging/tags.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.2.3/qualyspy/assets/__init__.py
--rw-r--r--   0        0        0    30142 2020-02-02 00:00:00.000000 qualyspy-0.2.3/qualyspy/assets/host_list.py
--rw-r--r--   0        0        0    40811 2020-02-02 00:00:00.000000 qualyspy-0.2.3/qualyspy/assets/host_list_detection.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.2.3/qualyspy/certview/__init__.py
--rw-r--r--   0        0        0    15230 2020-02-02 00:00:00.000000 qualyspy-0.2.3/qualyspy/certview/certificate.py
--rw-r--r--   0        0        0     5068 2020-02-02 00:00:00.000000 qualyspy-0.2.3/qualyspy/certview/sql/certview_init.sql
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.2.3/qualyspy/scan_configuration/__init__.py
--rw-r--r--   0        0        0    24210 2020-02-02 00:00:00.000000 qualyspy-0.2.3/qualyspy/scan_configuration/knowledgebase.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 qualyspy-0.2.3/requirements/deploy.txt
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 qualyspy-0.2.3/requirements/dev.txt
--rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 qualyspy-0.2.3/.gitignore
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 qualyspy-0.2.3/LICENSE
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 qualyspy-0.2.3/README.md
--rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 qualyspy-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 qualyspy-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 qualyspy-0.2.4/.vscode/launch.json
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 qualyspy-0.2.4/.vscode/settings.json
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 qualyspy-0.2.4/.vscode/tasks.json
+-rwxr-xr-x   0        0        0      112 2020-02-02 00:00:00.000000 qualyspy-0.2.4/debug/build.sh
+-rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 qualyspy-0.2.4/debug/dtd.txt
+-rw-r--r--   0        0        0     5215 2020-02-02 00:00:00.000000 qualyspy-0.2.4/debug/output.txt
+-rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 qualyspy-0.2.4/debug/parse_dtd.py
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 qualyspy-0.2.4/debug/quickscan.py
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 qualyspy-0.2.4/debug/remove_cookies.py
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 qualyspy-0.2.4/debug/test.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 qualyspy-0.2.4/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 qualyspy-0.2.4/docs/make.bat
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 qualyspy-0.2.4/docs/source/conf.py
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 qualyspy-0.2.4/docs/source/index.rst
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 qualyspy-0.2.4/docs/source/modules.rst
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 qualyspy-0.2.4/docs/source/qualyspy.assets.host_list.rst
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 qualyspy-0.2.4/docs/source/qualyspy.assets.host_list_detection.rst
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 qualyspy-0.2.4/docs/source/qualyspy.qualysapi.rst
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 qualyspy-0.2.4/docs/source/qualyspy.qutils.rst
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 qualyspy-0.2.4/docs/source/qualyspy.rst
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 qualyspy-0.2.4/docs/source/qualyspy.scan_configuration.knowledgebase.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.2.4/qualyspy/__init__.py
+-rw-r--r--   0        0        0    17347 2020-02-02 00:00:00.000000 qualyspy-0.2.4/qualyspy/qualysapi.py
+-rw-r--r--   0        0        0    16528 2020-02-02 00:00:00.000000 qualyspy-0.2.4/qualyspy/qutils.py
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 qualyspy-0.2.4/qualyspy/urls.json
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 qualyspy-0.2.4/qualyspy/asset_mgmt_tagging/__init__.py
+-rw-r--r--   0        0        0     4056 2020-02-02 00:00:00.000000 qualyspy-0.2.4/qualyspy/asset_mgmt_tagging/asset.py
+-rw-r--r--   0        0        0     9905 2020-02-02 00:00:00.000000 qualyspy-0.2.4/qualyspy/asset_mgmt_tagging/tags.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.2.4/qualyspy/assets/__init__.py
+-rw-r--r--   0        0        0    30142 2020-02-02 00:00:00.000000 qualyspy-0.2.4/qualyspy/assets/host_list.py
+-rw-r--r--   0        0        0    40811 2020-02-02 00:00:00.000000 qualyspy-0.2.4/qualyspy/assets/host_list_detection.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.2.4/qualyspy/certview/__init__.py
+-rw-r--r--   0        0        0    15254 2020-02-02 00:00:00.000000 qualyspy-0.2.4/qualyspy/certview/certificate.py
+-rw-r--r--   0        0        0     5068 2020-02-02 00:00:00.000000 qualyspy-0.2.4/qualyspy/certview/sql/certview_init.sql
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.2.4/qualyspy/scan_configuration/__init__.py
+-rw-r--r--   0        0        0    24210 2020-02-02 00:00:00.000000 qualyspy-0.2.4/qualyspy/scan_configuration/knowledgebase.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 qualyspy-0.2.4/requirements/deploy.txt
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 qualyspy-0.2.4/requirements/dev.txt
+-rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 qualyspy-0.2.4/.gitignore
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 qualyspy-0.2.4/LICENSE
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 qualyspy-0.2.4/README.md
+-rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 qualyspy-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 qualyspy-0.2.4/PKG-INFO
```

### Comparing `qualyspy-0.2.3/.vscode/launch.json` & `qualyspy-0.2.4/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.3/debug/dtd.txt` & `qualyspy-0.2.4/debug/dtd.txt`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.3/debug/output.txt` & `qualyspy-0.2.4/debug/output.txt`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.3/debug/parse_dtd.py` & `qualyspy-0.2.4/debug/parse_dtd.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.3/debug/quickscan.py` & `qualyspy-0.2.4/debug/quickscan.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.3/debug/remove_cookies.py` & `qualyspy-0.2.4/debug/remove_cookies.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.3/debug/test.py` & `qualyspy-0.2.4/debug/test.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,32 +12,39 @@
 parentdir = os.path.dirname(currentdir)
 sys.path.insert(0, parentdir)
 
 from qualyspy.qualysapi import Connection
 import qualyspy.certview.certificate as cert
 
 if __name__ == "__main__":
-    conn = Connection(apis = ["CertView"])
+    conn = Connection(apis=["CertView"])
     api = cert.List_Certificates_V2(conn)
 
     # fvo = cert.Field_Value_Operator(field="certificate.id", operator="EQUALS", value="39534")
     # filter = cert.Filter(filters=[fvo])
     # input = cert.List_CertView_Certificates_V2_Input(filter=filter)
     # test = api.call(input)
 
-    #api.reset(echo = True)
-    #test = api.load(echo=True)
+    # api.reset(echo = True)
+    # test = api.load(echo=True)
 
-    stmt = sa.Select(cert.Certificate_ORM).where(cert.Certificate_ORM.self_signed == False)
-    test = api.query(stmt, echo = True)
+    # stmt = sa.Select(cert.Certificate_ORM).where(cert.Certificate_ORM.self_signed == False)
+    # test = api.query(stmt, echo = True)
 
-    # stmt = sa.select(
-    # cert.Host_Instance_ORM.fqdn,
-    # cert.Host_Instance_ORM.protocol,
-    # cert.Host_Instance_ORM.port,
-    # )
-
-    # hosts = api.query(stmt, echo=True)
-    # for host in hosts:
-    #    print(host)
+    stmt = (
+        sa.select(
+            cert.Subject_ORM.name,
+            cert.Asset_Interface_ORM.address,
+            cert.Host_Instance_ORM.protocol,
+            cert.Host_Instance_ORM.port,
+        )
+        .join(cert.Certificate_ORM)
+        .join(cert.Asset_ORM)
+        .join(cert.Asset_Interface_ORM)
+        .join(cert.Asset_ORM.host_instances)
+    )
+
+    hosts = api.query(stmt, echo=True)
+    for host in hosts:
+        print(host)
 
     print("test")
```

### Comparing `qualyspy-0.2.3/docs/Makefile` & `qualyspy-0.2.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.3/docs/make.bat` & `qualyspy-0.2.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.3/docs/source/conf.py` & `qualyspy-0.2.4/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.3/qualyspy/qualysapi.py` & `qualyspy-0.2.4/qualyspy/qualysapi.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.3/qualyspy/qutils.py` & `qualyspy-0.2.4/qualyspy/qutils.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.3/qualyspy/urls.json` & `qualyspy-0.2.4/qualyspy/urls.json`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.3/qualyspy/asset_mgmt_tagging/asset.py` & `qualyspy-0.2.4/qualyspy/asset_mgmt_tagging/asset.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.3/qualyspy/asset_mgmt_tagging/tags.py` & `qualyspy-0.2.4/qualyspy/asset_mgmt_tagging/tags.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.3/qualyspy/assets/host_list.py` & `qualyspy-0.2.4/qualyspy/assets/host_list.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.3/qualyspy/assets/host_list_detection.py` & `qualyspy-0.2.4/qualyspy/assets/host_list_detection.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.3/qualyspy/certview/certificate.py` & `qualyspy-0.2.4/qualyspy/certview/certificate.py`

 * *Files 0% similar despite different names*

```diff
@@ -261,15 +261,15 @@
 
     id: orm.Mapped[int] = orm.mapped_column(primary_key=True)
     uuid: orm.Mapped[str]
     netbios_name: orm.Mapped[str]
     name: orm.Mapped[str]
     operating_system: orm.Mapped[str | None]
     host_instances: orm.Mapped[list[Host_Instance_ORM]] = orm.relationship(
-        secondary=asset_host_instance_association_table
+        secondary=asset_host_instance_association_table, back_populates="asset"
     )
     asset_interfaces: orm.Mapped[list[Asset_Interface_ORM] | None] = orm.relationship(
         back_populates="asset"
     )
 
     certificate_id: orm.Mapped[int] = orm.mapped_column(sa.ForeignKey("certificate.id"))
     certificate: orm.Mapped["Certificate_ORM"] = orm.relationship(
```

### Comparing `qualyspy-0.2.3/qualyspy/certview/sql/certview_init.sql` & `qualyspy-0.2.4/qualyspy/certview/sql/certview_init.sql`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.3/qualyspy/scan_configuration/knowledgebase.py` & `qualyspy-0.2.4/qualyspy/scan_configuration/knowledgebase.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.3/.gitignore` & `qualyspy-0.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.3/LICENSE` & `qualyspy-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.3/pyproject.toml` & `qualyspy-0.2.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "QualysPy"
-version = "0.2.3"
+version = "0.2.4"
 authors = [
   { name="Jordan Barnartt", email="jbarnart@uwaterloo.ca" },
 ]
 description = "A Python wrapper for the Qualys API."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `qualyspy-0.2.3/PKG-INFO` & `qualyspy-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QualysPy
-Version: 0.2.3
+Version: 0.2.4
 Summary: A Python wrapper for the Qualys API.
 Project-URL: Homepage, https://github.com/JordanBarnartt/qualyspy
 Project-URL: Bug Tracker, https://github.com/JordanBarnartt/qualyspy/issues
 Author-email: Jordan Barnartt <jbarnart@uwaterloo.ca>
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Information Technology
```

