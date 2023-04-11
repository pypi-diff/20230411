# Comparing `tmp/pydantic_factur_x-0.1.6.tar.gz` & `tmp/pydantic_factur_x-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_factur_x-0.1.6.tar", max compression
+gzip compressed data, was "pydantic_factur_x-0.1.7.tar", max compression
```

## Comparing `pydantic_factur_x-0.1.6.tar` & `pydantic_factur_x-0.1.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1569 2023-03-11 14:45:16.994968 pydantic_factur_x-0.1.6/README.md
--rw-r--r--   0        0        0        0 2023-03-10 19:07:13.275171 pydantic_factur_x-0.1.6/pydantic_factur_x/__init__.py
--rw-r--r--   0        0        0     3263 2023-04-06 08:42:17.588924 pydantic_factur_x-0.1.6/pydantic_factur_x/factur_x/__init__.py
--rw-r--r--   0        0        0     2275 2023-03-29 16:41:36.327089 pydantic_factur_x-0.1.6/pydantic_factur_x/factur_x/_nsmaps.py
--rw-r--r--   0        0        0     2586 2023-03-30 09:36:17.303512 pydantic_factur_x-0.1.6/pydantic_factur_x/factur_x/address.py
--rw-r--r--   0        0        0      260 2023-03-30 12:21:57.198680 pydantic_factur_x-0.1.6/pydantic_factur_x/factur_x/code_lists/__init__.py
--rw-r--r--   0        0        0     1770 2023-03-16 09:53:16.427279 pydantic_factur_x-0.1.6/pydantic_factur_x/factur_x/code_lists/untdid_1001.py
--rw-r--r--   0        0        0      418 2023-03-16 14:07:23.374186 pydantic_factur_x-0.1.6/pydantic_factur_x/factur_x/code_lists/untdid_1229.py
--rw-r--r--   0        0        0      305 2023-03-16 10:06:27.017530 pydantic_factur_x-0.1.6/pydantic_factur_x/factur_x/code_lists/untdid_1373.py
--rw-r--r--   0        0        0      248 2023-03-16 10:35:39.940578 pydantic_factur_x-0.1.6/pydantic_factur_x/factur_x/code_lists/untdid_2379.py
--rw-r--r--   0        0        0     6378 2023-03-16 13:14:18.733404 pydantic_factur_x-0.1.6/pydantic_factur_x/factur_x/code_lists/untdid_4451.py
--rw-r--r--   0        0        0     3202 2023-03-30 12:20:22.530590 pydantic_factur_x-0.1.6/pydantic_factur_x/factur_x/code_lists/untdid_4461.py
--rw-r--r--   0        0        0     4492 2023-03-31 08:34:01.604788 pydantic_factur_x-0.1.6/pydantic_factur_x/factur_x/common.py
--rw-r--r--   0        0        0     2254 2023-03-29 16:25:04.834377 pydantic_factur_x-0.1.6/pydantic_factur_x/factur_x/contact.py
--rw-r--r--   0        0        0     3304 2023-03-29 16:25:17.623365 pydantic_factur_x-0.1.6/pydantic_factur_x/factur_x/document_context.py
--rw-r--r--   0        0        0      620 2023-03-29 16:25:25.445510 pydantic_factur_x-0.1.6/pydantic_factur_x/factur_x/document_reference.py
--rw-r--r--   0        0        0     6458 2023-03-30 09:39:52.351758 pydantic_factur_x-0.1.6/pydantic_factur_x/factur_x/exchanged_document.py
--rw-r--r--   0        0        0     3744 2023-03-29 16:43:31.173714 pydantic_factur_x-0.1.6/pydantic_factur_x/factur_x/root.py
--rw-r--r--   0        0        0    56776 2023-04-06 08:32:31.901032 pydantic_factur_x-0.1.6/pydantic_factur_x/factur_x/supply_chain_trade_transaction.py
--rw-r--r--   0        0        0     5276 2023-03-29 16:27:52.619351 pydantic_factur_x-0.1.6/pydantic_factur_x/factur_x/trade_party.py
--rw-r--r--   0        0        0       34 2023-03-10 19:08:25.401902 pydantic_factur_x-0.1.6/pydantic_factur_x/order-x/__init__.py
--rw-r--r--   0        0        0     1316 2023-04-04 14:46:29.384089 pydantic_factur_x-0.1.6/pydantic_factur_x/tests/fixtures/invoice_1.json
--rw-r--r--   0        0        0      684 2023-04-04 14:54:37.569796 pydantic_factur_x-0.1.6/pydantic_factur_x/tests/test_facturx_from_json.py
--rw-r--r--   0        0        0     8379 2023-04-06 07:00:13.246492 pydantic_factur_x-0.1.6/pydantic_factur_x/tests/test_full_orderx_manual.py
--rw-r--r--   0        0        0      569 2023-04-06 09:24:00.466946 pydantic_factur_x-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     2077 1970-01-01 00:00:00.000000 pydantic_factur_x-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1569 2023-03-11 14:45:16.994968 pydantic_factur_x-0.1.7/README.md
+-rw-r--r--   0        0        0        0 2023-03-10 19:07:13.275171 pydantic_factur_x-0.1.7/pydantic_factur_x/__init__.py
+-rw-r--r--   0        0        0     3373 2023-04-11 14:25:42.198251 pydantic_factur_x-0.1.7/pydantic_factur_x/factur_x/__init__.py
+-rw-r--r--   0        0        0     2275 2023-03-29 16:41:36.327089 pydantic_factur_x-0.1.7/pydantic_factur_x/factur_x/_nsmaps.py
+-rw-r--r--   0        0        0     2586 2023-03-30 09:36:17.303512 pydantic_factur_x-0.1.7/pydantic_factur_x/factur_x/address.py
+-rw-r--r--   0        0        0      260 2023-03-30 12:21:57.198680 pydantic_factur_x-0.1.7/pydantic_factur_x/factur_x/code_lists/__init__.py
+-rw-r--r--   0        0        0     1770 2023-03-16 09:53:16.427279 pydantic_factur_x-0.1.7/pydantic_factur_x/factur_x/code_lists/untdid_1001.py
+-rw-r--r--   0        0        0      418 2023-03-16 14:07:23.374186 pydantic_factur_x-0.1.7/pydantic_factur_x/factur_x/code_lists/untdid_1229.py
+-rw-r--r--   0        0        0      305 2023-03-16 10:06:27.017530 pydantic_factur_x-0.1.7/pydantic_factur_x/factur_x/code_lists/untdid_1373.py
+-rw-r--r--   0        0        0      248 2023-03-16 10:35:39.940578 pydantic_factur_x-0.1.7/pydantic_factur_x/factur_x/code_lists/untdid_2379.py
+-rw-r--r--   0        0        0     6378 2023-03-16 13:14:18.733404 pydantic_factur_x-0.1.7/pydantic_factur_x/factur_x/code_lists/untdid_4451.py
+-rw-r--r--   0        0        0     3202 2023-03-30 12:20:22.530590 pydantic_factur_x-0.1.7/pydantic_factur_x/factur_x/code_lists/untdid_4461.py
+-rw-r--r--   0        0        0     4492 2023-03-31 08:34:01.604788 pydantic_factur_x-0.1.7/pydantic_factur_x/factur_x/common.py
+-rw-r--r--   0        0        0     2254 2023-03-29 16:25:04.834377 pydantic_factur_x-0.1.7/pydantic_factur_x/factur_x/contact.py
+-rw-r--r--   0        0        0     3304 2023-03-29 16:25:17.623365 pydantic_factur_x-0.1.7/pydantic_factur_x/factur_x/document_context.py
+-rw-r--r--   0        0        0      620 2023-03-29 16:25:25.445510 pydantic_factur_x-0.1.7/pydantic_factur_x/factur_x/document_reference.py
+-rw-r--r--   0        0        0     6458 2023-03-30 09:39:52.351758 pydantic_factur_x-0.1.7/pydantic_factur_x/factur_x/exchanged_document.py
+-rw-r--r--   0        0        0     3744 2023-03-29 16:43:31.173714 pydantic_factur_x-0.1.7/pydantic_factur_x/factur_x/root.py
+-rw-r--r--   0        0        0    59280 2023-04-11 14:25:18.220106 pydantic_factur_x-0.1.7/pydantic_factur_x/factur_x/supply_chain_trade_transaction.py
+-rw-r--r--   0        0        0     5276 2023-03-29 16:27:52.619351 pydantic_factur_x-0.1.7/pydantic_factur_x/factur_x/trade_party.py
+-rw-r--r--   0        0        0       34 2023-03-10 19:08:25.401902 pydantic_factur_x-0.1.7/pydantic_factur_x/order-x/__init__.py
+-rw-r--r--   0        0        0     1316 2023-04-04 14:46:29.384089 pydantic_factur_x-0.1.7/pydantic_factur_x/tests/fixtures/invoice_1.json
+-rw-r--r--   0        0        0      684 2023-04-04 14:54:37.569796 pydantic_factur_x-0.1.7/pydantic_factur_x/tests/test_facturx_from_json.py
+-rw-r--r--   0        0        0     8660 2023-04-11 14:26:24.678121 pydantic_factur_x-0.1.7/pydantic_factur_x/tests/test_full_orderx_manual.py
+-rw-r--r--   0        0        0      569 2023-04-11 14:26:45.505392 pydantic_factur_x-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     2077 1970-01-01 00:00:00.000000 pydantic_factur_x-0.1.7/PKG-INFO
```

### Comparing `pydantic_factur_x-0.1.6/README.md` & `pydantic_factur_x-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `pydantic_factur_x-0.1.6/pydantic_factur_x/factur_x/__init__.py` & `pydantic_factur_x-0.1.7/pydantic_factur_x/factur_x/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,14 +43,16 @@
     ApplicableTradeTax,
     SpecifiedLineTradeSettlement,
     SpecifiedLineTradeDelivery,
     SpecifiedTradeSettlementLineMonetarySummation,
     IncludedSupplyChainTradeLineItem,
     ApplicableHeaderTradeAgreement,
     ApplicableHeaderTradeDelivery,
+    DueDateDateTime,
+    SpecifiedTradePaymentTerms,
     SpecifiedTradeSettlementHeaderMonetarySummation,
     ReceivableSpecifiedTradeAccountingAccount,
     ApplicableHeaderTradeSettlement,
     SupplyChainTradeTransaction,
 )
 from .root import (
     SCRDMCCBDACIOMessageStructure,
@@ -105,14 +107,16 @@
     "ApplicableTradeTax",
     "SpecifiedLineTradeSettlement",
     "SpecifiedLineTradeDelivery",
     "SpecifiedTradeSettlementLineMonetarySummation",
     "IncludedSupplyChainTradeLineItem",
     "ApplicableHeaderTradeAgreement",
     "ApplicableHeaderTradeDelivery",
+    "DueDateDateTime",
+    "SpecifiedTradePaymentTerms",
     "SpecifiedTradeSettlementHeaderMonetarySummation",
     "ReceivableSpecifiedTradeAccountingAccount",
     "ApplicableHeaderTradeSettlement",
     "SupplyChainTradeTransaction",
     # --- root
     "SCRDMCCBDACIOMessageStructure",
     "CrossIndustryInvoice",
```

