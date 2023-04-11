# Comparing `tmp/nafigator-0.1.8-py2.py3-none-any.whl.zip` & `tmp/nafigator-0.1.9-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 24488 bytes, number of entries: 17
--rw-rw-rw-  2.0 fat      249 b- defN 21-Apr-29 10:54 nafigator/__init__.py
+Zip file size: 24497 bytes, number of entries: 17
+-rw-rw-rw-  2.0 fat      249 b- defN 21-Apr-29 12:43 nafigator/__init__.py
 -rw-rw-rw-  2.0 fat      416 b- defN 21-Apr-26 09:22 nafigator/cli.py
 -rw-rw-rw-  2.0 fat     1754 b- defN 21-Apr-28 06:55 nafigator/const.py
 -rw-rw-rw-  2.0 fat     5031 b- defN 21-Apr-28 07:00 nafigator/linguisticprocessor.py
--rw-rw-rw-  2.0 fat    36510 b- defN 21-Apr-29 09:27 nafigator/nafdocument.py
+-rw-rw-rw-  2.0 fat    36697 b- defN 21-Apr-29 12:34 nafigator/nafdocument.py
 -rw-rw-rw-  2.0 fat    15521 b- defN 21-Apr-21 09:35 nafigator/nafigator.py
 -rw-rw-rw-  2.0 fat      554 b- defN 21-Apr-29 09:27 nafigator/opennaf.py
--rw-rw-rw-  2.0 fat    17798 b- defN 21-Apr-29 09:23 nafigator/parse.py
+-rw-rw-rw-  2.0 fat    17947 b- defN 21-Apr-29 12:43 nafigator/parse.py
 -rw-rw-rw-  2.0 fat     1959 b- defN 21-Apr-28 06:58 nafigator/preprocessprocessor.py
 -rw-rw-rw-  2.0 fat     1069 b- defN 21-Apr-28 07:01 nafigator/utils.py
--rw-rw-rw-  2.0 fat      180 b- defN 21-Apr-29 10:54 nafigator-0.1.8.dist-info/AUTHORS.rst
--rw-rw-rw-  2.0 fat     1100 b- defN 21-Apr-29 10:54 nafigator-0.1.8.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     7625 b- defN 21-Apr-29 10:54 nafigator-0.1.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat      116 b- defN 21-Apr-29 10:54 nafigator-0.1.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       50 b- defN 21-Apr-29 10:54 nafigator-0.1.8.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       10 b- defN 21-Apr-29 10:54 nafigator-0.1.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1378 b- defN 21-Apr-29 10:54 nafigator-0.1.8.dist-info/RECORD
-17 files, 91320 bytes uncompressed, 22236 bytes compressed:  75.7%
+-rw-rw-rw-  2.0 fat      180 b- defN 21-Apr-29 12:43 nafigator-0.1.9.dist-info/AUTHORS.rst
+-rw-rw-rw-  2.0 fat     1100 b- defN 21-Apr-29 12:43 nafigator-0.1.9.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     7625 b- defN 21-Apr-29 12:43 nafigator-0.1.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      116 b- defN 21-Apr-29 12:43 nafigator-0.1.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       50 b- defN 21-Apr-29 12:43 nafigator-0.1.9.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       10 b- defN 21-Apr-29 12:43 nafigator-0.1.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1378 b- defN 21-Apr-29 12:43 nafigator-0.1.9.dist-info/RECORD
+17 files, 91656 bytes uncompressed, 22245 bytes compressed:  75.7%
```

## zipnote {}

```diff
@@ -24,29 +24,29 @@
 
 Filename: nafigator/preprocessprocessor.py
 Comment: 
 
 Filename: nafigator/utils.py
 Comment: 
 
-Filename: nafigator-0.1.8.dist-info/AUTHORS.rst
+Filename: nafigator-0.1.9.dist-info/AUTHORS.rst
 Comment: 
 
