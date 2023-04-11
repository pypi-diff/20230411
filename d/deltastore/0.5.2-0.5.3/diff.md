# Comparing `tmp/deltastore-0.5.2-py3-none-any.whl.zip` & `tmp/deltastore-0.5.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 14926 bytes, number of entries: 13
+Zip file size: 14944 bytes, number of entries: 13
 -rw-r--r--  2.0 unx     1313 b- defN 23-Mar-20 09:12 deltastore/__init__.py
 -rw-r--r--  2.0 unx      856 b- defN 23-Jan-12 07:25 deltastore/_yarl_patch.py
 -rw-r--r--  2.0 unx    10501 b- defN 23-Mar-20 06:50 deltastore/converters.py
--rw-r--r--  2.0 unx     2873 b- defN 23-Mar-31 07:11 deltastore/helpers.py
+-rw-r--r--  2.0 unx     2873 b- defN 23-Apr-05 23:39 deltastore/helpers.py
 -rw-r--r--  2.0 unx     2390 b- defN 23-Mar-20 09:12 deltastore/profile.py
 -rw-r--r--  2.0 unx     6151 b- defN 23-Mar-20 09:12 deltastore/protocols.py
--rw-r--r--  2.0 unx    10542 b- defN 23-Mar-31 07:01 deltastore/reader.py
+-rw-r--r--  2.0 unx    10806 b- defN 23-Apr-10 23:45 deltastore/reader.py
 -rw-r--r--  2.0 unx    15327 b- defN 23-Mar-20 09:12 deltastore/rest_client.py
--rw-r--r--  2.0 unx      626 b- defN 23-Mar-31 07:11 deltastore/version.py
--rw-r--r--  2.0 unx      308 b- defN 23-Mar-31 07:12 deltastore-0.5.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-31 07:12 deltastore-0.5.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Mar-31 07:12 deltastore-0.5.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1025 b- defN 23-Mar-31 07:12 deltastore-0.5.2.dist-info/RECORD
-13 files, 52015 bytes uncompressed, 13232 bytes compressed:  74.6%
+-rw-r--r--  2.0 unx      626 b- defN 23-Apr-10 23:45 deltastore/version.py
+-rw-r--r--  2.0 unx      308 b- defN 23-Apr-10 23:59 deltastore-0.5.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-10 23:59 deltastore-0.5.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Apr-10 23:59 deltastore-0.5.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1025 b- defN 23-Apr-10 23:59 deltastore-0.5.3.dist-info/RECORD
+13 files, 52279 bytes uncompressed, 13250 bytes compressed:  74.7%
```

## zipnote {}

```diff
@@ -21,20 +21,20 @@
 
 Filename: deltastore/rest_client.py
 Comment: 
 
 Filename: deltastore/version.py
 Comment: 
 
-Filename: deltastore-0.5.2.dist-info/METADATA
+Filename: deltastore-0.5.3.dist-info/METADATA
 Comment: 
 
-Filename: deltastore-0.5.2.dist-info/WHEEL
+Filename: deltastore-0.5.3.dist-info/WHEEL
 Comment: 
 
-Filename: deltastore-0.5.2.dist-info/top_level.txt
+Filename: deltastore-0.5.3.dist-info/top_level.txt
 Comment: 
 
-Filename: deltastore-0.5.2.dist-info/RECORD
+Filename: deltastore-0.5.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## deltastore/reader.py