### Comparing `pydantic_factur_x-0.1.6/pydantic_factur_x/factur_x/_nsmaps.py` & `pydantic_factur_x-0.1.7/pydantic_factur_x/factur_x/_nsmaps.py`

 * *Files identical despite different names*

### Comparing `pydantic_factur_x-0.1.6/pydantic_factur_x/factur_x/address.py` & `pydantic_factur_x-0.1.7/pydantic_factur_x/factur_x/address.py`

 * *Files identical despite different names*

### Comparing `pydantic_factur_x-0.1.6/pydantic_factur_x/factur_x/code_lists/untdid_1001.py` & `pydantic_factur_x-0.1.7/pydantic_factur_x/factur_x/code_lists/untdid_1001.py`

 * *Files identical despite different names*

### Comparing `pydantic_factur_x-0.1.6/pydantic_factur_x/factur_x/code_lists/untdid_4451.py` & `pydantic_factur_x-0.1.7/pydantic_factur_x/factur_x/code_lists/untdid_4451.py`

 * *Files identical despite different names*

### Comparing `pydantic_factur_x-0.1.6/pydantic_factur_x/factur_x/code_lists/untdid_4461.py` & `pydantic_factur_x-0.1.7/pydantic_factur_x/factur_x/code_lists/untdid_4461.py`

 * *Files identical despite different names*

