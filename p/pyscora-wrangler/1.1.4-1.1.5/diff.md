# Comparing `tmp/pyscora_wrangler-1.1.4.tar.gz` & `tmp/pyscora_wrangler-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyscora_wrangler-1.1.4.tar", max compression
+gzip compressed data, was "pyscora_wrangler-1.1.5.tar", max compression
```

## Comparing `pyscora_wrangler-1.1.4.tar` & `pyscora_wrangler-1.1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1049 2023-04-10 18:51:21.191627 pyscora_wrangler-1.1.4/LICENSE
--rw-r--r--   0        0        0      659 2023-04-10 18:51:21.191627 pyscora_wrangler-1.1.4/README.md
--rw-r--r--   0        0        0     1116 2023-04-10 18:51:21.191627 pyscora_wrangler-1.1.4/pyproject.toml
--rw-r--r--   0        0        0       51 2023-04-10 18:51:21.191627 pyscora_wrangler-1.1.4/pyscora_wrangler/__init__.py
--rw-r--r--   0        0        0    14258 2023-04-10 18:51:21.191627 pyscora_wrangler-1.1.4/pyscora_wrangler/aws/README.md
--rw-r--r--   0        0        0       85 2023-04-10 18:51:21.191627 pyscora_wrangler-1.1.4/pyscora_wrangler/aws/__init__.py
--rw-r--r--   0        0        0     7114 2023-04-10 18:51:21.191627 pyscora_wrangler-1.1.4/pyscora_wrangler/aws/athena/__init__.py
--rw-r--r--   0        0        0    15796 2023-04-10 18:51:21.191627 pyscora_wrangler-1.1.4/pyscora_wrangler/aws/cognito/__init__.py
--rw-r--r--   0        0        0       88 2023-04-10 18:51:21.191627 pyscora_wrangler-1.1.4/pyscora_wrangler/aws/constants.py
--rw-r--r--   0        0        0     6697 2023-04-10 18:51:21.191627 pyscora_wrangler-1.1.4/pyscora_wrangler/aws/dynamodb/__init__.py
--rw-r--r--   0        0        0      671 2023-04-10 18:51:21.191627 pyscora_wrangler-1.1.4/pyscora_wrangler/aws/utils.py
--rw-r--r--   0        0        0      165 2023-04-10 18:51:21.191627 pyscora_wrangler-1.1.4/pyscora_wrangler/constants.py
--rw-r--r--   0        0        0      513 2023-04-10 18:51:21.191627 pyscora_wrangler-1.1.4/pyscora_wrangler/ldap/README.md
--rw-r--r--   0        0        0       60 2023-04-10 18:51:21.191627 pyscora_wrangler-1.1.4/pyscora_wrangler/ldap/__init__.py
--rw-r--r--   0        0        0     7761 2023-04-10 18:51:21.191627 pyscora_wrangler-1.1.4/pyscora_wrangler/ldap/service/__init__.py
--rw-r--r--   0        0        0       22 2023-04-10 18:51:21.191627 pyscora_wrangler-1.1.4/pyscora_wrangler/ldap/utils.py
--rw-r--r--   0        0        0     2692 2023-04-10 18:51:21.191627 pyscora_wrangler-1.1.4/pyscora_wrangler/utils.py
--rw-r--r--   0        0        0     1998 1970-01-01 00:00:00.000000 pyscora_wrangler-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1049 2023-04-11 01:17:18.607700 pyscora_wrangler-1.1.5/LICENSE
+-rw-r--r--   0        0        0      659 2023-04-11 01:17:18.607700 pyscora_wrangler-1.1.5/README.md
+-rw-r--r--   0        0        0     1116 2023-04-11 01:17:18.607700 pyscora_wrangler-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0       51 2023-04-11 01:17:18.607700 pyscora_wrangler-1.1.5/pyscora_wrangler/__init__.py
+-rw-r--r--   0        0        0    14258 2023-04-11 01:17:18.607700 pyscora_wrangler-1.1.5/pyscora_wrangler/aws/README.md
+-rw-r--r--   0        0        0       85 2023-04-11 01:17:18.607700 pyscora_wrangler-1.1.5/pyscora_wrangler/aws/__init__.py
+-rw-r--r--   0        0        0     7114 2023-04-11 01:17:18.607700 pyscora_wrangler-1.1.5/pyscora_wrangler/aws/athena/__init__.py
+-rw-r--r--   0        0        0    15796 2023-04-11 01:17:18.607700 pyscora_wrangler-1.1.5/pyscora_wrangler/aws/cognito/__init__.py
+-rw-r--r--   0        0        0       88 2023-04-11 01:17:18.607700 pyscora_wrangler-1.1.5/pyscora_wrangler/aws/constants.py
+-rw-r--r--   0        0        0     6697 2023-04-11 01:17:18.607700 pyscora_wrangler-1.1.5/pyscora_wrangler/aws/dynamodb/__init__.py
+-rw-r--r--   0        0        0      671 2023-04-11 01:17:18.607700 pyscora_wrangler-1.1.5/pyscora_wrangler/aws/utils.py
+-rw-r--r--   0        0        0      165 2023-04-11 01:17:18.607700 pyscora_wrangler-1.1.5/pyscora_wrangler/constants.py
+-rw-r--r--   0        0        0      495 2023-04-11 01:17:18.607700 pyscora_wrangler-1.1.5/pyscora_wrangler/ldap/README.md
+-rw-r--r--   0        0        0       60 2023-04-11 01:17:18.607700 pyscora_wrangler-1.1.5/pyscora_wrangler/ldap/__init__.py
+-rw-r--r--   0        0        0     7585 2023-04-11 01:17:18.611699 pyscora_wrangler-1.1.5/pyscora_wrangler/ldap/service/__init__.py
+-rw-r--r--   0        0        0       22 2023-04-11 01:17:18.611699 pyscora_wrangler-1.1.5/pyscora_wrangler/ldap/utils.py
+-rw-r--r--   0        0        0     2692 2023-04-11 01:17:18.611699 pyscora_wrangler-1.1.5/pyscora_wrangler/utils.py
+-rw-r--r--   0        0        0     1998 1970-01-01 00:00:00.000000 pyscora_wrangler-1.1.5/PKG-INFO
```

### Comparing `pyscora_wrangler-1.1.4/LICENSE` & `pyscora_wrangler-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyscora_wrangler-1.1.4/README.md` & `pyscora_wrangler-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `pyscora_wrangler-1.1.4/pyproject.toml` & `pyscora_wrangler-1.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyscora-wrangler"
-version = "1.1.4"
+version = "1.1.5"
 description = "Python lib for DE"
 authors = ["Oncase <suporte@oncase.com.br>"]
 maintainers = ["Guilherme Morone <guilherme.morone@oncase.com.br>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/oncase/pyscora-wrangler"
 repository = "https://github.com/oncase/pyscora-wrangler"
```