-Filename: nafigator-0.1.8.dist-info/LICENSE
+Filename: nafigator-0.1.9.dist-info/LICENSE
 Comment: 
 
-Filename: nafigator-0.1.8.dist-info/METADATA
+Filename: nafigator-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: nafigator-0.1.8.dist-info/WHEEL
+Filename: nafigator-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: nafigator-0.1.8.dist-info/entry_points.txt
+Filename: nafigator-0.1.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: nafigator-0.1.8.dist-info/top_level.txt
+Filename: nafigator-0.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: nafigator-0.1.8.dist-info/RECORD
+Filename: nafigator-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## nafigator/__init__.py

```diff
@@ -1,10 +1,10 @@
 """Top-level package for nafigator."""
 
-__version__ = '0.1.8'
+__version__ = '0.1.9'
 
 from .parse import *
 from .opennaf import *
 from .cli import *
 from .const import *
 from .linguisticprocessor import *
 from .preprocessprocessor import *
```

## nafigator/nafdocument.py

```diff
@@ -52,15 +52,15 @@
     return name
     # qname = etree.QName('{'+namespaces[prefix]+'}'+name, name)
     # return qname
 
 
 namespaces = {
     PREFIX_DC: "http://purl.org/dc/elements/1.1/",
-    PREFIX_NAF_BASE: "https://dnb.nl/naf-Base/elements/1.0/",
+    # PREFIX_NAF_BASE: "https://dnb.nl/naf-Base/elements/1.0/",
 }
 
 
 class NafDocument(etree._ElementTree):
 
     def generate(self, params: dict):
         self._setroot(etree.Element("NAF", nsmap=namespaces))
@@ -71,15 +71,15 @@
         self.add_public_element(params["public"])
 
     def open(self, input):
         with open(input, "r", encoding="utf-8") as f:
             self._setroot(etree.parse(f).getroot())
         return self
 
-    def write(self, output, output_type):
+    def write(self, output):
         super().write(output, encoding="utf-8", pretty_print=True, xml_declaration=True)
 
     def __getattr__(self, name):
 
         if name == "version":
             return self.getroot().get("version")
 
@@ -433,31 +433,35 @@
             # no chars between two token (for example with a dot .)
             if delta == 0:
                 trailing_chars = ""
             elif delta >= 1:
                 # 1 or more characters between tokens -> n spaces added
                 trailing_chars = " " * delta
             elif delta < 0:
-                raise AssertionError(
-                    f"please check the offsets of {prev_wf.text} and {cur_wf.text} (delta of {delta})"
+                logging.warning("please check the offsets of "+
+                                str(prev_wf.text)+" and "+
+                                str(cur_wf.text)+" (delta of "+
+                                str(delta)+")"
                 )
             tokens.append(trailing_chars + cur_wf.text)
         raw_text = "".join(tokens)
         if cdata:
             layer.text = etree.CDATA(raw_text)
         else:
             layer.text = raw_text
         # verify alignment between raw and token layer
         for wf in self.getroot().xpath("text/wf"):
             start = int(wf.get("offset"))
             end = start + int(wf.get("length"))
             token = layer.text[start:end]
-            assert (
-                wf.text == token
-            ), f'mismatch in alignment of wf element {wf.text} ({wf.get("id")}) with raw layer (expected length {wf.get("length")}'
+            if wf.text != token:
+                logging.error("mismatch in alignment of wf element "+
+                              str(wf.text)+" ("+str(wf.get("id"))+
+                              ") with raw layer (expected length "+
+                              str(wf.get("length")))
 
     def add_dependency_element(self, data: DependencyRelation, comments: bool):
         """
         <!-- DEPS ELEMENT -->
         <!ELEMENT deps (dep)+>
 
         <!-- DEP ELEMENT -->
@@ -530,17 +534,16 @@
         if comments:
             text = " ".join(data.text)
             text = self.prepare_comment_text(text)
             span.append(etree.Comment(text))
         for target in data.targets:
             target_el = etree.SubElement(span, TARGET_OCCURRENCE_TAG)
             target_el.set("id", target)
-        assert (
-            type(data.ext_refs) == list
-        ), f"ext_refs should be a list of dictionaries (can be empty)"
+        if type(data.ext_refs) != list:
+            logging.info("ext_refs should be a list of dictionaries (can be empty)")
         ext_refs_el = etree.SubElement(entity, "externalReferences")
         for ext_ref_info in data.ext_refs:
             one_ext_ref_el = etree.SubElement(ext_refs_el, "externalRef")
             one_ext_ref_el.set("reference", ext_ref_info["reference"])
             for optional_attr in ["resource", "source", "timestamp"]:
                 if optional_attr in ext_ref_info:
                     one_ext_ref_el.set(optional_attr, ext_ref_info[optional_attr])
```