### Comparing `pydantic_factur_x-0.1.6/pydantic_factur_x/factur_x/common.py` & `pydantic_factur_x-0.1.7/pydantic_factur_x/factur_x/common.py`

 * *Files identical despite different names*

### Comparing `pydantic_factur_x-0.1.6/pydantic_factur_x/factur_x/contact.py` & `pydantic_factur_x-0.1.7/pydantic_factur_x/factur_x/contact.py`

 * *Files identical despite different names*

### Comparing `pydantic_factur_x-0.1.6/pydantic_factur_x/factur_x/document_context.py` & `pydantic_factur_x-0.1.7/pydantic_factur_x/factur_x/document_context.py`

 * *Files identical despite different names*

### Comparing `pydantic_factur_x-0.1.6/pydantic_factur_x/factur_x/document_reference.py` & `pydantic_factur_x-0.1.7/pydantic_factur_x/factur_x/document_reference.py`

 * *Files identical despite different names*

### Comparing `pydantic_factur_x-0.1.6/pydantic_factur_x/factur_x/exchanged_document.py` & `pydantic_factur_x-0.1.7/pydantic_factur_x/factur_x/exchanged_document.py`

 * *Files identical despite different names*

### Comparing `pydantic_factur_x-0.1.6/pydantic_factur_x/factur_x/root.py` & `pydantic_factur_x-0.1.7/pydantic_factur_x/factur_x/root.py`

 * *Files identical despite different names*