### Comparing `pyscora_wrangler-1.1.4/pyscora_wrangler/aws/README.md` & `pyscora_wrangler-1.1.5/pyscora_wrangler/aws/README.md`

 * *Files identical despite different names*

### Comparing `pyscora_wrangler-1.1.4/pyscora_wrangler/aws/athena/__init__.py` & `pyscora_wrangler-1.1.5/pyscora_wrangler/aws/athena/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,18 +172,18 @@
             database=database,
             s3_staging_dir=f'{base_path}/athena-results',
             athena_work_group=table_meta.get('athena_work_group'),
             verbose=True,
             boto3_session=session,
         )
 
-        return {"table": table}
+        return {'table': table}
 
     async def _process_async(tables: Type[tables]):
-        logger.info("[athena_refresh_process_async] {0:<30} {1:>20}".format("File", "Completed at"))
+        logger.info('[athena_refresh_process_async] {0:<30} {1:>20}'.format('File', 'Completed at'))
         with ThreadPoolExecutor(max_workers=15) as executor:
             loop = asyncio.get_event_loop()
             tasks = [loop.run_in_executor(executor, _process, *table_meta) for table_meta in tables]
 
             for finished_task in await asyncio.gather(*tasks):
                 logger.info(
                     f"[athena_refresh_process_async] Table {finished_task.get('table')} refreshed with success."
```

### Comparing `pyscora_wrangler-1.1.4/pyscora_wrangler/aws/cognito/__init__.py` & `pyscora_wrangler-1.1.5/pyscora_wrangler/aws/cognito/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -321,15 +321,15 @@
     try:
         client.admin_set_user_password(
             UserPoolId=userpool_id, Username=username, Password=password, Permanent=permanent
         )
     except client.exceptions.UserNotFoundException:
         logger.warning(f'[set_user_password] User {username} does not exists. Skipping...')
     except Exception as err:
-        logger.error(f"[set_user_password] {err}")
+        logger.error(f'[set_user_password] {err}')
 
 
 def authenticate_user(
     userpool_id: str,
     client_id: str,
     username: str,
     password: str,
```

### Comparing `pyscora_wrangler-1.1.4/pyscora_wrangler/aws/dynamodb/__init__.py` & `pyscora_wrangler-1.1.5/pyscora_wrangler/aws/dynamodb/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,15 @@
     session = get_boto3_session(boto3_session)
     resource = session.resource(DYNAMODB_SERVICE_NAME)
 
     data = None
 
     dynamo_table = resource.Table(table_name)
     response = dynamo_table.query(KeyConditionExpression=Key(key).eq(value))
-    response = response.get("Items", [])
+    response = response.get('Items', [])
 
     if len(response) > 0:
         data = get_data_decoded(response[0]) if decode_data else response[0]
 
     if fields != None and data:
         data = {field: data.get(field) for field in fields}
```

### Comparing `pyscora_wrangler-1.1.4/pyscora_wrangler/aws/utils.py` & `pyscora_wrangler-1.1.5/pyscora_wrangler/aws/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,13 +12,13 @@
 def get_user_secret_hash(client_id: str, app_client_secret: str, username: str) -> str | None:
     msg = username + client_id
 
     if not client_id or not app_client_secret or not username:
         return None
 
     try:
-        dig = hmac.new(app_client_secret.encode("utf-8"), msg=msg.encode("utf-8"), digestmod=hashlib.sha256).digest()
+        dig = hmac.new(app_client_secret.encode('utf-8'), msg=msg.encode('utf-8'), digestmod=hashlib.sha256).digest()
         d2 = base64.b64encode(dig).decode()
 
         return d2
     except:
         return None
```

### Comparing `pyscora_wrangler-1.1.4/pyscora_wrangler/ldap/service/__init__.py` & `pyscora_wrangler-1.1.5/pyscora_wrangler/ldap/service/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -118,39 +118,40 @@
             if not self.__ldap_username or not self.__ldap_password:
                 logger_msg = 'Username argument cannot be null or empty.' if not self.__ldap_username else ''
                 logger_msg += 'Password argument cannot be null or empty.' if not self.__ldap_password else ''
                 logger.error(f'[auth] {logger_msg}')
 
                 raise ValueError('Invalid credentials.')
 
+            root_dn = self.ldap_config.get('root_dn')
             port = int(self.ldap_config.get('port', 389))
             server_alias = self.ldap_config.get('server_alias', [])
 
             server = Server(
                 self.ldap_config.get('server', ''),
                 get_info=ALL,
                 port=port,
                 allowed_referral_hosts=[(sa, True) for sa in server_alias]
                 if server_alias and len(server_alias)
                 else None,
             )
 
             self.__ldap_connection = Connection(
                 server,
-                user=self.__ldap_username,
+                user=f'CN={self.__ldap_username},{root_dn}',
                 password=self.__ldap_password,
                 authentication='SIMPLE',
                 raise_exceptions=False,
             )
 
             if self.__ldap_connection.bind():
                 self.__user_is_authenticated = True
-                logger.info("[auth] Successful bind to ldap server.")
+                logger.info('[auth] Successful bind to ldap server.')
             else:
-                logger.error(f"[auth] Cannot bind to ldap server: {self.__ldap_connection.last_error}.")
+                logger.error(f'[auth] Cannot bind to ldap server: {self.__ldap_connection.last_error}.')
         except Exception as err:
             logger.error(f'[auth] {err}')
 
         return self.is_user_authenticated()
 
     def logout(self) -> None:
         """Unbind the connect to the ldap server"""
@@ -158,65 +159,64 @@
         if self.__ldap_connection:
             try:
                 self.__ldap_connection.unbind()
             except Exception as err:
                 logger.error(f'[logout] {err}')
 
     def get_ldap_groups(self) -> List[str]:
-        """Returns A list containing the ldap groups."""
+        """Returns A list containing the ldap groups"""
 
         return self.__ldap_groups
 
     def get_ldap_users(self) -> List[str]:
-        """Returns A list containing the ldap users."""
+        """Returns A list containing the ldap users"""
 
         return self.__ldap_users
 
-    def set_ldap_users_and_groups(self) -> Tuple[List[str], List[str]] | None:
-        """Set the ldap groups and users.
+    def __set_ldap_arrays(self, search_filter: str) -> List[str]:
+        root_dn = self.ldap_config.get('root_dn', '')
+
+        self.__ldap_connection.search(
+            search_base=root_dn, search_filter=search_filter, search_scope=SUBTREE, size_limit=0
+        )
+
+        arr = []
+        for entry in self.__ldap_connection.entries:
+            arr.append(entry.entry_dn)
+
+        return arr
+
+    def set_ldap_users(self) -> List[str] | None:
+        """Set the ldap users
 
         Returns:
-            Tuple[List[str], List[str]] | None: Returns None if an error occurs in the process. Otherwise, returns a Tuple the lists of the ldap groups and the ldap users.
+            List[str] | None: Returns None if an error occurs in the process. Otherwise, returns the list of the ldap users.
         """
 
         if not self.is_user_authenticated():
-            logger.warning('[set_ldap_users_and_groups] User is not authenticated. Skipping...')
+            logger.warning('[set_ldap_users] User is not authenticated. Skipping...')
             return None
 
-        groups = []
-        root_dn = self.ldap_config.get('root_dn', '')
-
-        try:
-            self.__ldap_connection.search(
-                search_base=root_dn,
-                search_filter="(objectclass=*)",
-                search_scope=SUBTREE,
-                attributes=["member"],
-                size_limit=0,
-            )
+        users_search_filter = '(objectClass=person)'
+        users_dn = self.__set_ldap_arrays(search_filter=users_search_filter)
 
-            response = json.loads(self.__ldap_connection.response_to_json())
+        self.__ldap_users = [user.split('=')[1].split(',')[0] for user in users_dn]
 
-            if type(response.get("entries")) == list and len(response.get("entries")) > 0:
-                for entry in response.get("entries"):
-                    for member in entry.member.values:
-                        self.__ldap_connection.search(
-                            search_base=root_dn,
-                            search_filter=f"(distinguishedName={member})",
-                            attributes=["sAMAccountName"],
-                        )
+        return self.get_ldap_users()
 
-                        user = self.__ldap_connection.entries[0].sAMAccountName.values
+    def set_ldap_groups(self) -> List[str] | None:
+        """Set the ldap groups
 
-                        self.__ldap_users.append(user)
+        Returns:
+            List[str] | None: Returns None if an error occurs in the process. Otherwise, returns the list of the ldap groups.
+        """
 
-                cn_groups = response.get("entries")[0].get("attributes").get("member")
+        if not self.is_user_authenticated():
+            logger.warning('[set_ldap_users] User is not authenticated. Skipping...')
+            return None
 
-                for cn_group in cn_groups:
-                    groups.append(cn_group.split(",")[0].replace("CN=", ""))
+        groups_search_filter = '(objectClass=groupOfNames)'
+        groups_dn = self.__set_ldap_arrays(search_filter=groups_search_filter)
 
-                self.__ldap_groups = groups
-        except Exception as err:
-            logger.error(f'[set_ldap_users_and_groups] {err}')
-            return None
+        self.__ldap_groups = [group.split('=')[1].split(',')[0] for group in groups_dn]
 
-        return self.get_ldap_users(), self.get_ldap_groups()
+        return self.get_ldap_groups()
```

### Comparing `pyscora_wrangler-1.1.4/pyscora_wrangler/utils.py` & `pyscora_wrangler-1.1.5/pyscora_wrangler/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,23 +77,23 @@
     @wraps(func)
     def _time_it(*args, **kwargs):
         start = int(round(time() * 1000))
         try:
             return func(*args, **kwargs)
         finally:
             end_ = int(round(time() * 1000)) - start
-            print(f"{func.__name__} execution time: {end_ if end_ > 0 else 0} ms")
+            print(f'{func.__name__} execution time: {end_ if end_ > 0 else 0} ms')
 
     return _time_it
 
 
 def get_metadata_from_yaml(file_path: str) -> Any:
     data = []
 
-    with open(file_path, encoding="utf-8") as file:
+    with open(file_path, encoding='utf-8') as file:
         data = yaml.load(file, Loader=yaml.FullLoader)
 
     return data
 
 
 def get_copy_metadata(file_path: str) -> Any:
-    return get_metadata_from_yaml(file_path).get("copy")
+    return get_metadata_from_yaml(file_path).get('copy')
```

### Comparing `pyscora_wrangler-1.1.4/PKG-INFO` & `pyscora_wrangler-1.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyscora-wrangler
-Version: 1.1.4
+Version: 1.1.5
 Summary: Python lib for DE
 Home-page: https://github.com/oncase/pyscora-wrangler
 License: MIT
 Keywords: wrapper,scora,python,data_engineering
 Author: Oncase
 Author-email: suporte@oncase.com.br
 Maintainer: Guilherme Morone
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyscora-wrangler Version: 1.1.4 Summary: Python lib
+Metadata-Version: 2.1 Name: pyscora-wrangler Version: 1.1.5 Summary: Python lib
 for DE Home-page: https://github.com/oncase/pyscora-wrangler License: MIT
 Keywords: wrapper,scora,python,data_engineering Author: Oncase Author-email:
 suporte@oncase.com.br Maintainer: Guilherme Morone Maintainer-email:
 guilherme.morone@oncase.com.br Requires-Python: >=3.8,<4.0 Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
```

