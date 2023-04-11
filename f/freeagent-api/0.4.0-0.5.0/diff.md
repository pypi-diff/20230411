# Comparing `tmp/freeagent_api-0.4.0.tar.gz` & `tmp/freeagent_api-0.5.0.tar.gz`

## Comparing `freeagent_api-0.4.0.tar` & `freeagent_api-0.5.0.tar`

### file list

```diff
@@ -1,22 +1,27 @@
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 freeagent_api-0.4.0/.editorconfig
--rwxr-xr-x   0        0        0       83 2020-02-02 00:00:00.000000 freeagent_api-0.4.0/.git-commit-msg-hook
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 freeagent_api-0.4.0/.markdownlint.yaml
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 freeagent_api-0.4.0/.pydocstylerc
--rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 freeagent_api-0.4.0/.pylintrc
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 freeagent_api-0.4.0/.sv4git.yml
--rw-r--r--   0        0        0    10443 2020-02-02 00:00:00.000000 freeagent_api-0.4.0/src/freeagent_api/__init__.py
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 freeagent_api-0.4.0/src/freeagent_api/accounting_category.py
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 freeagent_api-0.4.0/src/freeagent_api/bank_account.py
--rw-r--r--   0        0        0     5125 2020-02-02 00:00:00.000000 freeagent_api-0.4.0/src/freeagent_api/base_object.py
--rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 freeagent_api-0.4.0/src/freeagent_api/company.py
--rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 freeagent_api-0.4.0/src/freeagent_api/contact.py
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 freeagent_api-0.4.0/src/freeagent_api/invoice.py
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 freeagent_api-0.4.0/src/freeagent_api/invoice_item.py
--rw-r--r--   0        0        0     5056 2020-02-02 00:00:00.000000 freeagent_api-0.4.0/src/freeagent_api/oauth.py
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 freeagent_api-0.4.0/src/freeagent_api/project.py
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 freeagent_api-0.4.0/src/freeagent_api/user.py
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 freeagent_api-0.4.0/.gitignore
--rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 freeagent_api-0.4.0/LICENSE
--rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 freeagent_api-0.4.0/README.md
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 freeagent_api-0.4.0/pyproject.toml
--rw-r--r--   0        0        0    42957 2020-02-02 00:00:00.000000 freeagent_api-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 freeagent_api-0.5.0/.editorconfig
+-rwxr-xr-x   0        0        0       83 2020-02-02 00:00:00.000000 freeagent_api-0.5.0/.git-commit-msg-hook
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 freeagent_api-0.5.0/.markdownlint.yaml
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 freeagent_api-0.5.0/.pydocstylerc
+-rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 freeagent_api-0.5.0/.pylintrc
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 freeagent_api-0.5.0/.sv4git.yml
+-rw-r--r--   0        0        0    56144 2020-02-02 00:00:00.000000 freeagent_api-0.5.0/noun-accounting.png
+-rw-r--r--   0        0        0    14464 2020-02-02 00:00:00.000000 freeagent_api-0.5.0/noun-accounting.svg
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 freeagent_api-0.5.0/src/freeagent_api/Pipfile
+-rw-r--r--   0        0        0    13170 2020-02-02 00:00:00.000000 freeagent_api-0.5.0/src/freeagent_api/__init__.py
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 freeagent_api-0.5.0/src/freeagent_api/accounting_category.py
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 freeagent_api-0.5.0/src/freeagent_api/bank_account.py
+-rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 freeagent_api-0.5.0/src/freeagent_api/bank_transaction.py
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 freeagent_api-0.5.0/src/freeagent_api/bank_transaction_explanation.py
+-rw-r--r--   0        0        0     5244 2020-02-02 00:00:00.000000 freeagent_api-0.5.0/src/freeagent_api/base_object.py
+-rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 freeagent_api-0.5.0/src/freeagent_api/company.py
+-rw-r--r--   0        0        0     2723 2020-02-02 00:00:00.000000 freeagent_api-0.5.0/src/freeagent_api/contact.py
+-rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 freeagent_api-0.5.0/src/freeagent_api/invoice.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 freeagent_api-0.5.0/src/freeagent_api/invoice_item.py
+-rw-r--r--   0        0        0     5056 2020-02-02 00:00:00.000000 freeagent_api-0.5.0/src/freeagent_api/oauth.py
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 freeagent_api-0.5.0/src/freeagent_api/project.py
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 freeagent_api-0.5.0/src/freeagent_api/user.py
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 freeagent_api-0.5.0/.gitignore
+-rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 freeagent_api-0.5.0/LICENSE
+-rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 freeagent_api-0.5.0/README.md
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 freeagent_api-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0    43272 2020-02-02 00:00:00.000000 freeagent_api-0.5.0/PKG-INFO
```

