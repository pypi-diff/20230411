# Comparing `tmp/qualyspy-0.2.2.tar.gz` & `tmp/qualyspy-0.2.3.tar.gz`

## Comparing `qualyspy-0.2.2.tar` & `qualyspy-0.2.3.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 qualyspy-0.2.2/.vscode/launch.json
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 qualyspy-0.2.2/.vscode/settings.json
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 qualyspy-0.2.2/.vscode/tasks.json
--rwxr-xr-x   0        0        0      112 2020-02-02 00:00:00.000000 qualyspy-0.2.2/debug/build.sh
--rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 qualyspy-0.2.2/debug/dtd.txt
--rw-r--r--   0        0        0     5215 2020-02-02 00:00:00.000000 qualyspy-0.2.2/debug/output.txt
--rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 qualyspy-0.2.2/debug/parse_dtd.py
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 qualyspy-0.2.2/debug/quickscan.py
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 qualyspy-0.2.2/debug/remove_cookies.py
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 qualyspy-0.2.2/debug/test.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 qualyspy-0.2.2/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 qualyspy-0.2.2/docs/make.bat
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 qualyspy-0.2.2/docs/source/conf.py
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 qualyspy-0.2.2/docs/source/index.rst
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 qualyspy-0.2.2/docs/source/modules.rst
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 qualyspy-0.2.2/docs/source/qualyspy.assets.host_list.rst
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 qualyspy-0.2.2/docs/source/qualyspy.assets.host_list_detection.rst
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 qualyspy-0.2.2/docs/source/qualyspy.qualysapi.rst
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 qualyspy-0.2.2/docs/source/qualyspy.qutils.rst
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 qualyspy-0.2.2/docs/source/qualyspy.rst
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 qualyspy-0.2.2/docs/source/qualyspy.scan_configuration.knowledgebase.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.2.2/qualyspy/__init__.py
--rw-r--r--   0        0        0    17347 2020-02-02 00:00:00.000000 qualyspy-0.2.2/qualyspy/qualysapi.py
--rw-r--r--   0        0        0    16528 2020-02-02 00:00:00.000000 qualyspy-0.2.2/qualyspy/qutils.py
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 qualyspy-0.2.2/qualyspy/urls.json
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 qualyspy-0.2.2/qualyspy/asset_mgmt_tagging/__init__.py
--rw-r--r--   0        0        0     4056 2020-02-02 00:00:00.000000 qualyspy-0.2.2/qualyspy/asset_mgmt_tagging/asset.py
--rw-r--r--   0        0        0     9905 2020-02-02 00:00:00.000000 qualyspy-0.2.2/qualyspy/asset_mgmt_tagging/tags.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.2.2/qualyspy/assets/__init__.py
--rw-r--r--   0        0        0    30142 2020-02-02 00:00:00.000000 qualyspy-0.2.2/qualyspy/assets/host_list.py
--rw-r--r--   0        0        0    40811 2020-02-02 00:00:00.000000 qualyspy-0.2.2/qualyspy/assets/host_list_detection.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.2.2/qualyspy/certview/__init__.py
--rw-r--r--   0        0        0    17219 2020-02-02 00:00:00.000000 qualyspy-0.2.2/qualyspy/certview/certificate.py
--rw-r--r--   0        0        0     5068 2020-02-02 00:00:00.000000 qualyspy-0.2.2/qualyspy/certview/sql/certview_init.sql
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.2.2/qualyspy/scan_configuration/__init__.py
--rw-r--r--   0        0        0    24210 2020-02-02 00:00:00.000000 qualyspy-0.2.2/qualyspy/scan_configuration/knowledgebase.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 qualyspy-0.2.2/requirements/deploy.txt
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 qualyspy-0.2.2/requirements/dev.txt
--rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 qualyspy-0.2.2/.gitignore
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 qualyspy-0.2.2/LICENSE
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 qualyspy-0.2.2/README.md
--rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 qualyspy-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 qualyspy-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 qualyspy-0.2.3/.vscode/launch.json
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 qualyspy-0.2.3/.vscode/settings.json
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 qualyspy-0.2.3/.vscode/tasks.json
+-rwxr-xr-x   0        0        0      112 2020-02-02 00:00:00.000000 qualyspy-0.2.3/debug/build.sh
+-rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 qualyspy-0.2.3/debug/dtd.txt
+-rw-r--r--   0        0        0     5215 2020-02-02 00:00:00.000000 qualyspy-0.2.3/debug/output.txt
+-rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 qualyspy-0.2.3/debug/parse_dtd.py
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 qualyspy-0.2.3/debug/quickscan.py
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 qualyspy-0.2.3/debug/remove_cookies.py
+-rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 qualyspy-0.2.3/debug/test.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 qualyspy-0.2.3/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 qualyspy-0.2.3/docs/make.bat
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 qualyspy-0.2.3/docs/source/conf.py
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 qualyspy-0.2.3/docs/source/index.rst
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 qualyspy-0.2.3/docs/source/modules.rst
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 qualyspy-0.2.3/docs/source/qualyspy.assets.host_list.rst
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 qualyspy-0.2.3/docs/source/qualyspy.assets.host_list_detection.rst
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 qualyspy-0.2.3/docs/source/qualyspy.qualysapi.rst
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 qualyspy-0.2.3/docs/source/qualyspy.qutils.rst
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 qualyspy-0.2.3/docs/source/qualyspy.rst
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 qualyspy-0.2.3/docs/source/qualyspy.scan_configuration.knowledgebase.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.2.3/qualyspy/__init__.py
+-rw-r--r--   0        0        0    17347 2020-02-02 00:00:00.000000 qualyspy-0.2.3/qualyspy/qualysapi.py
+-rw-r--r--   0        0        0    16528 2020-02-02 00:00:00.000000 qualyspy-0.2.3/qualyspy/qutils.py
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 qualyspy-0.2.3/qualyspy/urls.json
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 qualyspy-0.2.3/qualyspy/asset_mgmt_tagging/__init__.py
+-rw-r--r--   0        0        0     4056 2020-02-02 00:00:00.000000 qualyspy-0.2.3/qualyspy/asset_mgmt_tagging/asset.py
+-rw-r--r--   0        0        0     9905 2020-02-02 00:00:00.000000 qualyspy-0.2.3/qualyspy/asset_mgmt_tagging/tags.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.2.3/qualyspy/assets/__init__.py
+-rw-r--r--   0        0        0    30142 2020-02-02 00:00:00.000000 qualyspy-0.2.3/qualyspy/assets/host_list.py
+-rw-r--r--   0        0        0    40811 2020-02-02 00:00:00.000000 qualyspy-0.2.3/qualyspy/assets/host_list_detection.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.2.3/qualyspy/certview/__init__.py
+-rw-r--r--   0        0        0    15230 2020-02-02 00:00:00.000000 qualyspy-0.2.3/qualyspy/certview/certificate.py
+-rw-r--r--   0        0        0     5068 2020-02-02 00:00:00.000000 qualyspy-0.2.3/qualyspy/certview/sql/certview_init.sql
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.2.3/qualyspy/scan_configuration/__init__.py
+-rw-r--r--   0        0        0    24210 2020-02-02 00:00:00.000000 qualyspy-0.2.3/qualyspy/scan_configuration/knowledgebase.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 qualyspy-0.2.3/requirements/deploy.txt
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 qualyspy-0.2.3/requirements/dev.txt
+-rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 qualyspy-0.2.3/.gitignore
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 qualyspy-0.2.3/LICENSE
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 qualyspy-0.2.3/README.md
+-rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 qualyspy-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 qualyspy-0.2.3/PKG-INFO
```

### Comparing `qualyspy-0.2.2/.vscode/launch.json` & `qualyspy-0.2.3/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.2/debug/dtd.txt` & `qualyspy-0.2.3/debug/dtd.txt`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.2/debug/output.txt` & `qualyspy-0.2.3/debug/output.txt`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.2/debug/parse_dtd.py` & `qualyspy-0.2.3/debug/parse_dtd.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.2/debug/quickscan.py` & `qualyspy-0.2.3/debug/quickscan.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.2/debug/remove_cookies.py` & `qualyspy-0.2.3/debug/remove_cookies.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.2/debug/test.py` & `qualyspy-0.2.3/debug/test.py`

 * *Files 18% similar despite different names*

```diff
@@ -26,8 +26,18 @@
 
     #api.reset(echo = True)
     #test = api.load(echo=True)
 
     stmt = sa.Select(cert.Certificate_ORM).where(cert.Certificate_ORM.self_signed == False)
     test = api.query(stmt, echo = True)
 