## nafigator/parse.py

```diff
@@ -70,15 +70,15 @@
     tree = generate_naf(
         input=input,
         engine=engine,
         language=language,
         naf_version=naf_version,
         dtd_validation=dtd_validation,
     )
-    tree.write(output, "xml")
+    tree.write(output)
 
 
 def generate_naf(
     input: str = None,
     engine: str = None,
     language: str = None,
     naf_version: str = None,
@@ -146,18 +146,18 @@
 
     process_linguistic_steps(params)
 
     # check it lengths match
     doc_text = params["engine"].document_text(params["doc"])
     raw = params["tree"].raw
     text_to_use = params["text"]
-    assert raw.strip() == doc_text.strip(), f"{len(raw)} - {len(doc_text)}"
-    assert (
-        raw.strip() == text_to_use.strip()
-    ), f"{len(raw)} - {len(text_to_use)}"
+    if raw.strip() != doc_text.strip():
+        logging.error("raw length ("+str(len(raw))+") != doc length ("+str(len(doc_text))+")")
+    if raw.strip() != text_to_use.strip():
+        logging.error("raw length ("+str(len(raw))+") != text to use ("+str(len(text_to_use))+")")
 
     # validate naf tree
     if params["dtd_validation"]:
         params["tree"].validate()
 
     return params["tree"]
 
@@ -177,15 +177,16 @@
         params["fileDesc"]["pages"] = params["pages"]
 
     text = params["pdftotext"]
     if params["replace_hidden_characters"]:
         text_to_use = text.translate(hidden_table)
     else:
         text_to_use = text
-    assert len(text) == len(text_to_use)
+    if len(text) != len(text_to_use):
+        logging.info("len text != len text.translate")
     params["text"] = text_to_use
 
 
 def process_linguistic_steps(params: dict):
     """ """
     engine_name = params["engine_name"]
     nlp = params["nlp_object"]
```

## Comparing `nafigator-0.1.8.dist-info/LICENSE` & `nafigator-0.1.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `nafigator-0.1.8.dist-info/METADATA` & `nafigator-0.1.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nafigator
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python package to convert spaCy and Stanza documents to NLP Annotation Format (NAF)
 Home-page: https://github.com/wjwillemse/nafigator
 Author: Willem Jan Willemse
 Author-email: w.j.willemse@xs4all.nl
 License: MIT license
 Keywords: nafigator
 Platform: UNKNOWN
```

## Comparing `nafigator-0.1.8.dist-info/RECORD` & `nafigator-0.1.9.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-nafigator/__init__.py,sha256=M8wxLSCN9mCUfICxYTwloFPxTWPUSbqaMmU4T2t-eis,249
+nafigator/__init__.py,sha256=34b_W7zLGgkaWorFUHYyUvWPCm4ckgZkjPsNg7aVoUs,249
 nafigator/cli.py,sha256=QlyNG2eSMbpX2BO6J7oFeF3iLry9rEfqwi7NVSlTnGM,416
 nafigator/const.py,sha256=nU_lauOPOGREk3-ezZxmXQnoEOpEreqI5hJiXIFcBqo,1754
 nafigator/linguisticprocessor.py,sha256=tRIJetYCfI6C2TTDGTgIG93d7oYmJNm5cb7dMijP5NM,5031