```diff
@@ -39,22 +39,26 @@
 
     def load_pandas(
         self,
         table: Table,
         predicates: Optional[Sequence[str]] = None,
         columns: Optional[Sequence[str]] = None,
         limit: Optional[int] = None,
+        version: Optional[int] = None,
     ) -> pd.DataFrame:
         if limit is not None:
             assert (
                 isinstance(limit, int) and limit >= 0
             ), "'limit' must be a non-negative int"
 
         response = self._rest_client.list_files_in_table(
-            table, predicateHints=get_deltasharing_filters(predicates), limitHint=limit
+            table,
+            predicateHints=get_deltasharing_filters(predicates),
+            limitHint=limit,
+            version=version,
         )
 
         schema_json = json.loads(response.metadata.schema_string)
 
         if len(response.add_files) == 0 or limit == 0:
             return PandasConverter.get_empty_table(schema_json)
 
@@ -107,22 +111,26 @@
 
     def load_arrow(
         self,
         table: Table,
         predicates: Optional[Sequence[str]] = None,
         columns: Optional[Sequence[str]] = None,
         limit: Optional[int] = None,
+        version: Optional[int] = None,
     ) -> pa.Table:
         if limit is not None:
             assert (
                 isinstance(limit, int) and limit >= 0
             ), "'limit' must be a non-negative int"
 
         response = self._rest_client.list_files_in_table(
-            table, predicateHints=get_deltasharing_filters(predicates), limitHint=limit
+            table,
+            predicateHints=get_deltasharing_filters(predicates),
+            limitHint=limit,
+            version=version,
         )
 
         schema_json = json.loads(response.metadata.schema_string)
 
         if len(response.add_files) == 0 or limit == 0:
             return PyArrowConverter.get_empty_table(schema_json)
 
@@ -280,27 +288,29 @@
                             raise ValueError(
                                 "Cannot partition on binary or complex columns"
                             )
 
         return _table
 
 
-def load_as_pandas(url, predicates=None, columns=None, limit=None):
+def load_as_pandas(url, predicates=None, columns=None, limit=None, version=None):
     profile_json, share, schema, table = parse_deltasharing_profile_url(url)
     profile = DeltaSharingProfile.read_from_file(profile_json)
     return DeltaSharingReader(rest_client=DeltaSharingRestClient(profile)).load_pandas(
         table=Table(name=table, share=share, schema=schema),
         predicates=predicates,
         columns=columns,
         limit=limit,
+        version=version,
     )
 
 
-def load_as_arrow(url, predicates=None, columns=None, limit=None):
+def load_as_arrow(url, predicates=None, columns=None, limit=None, version=None):
     profile_json, share, schema, table = parse_deltasharing_profile_url(url)
     profile = DeltaSharingProfile.read_from_file(profile_json)
     return DeltaSharingReader(rest_client=DeltaSharingRestClient(profile)).load_arrow(
         table=Table(name=table, share=share, schema=schema),
         predicates=predicates,
         columns=columns,
         limit=limit,
+        version=version,
     )
```

## deltastore/version.py

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-__version__ = "0.5.2"
+__version__ = "0.5.3"
```

## Comparing `deltastore-0.5.2.dist-info/RECORD` & `deltastore-0.5.3.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 deltastore/__init__.py,sha256=ex5VX_vAosVgEaO3Bu3DZAhIcPoodhOWxCsXCnX2mGY,1313
 deltastore/_yarl_patch.py,sha256=lJhJBSt1p-_PebLBs0PdcqIwM8J1K17wN9tImW7yRO0,856
 deltastore/converters.py,sha256=pN1CcDWKwc08d7HJIV29C-qISBdDmbTS9XjrjC7koN0,10501
 deltastore/helpers.py,sha256=zbcawsKjO7QJW92f_MwK2iSkEmX3KhQOXsaqaAD4f7E,2873
 deltastore/profile.py,sha256=f0MZecysGb99klCMFLISs5cCRc6xUujMJ8GAXj6SaCo,2390
 deltastore/protocols.py,sha256=ygRdTX2TlXf9orgscFLnL6xGk0Aw5l08HvEisklsZsQ,6151
-deltastore/reader.py,sha256=naZryvPz65EvDUKD77QTUn4CUktq2_439xDuXYcjbOM,10542
+deltastore/reader.py,sha256=j-bupni-xpDDpI5kfCUQCZ9x5gagn-fRjUI0S2BQpHg,10806
 deltastore/rest_client.py,sha256=y41coNnpqZ-5_K3NuiVTk-j_LB3YMv4gnFo7Nq7LuWU,15327
-deltastore/version.py,sha256=cwflVJcSWLuefPDgizqLMFd_xJzXf_Q_XNL_irxLIfE,626
-deltastore-0.5.2.dist-info/METADATA,sha256=phW8ZxMoEbeLT1A3G79HRguPO_yNVqv6Ut2FF1ivBiM,308
-deltastore-0.5.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-deltastore-0.5.2.dist-info/top_level.txt,sha256=8tDaZb5xn-A6Gsls-PCnuVapf-VYdtFicFxnJyQI5xY,11
-deltastore-0.5.2.dist-info/RECORD,,
+deltastore/version.py,sha256=umkzcFYrheVdMnOGXdgdPYCezpzE1ksWgCbTbThl00M,626
+deltastore-0.5.3.dist-info/METADATA,sha256=5Wnh7K-ZiKu9IQlFLxRl8II8CcO4hvQOI7X9yVBwRpk,308
+deltastore-0.5.3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+deltastore-0.5.3.dist-info/top_level.txt,sha256=8tDaZb5xn-A6Gsls-PCnuVapf-VYdtFicFxnJyQI5xY,11
+deltastore-0.5.3.dist-info/RECORD,,
```