+    # stmt = sa.select(
+    # cert.Host_Instance_ORM.fqdn,
+    # cert.Host_Instance_ORM.protocol,
+    # cert.Host_Instance_ORM.port,
+    # )
+
+    # hosts = api.query(stmt, echo=True)
+    # for host in hosts:
+    #    print(host)
+
     print("test")
```

### Comparing `qualyspy-0.2.2/docs/Makefile` & `qualyspy-0.2.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.2/docs/make.bat` & `qualyspy-0.2.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.2/docs/source/conf.py` & `qualyspy-0.2.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.2/qualyspy/qualysapi.py` & `qualyspy-0.2.3/qualyspy/qualysapi.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.2/qualyspy/qutils.py` & `qualyspy-0.2.3/qualyspy/qutils.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.2/qualyspy/urls.json` & `qualyspy-0.2.3/qualyspy/urls.json`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.2/qualyspy/asset_mgmt_tagging/asset.py` & `qualyspy-0.2.3/qualyspy/asset_mgmt_tagging/asset.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.2/qualyspy/asset_mgmt_tagging/tags.py` & `qualyspy-0.2.3/qualyspy/asset_mgmt_tagging/tags.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.2/qualyspy/assets/host_list.py` & `qualyspy-0.2.3/qualyspy/assets/host_list.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.2/qualyspy/assets/host_list_detection.py` & `qualyspy-0.2.3/qualyspy/assets/host_list_detection.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.2/qualyspy/certview/certificate.py` & `qualyspy-0.2.3/qualyspy/certview/certificate.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import datetime
 import importlib.resources
 import ipaddress
-from typing import Any
+from typing import Any, TypeVar
 
 import psycopg2.extensions
 import pydantic as pd
 import pydantic.networks
 import pydantic.utils
 import sqlalchemy as sa
 import sqlalchemy.dialects.postgresql as sa_pg
@@ -35,75 +35,63 @@
 )
 
 
 ####################################################################################################
 # Subject_Alternative_Name
 
 
-class Subject_Alternative_Name_DNS_ORM(Base):
-    __tablename__ = "subject_alternative_name_dns"
-
-    name: orm.Mapped[str] = orm.mapped_column(primary_key=True)
-    sans_id: orm.Mapped[int] = orm.mapped_column(
-        sa.ForeignKey("subject_alternative_name.id")
-    )
-    sans: orm.Mapped["Subject_Alternative_Names_ORM"] = orm.relationship(
-        back_populates="dns_names", uselist=False
-    )
-
-
-class Subject_Alternative_Name_IP_ORM(Base):
-    __tablename__ = "subject_alternative_name_ip"
+class Subject_Alternative_Names(pd.BaseModel):
+    dns_names = list[str]
+    ip_address = list[str]
 
-    ip: orm.Mapped[ipaddress.IPv4Address | ipaddress.IPv6Address] = orm.mapped_column(
-        "ip", sa_pg.INET, primary_key=True
-    )
-    sans_id: orm.Mapped[int] = orm.mapped_column(
-        sa.ForeignKey("subject_alternative_name.id")
-    )
-    sans: orm.Mapped["Subject_Alternative_Names_ORM"] = orm.relationship(
-        back_populates="ips", uselist=False
-    )
+    class Config:
+        alias_generator = qutils.to_lower_camel
+        orm_mode = True
+        allow_population_by_field_name = True
 
 
 class Subject_Alternative_Names_ORM(Base):
     __tablename__ = "subject_alternative_name"
+    pd_class = Subject_Alternative_Names
 
     id: orm.Mapped[int] = orm.mapped_column(primary_key=True)
-    dns_names: orm.Mapped[list[Subject_Alternative_Name_DNS_ORM]] = orm.relationship(
-        back_populates="sans"
-    )
-    ips: orm.Mapped[list[Subject_Alternative_Name_IP_ORM]] = orm.relationship(
-        back_populates="sans"
-    )
+    dns_names: orm.Mapped[list[str] | None] = orm.mapped_column(sa.ARRAY(sa.String))
+    ips: orm.Mapped[
+        list[ipaddress.IPv4Address | ipaddress.IPv6Address] | None
+    ] = orm.mapped_column(sa.ARRAY(sa_pg.INET))
 
     certificate_id: orm.Mapped[int] = orm.mapped_column(sa.ForeignKey("certificate.id"))
     certificate: orm.Mapped["Certificate_ORM"] = orm.relationship(
         back_populates="subject_alternative_names", uselist=False
     )
 
 
-class Subject_Alternative_Names(pd.BaseModel):
-    dns_names = list[str]
-    ip_address = list[str]
+####################################################################################################
+
+####################################################################################################
+# Subject
+
+
+class Subject(pd.BaseModel):
+    organization: str
+    locality: str
+    name: str
+    state: str
+    country: str
+    organization_unit: list[str] | None
 
     class Config:
         alias_generator = qutils.to_lower_camel
         orm_mode = True
         allow_population_by_field_name = True
 
 
-####################################################################################################
-
-####################################################################################################
-# Subject
-
-
 class Subject_ORM(Base):
     __tablename__ = "subject"
+    pd_class = Subject
 
     organization: orm.Mapped[str]
     locality: orm.Mapped[str]
     name: orm.Mapped[str] = orm.mapped_column(primary_key=True)
     state: orm.Mapped[str]
     country: orm.Mapped[str]
 
@@ -113,36 +101,38 @@
         sa.ForeignKey("certificate.id"), primary_key=True
     )
     certificate: orm.Mapped["Certificate_ORM"] = orm.relationship(
         back_populates="subject", uselist=False
     )
 
 
-class Subject(pd.BaseModel):
+####################################################################################################
+
+####################################################################################################
+# Issuer
+
+
+class Issuer(pd.BaseModel):
     organization: str
-    locality: str
+    organization_unit: list[str]
     name: str
-    state: str
     country: str
-    organization_unit: list[str] | None
+    state: str
+    certhash: str
+    locality: str
 
     class Config:
         alias_generator = qutils.to_lower_camel
         orm_mode = True
         allow_population_by_field_name = True
 
 
-####################################################################################################
-
-####################################################################################################
-# Issuer
-
-
 class Issuer_ORM(Base):
     __tablename__ = "issuer"
+    pd_class = Issuer
 
     organization: orm.Mapped[str]
     organization_unit: orm.Mapped[list[str]] = orm.mapped_column(sa.ARRAY(sa.String))
     name: orm.Mapped[str]
     country: orm.Mapped[str]
     state: orm.Mapped[str]
     certhash: orm.Mapped[str] = orm.mapped_column(primary_key=True)
@@ -151,46 +141,46 @@
     issuer_of: orm.Mapped[list["Certificate_ORM"]] = orm.relationship(
         back_populates="issuer"
     )
 
 
 class RootIssuer_ORM(Base):
     __tablename__ = "rootissuer"
+    pd_class = Issuer
 
     organization: orm.Mapped[str]
     organization_unit: orm.Mapped[list[str]] = orm.mapped_column(sa.ARRAY(sa.String))
     name: orm.Mapped[str]
     country: orm.Mapped[str]
     state: orm.Mapped[str]
     certhash: orm.Mapped[str] = orm.mapped_column(primary_key=True)
     locality: orm.Mapped[str]
 
     rootissuer_of: orm.Mapped[list["Certificate_ORM"]] = orm.relationship(
         back_populates="rootissuer"
     )
 
 
-class Issuer(pd.BaseModel):
-    organization: str
-    organization_unit: list[str]
-    name: str
-    country: str
-    state: str
-    certhash: str
-    locality: str
+####################################################################################################
+# Host_Instance
+
+
+class Host_Instance(pd.BaseModel):
+    id: int
+    port: int
+    fqdn: str
+    protocol: str
+    service: str | None
+    grade: str
 
     class Config:
-        alias_generator = qutils.to_lower_camel
         orm_mode = True
         allow_population_by_field_name = True
 
 
-####################################################################################################
-# Host_Instance
-
 asset_host_instance_association_table = sa.Table(
     "asset_host_instance",
     Base.metadata,
     sa.Column("asset_id", sa.INTEGER, sa.ForeignKey("asset.id"), primary_key=True),
     sa.Column(
         "host_instance_id",
         sa.INTEGER,
@@ -198,75 +188,80 @@
         primary_key=True,
     ),
 )
 
 
 class Host_Instance_ORM(Base):
     __tablename__ = "host_instance"
+    pd_class = Host_Instance
 
     id: orm.Mapped[int] = orm.mapped_column(primary_key=True)
     port: orm.Mapped[int]
     fqdn: orm.Mapped[str]
     protocol: orm.Mapped[str]
     service: orm.Mapped[str | None]
     grade: orm.Mapped[str]
 
     asset: orm.Mapped[list["Asset_ORM"]] = orm.relationship(
         secondary=asset_host_instance_association_table
     )
 
 
-class Host_Instance(pd.BaseModel):
-    id: int
-    port: int
-    fqdn: str
-    protocol: str
-    service: str | None
-    grade: str
+####################################################################################################
+# Asset_Interface
+
+
+class Asset_Interface(pd.BaseModel):
+    hostname: str | None
+    address: pd.IPvAnyAddress
 
     class Config:
         orm_mode = True
         allow_population_by_field_name = True
 
 
-####################################################################################################
-# Asset_Interface
-
-
 class Asset_Interface_ORM(Base):
     __tablename__ = "asset_interface"
+    pd_class = Asset_Interface
 
     hostname: orm.Mapped[str | None]
     address: orm.Mapped[
         ipaddress.IPv4Address | ipaddress.IPv6Address
     ] = orm.mapped_column("address", sa_pg.INET, primary_key=True)
 
     asset_id: orm.Mapped[int] = orm.mapped_column(sa.ForeignKey("asset.id"))
     asset: orm.Mapped["Asset_ORM"] = orm.relationship(
         back_populates="asset_interfaces", uselist=False
     )
 
 
-class Asset_Interface(pd.BaseModel):
-    hostname: str | None
-    address: pd.IPvAnyAddress
-
-    class Config:
-        orm_mode = True
-        allow_population_by_field_name = True
-
-
 ####################################################################################################
 
 ####################################################################################################
 # Asset
 
 
+class Asset(pd.BaseModel):
+    id: int
+    uuid: str
+    netbios_name: str
+    name: str
+    operating_system: str | None
+    host_instances: list[Host_Instance]
+    asset_interfaces: list[Asset_Interface] | None
+
+    class Config:
+        alias_generator = qutils.to_lower_camel
+        orm_mode = True
+        allow_population_by_field_name = True
+
+
 class Asset_ORM(Base):
     __tablename__ = "asset"
+    pd_class = Asset
 
     id: orm.Mapped[int] = orm.mapped_column(primary_key=True)
     uuid: orm.Mapped[str]
     netbios_name: orm.Mapped[str]
     name: orm.Mapped[str]
     operating_system: orm.Mapped[str | None]
     host_instances: orm.Mapped[list[Host_Instance_ORM]] = orm.relationship(
@@ -278,62 +273,58 @@
 
     certificate_id: orm.Mapped[int] = orm.mapped_column(sa.ForeignKey("certificate.id"))
     certificate: orm.Mapped["Certificate_ORM"] = orm.relationship(
         back_populates="assets", uselist=False
     )
 
 
-class Asset(pd.BaseModel):
+####################################################################################################
+# Certificate
+
+
+class Certificate(pd.BaseModel):
     id: int
-    uuid: str
-    netbios_name: str
-    name: str
-    operating_system: str | None
-    host_instances: list[Host_Instance]
-    asset_interfaces: list[Asset_Interface] | None
+    certhash: str
+    key_size: int
+    serial_number: str
+    valid_to_date: datetime.datetime
+    valid_to: int
+    valid_from_date: datetime.datetime
+    valid_from: int
+    signature_algorithm: str
+    extended_validation: bool
+    created_date: datetime.datetime
+    dn: str | None
+    subject: Subject
+    update_date: datetime.datetime
+    last_found: int
+    imported: bool
+    self_signed: bool
+    issuer: Issuer | None
+    rootissuer: Issuer | None
+    issuer_category: str
+    instance_count: int
+    asset_count: int
+    assets: list[Asset]
+    key_usage: list[str]
+    raw_data: str
+    enhanced_key_usage: list[str] | None
+    subject_key_identifier: str | None
+    auth_key_identifier: str | None
+    subject_alternative_names: Subject_Alternative_Names | None
 
     class Config:
         alias_generator = qutils.to_lower_camel
         orm_mode = True
         allow_population_by_field_name = True
 
 
-####################################################################################################
-# Certificate
-
-certificate_key_usage_association_table = sa.Table(
-    "certificate_key_usage",
-    Base.metadata,
-    sa.Column(
-        "certificate_id", sa.Integer, sa.ForeignKey("certificate.id"), primary_key=True
-    ),
-    sa.Column("usage", sa.Text, sa.ForeignKey("key_usage.usage"), primary_key=True),
-)
-
-certificate_enhanced_key_usage_association_table = sa.Table(
-    "certificate_enhanced_key_usage",
-    Base.metadata,
-    sa.Column(
-        "certificate_id", sa.Integer, sa.ForeignKey("certificate.id"), primary_key=True
-    ),
-    sa.Column("usage", sa.Text, sa.ForeignKey("key_usage.usage"), primary_key=True),
-)
-
-
-class Key_Usage_ORM(Base):
-    __tablename__ = "key_usage"
-
-    usage: orm.Mapped[str] = orm.mapped_column(primary_key=True)
-    certificates: orm.Mapped[list["Certificate_ORM"]] = orm.relationship(
-        secondary=certificate_key_usage_association_table
-    )
-
-
 class Certificate_ORM(Base):
     __tablename__ = "certificate"
+    pd_class = Certificate
 
     id: orm.Mapped[int] = orm.mapped_column(primary_key=True)
     certhash: orm.Mapped[str]
     key_size: orm.Mapped[int]
     serial_number: orm.Mapped[str]
     valid_to_date: orm.Mapped[datetime.datetime]
     valid_to: orm.Mapped[int] = orm.mapped_column(sa.BigInteger)
@@ -362,77 +353,26 @@
     rootissuer: orm.Mapped[RootIssuer_ORM | None] = orm.relationship(
         back_populates="rootissuer_of", uselist=False
     )
     issuer_category: orm.Mapped[str]
     instance_count: orm.Mapped[int]
     asset_count: orm.Mapped[int]
     assets: orm.Mapped[list[Asset_ORM]] = orm.relationship(back_populates="certificate")
-    key_usage: orm.Mapped[list[Key_Usage_ORM]] = orm.relationship(
-        secondary=certificate_key_usage_association_table
-    )
+    key_usage: orm.Mapped[list[str]] = orm.mapped_column(sa.ARRAY(sa.String))
     raw_data: orm.Mapped[str]
-    enhanced_key_usage: orm.Mapped[list[Key_Usage_ORM] | None] = orm.relationship(
-        secondary=certificate_enhanced_key_usage_association_table
+    enhanced_key_usage: orm.Mapped[list[str] | None] = orm.mapped_column(
+        sa.ARRAY(sa.String)
     )
     subject_key_identifier: orm.Mapped[str | None]
     auth_key_identifier: orm.Mapped[str | None]
     subject_alternative_names: orm.Mapped[
         Subject_Alternative_Names_ORM | None
     ] = orm.relationship(back_populates="certificate", uselist=False)
 
 
-class Certiticate_Getter(pydantic.utils.GetterDict):
-    def get(self, key: str, default: Any = None) -> Any:
-        if key == "key_usage":
-            return [ku.usage for ku in self._obj.key_usage]
-        elif key == "enhanced_key_usage":
-            if self._obj.enhanced_key_usage is None:
-                return None
-            return [ku.usage for ku in self._obj.enhanced_key_usage]
-        return super().get(key, default)
-
-
-class Certificate(pd.BaseModel):
-    id: int
-    certhash: str
-    key_size: int
-    serial_number: str
-    valid_to_date: datetime.datetime
-    valid_to: int
-    valid_from_date: datetime.datetime
-    valid_from: int
-    signature_algorithm: str
-    extended_validation: bool
-    created_date: datetime.datetime
-    dn: str | None
-    subject: Subject
-    update_date: datetime.datetime
-    last_found: int
-    imported: bool
-    self_signed: bool
-    issuer: Issuer | None
-    rootissuer: Issuer | None
-    issuer_category: str
-    instance_count: int
-    asset_count: int
-    assets: list[Asset]
-    key_usage: list[str]
-    raw_data: str
-    enhanced_key_usage: list[str] | None
-    subject_key_identifier: str | None
-    auth_key_identifier: str | None
-    subject_alternative_names: Subject_Alternative_Names | None
-
-    class Config:
-        alias_generator = qutils.to_lower_camel
-        orm_mode = True
-        allow_population_by_field_name = True
-        getter_dict = Certiticate_Getter
-
-
 ####################################################################################################
 
 ####################################################################################################
 # Function input
 
 
 class Field_Value_Operator(pd.BaseModel):
@@ -455,14 +395,16 @@
     class Config:
         alias_generator = qutils.to_lower_camel
         allow_population_by_field_name = True
 
 
 ####################################################################################################
 
+_C = TypeVar("_C")
+
 
 class List_Certificates_V2:
     def __init__(self, conn: qualysapi.Connection) -> None:
         self.conn = conn
 
     def __call_once(
         self, params: List_CertView_Certificates_V2_Input
@@ -530,25 +472,28 @@
                     )
                     obj = session.merge(obj)
                     session.add(obj)
                     session.commit()
 
             params.page_number += 1
 
-    def query(self, stmt: Any, *, echo: bool = False) -> list[Certificate]:
+    def query(self, stmt: Any, *, echo: bool = False) -> list[_C]:
         engine = sa.create_engine(qutils.E_URL, echo=echo)
 
-        certificates: list[Certificate] = []
+        output: list[_C] = []
         with orm.Session(engine) as session:
-            results = session.scalars(stmt)
+            results = session.execute(stmt)
             for result in results.all():
-                c = Certificate.from_orm(result)
-                certificates.append(c)
+                if issubclass(type(result), Base):
+                    i = type(result).pd_class.from_orm(result.scalars())  # type: ignore
+                else:
+                    i = result
+                output.append(i)
 
-        return certificates
+        return output
 
     def reset(self, *, echo: bool = False) -> None:
         engine = sa.create_engine(qutils.E_URL, echo=echo)
 
         stmt = sa.text("DROP SCHEMA IF EXISTS certificate CASCADE")
         with orm.Session(engine) as session:
             session.execute(stmt)
```