### Comparing `pydantic_factur_x-0.1.6/pydantic_factur_x/factur_x/supply_chain_trade_transaction.py` & `pydantic_factur_x-0.1.7/pydantic_factur_x/factur_x/supply_chain_trade_transaction.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from enum import Enum
 from typing import Optional, List
 from pydantic_xml import BaseXmlModel, attr, element
 
 from ._nsmaps import RSM, UDT, QTD, RAM, XSI
 from .code_lists import UntDid1229, UntDid4461
 from .common import (
+    DateTimeString,
     DateString,
     BoolIndicator,
     IncludedNote,
     GlobalID,
     ValueMeasure,
     Quantity,
     Amount,
@@ -1447,14 +1448,86 @@
         tag="AppliedTradeTax",
         ns="ram",
         # nsmap=RAM,
         profiles={"factur-x": "extended", "order-x": "extended"},
     )
 
 
+class DueDateDateTime(
+    BaseXmlModel,
+    tag="DueDateDateTime",
+    ns_attrs=True,
+    ns="ram",
+    nsmap=RAM,
+):
+    """rsm:DueDateDateTime
+
+    Profiles:
+        - Factur-X: basic_wl
+        - Order-X: comfort
+    """
+
+    date_time_string: DateTimeString = element(
+        tag="DateTimeString",
+        ns="udt",
+        # nsmap=RAM,
+        profiles={"factur-x": "basic_wl", "order-x": None},
+        description="""The date when the payment is due.""",
+        usage="""The payment due date reflects the due date of the net payment.
+        For partial payments it states the first net due date.
+        The corresponding description of more complex payment terms
+        can be stated in BT-20 Payment terms.""",
+    )
+
+
+class SpecifiedTradePaymentTerms(
+    BaseXmlModel,
+    tag="SpecifiedTradePaymentTerms",
+    ns_attrs=True,
+    ns="ram",
+    nsmap=RAM,
+):
+    """rsm:SpecifiedTradePaymentTerms
+
+    Profiles:
+        - Factur-X: basic_wl
+        - Order-X: comfort
+    """
+
+    description: str = element(
+        tag="Description",
+        ns="ram",
+        # nsmap=RAM,
+        profiles={"factur-x": "basic_wl", "order-x": "comfort"},
+        description="""A textual description of the payment terms that apply to the amount
+        due for payment (Including description of possible penalties).""",
+        usage="""This element may contain multiple lines and multiple terms.""",
+    )
+    due_date: Optional[DueDateDateTime] = element(
+        tag="DueDateDateTime",
+        ns="ram",
+        # nsmap=RAM,
+        profiles={"factur-x": "basic_wl", "order-x": None},
+        description="""The date when the payment is due.""",
+        usage="""The payment due date reflects the due date of the net payment.
+        For partial payments it states the first net due date.
+        The corresponding description of more complex payment terms
+        can be stated in BT-20 Payment terms.""",
+    )
+    direct_debit_mandate_id: Optional[str] = element(
+        tag="DirectDebitMandateID",
+        ns="ram",
+        # nsmap=RAM,
+        profiles={"factur-x": "basic_wl", "order-x": None},
+        description="""Unique identifier assigned by the Payee
+        for referencing the direct debit mandate.""",
+        usage="""Used in order to pre-notify the Buyer of a SEPA direct debit.""",
+    )
+
+
 class ApplicableHeaderTradeSettlement(
     BaseXmlModel,
     tag="ApplicableHeaderTradeSettlement",
     ns_attrs=True,
     ns="ram",
     nsmap=RAM,
 ):