### Comparing `freeagent_api-0.4.0/.pylintrc` & `freeagent_api-0.5.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `freeagent_api-0.4.0/.sv4git.yml` & `freeagent_api-0.5.0/.sv4git.yml`

 * *Files identical despite different names*

### Comparing `freeagent_api-0.4.0/src/freeagent_api/__init__.py` & `freeagent_api-0.5.0/src/freeagent_api/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from time import sleep
 import logging
 import requests
 
 from freeagent_api.oauth import OAuthHandler
 
 from freeagent_api.bank_account import BankAccount
+from freeagent_api.bank_transaction import BankTransaction
 from freeagent_api.company import Company
 from freeagent_api.contact import Contact
 from freeagent_api.invoice import Invoice
 from freeagent_api.invoice_item import InvoiceItem
 from freeagent_api.project import Project
 from freeagent_api.user import User
 from freeagent_api.accounting_category import AccountingCategory
@@ -52,15 +53,16 @@
         self.use_sandbox = use_sandbox
 
         if use_sandbox:
             self.api_base = SANDBOX_API_BASE
         else:
             self.api_base = PRODUCTION_API_BASE
 
-        self.logger = logging.getLogger(__name__)
+        logging.basicConfig(level=logging.INFO)
+
         self.oauth = OAuthHandler(client_id, client_secret, use_sandbox)
 
 
     def do_auth(self, only_listen_on_localhost: bool = True):
         """Get an authentication token for the users's account.
 
         Just a pass-through function to the OAuthHandler instance.
@@ -94,29 +96,29 @@
 
         Returns:
             dict: Request response as decoded JSON object
         """
         if not endpoint.startswith('/'):
             endpoint = '/' + endpoint
 
-        #print("GET", self.api_base + endpoint, "with params", params)
+        logging.debug("GET %s with params %s", self.api_base + endpoint, params)
 
         self.oauth.update_tokens()
         response = None
         retries = MAX_RETRIES
         while retries > 0:
             response = requests.get(
                 self.api_base + endpoint,
                 headers = { "Authorization": self.oauth.authorisation_header },
                 timeout = 10,
                 params = params,
             )
 
             if 'retry-after' in response.headers:
-                self.logger.info(
+                logging.info(
                     "Hit API rate limit, waiting %s seconds before retrying",
                     response.headers['Retry-After'],
                 )
                 retries -= 1
                 if retries > 0:
                     sleep(int(response.headers['retry-after']))
                 else:
@@ -247,28 +249,96 @@
         """
         data = self._get(f"/invoices/{invoice_id}")
 
         invoice = Invoice(data.get('invoice'))
         return invoice
 
 
+    def get_bank_accounts(self, account_type: str = 'all') -> list[BankAccount]:
+        """Get a list of bank accounts.
+
+        Args:
+            account_type (str, optional): One of 'all', 'standard_bank', 'credit_card', 'paypal'.
+                Defaults to 'standard_bank'.
+
+        Returns:
+            List[BankAccount]: List of matching BankAccount objects.
+        """
+        if account_type not in ['all', 'standard_bank', 'credit_card', 'paypal']:
+            raise ValueError("Bank account type not valid")
+
+        if account_type == 'all':
+            data = self._get('/bank_accounts')
+        else:
+            data = self._get('/bank_accounts', {'view': account_type + "_accounts"})
+
+        bank_accounts = []
+        for bank_account_data in data.get('bank_accounts'):
+            bank_accounts.append(BankAccount(bank_account_data))
+        return bank_accounts
+
+
     def get_bank_account(self, account_id: int) -> BankAccount:
         """Get bank account data.
 
         Args:
             account_id (int): ID of the account. Typically obtained from the
                 bank_account field of a freeagent.Invoice object or similar.
 
         Returns:
             BankAccount: Bank account data object.
         """
         data = self._get(f'/bank_accounts/{int(account_id)}')
         return BankAccount(data.get('bank_account'))
 
 
+    def get_bank_transactions(self,
+        account_id: int,
+        from_date: datetime.date = None,
+        to_date: datetime.date = None,
+        updated_since: datetime.date = None,
+        status: str = 'all',
+    ) -> list[BankTransaction]:
+        """Get a list of bank transactions for the specified account.
+
+        Args:
+            account_id (int): ID of the bank account.
+            from_date (datetime.date, optional): Earliest date for transaction filter. Defaults to
+                None.
+            to_date (datetime.date, optional): Latest date for transaction filter. Defaults to None.
+            updated_since (datetime.date, optional): Only show transactions updated since this date.
+                Defaults to None.
+            status (str, optional): Filter transactions by status. Must be one of 'all',
+                'unexplained', 'explained', 'manual', 'imported', 'marked_for_review'. Defaults to
+                'all'.
+
+        Returns:
+            list[BankTransaction]: List of transaction objects.
+        """
+        if status not in ['all', 'unexplained', 'explained', 'manual', 'imported', 'marked_for_review']:
+            raise ValueError("Status not valid")
+
+        params = {
+            'bank_account': account_id,
+            'view': status,
+        }
+        if from_date:
+            params['from_date'] = from_date.isoformat()
+        if to_date:
+            params['to_date'] = to_date.isoformat()
+        if updated_since:
+            params['updated_since'] = updated_since.isoformat()
+
+        data = self._get('/bank_transactions', params)
+        transactions = []
+        for transaction_data in data['bank_transactions']:
+            transactions.append(BankTransaction(transaction_data))
+        return transactions
+
+
     def get_project(self, project_id: int) -> Project:
         """Get project data.
 
         Args:
             project_id (int): ID of the project. Typically obtained from the
                 project field of a freeagent.Invoice object or similar.
```

### Comparing `freeagent_api-0.4.0/src/freeagent_api/accounting_category.py` & `freeagent_api-0.5.0/src/freeagent_api/accounting_category.py`

 * *Files identical despite different names*

### Comparing `freeagent_api-0.4.0/src/freeagent_api/bank_account.py` & `freeagent_api-0.5.0/src/freeagent_api/bank_account.py`

 * *Files identical despite different names*

### Comparing `freeagent_api-0.4.0/src/freeagent_api/base_object.py` & `freeagent_api-0.5.0/src/freeagent_api/base_object.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,26 +33,27 @@
     return value
 
 
 class BaseObject:
     """Base object for other API objects."""
 
     # Provide empty lists in case derived classes don't define these
-    PARSED_API_FIELDS = []
 
     def __init__(self, data=None):
         """Initialise the object."""
+        self.parsed_api_fields = []
         self._data = {}
+
         if data is not None:
             # Parse types out of the field names
             for field in self.API_FIELDS:
                 try:
                     field, field_type = field.split(':')
                     value = data.get(field)
-                    self.PARSED_API_FIELDS.append(field)
+                    self.parsed_api_fields.append(field)
 
                     if field_type == 'integer':
                         self._data[field] = int(value or 0)
                     elif field_type == 'decimal':
                         self._data[field] = Decimal(value or 0)
                     elif field_type == 'boolean':
                         self._data[field] = bool(value)
@@ -64,15 +65,15 @@
                         matches = re.search(r"(\d+)$", value or "")
                         self._data[field] = matches.group(0) if matches else None
 
                     else:
                         raise TypeError(f"Unknown type mapping '{field_type}' for {field}")
 
                 except ValueError:
-                    self.PARSED_API_FIELDS.append(field)
+                    self.parsed_api_fields.append(field)
                     value = data.get(field)
                     self._data[field] = value
 
                     if field == 'url' and value is not None:
                         matches = re.search(r"(\d+)$", value or "")
                         self._data['id'] = matches.group(0) if matches else None
 
@@ -83,15 +84,18 @@
         This overrides the basic object attribute getter to return data from the
         stored API data if the requested attribute name is an API field, and
         then look for a normal attribute of the object.
 
         Fields containing ID values are overridden to extract just the numerical
         ID instead of the full URL.
         """
-        if name in self.PARSED_API_FIELDS or name == 'id':
+        if name == 'parsed_api_fields':
+            return self.__dict__.get(name)
+
+        if name in self.parsed_api_fields or name == 'id':
             return self._data.get(name)
 
         if f"_{name}" in self.__dict__:
             return self.__dict__[f"_{name}"]
 
         raise AttributeError(f"{self.__class__.__name__} object has no attribute '{name}'")
 
@@ -103,15 +107,18 @@
         object data as if it were stored in normal attributes. Attributes not
         listed in the API fields will actually be set as normal object
         attributes.
 
         Should probably check the type being set (int/bool/etc), but currently
         doesn't.
         """
-        if name in self.PARSED_API_FIELDS or name == 'id':
+        if name == 'parsed_api_fields':
+            self.__dict__[name] = value
+
+        if name in self.parsed_api_fields or name == 'id':
             self._data[name] = value
         else:
             self.__dict__[name] = value
 
 
     def as_dict(self) -> dict:
         """Get a dictionary based representation of the object.
@@ -120,19 +127,18 @@
 
         Returns:
             dict: Contents of object.
         """
         data = {}
 
         # Get API data
-        for key in self.PARSED_API_FIELDS:
-            if key in self._data:
-                data[key] = _var_to_serialisable(self._data[key])
+        for key in self.parsed_api_fields:
+            data[key] = _var_to_serialisable(self._data.get(key))
 
         # Other properties
         for key,value in self.__dict__.items():
-            if not key.startswith("_") and value is not None:
+            if not key.startswith("_"):
                 data[key] = _var_to_serialisable(value)
 
         data['id'] = self.id
 
         return data
```

### Comparing `freeagent_api-0.4.0/src/freeagent_api/company.py` & `freeagent_api-0.5.0/src/freeagent_api/company.py`

 * *Files identical despite different names*

### Comparing `freeagent_api-0.4.0/src/freeagent_api/contact.py` & `freeagent_api-0.5.0/src/freeagent_api/contact.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,16 @@
         any methods that can be called without requiring parameters.
 
         Returns:
             dict: Contents of object.
         """
         obj = super().as_dict()
         obj['address'] = self.address()
+        obj['fullname'] = self.fullname
+        obj['name'] = self.name
         return obj
 
 
     @property
     def fullname(self) -> str:
         """Get the full name of the contact.
```

### Comparing `freeagent_api-0.4.0/src/freeagent_api/invoice.py` & `freeagent_api-0.5.0/src/freeagent_api/invoice.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,10 +64,11 @@
 
     def __init__(self, data = None):
         """Initialise the Invoice object.
 
         Converts the invoice items from dict to InvoiceItem object.
         """
         super().__init__(data)
-        self._data['invoice_items'] = []
-        for item_data in data['invoice_items']:
-            self._data['invoice_items'].append(InvoiceItem(item_data))
+        if data:
+            self._data['invoice_items'] = []
+            for item_data in data['invoice_items']:
+                self._data['invoice_items'].append(InvoiceItem(item_data))
```

### Comparing `freeagent_api-0.4.0/src/freeagent_api/invoice_item.py` & `freeagent_api-0.5.0/src/freeagent_api/invoice_item.py`

 * *Files identical despite different names*

### Comparing `freeagent_api-0.4.0/src/freeagent_api/oauth.py` & `freeagent_api-0.5.0/src/freeagent_api/oauth.py`

 * *Files identical despite different names*

### Comparing `freeagent_api-0.4.0/src/freeagent_api/project.py` & `freeagent_api-0.5.0/src/freeagent_api/project.py`

 * *Files identical despite different names*

### Comparing `freeagent_api-0.4.0/src/freeagent_api/user.py` & `freeagent_api-0.5.0/src/freeagent_api/user.py`

 * *Files identical despite different names*

### Comparing `freeagent_api-0.4.0/LICENSE` & `freeagent_api-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `freeagent_api-0.4.0/README.md` & `freeagent_api-0.5.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -78,7 +78,13 @@
     contact's full name or company name, depending on which is defined and the
     contact_name_on_invoices setting for the contact.
 
 ### freeagent_api.User
 
 -   `fullname` returns the first and last name of the authorised user as a
     single string.
+
+---
+
+## Acknowledgements
+
+Repository ison is adapted from ['accounting'](https://thenounproject.com/icon/accounting-1848937/) by [Vectors Market](https://thenounproject.com/vectorsmarket/) from [Noun Project](https://thenounproject.com/browse/icons/term/accounting) (CC BY 3.0), with the currency symbol replaced.
```

### Comparing `freeagent_api-0.4.0/pyproject.toml` & `freeagent_api-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `freeagent_api-0.4.0/PKG-INFO` & `freeagent_api-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freeagent_api
-Version: 0.4.0
+Version: 0.5.0
 Summary: Interface to the FreeAgent accounting software API
 Project-URL: Bug Tracker, https://gitlab.com/inutt/python-freeagent-api/-/issues
 Project-URL: Repository, https://gitlab.com/inutt/python-freeagent-api
 Author-email: Richard Davis <inutt.dev@gmail.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
@@ -756,7 +756,13 @@
     contact's full name or company name, depending on which is defined and the
     contact_name_on_invoices setting for the contact.
 
 ### freeagent_api.User
 
 -   `fullname` returns the first and last name of the authorised user as a
     single string.
+
+---
+
+## Acknowledgements
+
+Repository ison is adapted from ['accounting'](https://thenounproject.com/icon/accounting-1848937/) by [Vectors Market](https://thenounproject.com/vectorsmarket/) from [Noun Project](https://thenounproject.com/browse/icons/term/accounting) (CC BY 3.0), with the currency symbol replaced.
```