-nafigator/nafdocument.py,sha256=s9pSpuu5XaUVYUuuJq6QPhTFC1rdZkMuo5m_4QfUepo,36510
+nafigator/nafdocument.py,sha256=6-UuizWKismNwDWplZNEBS_8Lx6PbsWrSqX7JYt87WE,36697
 nafigator/nafigator.py,sha256=D6LFLE-FBFoOsDIwCodmdEh1Q1ZzhEUnt9UuTnQFDJg,15521
 nafigator/opennaf.py,sha256=Lsodb0TNdhKLmF2uX2QEzDuVU1sYT_h5V1r5-pP1PdE,554
-nafigator/parse.py,sha256=9XOSAfoISmVqzjemVvESIxKEqCNQE_ALIKCSABybqWc,17798
+nafigator/parse.py,sha256=C_DvEho5P1lj3CFePk6e8sWMZNVL7G402e6QK00FEg0,17947
 nafigator/preprocessprocessor.py,sha256=WVVODvzM3Q-enc104rBFccEvVFc7HSdTPYHNBFL6muI,1959
 nafigator/utils.py,sha256=v1PLEjc2fYKv3wgW32O2i9qoc727sFcUmmwWxUK2ZGc,1069
-nafigator-0.1.8.dist-info/AUTHORS.rst,sha256=AKy7tsICd5NimQGDNVicVu4AAcRG4TpuQGREHAnD4CA,180
-nafigator-0.1.8.dist-info/LICENSE,sha256=ro3FN8W3hEZyMClEVPJT8rYEFRJNRL4N5r5NcptQ2cc,1100
-nafigator-0.1.8.dist-info/METADATA,sha256=JBhcQ3ojrj79IbbUiOt6kSJUFo7mMi-l6BeA68fYDPM,7625
-nafigator-0.1.8.dist-info/WHEEL,sha256=6T3TYZE4YFi2HTS1BeZHNXAi8N52OZT4O-dJ6-ome_4,116
-nafigator-0.1.8.dist-info/entry_points.txt,sha256=BJhvB3ReUK8vb1NH1CdxNVK3jBLvWue7y-Uv0Tczh84,50
-nafigator-0.1.8.dist-info/top_level.txt,sha256=ojTnD5FA2oYo1GK1llRnjg725_vRAgUtQbEfmXqPrfc,10
-nafigator-0.1.8.dist-info/RECORD,,
+nafigator-0.1.9.dist-info/AUTHORS.rst,sha256=AKy7tsICd5NimQGDNVicVu4AAcRG4TpuQGREHAnD4CA,180
+nafigator-0.1.9.dist-info/LICENSE,sha256=ro3FN8W3hEZyMClEVPJT8rYEFRJNRL4N5r5NcptQ2cc,1100
+nafigator-0.1.9.dist-info/METADATA,sha256=oxqPouCgRLWS9nskcztSLsO_-qM5kgwuzb6zkgIdJbg,7625
+nafigator-0.1.9.dist-info/WHEEL,sha256=6T3TYZE4YFi2HTS1BeZHNXAi8N52OZT4O-dJ6-ome_4,116
+nafigator-0.1.9.dist-info/entry_points.txt,sha256=BJhvB3ReUK8vb1NH1CdxNVK3jBLvWue7y-Uv0Tczh84,50
+nafigator-0.1.9.dist-info/top_level.txt,sha256=ojTnD5FA2oYo1GK1llRnjg725_vRAgUtQbEfmXqPrfc,10
+nafigator-0.1.9.dist-info/RECORD,,
```