@@ -1542,15 +1615,20 @@
         ns="ram",
         # nsmap=RAM,
         profiles={"factur-x": "extended", "order-x": "extended"},
         description="""A logistics service charge specified for this header
         trade settlement.
         """,
     )
-    # specified_trade_payment_terms # SpecifiedTradePaymentTerms
+    specified_trade_payment_terms: Optional[SpecifiedTradePaymentTerms] = element(
+        tag="SpecifiedTradePaymentTerms",
+        ns="ram",
+        # nsmap=RAM,
+        profiles={"factur-x": "basic_wl", "order-x": "comfort"},
+    )
 
     total_amounts: SpecifiedTradeSettlementHeaderMonetarySummation = element(
         tag="SpecifiedTradeSettlementHeaderMonetarySummation",
         ns="ram",
         # nsmap=RAM,
         profiles={"factur-x": "minimum", "order-x": "basic"},
         description="""A group of business terms providing the monetary totals
```

### Comparing `pydantic_factur_x-0.1.6/pydantic_factur_x/factur_x/trade_party.py` & `pydantic_factur_x-0.1.7/pydantic_factur_x/factur_x/trade_party.py`

 * *Files identical despite different names*

### Comparing `pydantic_factur_x-0.1.6/pydantic_factur_x/tests/fixtures/invoice_1.json` & `pydantic_factur_x-0.1.7/pydantic_factur_x/tests/fixtures/invoice_1.json`

 * *Files identical despite different names*

### Comparing `pydantic_factur_x-0.1.6/pydantic_factur_x/tests/test_facturx_from_json.py` & `pydantic_factur_x-0.1.7/pydantic_factur_x/tests/test_facturx_from_json.py`

 * *Files identical despite different names*

### Comparing `pydantic_factur_x-0.1.6/pydantic_factur_x/tests/test_full_orderx_manual.py` & `pydantic_factur_x-0.1.7/pydantic_factur_x/tests/test_full_orderx_manual.py`

 * *Files 3% similar despite different names*

```diff
@@ -173,14 +173,20 @@
                     calculated_amount=5.22,  # total vat for this vat
                     type_code="VAT",
                     basis_amount=6.44,
                     category_code="S",
                     rate_applicable_percent="5.5",
                 ),
             ],
+            specified_trade_payment_terms=SpecifiedTradePaymentTerms(
+                description="Payment terms",
+                # due_date=DueDateDateTime(
+                #     date_time_string=DateTimeString(text="20201201", format="102"),
+                # ),
+            ),
             total_amounts=SpecifiedTradeSettlementHeaderMonetarySummation(
                 line_total_amount=42.42,
             ),
         ),
     ),
 )
```

### Comparing `pydantic_factur_x-0.1.6/pyproject.toml` & `pydantic_factur_x-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic_factur_x"
-version = "0.1.6"
+version = "0.1.7"
 description = "Python library for pydantic factur-x bindings"
 authors = ["Thomas chiroux <thomas@chiroux.org>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "pydantic_factur_x" }]
 
 [tool.poetry.dependencies]
```

### Comparing `pydantic_factur_x-0.1.6/PKG-INFO` & `pydantic_factur_x-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-factur-x
-Version: 0.1.6
+Version: 0.1.7
 Summary: Python library for pydantic factur-x bindings
 License: MIT
 Author: Thomas chiroux
 Author-email: thomas@chiroux.org
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