### Comparing `qualyspy-0.2.2/qualyspy/certview/sql/certview_init.sql` & `qualyspy-0.2.3/qualyspy/certview/sql/certview_init.sql`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.2/qualyspy/scan_configuration/knowledgebase.py` & `qualyspy-0.2.3/qualyspy/scan_configuration/knowledgebase.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.2/.gitignore` & `qualyspy-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.2/LICENSE` & `qualyspy-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.2/pyproject.toml` & `qualyspy-0.2.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "QualysPy"
-version = "0.2.2"
+version = "0.2.3"
 authors = [
   { name="Jordan Barnartt", email="jbarnart@uwaterloo.ca" },
 ]
 description = "A Python wrapper for the Qualys API."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -37,8 +37,9 @@
 [tool.pyright]
 reportUnboundVariable = false
 reportUnknownArgumentType = false
 reportPrivateUsage = false
 reportUnknownVariableType = false
 reportUnknownMemberType = false
 reportGeneralTypeIssues = false
-reportUntypedBaseClass = false
+reportUntypedBaseClass = false
+reportInvalidTypeVarUse = false
```

### Comparing `qualyspy-0.2.2/PKG-INFO` & `qualyspy-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QualysPy
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Python wrapper for the Qualys API.
 Project-URL: Homepage, https://github.com/JordanBarnartt/qualyspy
 Project-URL: Bug Tracker, https://github.com/JordanBarnartt/qualyspy/issues
 Author-email: Jordan Barnartt <jbarnart@uwaterloo.ca>
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Information Technology
```

